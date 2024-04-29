# Comparing `tmp/vonage_http_client-1.3.0.tar.gz` & `tmp/vonage_http_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_http_client-1.3.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_http_client-1.3.1.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
```

## Comparing `vonage_http_client-1.3.0.tar` & `vonage_http_client-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.228591 vonage_http_client-1.3.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     3868 2024-04-23 14:16:53.227809 vonage_http_client-1.3.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2995 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      910 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.228673 vonage_http_client-1.3.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.219162 vonage_http_client-1.3.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.224076 vonage_http_client-1.3.0/src/vonage_http_client/
--rw-r--r--   0 mkahan     (503) staff       (20)      602 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/src/vonage_http_client/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5021 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/src/vonage_http_client/auth.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4824 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/src/vonage_http_client/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     9623 2024-04-23 14:16:51.000000 vonage_http_client-1.3.0/src/vonage_http_client/http_client.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.227017 vonage_http_client-1.3.0/src/vonage_http_client.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     3868 2024-04-23 14:16:53.000000 vonage_http_client-1.3.0/src/vonage_http_client.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      406 2024-04-23 14:16:53.000000 vonage_http_client-1.3.0/src/vonage_http_client.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_http_client-1.3.0/src/vonage_http_client.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       96 2024-04-23 14:16:53.000000 vonage_http_client-1.3.0/src/vonage_http_client.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       19 2024-04-23 14:16:53.000000 vonage_http_client-1.3.0/src/vonage_http_client.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.660280 vonage_http_client-1.3.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3868 2024-04-29 01:52:07.659565 vonage_http_client-1.3.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2995 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      910 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.660358 vonage_http_client-1.3.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.646996 vonage_http_client-1.3.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.651584 vonage_http_client-1.3.1/src/vonage_http_client/
+-rw-r--r--   0 mkahan     (503) staff       (20)      602 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/src/vonage_http_client/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5021 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/src/vonage_http_client/auth.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     4824 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/src/vonage_http_client/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     9623 2024-04-29 01:52:06.000000 vonage_http_client-1.3.1/src/vonage_http_client/http_client.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.657825 vonage_http_client-1.3.1/src/vonage_http_client.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3868 2024-04-29 01:52:07.000000 vonage_http_client-1.3.1/src/vonage_http_client.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      406 2024-04-29 01:52:07.000000 vonage_http_client-1.3.1/src/vonage_http_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_http_client-1.3.1/src/vonage_http_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       96 2024-04-29 01:52:07.000000 vonage_http_client-1.3.1/src/vonage_http_client.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       19 2024-04-29 01:52:07.000000 vonage_http_client-1.3.1/src/vonage_http_client.egg-info/top_level.txt
```

### Comparing `vonage_http_client-1.3.0/PKG-INFO` & `vonage_http_client-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: vonage-http-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: An HTTP client for making requests to Vonage APIs.
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
-Requires-Dist: vonage-utils>=1.1.0
+Requires-Dist: vonage-utils>=1.1.1
 Requires-Dist: vonage-jwt>=1.1.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: typing-extensions>=4.9.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage HTTP Client Package
 
 This Python package provides a synchronous HTTP client for sending authenticated requests to Vonage APIs.
 
 This package (`vonage-http-client`) is used by the `vonage` Python package and SDK so doesn't require manual installation or config unless you're using this package independently of a SDK.
```

### Comparing `vonage_http_client-1.3.0/README.md` & `vonage_http_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage_http_client-1.3.0/backend_shim.py` & `vonage_http_client-1.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_http_client-1.3.0/pyproject.toml` & `vonage_http_client-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "vonage-http-client"
-version = "1.3.0"
+version = "1.3.1"
 description = "An HTTP client for making requests to Vonage APIs."
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-utils>=1.1.0",
+  "vonage-utils>=1.1.1",
   "vonage-jwt>=1.1.0",
   "requests>=2.27.0",
   "typing-extensions>=4.9.0",
-  "pydantic>=2.6.1",
+  "pydantic>=2.7.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage_http_client-1.3.0/src/vonage_http_client/__init__.py` & `vonage_http_client-1.3.1/src/vonage_http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage_http_client-1.3.0/src/vonage_http_client/auth.py` & `vonage_http_client-1.3.1/src/vonage_http_client/auth.py`

 * *Files identical despite different names*

### Comparing `vonage_http_client-1.3.0/src/vonage_http_client/errors.py` & `vonage_http_client-1.3.1/src/vonage_http_client/errors.py`

 * *Files identical despite different names*

### Comparing `vonage_http_client-1.3.0/src/vonage_http_client/http_client.py` & `vonage_http_client-1.3.1/src/vonage_http_client/http_client.py`

 * *Files identical despite different names*

### Comparing `vonage_http_client-1.3.0/src/vonage_http_client.egg-info/PKG-INFO` & `vonage_http_client-1.3.1/src/vonage_http_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: vonage-http-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: An HTTP client for making requests to Vonage APIs.
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
-Requires-Dist: vonage-utils>=1.1.0
+Requires-Dist: vonage-utils>=1.1.1
 Requires-Dist: vonage-jwt>=1.1.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: typing-extensions>=4.9.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage HTTP Client Package
 
 This Python package provides a synchronous HTTP client for sending authenticated requests to Vonage APIs.
 
 This package (`vonage-http-client`) is used by the `vonage` Python package and SDK so doesn't require manual installation or config unless you're using this package independently of a SDK.
```

