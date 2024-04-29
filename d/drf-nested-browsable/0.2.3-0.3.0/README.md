# Comparing `tmp/drf_nested_browsable-0.2.3.tar.gz` & `tmp/drf_nested_browsable-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_nested_browsable-0.2.3.tar", max compression
+gzip compressed data, was "drf_nested_browsable-0.3.0.tar", max compression
```

## Comparing `drf_nested_browsable-0.2.3.tar` & `drf_nested_browsable-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1656 2024-02-08 16:17:25.775220 drf_nested_browsable-0.2.3/README.md
--rw-r--r--   0        0        0      213 2024-02-08 16:17:25.775220 drf_nested_browsable-0.2.3/drf_nested_browsable/__init__.py
--rw-r--r--   0        0        0     6869 2024-02-08 16:17:25.775220 drf_nested_browsable-0.2.3/drf_nested_browsable/serializers.py
--rw-r--r--   0        0        0     3419 2024-02-08 16:17:25.775220 drf_nested_browsable-0.2.3/drf_nested_browsable/templates/writable_list.html
--rw-r--r--   0        0        0        0 2024-02-08 16:17:25.775220 drf_nested_browsable-0.2.3/drf_nested_browsable/templatetags/__init__.py
--rw-r--r--   0        0        0     4200 2024-02-08 16:17:25.775220 drf_nested_browsable-0.2.3/drf_nested_browsable/templatetags/drf_nested_browsable.py
--rw-r--r--   0        0        0     1152 2024-02-08 16:24:55.723917 drf_nested_browsable-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1783 2024-04-29 08:01:11.719321 drf_nested_browsable-0.3.0/README.md
+-rw-r--r--   0        0        0      213 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/__init__.py
+-rw-r--r--   0        0        0     7010 2024-04-29 07:57:24.554538 drf_nested_browsable-0.3.0/drf_nested_browsable/serializers.py
+-rw-r--r--   0        0        0     3419 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/templates/writable_list.html
+-rw-r--r--   0        0        0        0 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/templatetags/__init__.py
+-rw-r--r--   0        0        0     4200 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/templatetags/drf_nested_browsable.py
+-rw-r--r--   0        0        0     1193 2024-04-29 08:02:55.806714 drf_nested_browsable-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2795 1970-01-01 00:00:00.000000 drf_nested_browsable-0.3.0/PKG-INFO
```

### Comparing `drf_nested_browsable-0.2.3/README.md` & `drf_nested_browsable-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 ### Done
 
 * Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class
 * Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API
 * Arbitrary nesting depth
 * Dynamically removing the parent field from serializers when used as an inner serializer
 * Basic example
+* Support `RecursiveField` from
+  [`djangorestframework-recursive`](https://github.com/heywbj/django-rest-framework-recursive)
 
 ### To do
 
 * Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)
 * Write tests/specs (from example ?)
 * Better form design
 * Add `ManyToMany` to example (and test it)
```

### Comparing `drf_nested_browsable-0.2.3/drf_nested_browsable/serializers.py` & `drf_nested_browsable-0.3.0/drf_nested_browsable/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Provides abstract writable nested serializers for Django Rest Framework
 
 These serializers require some additionnal configuration, that is done through the Meta
 class of the concrete classes
 """
 from rest_framework.serializers import ListSerializer, ModelSerializer
+from rest_framework_recursive.fields import RecursiveField
 
 
 class WritableNestedListSerializer(ListSerializer):
     """
     Can be set as the `list_serializer_class` for any serializer. This will make the
     `many=True` version of the serializer writable and render an appropriate browsable
     API form.
@@ -182,14 +183,16 @@
             ser.set_parent_instance(instance)
             ser.create(list_data)
         return instance
 
     def update(self, instance, validated_data):
         many_children = {}
         for k, ser in self.fields.items():
+            if isinstance(ser, RecursiveField):
+                ser = ser.proxied
             if isinstance(ser, WritableNestedListSerializer):
                 ser.set_parent_instance(instance)
                 many_children.update({k: (ser, validated_data.pop(k, None))})
         instance = super().update(instance, validated_data)
         for k, (ser, list_data) in many_children.items():
             ser.update(getattr(instance, k), list_data)
         return instance
```

### Comparing `drf_nested_browsable-0.2.3/drf_nested_browsable/templates/writable_list.html` & `drf_nested_browsable-0.3.0/drf_nested_browsable/templates/writable_list.html`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.2.3/drf_nested_browsable/templatetags/drf_nested_browsable.py` & `drf_nested_browsable-0.3.0/drf_nested_browsable/templatetags/drf_nested_browsable.py`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.2.3/pyproject.toml` & `drf_nested_browsable-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-nested-browsable"
-version = "0.2.3"
+version = "0.3.0"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Framework :: Django",
     "Intended Audience :: Developers"
 ]
 description = "Writable nested serializers with forms for the Browsable API"
 keywords = ["django", "rest framework", "drf", "browsable api", "nested serializers"]
@@ -15,14 +15,15 @@
 readme = "README.md"
 packages = [{include = "drf_nested_browsable"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 djangorestframework = "^3.14.0"
 django = ">=4.2, <6.0"
+djangorestframework-recursive = "^0.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 python-lsp-server = "^1.7.2"
 pylint = "^2.17.2"
 mypy = "^1.2.0"
 djangorestframework-stubs = "^1.10.0"
```

### Comparing `drf_nested_browsable-0.2.3/PKG-INFO` & `drf_nested_browsable-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: drf-nested-browsable
-Version: 0.2.3
+Version: 0.3.0
 Summary: Writable nested serializers with forms for the Browsable API
 Home-page: https://pierre-couy.dev/projects/drf-nested-browsable.html
 License: MIT
 Keywords: django,rest framework,drf,browsable api,nested serializers
 Author: Pierre Couy
 Author-email: contact@pierre-couy.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=4.2,<6.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: djangorestframework-recursive (>=0.1.2,<0.2.0)
 Project-URL: Repository, https://github.com/pcouy/drf-nested-browsable
 Description-Content-Type: text/markdown
 
 :warning: Work In Progress :warning:
 
 # Writable Nested Serializers with Browsable API Forms
 
@@ -47,14 +49,16 @@
 ### Done
 
 * Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class
 * Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API
 * Arbitrary nesting depth
 * Dynamically removing the parent field from serializers when used as an inner serializer
 * Basic example
+* Support `RecursiveField` from
+  [`djangorestframework-recursive`](https://github.com/heywbj/django-rest-framework-recursive)
 
 ### To do
 
 * Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)
 * Write tests/specs (from example ?)
 * Better form design
 * Add `ManyToMany` to example (and test it)
```

