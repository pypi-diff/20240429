# Comparing `tmp/progress-table-2.2.0.tar.gz` & `tmp/progress-table-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-2.2.0.tar", last modified: Mon Apr 29 17:54:07 2024, max compression
+gzip compressed data, was "progress-table-2.2.1.tar", last modified: Mon Apr 29 18:04:41 2024, max compression
```

## Comparing `progress-table-2.2.0.tar` & `progress-table-2.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.0/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 17:54:07.200280 progress-table-2.2.0/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4139 2024-04-28 20:30:22.000000 progress-table-2.2.0/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.0/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.0/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.0/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.0/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/v1/common.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     7400 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.0/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-29 17:54:07.200280 progress-table-2.2.0/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.2.0/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.2.0/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.2.0/tests/test_examples_automated.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.1/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 18:04:40.996192 progress-table-2.2.1/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4139 2024-04-28 20:30:22.000000 progress-table-2.2.1/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-29 18:02:33.000000 progress-table-2.2.1/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.1/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.1/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.1/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.1/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.1/progress_table/v1/common.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-29 17:54:03.000000 progress-table-2.2.1/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     7475 2024-04-29 18:02:33.000000 progress-table-2.2.1/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.1/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-29 18:04:40.000000 progress-table-2.2.1/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.1/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-29 18:04:40.996192 progress-table-2.2.1/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.2.1/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:04:40.996192 progress-table-2.2.1/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.2.1/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.2.1/tests/test_examples_automated.py
```

### Comparing `progress-table-2.2.0/LICENSE.txt` & `progress-table-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/PKG-INFO` & `progress-table-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.2.0
+Version: 2.2.1
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-2.2.0/README.md` & `progress-table-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/progress_table/v0/progress_table.py` & `progress-table-2.2.1/progress_table/v0/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/progress_table/v0/symbols.py` & `progress-table-2.2.1/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/progress_table/v1/common.py` & `progress-table-2.2.1/progress_table/v1/common.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/progress_table/v1/progress_table.py` & `progress-table-2.2.1/progress_table/v1/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/progress_table/v1/styles.py` & `progress-table-2.2.1/progress_table/v1/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #  Copyright (c) 2022-2024 Szymon Mikler
 
+from __future__ import annotations
+
+from typing import Tuple, Union
+
 from progress_table.v1.common import ALL_COLOR_NAME, maybe_convert_to_colorama
 
 
 def contains_word(short, long):
     return any([short == word.strip(" ") for word in long.split(" ")])
 
 
@@ -69,15 +73,15 @@
 #################
 
 
 class PbarStyleBase:
     name: str
     filled: str
     empty: str
-    head: str | tuple[str, ...]
+    head: Union[str, Tuple[str, ...]]
     color: str = ""
     color_empty: str = ""
 
     def __init__(self, alt=False, clean=False, color=None, color_empty=None):
         if color is not None:
             self.color = maybe_convert_to_colorama(color)
         if color_empty is not None:
```

### Comparing `progress-table-2.2.0/progress_table.egg-info/PKG-INFO` & `progress-table-2.2.1/progress_table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.2.0
+Version: 2.2.1
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-2.2.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-2.2.1/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/progress_table.egg-info/SOURCES.txt` & `progress-table-2.2.1/progress_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/setup.py` & `progress-table-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/tests/test_docs_automated.py` & `progress-table-2.2.1/tests/test_docs_automated.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.0/tests/test_examples_automated.py` & `progress-table-2.2.1/tests/test_examples_automated.py`

 * *Files identical despite different names*

