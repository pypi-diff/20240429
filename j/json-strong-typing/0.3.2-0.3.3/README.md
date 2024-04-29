# Comparing `tmp/json_strong_typing-0.3.2.tar.gz` & `tmp/json_strong_typing-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_strong_typing-0.3.2.tar", last modified: Tue Jan  9 18:16:05 2024, max compression
+gzip compressed data, was "json_strong_typing-0.3.3.tar", last modified: Mon Apr 29 11:05:03 2024, max compression
```

## Comparing `json_strong_typing-0.3.2.tar` & `json_strong_typing-0.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-01-09 18:16:05.097783 json_strong_typing-0.3.2/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1171 2024-01-09 18:15:24.000000 json_strong_typing-0.3.2/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       29 2023-10-28 22:57:42.000000 json_strong_typing-0.3.2/MANIFEST.in
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13911 2024-01-09 18:16:05.096834 json_strong_typing-0.3.2/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12794 2022-11-15 09:06:08.000000 json_strong_typing-0.3.2/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-01-09 18:16:05.095681 json_strong_typing-0.3.2/json_strong_typing.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13911 2024-01-09 18:16:05.000000 json_strong_typing-0.3.2/json_strong_typing.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1066 2024-01-09 18:16:05.000000 json_strong_typing-0.3.2/json_strong_typing.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-01-09 18:16:05.000000 json_strong_typing-0.3.2/json_strong_typing.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       68 2024-01-09 18:16:05.000000 json_strong_typing-0.3.2/json_strong_typing.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       14 2024-01-09 18:16:05.000000 json_strong_typing-0.3.2/json_strong_typing.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-01-09 18:16:04.000000 json_strong_typing-0.3.2/json_strong_typing.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-22 08:15:05.000000 json_strong_typing-0.3.2/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1293 2024-01-09 18:16:05.098733 json_strong_typing-0.3.2/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      257 2023-09-24 16:34:06.000000 json_strong_typing-0.3.2/setup.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-01-09 18:16:05.080999 json_strong_typing-0.3.2/strong_typing/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      410 2024-01-09 18:15:09.000000 json_strong_typing-0.3.2/strong_typing/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5745 2023-11-18 16:20:57.000000 json_strong_typing-0.3.2/strong_typing/auxiliary.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13823 2024-01-04 15:09:32.000000 json_strong_typing-0.3.2/strong_typing/classdef.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      724 2023-07-28 21:41:22.000000 json_strong_typing-0.3.2/strong_typing/core.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    33569 2023-12-07 17:01:32.000000 json_strong_typing-0.3.2/strong_typing/deserializer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13186 2023-11-18 16:27:12.000000 json_strong_typing-0.3.2/strong_typing/docstring.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      476 2022-11-16 19:14:59.000000 json_strong_typing-0.3.2/strong_typing/exception.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    32004 2024-01-02 20:02:30.000000 json_strong_typing-0.3.2/strong_typing/inspection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1029 2023-04-21 22:50:41.000000 json_strong_typing-0.3.2/strong_typing/mapping.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6453 2023-09-18 19:44:49.000000 json_strong_typing-0.3.2/strong_typing/name.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:28:31.000000 json_strong_typing-0.3.2/strong_typing/py.typed
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    25383 2023-05-30 22:00:01.000000 json_strong_typing-0.3.2/strong_typing/schema.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3432 2023-12-09 09:14:13.000000 json_strong_typing-0.3.2/strong_typing/serialization.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16571 2023-12-07 17:04:02.000000 json_strong_typing-0.3.2/strong_typing/serializer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      749 2023-04-21 20:51:57.000000 json_strong_typing-0.3.2/strong_typing/slots.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2590 2023-10-28 23:33:23.000000 json_strong_typing-0.3.2/strong_typing/topological.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-01-09 18:16:05.094448 json_strong_typing-0.3.2/tests/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2021-11-23 16:57:16.000000 json_strong_typing-0.3.2/tests/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-11-03 09:17:55.000000 json_strong_typing-0.3.2/tests/empty.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       43 2022-08-04 16:51:47.000000 json_strong_typing-0.3.2/tests/sample_exceptions.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4727 2023-11-16 23:55:25.000000 json_strong_typing-0.3.2/tests/sample_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    14930 2024-01-02 19:48:01.000000 json_strong_typing-0.3.2/tests/test_classdef.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10652 2023-12-09 09:23:29.000000 json_strong_typing-0.3.2/tests/test_deserialization.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10370 2023-10-29 00:09:10.000000 json_strong_typing-0.3.2/tests/test_docstring.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10206 2023-10-29 18:52:49.000000 json_strong_typing-0.3.2/tests/test_inspection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3453 2023-09-18 19:42:06.000000 json_strong_typing-0.3.2/tests/test_name.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3065 2023-10-29 00:09:24.000000 json_strong_typing-0.3.2/tests/test_performance.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12468 2023-11-18 16:29:18.000000 json_strong_typing-0.3.2/tests/test_schema.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8949 2023-12-07 17:13:35.000000 json_strong_typing-0.3.2/tests/test_serialization.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      783 2023-04-22 07:24:15.000000 json_strong_typing-0.3.2/tests/test_slots.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3015 2023-11-18 16:28:53.000000 json_strong_typing-0.3.2/tests/test_topological.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1201 2023-11-18 16:29:09.000000 json_strong_typing-0.3.2/tests/timer.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-29 11:05:03.009436 json_strong_typing-0.3.3/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1171 2024-01-09 18:15:24.000000 json_strong_typing-0.3.3/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       29 2023-10-28 22:57:42.000000 json_strong_typing-0.3.3/MANIFEST.in
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13911 2024-04-29 11:05:03.008480 json_strong_typing-0.3.3/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12794 2022-11-15 09:06:08.000000 json_strong_typing-0.3.3/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-29 11:05:03.007347 json_strong_typing-0.3.3/json_strong_typing.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13911 2024-04-29 11:05:02.000000 json_strong_typing-0.3.3/json_strong_typing.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1066 2024-04-29 11:05:02.000000 json_strong_typing-0.3.3/json_strong_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-04-29 11:05:02.000000 json_strong_typing-0.3.3/json_strong_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       68 2024-04-29 11:05:02.000000 json_strong_typing-0.3.3/json_strong_typing.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       14 2024-04-29 11:05:02.000000 json_strong_typing-0.3.3/json_strong_typing.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-04-29 11:05:02.000000 json_strong_typing-0.3.3/json_strong_typing.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-22 08:15:05.000000 json_strong_typing-0.3.3/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1293 2024-04-29 11:05:03.010843 json_strong_typing-0.3.3/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      257 2023-09-24 16:34:06.000000 json_strong_typing-0.3.3/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-29 11:05:02.994897 json_strong_typing-0.3.3/strong_typing/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      410 2024-04-29 11:04:01.000000 json_strong_typing-0.3.3/strong_typing/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5745 2023-11-18 16:20:57.000000 json_strong_typing-0.3.3/strong_typing/auxiliary.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13823 2024-01-04 15:09:32.000000 json_strong_typing-0.3.3/strong_typing/classdef.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      724 2023-07-28 21:41:22.000000 json_strong_typing-0.3.3/strong_typing/core.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    33596 2024-03-21 12:20:31.000000 json_strong_typing-0.3.3/strong_typing/deserializer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13186 2023-11-18 16:27:12.000000 json_strong_typing-0.3.3/strong_typing/docstring.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      476 2022-11-16 19:14:59.000000 json_strong_typing-0.3.3/strong_typing/exception.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    32679 2024-04-09 08:07:32.000000 json_strong_typing-0.3.3/strong_typing/inspection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1029 2023-04-21 22:50:41.000000 json_strong_typing-0.3.3/strong_typing/mapping.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6453 2023-09-18 19:44:49.000000 json_strong_typing-0.3.3/strong_typing/name.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:28:31.000000 json_strong_typing-0.3.3/strong_typing/py.typed
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    25383 2023-05-30 22:00:01.000000 json_strong_typing-0.3.3/strong_typing/schema.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3432 2023-12-09 09:14:13.000000 json_strong_typing-0.3.3/strong_typing/serialization.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16571 2023-12-07 17:04:02.000000 json_strong_typing-0.3.3/strong_typing/serializer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      749 2023-04-21 20:51:57.000000 json_strong_typing-0.3.3/strong_typing/slots.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2590 2023-10-28 23:33:23.000000 json_strong_typing-0.3.3/strong_typing/topological.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-29 11:05:03.006429 json_strong_typing-0.3.3/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2021-11-23 16:57:16.000000 json_strong_typing-0.3.3/tests/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-11-03 09:17:55.000000 json_strong_typing-0.3.3/tests/empty.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       43 2022-08-04 16:51:47.000000 json_strong_typing-0.3.3/tests/sample_exceptions.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4833 2024-03-21 12:20:41.000000 json_strong_typing-0.3.3/tests/sample_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    14930 2024-01-02 19:48:01.000000 json_strong_typing-0.3.3/tests/test_classdef.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11005 2024-03-21 12:21:30.000000 json_strong_typing-0.3.3/tests/test_deserialization.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10370 2023-10-29 00:09:10.000000 json_strong_typing-0.3.3/tests/test_docstring.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10206 2023-10-29 18:52:49.000000 json_strong_typing-0.3.3/tests/test_inspection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3453 2023-09-18 19:42:06.000000 json_strong_typing-0.3.3/tests/test_name.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3065 2023-10-29 00:09:24.000000 json_strong_typing-0.3.3/tests/test_performance.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12468 2023-11-18 16:29:18.000000 json_strong_typing-0.3.3/tests/test_schema.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8949 2023-12-07 17:13:35.000000 json_strong_typing-0.3.3/tests/test_serialization.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      783 2023-04-22 07:24:15.000000 json_strong_typing-0.3.3/tests/test_slots.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3015 2023-11-18 16:28:53.000000 json_strong_typing-0.3.3/tests/test_topological.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1201 2023-11-18 16:29:09.000000 json_strong_typing-0.3.3/tests/timer.py
```

### Comparing `json_strong_typing-0.3.2/LICENSE` & `json_strong_typing-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/PKG-INFO` & `json_strong_typing-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_strong_typing
-Version: 0.3.2
+Version: 0.3.3
 Summary: Type-safe data interchange for Python data classes
 Home-page: https://github.com/hunyadi/strong_typing
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `json_strong_typing-0.3.2/README.md` & `json_strong_typing-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/json_strong_typing.egg-info/PKG-INFO` & `json_strong_typing-0.3.3/json_strong_typing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_strong_typing
-Version: 0.3.2
+Version: 0.3.3
 Summary: Type-safe data interchange for Python data classes
 Home-page: https://github.com/hunyadi/strong_typing
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `json_strong_typing-0.3.2/json_strong_typing.egg-info/SOURCES.txt` & `json_strong_typing-0.3.3/json_strong_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/setup.cfg` & `json_strong_typing-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/auxiliary.py` & `json_strong_typing-0.3.3/strong_typing/auxiliary.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/classdef.py` & `json_strong_typing-0.3.3/strong_typing/classdef.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/core.py` & `json_strong_typing-0.3.3/strong_typing/core.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/deserializer.py` & `json_strong_typing-0.3.3/strong_typing/deserializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,16 +547,15 @@
         self, property_name: str, field_name: str, parser: Deserializer[T]
     ) -> None:
         self.property_name = property_name
         self.field_name = field_name
         self.parser = parser
 
     @abc.abstractmethod
