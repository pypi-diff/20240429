# Comparing `tmp/opyls-0.0.5.tar.gz` & `tmp/opyls-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyls-0.0.5.tar", last modified: Mon Apr 29 06:15:43 2024, max compression
+gzip compressed data, was "opyls-0.0.6.tar", last modified: Mon Apr 29 06:17:04 2024, max compression
```

## Comparing `opyls-0.0.5.tar` & `opyls-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:15:43.281986 opyls-0.0.5/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.5/LICENSE
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:15:43.281792 opyls-0.0.5/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.5/README.md
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:15:43.281189 opyls-0.0.5/opyls/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       80 2024-04-29 06:08:36.000000 opyls-0.0.5/opyls/__init__.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      877 2024-04-29 06:15:19.000000 opyls-0.0.5/opyls/json.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)     1320 2024-04-29 06:15:12.000000 opyls-0.0.5/opyls/load.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      644 2024-04-29 06:15:06.000000 opyls-0.0.5/opyls/paths.py
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:15:43.281602 opyls-0.0.5/opyls.egg-info/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:15:43.000000 opyls-0.0.5/opyls.egg-info/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      203 2024-04-29 06:15:43.000000 opyls-0.0.5/opyls.egg-info/SOURCES.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 06:15:43.000000 opyls-0.0.5/opyls.egg-info/dependency_links.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 06:15:43.000000 opyls-0.0.5/opyls.egg-info/top_level.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 06:15:43.282023 opyls-0.0.5/setup.cfg
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 06:15:41.000000 opyls-0.0.5/setup.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:17:04.578442 opyls-0.0.6/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.6/LICENSE
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:17:04.578212 opyls-0.0.6/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.6/README.md
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:17:04.577033 opyls-0.0.6/opyls/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       93 2024-04-29 06:16:42.000000 opyls-0.0.6/opyls/__init__.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      879 2024-04-29 06:16:46.000000 opyls-0.0.6/opyls/json.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)     1320 2024-04-29 06:15:12.000000 opyls-0.0.6/opyls/load.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      644 2024-04-29 06:15:06.000000 opyls-0.0.6/opyls/paths.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:17:04.577751 opyls-0.0.6/opyls.egg-info/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:17:04.000000 opyls-0.0.6/opyls.egg-info/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      203 2024-04-29 06:17:04.000000 opyls-0.0.6/opyls.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 06:17:04.000000 opyls-0.0.6/opyls.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 06:17:04.000000 opyls-0.0.6/opyls.egg-info/top_level.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 06:17:04.578482 opyls-0.0.6/setup.cfg
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 06:17:01.000000 opyls-0.0.6/setup.py
```

### Comparing `opyls-0.0.5/LICENSE` & `opyls-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opyls-0.0.5/PKG-INFO` & `opyls-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.5
+Version: 0.0.6
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.5/opyls/json.py` & `opyls-0.0.6/opyls/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pathlib import Path
 from typing import Any, Union, Optional
 
 
-def j_dumps(filepath: Union[str, Path], data: Any, indent: Optional[int] = None) -> Union[str, Path]:
+def json_dump(filepath: Union[str, Path], data: Any, indent: Optional[int] = None) -> Union[str, Path]:
     """
     Write JSON serializable data to a file.
 
     Args:
         filepath (Union[str, Path]): The file path where the JSON data will be written.
         data (Any): The JSON serializable data to be written to the file.
         indent (Optional[int]): If specified, the number of spaces used for indentation.
```

### Comparing `opyls-0.0.5/opyls/load.py` & `opyls-0.0.6/opyls/load.py`

 * *Files identical despite different names*

### Comparing `opyls-0.0.5/opyls/paths.py` & `opyls-0.0.6/opyls/paths.py`

 * *Files identical despite different names*

### Comparing `opyls-0.0.5/opyls.egg-info/PKG-INFO` & `opyls-0.0.6/opyls.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.5
+Version: 0.0.6
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.5/setup.py` & `opyls-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = "opa_oz's python utils"
 LONG_DESCRIPTION = "Python package with stuff that I'm interested in"
 
 setup(
     name="opyls",
     version=VERSION,
     author="Vladimir Levin",
```

