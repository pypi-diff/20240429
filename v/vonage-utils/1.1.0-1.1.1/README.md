# Comparing `tmp/vonage_utils-1.1.0.tar.gz` & `tmp/vonage_utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_utils-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_utils-1.1.1.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
```

## Comparing `vonage_utils-1.1.0.tar` & `vonage_utils-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.223748 vonage_utils-1.1.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-23 14:16:53.223090 vonage_utils-1.1.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      974 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      834 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.223877 vonage_utils-1.1.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.210651 vonage_utils-1.1.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.218127 vonage_utils-1.1.0/src/vonage_utils/
--rw-r--r--   0 mkahan     (503) staff       (20)      210 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/src/vonage_utils/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      325 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/src/vonage_utils/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)       70 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/src/vonage_utils/models.py
--rw-r--r--   0 mkahan     (503) staff       (20)      262 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/src/vonage_utils/types.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-23 14:16:51.000000 vonage_utils-1.1.0/src/vonage_utils/utils.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.222543 vonage_utils-1.1.0/src/vonage_utils.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-23 14:16:53.000000 vonage_utils-1.1.0/src/vonage_utils.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      374 2024-04-23 14:16:53.000000 vonage_utils-1.1.0/src/vonage_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_utils-1.1.0/src/vonage_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       41 2024-04-23 14:16:53.000000 vonage_utils-1.1.0/src/vonage_utils.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-23 14:16:53.000000 vonage_utils-1.1.0/src/vonage_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.637698 vonage_utils-1.1.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-29 01:52:07.636161 vonage_utils-1.1.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      974 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      834 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.637780 vonage_utils-1.1.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.621942 vonage_utils-1.1.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.628138 vonage_utils-1.1.1/src/vonage_utils/
+-rw-r--r--   0 mkahan     (503) staff       (20)      210 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      325 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)       70 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/models.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      262 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/types.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/utils.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.634440 vonage_utils-1.1.1/src/vonage_utils.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      374 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       41 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/top_level.txt
```

### Comparing `vonage_utils-1.1.0/PKG-INFO` & `vonage_utils-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utils package containing objects for use with Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions>=4.9.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage Utils Package
 
 This package contains utility code that is used by the Vonage Python SDK and other related packages.
 
 The utils module provides two utility functions: `format_phone_number` and `remove_none_values`. It also exposes the `VonageError` type that other exceptions related to Vonage SDK inherit from. This can also be accessed via the main SDK module with `vonage.VonageError`.
```

### Comparing `vonage_utils-1.1.0/README.md` & `vonage_utils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage_utils-1.1.0/backend_shim.py` & `vonage_utils-1.1.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_utils-1.1.0/pyproject.toml` & `vonage_utils-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = 'vonage-utils'
-version = '1.1.0'
+version = '1.1.1'
 description = 'Utils package containing objects for use with Vonage APIs'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
-dependencies = ["typing_extensions>=4.9.0", "pydantic>=2.6.1"]
+dependencies = ["typing_extensions>=4.9.0", "pydantic>=2.7.1"]
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage_utils-1.1.0/src/vonage_utils/utils.py` & `vonage_utils-1.1.1/src/vonage_utils/utils.py`

 * *Files identical despite different names*

### Comparing `vonage_utils-1.1.0/src/vonage_utils.egg-info/PKG-INFO` & `vonage_utils-1.1.1/src/vonage_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utils package containing objects for use with Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions>=4.9.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage Utils Package
 
 This package contains utility code that is used by the Vonage Python SDK and other related packages.
 
 The utils module provides two utility functions: `format_phone_number` and `remove_none_values`. It also exposes the `VonageError` type that other exceptions related to Vonage SDK inherit from. This can also be accessed via the main SDK module with `vonage.VonageError`.
```