-    def parse_field(self, data: Dict[str, JsonType]) -> R:
-        ...
+    def parse_field(self, data: Dict[str, JsonType]) -> R: ...
 
 
 class RequiredFieldDeserializer(FieldDeserializer[T, T]):
     "Deserializes a JSON property into a mandatory Python object field."
 
     def parse_field(self, data: Dict[str, JsonType]) -> T:
         if self.property_name not in data:
@@ -833,15 +832,15 @@
             if hasattr(context, typ.__forward_arg__):
                 cache_key = (context.__name__, typ.__forward_arg__)
 
         typ = evaluate_type(typ, context)
 
     typ = unwrap_annotated_type(typ) if is_type_annotated(typ) else typ
 
-    if isinstance(typ, type):
+    if isinstance(typ, type) and typing.get_origin(typ) is None:
         cache_key = (typ.__module__, typ.__name__)
 
     if cache_key is not None:
         deserializer = _CACHE.get(cache_key)
         if deserializer is None:
             deserializer = _create_deserializer(typ)
```

### Comparing `json_strong_typing-0.3.2/strong_typing/docstring.py` & `json_strong_typing-0.3.3/strong_typing/docstring.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/inspection.py` & `json_strong_typing-0.3.3/strong_typing/inspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,14 +430,39 @@
 def _unwrap_generic_list(typ: Type[List[T]]) -> Type[T]:
     "Extracts the item type of a list type (e.g. returns `T` for `List[T]`)."
 
     (list_type,) = typing.get_args(typ)  # unpack single tuple element
     return list_type
 
 
