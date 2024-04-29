# Comparing `tmp/nestipy_dynamic_module-0.1.5.tar.gz` & `tmp/nestipy_dynamic_module-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_dynamic_module-0.1.5.tar", max compression
+gzip compressed data, was "nestipy_dynamic_module-0.1.6.tar", max compression
```

## Comparing `nestipy_dynamic_module-0.1.5.tar` & `nestipy_dynamic_module-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_dynamic_module-0.1.5/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_dynamic_module-0.1.5/README.md
--rw-r--r--   0        0        0      399 2024-04-29 09:54:39.032827 nestipy_dynamic_module-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-24 07:15:09.916835 nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/__init__.py
--rw-r--r--   0        0        0     3490 2024-04-29 09:48:30.367789 nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/builder.py
--rw-r--r--   0        0        0      139 2024-04-24 07:14:46.993633 nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/module/__init__.py
--rw-r--r--   0        0        0      517 2024-04-24 07:08:05.538940 nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/module/consumer.py
--rw-r--r--   0        0        0      251 2024-04-24 07:14:10.682894 nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/module/interface.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 nestipy_dynamic_module-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_dynamic_module-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_dynamic_module-0.1.6/README.md
+-rw-r--r--   0        0        0      399 2024-04-29 10:50:12.526414 nestipy_dynamic_module-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-24 07:15:09.916835 nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/__init__.py
+-rw-r--r--   0        0        0     3510 2024-04-29 10:49:57.863158 nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-04-24 07:14:46.993633 nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-04-24 07:08:05.538940 nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-04-24 07:14:10.682894 nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/module/interface.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 nestipy_dynamic_module-0.1.6/PKG-INFO
```

### Comparing `nestipy_dynamic_module-0.1.5/LICENSE` & `nestipy_dynamic_module-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_dynamic_module-0.1.5/README.md` & `nestipy_dynamic_module-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/builder.py` & `nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     def set_extras(
             self,
             extras: dict[str, Any],
             extras_callback: Callable[[DynamicModule, dict[str, Any]], None]
     ):
         self._extras = extras
         self._extras_process_callback = extras_callback
+        return self
 
     def set_method(self, name: str):
         self._method_name = name
         return self
 
     def _extra_return(self, dynamic_module: DynamicModule) -> DynamicModule:
         if self._extras is not None and self._extras_process_callback is not None:
```

### Comparing `nestipy_dynamic_module-0.1.5/src/nestipy_dynamic_module/module/consumer.py` & `nestipy_dynamic_module-0.1.6/src/nestipy_dynamic_module/module/consumer.py`

 * *Files identical despite different names*

### Comparing `nestipy_dynamic_module-0.1.5/PKG-INFO` & `nestipy_dynamic_module-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy-dynamic-module
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy-dynamic-module Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nestipy-dynamic-module Version: 0.1.6 Summary:
 Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: nestipy-ioc (>=0.1.30,<0.2.0) Requires-Dist: nestipy-metadata
 (>=0.1.1,<0.2.0) Description-Content-Type: text/markdown
                                 [Nestipy Logo]
```

