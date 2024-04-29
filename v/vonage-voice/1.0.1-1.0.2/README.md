# Comparing `tmp/vonage_voice-1.0.1.tar.gz` & `tmp/vonage_voice-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_voice-1.0.1.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_voice-1.0.2.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
```

## Comparing `vonage_voice-1.0.1.tar` & `vonage_voice-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.641150 vonage_voice-1.0.1/
--rw-r--r--   0 mkahan     (503) staff       (20)     4517 2024-04-23 14:16:53.640545 vonage_voice-1.0.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     3744 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      830 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.641212 vonage_voice-1.0.1/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.633155 vonage_voice-1.0.1/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.635328 vonage_voice-1.0.1/src/vonage_voice/
--rw-r--r--   0 mkahan     (503) staff       (20)       95 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      232 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/errors.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.639565 vonage_voice-1.0.1/src/vonage_voice/models/
--rw-r--r--   0 mkahan     (503) staff       (20)     1396 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      955 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/common.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1080 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/connect_endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1733 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/enums.py
--rw-r--r--   0 mkahan     (503) staff       (20)      666 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/input_types.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5039 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/ncco.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2785 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1422 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/models/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     8327 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice/voice.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.640093 vonage_voice-1.0.1/src/vonage_voice.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     4517 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      613 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-23 14:16:53.000000 vonage_voice-1.0.1/src/vonage_voice.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.886000 vonage_voice-1.0.2/
+-rw-r--r--   0 mkahan     (503) staff       (20)     4516 2024-04-29 01:52:07.885331 vonage_voice-1.0.2/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     3743 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      830 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.886131 vonage_voice-1.0.2/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.872566 vonage_voice-1.0.2/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.875743 vonage_voice-1.0.2/src/vonage_voice/
+-rw-r--r--   0 mkahan     (503) staff       (20)       95 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      232 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/errors.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.884102 vonage_voice-1.0.2/src/vonage_voice/models/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1396 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      955 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/common.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1080 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/connect_endpoints.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1733 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/enums.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      666 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/input_types.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5039 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/ncco.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2785 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1422 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/models/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     8327 2024-04-29 01:52:06.000000 vonage_voice-1.0.2/src/vonage_voice/voice.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.884535 vonage_voice-1.0.2/src/vonage_voice.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     4516 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      613 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-29 01:52:07.000000 vonage_voice-1.0.2/src/vonage_voice.egg-info/top_level.txt
```

### Comparing `vonage_voice-1.0.1/PKG-INFO` & `vonage_voice-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-voice
-Version: 1.0.1
+Version: 1.0.2
 Summary: Vonage voice package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
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
-Requires-Dist: vonage-http-client>=1.3.0
-Requires-Dist: vonage-utils>=1.1.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage Voice Package
 
 This package contains the code to use [Vonage's Voice API](https://developer.vonage.com/en/voice/voice-api/overview) in Python. This package includes methods for working with the Voice API. It also contains an NCCO (Call Control Object) builder to help you to control call flow.
 
 ## Structure
 
@@ -54,15 +54,15 @@
 response = vonage_client.voice.create_call(call)
 print(response.model_dump())
 ```
 
 ### List Calls
 
 ```python
-# Gets the first 100 results and the record_index of the 
+# Gets the first 100 results and the record_index of the
 # next page if there's more than 100
 calls, next_record_index = vonage_client.voice.list_calls()
 
 # Specify filtering options
 from vonage_voice.models import ListCallsFilter
 
 call_filter = ListCallsFilter(
```

### Comparing `vonage_voice-1.0.1/README.md` & `vonage_voice-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 response = vonage_client.voice.create_call(call)
 print(response.model_dump())
 ```
 
 ### List Calls
 
 ```python
-# Gets the first 100 results and the record_index of the 
+# Gets the first 100 results and the record_index of the
 # next page if there's more than 100
 calls, next_record_index = vonage_client.voice.list_calls()
 
 # Specify filtering options
 from vonage_voice.models import ListCallsFilter
 
 call_filter = ListCallsFilter(
```

### Comparing `vonage_voice-1.0.1/backend_shim.py` & `vonage_voice-1.0.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/pyproject.toml` & `vonage_voice-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = 'vonage-voice'
-version = '1.0.1'
+version = '1.0.2'
 description = 'Vonage voice package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-http-client>=1.3.0",
-  "vonage-utils>=1.1.0",
-  "pydantic>=2.6.1",
+  "vonage-http-client>=1.3.1",
+  "vonage-utils>=1.1.1",
+  "pydantic>=2.7.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/__init__.py` & `vonage_voice-1.0.2/src/vonage_voice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/common.py` & `vonage_voice-1.0.2/src/vonage_voice/models/common.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/connect_endpoints.py` & `vonage_voice-1.0.2/src/vonage_voice/models/connect_endpoints.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/enums.py` & `vonage_voice-1.0.2/src/vonage_voice/models/enums.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/input_types.py` & `vonage_voice-1.0.2/src/vonage_voice/models/input_types.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/ncco.py` & `vonage_voice-1.0.2/src/vonage_voice/models/ncco.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/requests.py` & `vonage_voice-1.0.2/src/vonage_voice/models/requests.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/models/responses.py` & `vonage_voice-1.0.2/src/vonage_voice/models/responses.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice/voice.py` & `vonage_voice-1.0.2/src/vonage_voice/voice.py`

 * *Files identical despite different names*

### Comparing `vonage_voice-1.0.1/src/vonage_voice.egg-info/PKG-INFO` & `vonage_voice-1.0.2/src/vonage_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-voice
-Version: 1.0.1
+Version: 1.0.2
 Summary: Vonage voice package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
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
-Requires-Dist: vonage-http-client>=1.3.0
-Requires-Dist: vonage-utils>=1.1.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage Voice Package
 
 This package contains the code to use [Vonage's Voice API](https://developer.vonage.com/en/voice/voice-api/overview) in Python. This package includes methods for working with the Voice API. It also contains an NCCO (Call Control Object) builder to help you to control call flow.
 
 ## Structure
 
@@ -54,15 +54,15 @@
 response = vonage_client.voice.create_call(call)
 print(response.model_dump())
 ```
 
 ### List Calls
 
 ```python
-# Gets the first 100 results and the record_index of the 
+# Gets the first 100 results and the record_index of the
 # next page if there's more than 100
 calls, next_record_index = vonage_client.voice.list_calls()
 
 # Specify filtering options
 from vonage_voice.models import ListCallsFilter
 
 call_filter = ListCallsFilter(
```

### Comparing `vonage_voice-1.0.1/src/vonage_voice.egg-info/SOURCES.txt` & `vonage_voice-1.0.2/src/vonage_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

