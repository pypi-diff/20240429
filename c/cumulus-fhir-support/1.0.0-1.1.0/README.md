# Comparing `tmp/cumulus_fhir_support-1.0.0.tar.gz` & `tmp/cumulus_fhir_support-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_fhir_support-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_fhir_support-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_fhir_support-1.0.0.tar` & `cumulus_fhir_support-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      297 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/LICENSE
--rw-r--r--   0        0        0     1064 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/README.md
--rw-r--r--   0        0        0      118 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/cumulus_fhir_support/__init__.py
--rw-r--r--   0        0        0     8025 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/cumulus_fhir_support/schemas.py
--rw-r--r--   0        0        0     1025 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     7187 2023-11-22 16:00:20.641101 cumulus_fhir_support-1.0.0/tests/test_schemas.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 cumulus_fhir_support-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      297 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1064 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/README.md
+-rw-r--r--   0        0        0      118 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/cumulus_fhir_support/__init__.py
+-rw-r--r--   0        0        0     9924 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/cumulus_fhir_support/schemas.py
+-rw-r--r--   0        0        0     1025 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     9045 2024-04-29 12:32:02.221467 cumulus_fhir_support-1.1.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 cumulus_fhir_support-1.1.0/PKG-INFO
```

### Comparing `cumulus_fhir_support-1.0.0/LICENSE` & `cumulus_fhir_support-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulus_fhir_support-1.0.0/README.md` & `cumulus_fhir_support-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_fhir_support-1.0.0/cumulus_fhir_support/schemas.py` & `cumulus_fhir_support-1.1.0/cumulus_fhir_support/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,20 +35,24 @@
     Non-FHIR-spec fields will not be present in the final schema.
     All fields will be marked nullable.
 
     :param resource_type: the FHIR resource name to create a schema for
     :param rows: optionally a set of JSON FHIR resources to ensure are covered by the schema
     :returns: a PyArrow schema that covers the unified shape of all provided rows
     """
+    rows = list(rows or [])
+
     # Examine batch to see the full shape of it, in order to detect any deeply nested fields
     # that we want to make sure to include in the final schema (normally, we go wide but only as
     # deep as we need to)
-    batch_shape = _get_shape_of_dicts(None, rows and list(rows))
+    batch_shape = _get_shape_of_dicts(None, rows)
 
-    return _create_pyarrow_schema_for_resource(resource_type, batch_shape)
+    schema = _create_pyarrow_schema_for_resource(resource_type, batch_shape)
+    schema = _include_contained_schemas(schema, rows, batch_shape)
+    return schema
 
 
 def _get_shape_of_dicts(total_shape: Optional[dict], item: Any) -> dict:
     """
     Examines `item` and gives a description of its "shape".
 
     Shape here means a dictionary tree of fields, like {"id": {}, "code": {"text": {}}}
@@ -75,30 +79,77 @@
     elif isinstance(item, dict):
         for key, val in item.items():
             total_shape[key] = _get_shape_of_dicts(total_shape.get(key), val)
 
     return total_shape
 
 
-def _create_pyarrow_schema_for_resource(resource_type: str, batch_shape: dict) -> pyarrow.Schema:
+def _include_contained_schemas(
+    schema: pyarrow.Schema, rows: list[dict], batch_shape: dict
+) -> pyarrow.Schema:
+    """
+    This will include all contained resource schemas into one big contained schema.
+
+    Specifically, any field found in the shape of the "contained" field will be included,
+    as long as any resource in the contained list (detected via "resourceType") has the field.
+
+    Also see https://github.com/smart-on-fhir/cumulus-etl/issues/250 for discussion
+    of whether it is wise to just comingle the schemas like this.
+    """
+    # Grab all contained resource types that we have in the source data,
+    # which will inform the expected schema inside there.
+    contained_types = sorted(
+        filter(
+            None,
+            {
+                contained_obj.get("resourceType")
+                for row in rows
+                for contained_obj in row.get("contained", [])
+            },
+        )
+    )
+    if not contained_types:
+        return schema  # no need to do anything
+    contained_shape = batch_shape.get("contained")
+
+    # Allow any found fields in any of the contained types
+    fields = {}
+    for contained_type in contained_types:
+        subschema = _create_pyarrow_schema_for_resource(contained_type, contained_shape, wide=False)
+        for name in subschema.names:
+            fields[name] = subschema.field(name)  # will overwrite previous field of same name
+    fields = [fields[name] for name in sorted(fields)]  # sort for a consistent order
+
+    contained_index = schema.get_field_index("contained")
+    schema = schema.remove(contained_index)
+    return schema.insert(
+        contained_index,
+        pyarrow.field("contained", pyarrow.list_(pyarrow.struct(fields))),
+    )
+
+
+def _create_pyarrow_schema_for_resource(
+    resource_type: str, batch_shape: dict, wide: bool = True
+) -> pyarrow.Schema:
     """
     Creates a PyArrow schema based off the named resource (like 'Observation').
 
     This schema will be as wide as the spec is and as deep as the batch_shape is.
 
     batch_shape is a dictionary tree of fields to include, like {"id": {}, "code": {"text": {}}}
     where empty dictionaries indicate no children (but the parent should still be included).
     """
     instance = fhirelementfactory.FHIRElementFactory.instantiate(resource_type, None)
 
     # fhirclient doesn't include `resourceType` in the list of properties. So do that manually.
     type_field = pyarrow.field("resourceType", pyarrow.string())
 
+    level = 0 if wide else 2
     return pyarrow.schema(
-        [type_field, *_fhir_obj_to_pyarrow_fields(instance, batch_shape, level=0)]
+        [type_field, *_fhir_obj_to_pyarrow_fields(instance, batch_shape, level=level)]
     )
 
 
 def _fhir_obj_to_pyarrow_fields(
     base_obj: fhirabstractbase.FHIRAbstractBase, batch_shape: dict, *, level: int
 ) -> list[pyarrow.Field]:
     """Convert a FHIR instance to a PyArrow Field schema list"""
```

### Comparing `cumulus_fhir_support-1.0.0/pyproject.toml` & `cumulus_fhir_support-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cumulus_fhir_support-1.0.0/PKG-INFO` & `cumulus_fhir_support-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-fhir-support
-Version: 1.0.0
+Version: 1.1.0
 Summary: FHIR schema support code for the Cumulus project
 Author-email: Michael Terry <michael.terry@childrens.harvard.edu>
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

