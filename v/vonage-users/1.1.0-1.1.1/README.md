# Comparing `tmp/vonage_users-1.1.0.tar.gz` & `tmp/vonage_users-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_users-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_users-1.1.1.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
```

## Comparing `vonage_users-1.1.0.tar` & `vonage_users-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.210396 vonage_users-1.1.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     2531 2024-04-23 14:16:53.209779 vonage_users-1.1.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1758 2024-04-23 14:16:51.000000 vonage_users-1.1.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_users-1.1.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      830 2024-04-23 14:16:51.000000 vonage_users-1.1.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.210588 vonage_users-1.1.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.201973 vonage_users-1.1.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.205877 vonage_users-1.1.0/src/vonage_users/
--rw-r--r--   0 mkahan     (503) staff       (20)      205 2024-04-23 14:16:51.000000 vonage_users-1.1.0/src/vonage_users/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2071 2024-04-23 14:16:51.000000 vonage_users-1.1.0/src/vonage_users/common.py
--rw-r--r--   0 mkahan     (503) staff       (20)      597 2024-04-23 14:16:51.000000 vonage_users-1.1.0/src/vonage_users/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)      902 2024-04-23 14:16:51.000000 vonage_users-1.1.0/src/vonage_users/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4197 2024-04-23 14:16:51.000000 vonage_users-1.1.0/src/vonage_users/users.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.208953 vonage_users-1.1.0/src/vonage_users.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2531 2024-04-23 14:16:53.000000 vonage_users-1.1.0/src/vonage_users.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      380 2024-04-23 14:16:53.000000 vonage_users-1.1.0/src/vonage_users.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_users-1.1.0/src/vonage_users.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_users-1.1.0/src/vonage_users.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-23 14:16:53.000000 vonage_users-1.1.0/src/vonage_users.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.596697 vonage_users-1.1.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2531 2024-04-29 01:52:07.595094 vonage_users-1.1.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1758 2024-04-29 01:52:06.000000 vonage_users-1.1.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_users-1.1.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      830 2024-04-29 01:52:06.000000 vonage_users-1.1.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.596799 vonage_users-1.1.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.582601 vonage_users-1.1.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.588918 vonage_users-1.1.1/src/vonage_users/
+-rw-r--r--   0 mkahan     (503) staff       (20)      205 2024-04-29 01:52:06.000000 vonage_users-1.1.1/src/vonage_users/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2071 2024-04-29 01:52:06.000000 vonage_users-1.1.1/src/vonage_users/common.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      597 2024-04-29 01:52:06.000000 vonage_users-1.1.1/src/vonage_users/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      902 2024-04-29 01:52:06.000000 vonage_users-1.1.1/src/vonage_users/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     4197 2024-04-29 01:52:06.000000 vonage_users-1.1.1/src/vonage_users/users.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.593948 vonage_users-1.1.1/src/vonage_users.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2531 2024-04-29 01:52:07.000000 vonage_users-1.1.1/src/vonage_users.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      380 2024-04-29 01:52:07.000000 vonage_users-1.1.1/src/vonage_users.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_users-1.1.1/src/vonage_users.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-29 01:52:07.000000 vonage_users-1.1.1/src/vonage_users.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-29 01:52:07.000000 vonage_users-1.1.1/src/vonage_users.egg-info/top_level.txt
```

### Comparing `vonage_users-1.1.0/PKG-INFO` & `vonage_users-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-users
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vonage Users package
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
 
 # Vonage Users Package
 
 This package contains the code to use Vonage's Users API in Python.
 
 It includes methods for managing users.
```

### Comparing `vonage_users-1.1.0/README.md` & `vonage_users-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage_users-1.1.0/backend_shim.py` & `vonage_users-1.1.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_users-1.1.0/pyproject.toml` & `vonage_users-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = 'vonage-users'
-version = '1.1.0'
+version = '1.1.1'
 description = 'Vonage Users package'
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

### Comparing `vonage_users-1.1.0/src/vonage_users/common.py` & `vonage_users-1.1.1/src/vonage_users/common.py`

 * *Files identical despite different names*

### Comparing `vonage_users-1.1.0/src/vonage_users/requests.py` & `vonage_users-1.1.1/src/vonage_users/requests.py`

 * *Files identical despite different names*

### Comparing `vonage_users-1.1.0/src/vonage_users/responses.py` & `vonage_users-1.1.1/src/vonage_users/responses.py`

 * *Files identical despite different names*

### Comparing `vonage_users-1.1.0/src/vonage_users/users.py` & `vonage_users-1.1.1/src/vonage_users/users.py`

 * *Files identical despite different names*

### Comparing `vonage_users-1.1.0/src/vonage_users.egg-info/PKG-INFO` & `vonage_users-1.1.1/src/vonage_users.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-users
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vonage Users package
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
 
 # Vonage Users Package
 
 This package contains the code to use Vonage's Users API in Python.
 
 It includes methods for managing users.
```

