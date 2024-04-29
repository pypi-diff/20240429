# Comparing `tmp/GermGenie-0.0.1.tar.gz` & `tmp/GermGenie-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/sander/GermGenie/dist/.tmp-sy5tgxje/GermGenie-0.0.1.tar", last modified: Mon Apr 29 13:05:45 2024, max compression
+gzip compressed data, was "/home/sander/GermGenie/dist/.tmp-y9yu4i1n/GermGenie-0.0.2.tar", last modified: Mon Apr 29 13:17:47 2024, max compression
```

## Comparing `GermGenie-0.0.1.tar` & `GermGenie-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:05:45.000000 GermGenie-0.0.1/
--rw-r--r--   0 sander    (1000) sander    (1000)     1089 2024-04-29 12:50:21.000000 GermGenie-0.0.1/LICENSE
--rw-r--r--   0 sander    (1000) sander    (1000)     2533 2024-04-29 13:05:45.000000 GermGenie-0.0.1/PKG-INFO
--rw-r--r--   0 sander    (1000) sander    (1000)     1953 2024-04-29 12:51:34.000000 GermGenie-0.0.1/README.md
--rw-r--r--   0 sander    (1000) sander    (1000)      764 2024-04-29 13:05:34.000000 GermGenie-0.0.1/pyproject.toml
--rw-r--r--   0 sander    (1000) sander    (1000)       38 2024-04-29 13:05:45.000000 GermGenie-0.0.1/setup.cfg
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie/
--rw-r--r--   0 sander    (1000) sander    (1000)     1460 2024-04-29 12:54:55.000000 GermGenie-0.0.1/src/GermGenie/main.py
--rw-r--r--   0 sander    (1000) sander    (1000)     5189 2024-04-29 12:54:30.000000 GermGenie-0.0.1/src/GermGenie/pipeline.py
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie.egg-info/
--rw-r--r--   0 sander    (1000) sander    (1000)     2533 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie.egg-info/PKG-INFO
--rw-r--r--   0 sander    (1000) sander    (1000)      268 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie.egg-info/SOURCES.txt
--rw-r--r--   0 sander    (1000) sander    (1000)        1 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie.egg-info/dependency_links.txt
--rw-r--r--   0 sander    (1000) sander    (1000)       40 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie.egg-info/entry_points.txt
--rw-r--r--   0 sander    (1000) sander    (1000)       10 2024-04-29 13:05:45.000000 GermGenie-0.0.1/src/GermGenie.egg-info/top_level.txt
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:17:47.000000 GermGenie-0.0.2/
+-rw-r--r--   0 sander    (1000) sander    (1000)     1089 2024-04-29 12:50:21.000000 GermGenie-0.0.2/LICENSE
+-rw-r--r--   0 sander    (1000) sander    (1000)     2533 2024-04-29 13:17:47.000000 GermGenie-0.0.2/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)     1953 2024-04-29 12:51:34.000000 GermGenie-0.0.2/README.md
+-rw-r--r--   0 sander    (1000) sander    (1000)      774 2024-04-29 13:17:35.000000 GermGenie-0.0.2/pyproject.toml
+-rw-r--r--   0 sander    (1000) sander    (1000)       38 2024-04-29 13:17:47.000000 GermGenie-0.0.2/setup.cfg
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie/
+-rw-r--r--   0 sander    (1000) sander    (1000)     1460 2024-04-29 12:54:55.000000 GermGenie-0.0.2/src/GermGenie/main.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     5189 2024-04-29 13:15:45.000000 GermGenie-0.0.2/src/GermGenie/pipeline.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie.egg-info/
+-rw-r--r--   0 sander    (1000) sander    (1000)     2533 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie.egg-info/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)      268 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie.egg-info/SOURCES.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie.egg-info/dependency_links.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       50 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie.egg-info/entry_points.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       10 2024-04-29 13:17:47.000000 GermGenie-0.0.2/src/GermGenie.egg-info/top_level.txt
```

### Comparing `GermGenie-0.0.1/LICENSE` & `GermGenie-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GermGenie-0.0.1/PKG-INFO` & `GermGenie-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GermGenie
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for multi-sample 16S classification using EMU
 Author-email: Sander Boden <s.boden1@avans.nl>, Daan Brackel <dcj.brackel@student.avans.nl>
 Project-URL: Repository, https://github.com/Avans-ATLS/GermGenie
 Project-URL: Issues, https://github.com/Avans-ATLS/GermGenie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GermGenie-0.0.1/README.md` & `GermGenie-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GermGenie-0.0.1/pyproject.toml` & `GermGenie-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["plotly>=5.18.0", "osfclient==0.0.5", "pandas>=1.3.5", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "GermGenie"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Sander Boden", email="s.boden1@avans.nl"},
     {name="Daan Brackel", email="dcj.brackel@student.avans.nl"},
 ]
 description = "Python wrapper for multi-sample 16S classification using EMU"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-GermGenie = "main:main"
+GermGenie = "GermGenie.main:main"
 
 [project.urls]
 Repository = "https://github.com/Avans-ATLS/GermGenie"
 Issues = "https://github.com/Avans-ATLS/GermGenie/issues"
```

### Comparing `GermGenie-0.0.1/src/GermGenie/main.py` & `GermGenie-0.0.2/src/GermGenie/main.py`

 * *Files identical despite different names*

### Comparing `GermGenie-0.0.1/src/GermGenie/pipeline.py` & `GermGenie-0.0.2/src/GermGenie/pipeline.py`

 * *Files identical despite different names*

### Comparing `GermGenie-0.0.1/src/GermGenie.egg-info/PKG-INFO` & `GermGenie-0.0.2/src/GermGenie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GermGenie
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for multi-sample 16S classification using EMU
 Author-email: Sander Boden <s.boden1@avans.nl>, Daan Brackel <dcj.brackel@student.avans.nl>
 Project-URL: Repository, https://github.com/Avans-ATLS/GermGenie
 Project-URL: Issues, https://github.com/Avans-ATLS/GermGenie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

