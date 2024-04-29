# Comparing `tmp/vonage_sms-1.1.0.tar.gz` & `tmp/vonage_sms-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_sms-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_sms-1.1.1.tar", last modified: Mon Apr 29 01:52:08 2024, max compression
```

## Comparing `vonage_sms-1.1.0.tar` & `vonage_sms-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.642239 vonage_sms-1.1.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-04-23 14:16:53.641825 vonage_sms-1.1.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      714 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      826 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.642293 vonage_sms-1.1.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.636872 vonage_sms-1.1.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.639166 vonage_sms-1.1.0/src/vonage_sms/
--rw-r--r--   0 mkahan     (503) staff       (20)      285 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      517 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1912 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)      656 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3422 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/sms.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.641367 vonage_sms-1.1.0/src/vonage_sms.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      358 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       11 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.170046 vonage_sms-1.1.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-04-29 01:52:08.169654 vonage_sms-1.1.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      714 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      826 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:08.170098 vonage_sms-1.1.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.163576 vonage_sms-1.1.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.165983 vonage_sms-1.1.1/src/vonage_sms/
+-rw-r--r--   0 mkahan     (503) staff       (20)      285 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/src/vonage_sms/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      517 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/src/vonage_sms/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1912 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/src/vonage_sms/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      656 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/src/vonage_sms/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3422 2024-04-29 01:52:07.000000 vonage_sms-1.1.1/src/vonage_sms/sms.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.169205 vonage_sms-1.1.1/src/vonage_sms.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-04-29 01:52:08.000000 vonage_sms-1.1.1/src/vonage_sms.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      358 2024-04-29 01:52:08.000000 vonage_sms-1.1.1/src/vonage_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:08.000000 vonage_sms-1.1.1/src/vonage_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-29 01:52:08.000000 vonage_sms-1.1.1/src/vonage_sms.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       11 2024-04-29 01:52:08.000000 vonage_sms-1.1.1/src/vonage_sms.egg-info/top_level.txt
```

### Comparing `vonage_sms-1.1.0/PKG-INFO` & `vonage_sms-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-sms
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vonage SMS package
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
 
 # Vonage SMS Package
 
 This package contains the code to use Vonage's SMS API in Python.
 
 It includes a method for sending SMS messages and returns an `SmsResponse` class to handle the response.
```

### Comparing `vonage_sms-1.1.0/README.md` & `vonage_sms-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage_sms-1.1.0/backend_shim.py` & `vonage_sms-1.1.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_sms-1.1.0/pyproject.toml` & `vonage_sms-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = 'vonage-sms'
-version = '1.1.0'
+version = '1.1.1'
 description = 'Vonage SMS package'
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

### Comparing `vonage_sms-1.1.0/src/vonage_sms/errors.py` & `vonage_sms-1.1.1/src/vonage_sms/errors.py`

 * *Files identical despite different names*

### Comparing `vonage_sms-1.1.0/src/vonage_sms/requests.py` & `vonage_sms-1.1.1/src/vonage_sms/requests.py`

 * *Files identical despite different names*

### Comparing `vonage_sms-1.1.0/src/vonage_sms/responses.py` & `vonage_sms-1.1.1/src/vonage_sms/responses.py`

 * *Files identical despite different names*

### Comparing `vonage_sms-1.1.0/src/vonage_sms/sms.py` & `vonage_sms-1.1.1/src/vonage_sms/sms.py`

 * *Files identical despite different names*

### Comparing `vonage_sms-1.1.0/src/vonage_sms.egg-info/PKG-INFO` & `vonage_sms-1.1.1/src/vonage_sms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-sms
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vonage SMS package
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
 
 # Vonage SMS Package
 
 This package contains the code to use Vonage's SMS API in Python.
 
 It includes a method for sending SMS messages and returns an `SmsResponse` class to handle the response.
```

