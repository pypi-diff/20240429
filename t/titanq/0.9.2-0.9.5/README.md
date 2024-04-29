# Comparing `tmp/titanq-0.9.2.tar.gz` & `tmp/titanq-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.9.2.tar", last modified: Tue Apr 23 20:49:34 2024, max compression
+gzip compressed data, was "titanq-0.9.5.tar", last modified: Mon Apr 29 20:08:40 2024, max compression
```

## Comparing `titanq-0.9.2.tar` & `titanq-0.9.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-22 18:15:34.000000 titanq-0.9.2/LICENSE.txt
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6025 2024-04-23 20:49:34.415471 titanq-0.9.2/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5012 2024-04-22 18:15:34.000000 titanq-0.9.2/README.md
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1211 2024-04-23 20:35:00.000000 titanq-0.9.2/pyproject.toml
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-22 18:15:34.000000 titanq-0.9.2/requirements.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-23 20:49:34.415471 titanq-0.9.2/setup.cfg
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/tests/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-22 18:15:34.000000 titanq-0.9.2/tests/test_variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/__init__.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/_client/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_client/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_client/client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_client/model.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/_model/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/constraints.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/errors.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/manifest.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    29177 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2058 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/objective.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5236 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3499 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/variable.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_model/variable_list.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq/_storage/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/managed_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6643 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/s3_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-22 18:15:34.000000 titanq-0.9.2/titanq/_storage/storage_client.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-23 20:49:34.415471 titanq-0.9.2/titanq.egg-info/
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6025 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/requires.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-23 20:49:34.000000 titanq-0.9.2/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.650203 titanq-0.9.5/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-24 18:50:14.000000 titanq-0.9.5/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6025 2024-04-29 20:08:40.650203 titanq-0.9.5/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5012 2024-04-24 18:50:14.000000 titanq-0.9.5/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1402 2024-04-29 20:04:33.000000 titanq-0.9.5/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-24 18:50:14.000000 titanq-0.9.5/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-29 20:08:40.650203 titanq-0.9.5/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.646203 titanq-0.9.5/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-24 18:50:14.000000 titanq-0.9.5/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-24 18:50:14.000000 titanq-0.9.5/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-24 18:50:14.000000 titanq-0.9.5/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-24 18:50:14.000000 titanq-0.9.5/tests/test_optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-24 18:50:14.000000 titanq-0.9.5/tests/test_variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.650203 titanq-0.9.5/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      781 2024-04-29 20:05:25.000000 titanq-0.9.5/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.650203 titanq-0.9.5/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.650203 titanq-0.9.5/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/manifest.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    29177 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2058 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5236 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3499 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/variable.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_model/variable_list.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.650203 titanq-0.9.5/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-29 17:16:21.000000 titanq-0.9.5/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6643 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-24 18:50:14.000000 titanq-0.9.5/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-29 20:08:40.650203 titanq-0.9.5/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6025 2024-04-29 20:08:40.000000 titanq-0.9.5/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-29 20:08:40.000000 titanq-0.9.5/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-29 20:08:40.000000 titanq-0.9.5/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-29 20:08:40.000000 titanq-0.9.5/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-29 20:08:40.000000 titanq-0.9.5/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.9.2/LICENSE.txt` & `titanq-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/PKG-INFO` & `titanq-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.9.2
+Version: 0.9.5
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://sdk.titanq.infinityq.io
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.9.2/README.md` & `titanq-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/pyproject.toml` & `titanq-0.9.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
-dynamic = ["dependencies"]
+dynamic = [ "dependencies", "version"] # follows corresponding keys in [tool.setuptools.dynamic] section
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.9.2"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
@@ -34,8 +33,9 @@
 Examples = "https://github.com/infinityq-tech/titanq-examples"
 
 #Repository = "https://example.com"
 #Issues = "https://example.com"
 #Changelog = "https://example.com"
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = {file = ["requirements.txt"]}  # reads requirements.txt
+version = {attr = "titanq.__version__"}  # reads __version__ variable set in the titanq/__init__.py file
```

### Comparing `titanq-0.9.2/tests/test_client.py` & `titanq-0.9.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/tests/test_model.py` & `titanq-0.9.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/tests/test_numpy_util.py` & `titanq-0.9.5/tests/test_numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/tests/test_optimize_response.py` & `titanq-0.9.5/tests/test_optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/tests/test_variable.py` & `titanq-0.9.5/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/__init__.py` & `titanq-0.9.5/titanq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 from ._model import Model, Vtype, errors, Target, OptimizeResponse
 
 # S3Storage must be exposed to the end user if he wishes to use s3 buckets
 from ._storage import S3Storage
 
 # logger config
 import logging as _logging
-_logging.getLogger("TitanQ").addHandler(_logging.NullHandler())
+_logging.getLogger("TitanQ").addHandler(_logging.NullHandler())
+
+__version__ = 'v0.9.5'
```

### Comparing `titanq-0.9.2/titanq/_client/client.py` & `titanq-0.9.5/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_client/model.py` & `titanq-0.9.5/titanq/_client/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/constraints.py` & `titanq-0.9.5/titanq/_model/constraints.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/errors.py` & `titanq-0.9.5/titanq/_model/errors.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/manifest.py` & `titanq-0.9.5/titanq/_model/manifest.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/model.py` & `titanq-0.9.5/titanq/_model/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/numpy_util.py` & `titanq-0.9.5/titanq/_model/numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/objective.py` & `titanq-0.9.5/titanq/_model/objective.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/optimize_response.py` & `titanq-0.9.5/titanq/_model/optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/variable.py` & `titanq-0.9.5/titanq/_model/variable.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_model/variable_list.py` & `titanq-0.9.5/titanq/_model/variable_list.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_storage/managed_storage.py` & `titanq-0.9.5/titanq/_storage/managed_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_storage/s3_storage.py` & `titanq-0.9.5/titanq/_storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq/_storage/storage_client.py` & `titanq-0.9.5/titanq/_storage/storage_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.2/titanq.egg-info/PKG-INFO` & `titanq-0.9.5/titanq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.9.2
+Version: 0.9.5
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://sdk.titanq.infinityq.io
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.9.2/titanq.egg-info/SOURCES.txt` & `titanq-0.9.5/titanq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

