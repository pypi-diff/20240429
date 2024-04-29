# Comparing `tmp/figurify-0.0.1.tar.gz` & `tmp/figurify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figurify-0.0.1.tar", last modified: Mon Apr 29 16:49:30 2024, max compression
+gzip compressed data, was "figurify-0.0.2.tar", last modified: Mon Apr 29 17:49:49 2024, max compression
```

## Comparing `figurify-0.0.1.tar` & `figurify-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 16:49:30.183342 figurify-0.0.1/
--rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.1/LICENSE
--rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.1/MANIFEST.in
--rw-r--r--   0 julian    (1000) julian    (1000)    11525 2024-04-29 16:49:30.180009 figurify-0.0.1/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.1/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 16:02:25.000000 figurify-0.0.1/VERSION.txt
--rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.1/documentation.md
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 16:49:30.180009 figurify-0.0.1/figurify/
--rw-r--r--   0 julian    (1000) julian    (1000)     1329 2024-04-28 16:20:13.000000 figurify-0.0.1/figurify/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.1/figurify/material_properties.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.1/figurify/units.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 16:49:30.180009 figurify-0.0.1/figurify.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)    11525 2024-04-29 16:49:30.000000 figurify-0.0.1/figurify.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 16:49:30.000000 figurify-0.0.1/figurify.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 16:49:30.000000 figurify-0.0.1/figurify.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 16:49:30.000000 figurify-0.0.1/figurify.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 16:49:30.183342 figurify-0.0.1/setup.cfg
--rw-r--r--   0 julian    (1000) julian    (1000)      817 2024-04-29 16:02:25.000000 figurify-0.0.1/setup.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:49:49.400425 figurify-0.0.2/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.2/LICENSE
+-rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.2/MANIFEST.in
+-rw-r--r--   0 julian    (1000) julian    (1000)    11525 2024-04-29 17:49:49.400425 figurify-0.0.2/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.2/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 17:46:37.000000 figurify-0.0.2/VERSION.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.2/documentation.md
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:49:49.400425 figurify-0.0.2/figurify/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1329 2024-04-28 16:20:13.000000 figurify-0.0.2/figurify/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.2/figurify/material_properties.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.2/figurify/units.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:49:49.400425 figurify-0.0.2/figurify.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)    11525 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 17:49:49.400425 figurify-0.0.2/setup.cfg
+-rw-r--r--   0 julian    (1000) julian    (1000)      817 2024-04-29 16:02:25.000000 figurify-0.0.2/setup.py
```

### Comparing `figurify-0.0.1/LICENSE` & `figurify-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `figurify-0.0.1/PKG-INFO` & `figurify-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.1
+Version: 0.0.2
 Summary: With figurify you can calculate figures, surfaces and physics.
 Home-page: https://github.com/julian-hess/Figurify.git
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `figurify-0.0.1/README.md` & `figurify-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.1/documentation.md` & `figurify-0.0.2/documentation.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.1/figurify/__init__.py` & `figurify-0.0.2/figurify/__init__.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.1/figurify/material_properties.py` & `figurify-0.0.2/figurify/material_properties.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.1/figurify/units.py` & `figurify-0.0.2/figurify/units.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.1/figurify.egg-info/PKG-INFO` & `figurify-0.0.2/figurify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.1
+Version: 0.0.2
 Summary: With figurify you can calculate figures, surfaces and physics.
 Home-page: https://github.com/julian-hess/Figurify.git
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `figurify-0.0.1/setup.py` & `figurify-0.0.2/setup.py`

 * *Files identical despite different names*

