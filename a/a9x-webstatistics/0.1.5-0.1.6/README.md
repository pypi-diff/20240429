# Comparing `tmp/a9x_webstatistics-0.1.5.tar.gz` & `tmp/a9x_webstatistics-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics-0.1.5.tar", last modified: Sat Apr 27 16:35:46 2024, max compression
+gzip compressed data, was "a9x_webstatistics-0.1.6.tar", last modified: Mon Apr 29 19:59:40 2024, max compression
```

## Comparing `a9x_webstatistics-0.1.5.tar` & `a9x_webstatistics-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:35:46.150252 a9x_webstatistics-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-27 16:35:46.150252 a9x_webstatistics-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-27 16:35:46.154252 a9x_webstatistics-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:35:46.150252 a9x_webstatistics-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:35:46.150252 a9x_webstatistics-0.1.5/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics/module1.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics/updatestatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:35:46.150252 a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-27 16:35:46.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-27 16:35:46.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:35:46.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:35:46.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 16:35:46.000000 a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:35:46.150252 a9x_webstatistics-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-27 16:35:31.000000 a9x_webstatistics-0.1.5/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.456364 a9x_webstatistics-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.456364 a9x_webstatistics-0.1.6/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 19:59:40.000000 a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:59:40.460363 a9x_webstatistics-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 19:59:25.000000 a9x_webstatistics-0.1.6/tests/test_module1.py
```

### Comparing `a9x_webstatistics-0.1.5/LICENSE` & `a9x_webstatistics-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.5/PKG-INFO` & `a9x_webstatistics-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.5
+Version: 0.1.6
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.5/README.md` & `a9x_webstatistics-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.5/setup.py` & `a9x_webstatistics-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.5/src/a9x_webstatistics/updatestatistics.py` & `a9x_webstatistics-0.1.6/src/a9x_webstatistics/updatestatistics.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.5/src/a9x_webstatistics.egg-info/PKG-INFO` & `a9x_webstatistics-0.1.6/src/a9x_webstatistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.5
+Version: 0.1.6
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.5/tests/test_main001.py` & `a9x_webstatistics-0.1.6/tests/test_main001.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.5/tests/test_main010.py` & `a9x_webstatistics-0.1.6/tests/test_main010.py`

 * *Files identical despite different names*