+def is_generic_set(typ: object) -> TypeGuard[Type[set]]:
+    "True if the specified type is a generic set, i.e. `Set[T]`."
+
+    typ = unwrap_annotated_type(typ)
+    return typing.get_origin(typ) is set
+
+
+def unwrap_generic_set(typ: Type[Set[T]]) -> Type[T]:
+    """
+    Extracts the item type of a set type.
+
+    :param typ: The set type `Set[T]`.
+    :returns: The item type `T`.
+    """
+
+    return rewrap_annotated_type(_unwrap_generic_set, typ)
+
+
+def _unwrap_generic_set(typ: Type[Set[T]]) -> Type[T]:
+    "Extracts the item type of a set type (e.g. returns `T` for `Set[T]`)."
+
+    (set_type,) = typing.get_args(typ)  # unpack single tuple element
+    return set_type
+
+
 def is_generic_dict(typ: object) -> TypeGuard[Type[dict]]:
     "True if the specified type is a generic dictionary, i.e. `Dict[KeyType, ValueType]`."
 
     typ = unwrap_annotated_type(typ)
     return typing.get_origin(typ) is dict
```

### Comparing `json_strong_typing-0.3.2/strong_typing/mapping.py` & `json_strong_typing-0.3.3/strong_typing/mapping.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/name.py` & `json_strong_typing-0.3.3/strong_typing/name.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/schema.py` & `json_strong_typing-0.3.3/strong_typing/schema.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/serialization.py` & `json_strong_typing-0.3.3/strong_typing/serialization.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/serializer.py` & `json_strong_typing-0.3.3/strong_typing/serializer.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/slots.py` & `json_strong_typing-0.3.3/strong_typing/slots.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/strong_typing/topological.py` & `json_strong_typing-0.3.3/strong_typing/topological.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/sample_types.py` & `json_strong_typing-0.3.3/tests/sample_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,17 @@
 
 
 @dataclass
 class AnnotatedSimpleDataclass:
     "A simple data class with multiple properties."
 
     int_value: Annotated[int, IntegerRange(19, 82)] = 23
