# Comparing `tmp/opyls-0.0.1.tar.gz` & `tmp/opyls-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyls-0.0.1.tar", last modified: Mon Apr 29 05:27:40 2024, max compression
+gzip compressed data, was "opyls-0.0.2.tar", last modified: Mon Apr 29 05:38:11 2024, max compression
```

## Comparing `opyls-0.0.1.tar` & `opyls-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:27:40.344153 opyls-0.0.1/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.1/LICENSE
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 05:27:40.343921 opyls-0.0.1/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.1/README.md
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:27:40.343187 opyls-0.0.1/opyls/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       25 2024-04-29 05:21:28.000000 opyls-0.0.1/opyls/__init__.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      490 2024-04-29 05:21:06.000000 opyls-0.0.1/opyls/load.py
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:27:40.343697 opyls-0.0.1/opyls.egg-info/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 05:27:40.000000 opyls-0.0.1/opyls.egg-info/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      174 2024-04-29 05:27:40.000000 opyls-0.0.1/opyls.egg-info/SOURCES.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 05:27:40.000000 opyls-0.0.1/opyls.egg-info/dependency_links.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 05:27:40.000000 opyls-0.0.1/opyls.egg-info/top_level.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 05:27:40.344193 opyls-0.0.1/setup.cfg
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 05:22:40.000000 opyls-0.0.1/setup.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:38:11.230136 opyls-0.0.2/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.2/LICENSE
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 05:38:11.229927 opyls-0.0.2/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.2/README.md
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:38:11.229193 opyls-0.0.2/opyls/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       27 2024-04-29 05:37:43.000000 opyls-0.0.2/opyls/__init__.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      490 2024-04-29 05:21:06.000000 opyls-0.0.2/opyls/load.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:38:11.229652 opyls-0.0.2/opyls.egg-info/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 05:38:11.000000 opyls-0.0.2/opyls.egg-info/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      174 2024-04-29 05:38:11.000000 opyls-0.0.2/opyls.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 05:38:11.000000 opyls-0.0.2/opyls.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 05:38:11.000000 opyls-0.0.2/opyls.egg-info/top_level.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 05:38:11.230173 opyls-0.0.2/setup.cfg
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 05:37:57.000000 opyls-0.0.2/setup.py
```

### Comparing `opyls-0.0.1/LICENSE` & `opyls-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opyls-0.0.1/PKG-INFO` & `opyls-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.1
+Version: 0.0.2
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.1/opyls.egg-info/PKG-INFO` & `opyls-0.0.2/opyls.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.1
+Version: 0.0.2
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.1/setup.py` & `opyls-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = "opa_oz's python utils"
 LONG_DESCRIPTION = "Python package with stuff that I'm interested in"
 
 setup(
     name="opyls",
     version=VERSION,
     author="Vladimir Levin",
```

