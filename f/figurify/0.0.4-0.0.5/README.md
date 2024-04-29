# Comparing `tmp/figurify-0.0.4.tar.gz` & `tmp/figurify-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figurify-0.0.4.tar", last modified: Mon Apr 29 18:09:42 2024, max compression
+gzip compressed data, was "figurify-0.0.5.tar", last modified: Mon Apr 29 18:37:03 2024, max compression
```

## Comparing `figurify-0.0.4.tar` & `figurify-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:09:42.373798 figurify-0.0.4/
--rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.4/LICENSE
--rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.4/MANIFEST.in
--rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 18:09:42.373798 figurify-0.0.4/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.4/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 18:05:39.000000 figurify-0.0.4/VERSION.txt
--rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.4/documentation.md
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:09:42.373798 figurify-0.0.4/figurify/
--rw-r--r--   0 julian    (1000) julian    (1000)       96 2024-04-29 18:05:27.000000 figurify-0.0.4/figurify/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.4/figurify/material_properties.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.4/figurify/units.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:09:42.373798 figurify-0.0.4/figurify.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 18:09:42.000000 figurify-0.0.4/figurify.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 18:09:42.000000 figurify-0.0.4/figurify.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 18:09:42.000000 figurify-0.0.4/figurify.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 18:09:42.000000 figurify-0.0.4/figurify.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 18:09:42.373798 figurify-0.0.4/setup.cfg
--rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.0.4/setup.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:37:03.657186 figurify-0.0.5/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.5/LICENSE
+-rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.5/MANIFEST.in
+-rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 18:37:03.657186 figurify-0.0.5/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.5/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 18:36:09.000000 figurify-0.0.5/VERSION.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.5/documentation.md
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:37:03.657186 figurify-0.0.5/figurify/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1351 2024-04-29 18:32:44.000000 figurify-0.0.5/figurify/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.5/figurify/material_properties.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.5/figurify/units.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 18:37:03.657186 figurify-0.0.5/figurify.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 18:37:03.000000 figurify-0.0.5/figurify.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 18:37:03.000000 figurify-0.0.5/figurify.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 18:37:03.000000 figurify-0.0.5/figurify.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 18:37:03.000000 figurify-0.0.5/figurify.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 18:37:03.657186 figurify-0.0.5/setup.cfg
+-rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.0.5/setup.py
```

### Comparing `figurify-0.0.4/LICENSE` & `figurify-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `figurify-0.0.4/PKG-INFO` & `figurify-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.4
+Version: 0.0.5
 Summary: With figurify you can calculate figures, surfaces and physics.
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `figurify-0.0.4/README.md` & `figurify-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.4/documentation.md` & `figurify-0.0.5/documentation.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.4/figurify/material_properties.py` & `figurify-0.0.5/figurify/material_properties.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.4/figurify/units.py` & `figurify-0.0.5/figurify/units.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.4/figurify.egg-info/PKG-INFO` & `figurify-0.0.5/figurify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.4
+Version: 0.0.5
 Summary: With figurify you can calculate figures, surfaces and physics.
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `figurify-0.0.4/setup.py` & `figurify-0.0.5/setup.py`

 * *Files identical despite different names*

