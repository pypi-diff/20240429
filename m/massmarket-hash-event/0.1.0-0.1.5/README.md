# Comparing `tmp/massmarket_hash_event-0.1.0.tar.gz` & `tmp/massmarket_hash_event-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "massmarket_hash_event-0.1.0.tar", last modified: Mon Apr 29 14:35:13 2024, max compression
+gzip compressed data, was "massmarket_hash_event-0.1.5.tar", last modified: Mon Apr 29 08:30:57 2024, max compression
```

## Comparing `massmarket_hash_event-0.1.0.tar` & `massmarket_hash_event-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 14:35:13.154802 massmarket_hash_event-0.1.0/
--rw-r--r--   0 cryptix   (1001) users      (100)     1518 2024-04-29 08:04:49.000000 massmarket_hash_event-0.1.0/Makefile
--rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-29 14:35:13.153802 massmarket_hash_event-0.1.0/PKG-INFO
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 14:35:13.152802 massmarket_hash_event-0.1.0/massmarket_hash_event/
--rw-r--r--   0 cryptix   (1001) users      (100)     5636 2024-04-29 08:17:51.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/__init__.py
--rw-r--r--   0 cryptix   (1001) users      (100)     1952 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/authentication_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)     1782 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/authentication_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     1019 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/error_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)      479 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/error_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     6648 2024-04-29 08:16:37.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/store_events_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)    10868 2024-04-29 08:16:37.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/store_events_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     1992 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/store_requests_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)     1888 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/store_requests_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     2941 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/transport_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)     3394 2024-04-29 14:34:01.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/transport_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     3290 2024-04-29 08:16:57.000000 massmarket_hash_event-0.1.0/massmarket_hash_event/typedData.json
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 14:35:13.153802 massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/
--rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-29 14:35:13.000000 massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/PKG-INFO
--rw-r--r--   0 cryptix   (1001) users      (100)      777 2024-04-29 14:35:13.000000 massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/SOURCES.txt
--rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-04-29 14:35:13.000000 massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/dependency_links.txt
--rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-04-29 14:35:13.000000 massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/requires.txt
--rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-04-29 14:35:13.000000 massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/top_level.txt
--rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-04-29 14:34:15.000000 massmarket_hash_event-0.1.0/pyproject.toml
--rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-04-29 14:35:13.154802 massmarket_hash_event-0.1.0/setup.cfg
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 14:35:13.153802 massmarket_hash_event-0.1.0/tests/
--rw-r--r--   0 cryptix   (1001) users      (100)     1289 2024-04-29 08:21:53.000000 massmarket_hash_event-0.1.0/tests/test_encode.py
--rw-r--r--   0 cryptix   (1001) users      (100)     6515 2024-04-29 08:23:58.000000 massmarket_hash_event-0.1.0/tests/test_signatures.py
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.600065 massmarket_hash_event-0.1.5/
+-rw-r--r--   0 cryptix   (1001) users      (100)     1518 2024-04-29 08:04:49.000000 massmarket_hash_event-0.1.5/Makefile
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-29 08:30:57.600065 massmarket_hash_event-0.1.5/PKG-INFO
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.598065 massmarket_hash_event-0.1.5/massmarket_hash_event/
+-rw-r--r--   0 cryptix   (1001) users      (100)     5636 2024-04-29 08:17:51.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/__init__.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     1952 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     1782 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     1019 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/error_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)      479 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/error_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     6648 2024-04-29 08:16:37.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)    10868 2024-04-29 08:16:37.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     1992 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     1888 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     2941 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     3394 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     3290 2024-04-29 08:16:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/typedData.json
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.599065 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/PKG-INFO
+-rw-r--r--   0 cryptix   (1001) users      (100)      777 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/SOURCES.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/dependency_links.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/requires.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/top_level.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-04-29 08:16:06.000000 massmarket_hash_event-0.1.5/pyproject.toml
+-rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-04-29 08:30:57.600065 massmarket_hash_event-0.1.5/setup.cfg
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.599065 massmarket_hash_event-0.1.5/tests/
+-rw-r--r--   0 cryptix   (1001) users      (100)     1289 2024-04-29 08:21:53.000000 massmarket_hash_event-0.1.5/tests/test_encode.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     6515 2024-04-29 08:23:58.000000 massmarket_hash_event-0.1.5/tests/test_signatures.py
```

### Comparing `massmarket_hash_event-0.1.0/Makefile` & `massmarket_hash_event-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/PKG-INFO` & `massmarket_hash_event-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massmarket_hash_event
-Version: 0.1.0
+Version: 0.1.5
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/__init__.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/__init__.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/authentication_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/authentication_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/error_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/error_pb2.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/store_events_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/store_events_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/store_requests_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/store_requests_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.pyi`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/transport_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/transport_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event/typedData.json` & `massmarket_hash_event-0.1.5/massmarket_hash_event/typedData.json`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/PKG-INFO` & `massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massmarket-hash-event
-Version: 0.1.0
+Version: 0.1.5
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.1.0/massmarket_hash_event.egg-info/SOURCES.txt` & `massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/pyproject.toml` & `massmarket_hash_event-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "massmarket_hash_event"
-version = "0.1.0"
+version = "0.1.5"
 authors = [
     {name = "Henry Bubert", email = "henry@mass.market"},
 ]
 description = "Helper functions to hash events for signature creation and verification on Mass Market."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `massmarket_hash_event-0.1.0/tests/test_encode.py` & `massmarket_hash_event-0.1.5/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.0/tests/test_signatures.py` & `massmarket_hash_event-0.1.5/tests/test_signatures.py`

 * *Files identical despite different names*