-    float_value: Annotated[
-        float, Precision(significant_digits=6, decimal_digits=3)
-    ] = 4.5
+    float_value: Annotated[float, Precision(significant_digits=6, decimal_digits=3)] = (
+        4.5
+    )
     str_value: Annotated[str, MaxLength(64)] = "string"
 
 
 @dataclass
 class CompositeDataclass:
     list_value: List[str] = field(default_factory=list)
     dict_value: Dict[str, int] = field(default_factory=dict)
@@ -179,14 +179,20 @@
             "a": ValueExample(value=3),
             "b": ValueExample(value=4),
             "c": ValueExample(value=5),
         }
 
 
 @dataclass
+class NestedGenericType:
+    list_of_str: List[str]
+    list_of_dict: List[Dict[str, str]]
+
+
+@dataclass
 class NestedJson:
     json: JsonType
 
 
 @dataclass
 class ClassA:
     name: Literal["A", "a"]
```

### Comparing `json_strong_typing-0.3.2/tests/test_classdef.py` & `json_strong_typing-0.3.3/tests/test_classdef.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_deserialization.py` & `json_strong_typing-0.3.3/tests/test_deserialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     BinaryValueWrapper,
     ClassA,
     ClassB,
     ClassC,
     FrozenValueWrapper,
     LiteralWrapper,
     NestedDataclass,
+    NestedGenericType,
     NestedJson,
     OptionalValueWrapper,
     Side,
     SimpleDataclass,
     SimpleDerivedClass,
     SimpleValueWrapper,
     Suit,
@@ -161,14 +162,23 @@
         with self.assertRaises(TypeError):
             json_to_object(Literal["value", 1], "value")
         with self.assertRaises(TypeError):
             json_to_object(Literal[1, "value"], "value")
         with self.assertRaises(JsonTypeError):
             json_to_object(Literal["val1", "val2", "val3"], "value")
 
+    def test_deserialization_generic(self) -> None:
+        self.assertEqual(
+            json_to_object(
+                NestedGenericType,
+                {"list_of_str": ["str"], "list_of_dict": [{"key": "value"}]},
+            ),
+            NestedGenericType(list_of_str=["str"], list_of_dict=[{"key": "value"}]),
+        )
+
     def test_deserialization_union(self) -> None:
         # built-in types
         self.assertEqual(json_to_object(Union[int, str], 42), 42)
         self.assertEqual(json_to_object(Union[int, str], "a string"), "a string")
         self.assertEqual(json_to_object(Union[str, int], 42), 42)
         self.assertEqual(json_to_object(Union[str, int], "a string"), "a string")
         with self.assertRaises(JsonKeyError):
```

### Comparing `json_strong_typing-0.3.2/tests/test_docstring.py` & `json_strong_typing-0.3.3/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_inspection.py` & `json_strong_typing-0.3.3/tests/test_inspection.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_name.py` & `json_strong_typing-0.3.3/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_performance.py` & `json_strong_typing-0.3.3/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_schema.py` & `json_strong_typing-0.3.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_serialization.py` & `json_strong_typing-0.3.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_slots.py` & `json_strong_typing-0.3.3/tests/test_slots.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/test_topological.py` & `json_strong_typing-0.3.3/tests/test_topological.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.3.2/tests/timer.py` & `json_strong_typing-0.3.3/tests/timer.py`

 * *Files identical despite different names*

