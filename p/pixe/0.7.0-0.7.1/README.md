# Comparing `tmp/pixe-0.7.0.tar.gz` & `tmp/pixe-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixe-0.7.0.tar", last modified: Mon Apr 29 01:26:03 2024, max compression
+gzip compressed data, was "pixe-0.7.1.tar", last modified: Mon Apr 29 01:32:49 2024, max compression
```

## Comparing `pixe-0.7.0.tar` & `pixe-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.928824 pixe-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 01:26:00.000000 pixe-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:26:03.928824 pixe-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-29 01:26:00.000000 pixe-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 01:26:00.000000 pixe-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:26:03.928824 pixe-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:00.000000 pixe-0.7.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/src/filetypes/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/image_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/src/pixe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 01:26:00.000000 pixe-0.7.0/src/pixe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-29 01:26:00.000000 pixe-0.7.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-29 01:26:00.000000 pixe-0.7.0/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:32:49.958230 pixe-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 01:32:46.000000 pixe-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:32:49.958230 pixe-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-29 01:32:46.000000 pixe-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 01:32:46.000000 pixe-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:32:49.958230 pixe-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:32:49.954230 pixe-0.7.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:32:46.000000 pixe-0.7.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:32:49.958230 pixe-0.7.1/src/filetypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 01:32:46.000000 pixe-0.7.1/src/filetypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 01:32:46.000000 pixe-0.7.1/src/filetypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-29 01:32:46.000000 pixe-0.7.1/src/filetypes/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-29 01:32:46.000000 pixe-0.7.1/src/filetypes/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:32:49.958230 pixe-0.7.1/src/pixe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:32:49.000000 pixe-0.7.1/src/pixe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 01:32:49.000000 pixe-0.7.1/src/pixe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:32:49.000000 pixe-0.7.1/src/pixe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 01:32:49.000000 pixe-0.7.1/src/pixe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 01:32:49.000000 pixe-0.7.1/src/pixe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 01:32:49.000000 pixe-0.7.1/src/pixe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 01:32:46.000000 pixe-0.7.1/src/pixe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:32:49.958230 pixe-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-29 01:32:46.000000 pixe-0.7.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-29 01:32:46.000000 pixe-0.7.1/tests/test_unit.py
```

### Comparing `pixe-0.7.0/LICENSE` & `pixe-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixe-0.7.0/PKG-INFO` & `pixe-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixe
-Version: 0.7.0
+Version: 0.7.1
 Summary: A digital helper to keep your files neat and tidy
 Author-email: Chris Wells <chris@ithuna.com>
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/ithuna/pixe.git
 Keywords: archive,photos,organize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pixe-0.7.0/README.md` & `pixe-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pixe-0.7.0/pyproject.toml` & `pixe-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixe"
-version = "0.7.0"
+version = "0.7.1"
 description = "A digital helper to keep your files neat and tidy"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache License, Version 2.0"}
 keywords = ["archive", "photos", "organize"]
 authors = [
     {name = "Chris Wells", email = "chris@ithuna.com"},
```

### Comparing `pixe-0.7.0/src/filetypes/base.py` & `pixe-0.7.1/src/filetypes/base.py`

 * *Files identical despite different names*

### Comparing `pixe-0.7.0/src/filetypes/image_file.py` & `pixe-0.7.1/src/filetypes/image_file.py`

 * *Files identical despite different names*

### Comparing `pixe-0.7.0/src/filetypes/video_file.py` & `pixe-0.7.1/src/filetypes/video_file.py`

 * *Files identical despite different names*

### Comparing `pixe-0.7.0/src/pixe.egg-info/PKG-INFO` & `pixe-0.7.1/src/pixe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixe
-Version: 0.7.0
+Version: 0.7.1
 Summary: A digital helper to keep your files neat and tidy
 Author-email: Chris Wells <chris@ithuna.com>
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/ithuna/pixe.git
 Keywords: archive,photos,organize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pixe-0.7.0/src/pixe.py` & `pixe-0.7.1/src/pixe.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # setup logging
 LOGGER = logging.getLogger(__name__)
 
 # store a datetime of when this run began
 START_TIME = datetime.datetime.now()
 
-__version__ = "0.6.0"
+__version__ = "0.7.1"
 
 
 def process_file(file: filetypes, dest_str: str, move: bool = False, **kwargs) -> str:
     """
     process a single file
     :param file: a file to process
     :param dest_str: where should the processed files be moved/copied to
```

### Comparing `pixe-0.7.0/tests/test_integration.py` & `pixe-0.7.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pixe-0.7.0/tests/test_unit.py` & `pixe-0.7.1/tests/test_unit.py`

 * *Files identical despite different names*

