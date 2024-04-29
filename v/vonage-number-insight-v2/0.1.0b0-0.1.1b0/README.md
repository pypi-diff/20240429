# Comparing `tmp/vonage_number_insight_v2-0.1.0b0.tar.gz` & `tmp/vonage_number_insight_v2-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_number_insight_v2-0.1.0b0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_number_insight_v2-0.1.1b0.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
```

## Comparing `vonage_number_insight_v2-0.1.0b0.tar` & `vonage_number_insight_v2-0.1.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.214398 vonage_number_insight_v2-0.1.0b0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1627 2024-04-23 14:16:53.213523 vonage_number_insight_v2-0.1.0b0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      828 2024-04-23 14:16:51.000000 vonage_number_insight_v2-0.1.0b0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_number_insight_v2-0.1.0b0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      856 2024-04-23 14:16:51.000000 vonage_number_insight_v2-0.1.0b0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.214459 vonage_number_insight_v2-0.1.0b0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.203159 vonage_number_insight_v2-0.1.0b0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.207751 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2/
--rw-r--r--   0 mkahan     (503) staff       (20)      175 2024-04-23 14:16:51.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      152 2024-04-23 14:16:51.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2424 2024-04-23 14:16:51.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2/number_insight_v2.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.212387 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1627 2024-04-23 14:16:53.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      429 2024-04-23 14:16:53.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-04-23 14:16:53.000000 vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.915876 vonage_number_insight_v2-0.1.1b0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1627 2024-04-29 01:52:07.915323 vonage_number_insight_v2-0.1.1b0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      828 2024-04-29 01:52:06.000000 vonage_number_insight_v2-0.1.1b0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_number_insight_v2-0.1.1b0/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      856 2024-04-29 01:52:06.000000 vonage_number_insight_v2-0.1.1b0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.915939 vonage_number_insight_v2-0.1.1b0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.906849 vonage_number_insight_v2-0.1.1b0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.909674 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2/
+-rw-r--r--   0 mkahan     (503) staff       (20)      175 2024-04-29 01:52:06.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      152 2024-04-29 01:52:06.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2424 2024-04-29 01:52:06.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2/number_insight_v2.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.914863 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1627 2024-04-29 01:52:07.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      429 2024-04-29 01:52:07.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-29 01:52:07.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-04-29 01:52:07.000000 vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/top_level.txt
```

### Comparing `vonage_number_insight_v2-0.1.0b0/PKG-INFO` & `vonage_number_insight_v2-0.1.1b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-number-insight-v2
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: Vonage Number Insight v2 package
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
 
 # Vonage Number Insight Python SDK package
 
 This package contains the code to use v2 of Vonage's Number Insight API (currently in beta) in Python.
 
 It includes classes for making fraud check requests and handling the responses.
```

### Comparing `vonage_number_insight_v2-0.1.0b0/README.md` & `vonage_number_insight_v2-0.1.1b0/README.md`

 * *Files identical despite different names*

### Comparing `vonage_number_insight_v2-0.1.0b0/backend_shim.py` & `vonage_number_insight_v2-0.1.1b0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_number_insight_v2-0.1.0b0/pyproject.toml` & `vonage_number_insight_v2-0.1.1b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = 'vonage-number-insight-v2'
-version = '0.1.0b0'
+version = '0.1.1b0'
 description = 'Vonage Number Insight v2 package'
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

### Comparing `vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2/number_insight_v2.py` & `vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2/number_insight_v2.py`

 * *Files identical despite different names*

### Comparing `vonage_number_insight_v2-0.1.0b0/src/vonage_number_insight_v2.egg-info/PKG-INFO` & `vonage_number_insight_v2-0.1.1b0/src/vonage_number_insight_v2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-number-insight-v2
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: Vonage Number Insight v2 package
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
 
 # Vonage Number Insight Python SDK package
 
 This package contains the code to use v2 of Vonage's Number Insight API (currently in beta) in Python.
 
 It includes classes for making fraud check requests and handling the responses.
```

