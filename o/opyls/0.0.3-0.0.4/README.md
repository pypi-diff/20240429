# Comparing `tmp/opyls-0.0.3.tar.gz` & `tmp/opyls-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyls-0.0.3.tar", last modified: Mon Apr 29 05:59:10 2024, max compression
+gzip compressed data, was "opyls-0.0.4.tar", last modified: Mon Apr 29 06:08:45 2024, max compression
```

## Comparing `opyls-0.0.3.tar` & `opyls-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:59:10.340461 opyls-0.0.3/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.3/LICENSE
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 05:59:10.340270 opyls-0.0.3/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.3/README.md
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:59:10.339646 opyls-0.0.3/opyls/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       54 2024-04-29 05:58:56.000000 opyls-0.0.3/opyls/__init__.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      490 2024-04-29 05:21:06.000000 opyls-0.0.3/opyls/load.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      180 2024-04-29 05:58:44.000000 opyls-0.0.3/opyls/paths.py
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 05:59:10.340081 opyls-0.0.3/opyls.egg-info/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 05:59:10.000000 opyls-0.0.3/opyls.egg-info/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      189 2024-04-29 05:59:10.000000 opyls-0.0.3/opyls.egg-info/SOURCES.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 05:59:10.000000 opyls-0.0.3/opyls.egg-info/dependency_links.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 05:59:10.000000 opyls-0.0.3/opyls.egg-info/top_level.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 05:59:10.340497 opyls-0.0.3/setup.cfg
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 05:59:08.000000 opyls-0.0.3/setup.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:08:45.357194 opyls-0.0.4/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.4/LICENSE
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:08:45.356971 opyls-0.0.4/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.4/README.md
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:08:45.356344 opyls-0.0.4/opyls/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       80 2024-04-29 06:08:36.000000 opyls-0.0.4/opyls/__init__.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      925 2024-04-29 06:07:51.000000 opyls-0.0.4/opyls/json.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      958 2024-04-29 06:08:22.000000 opyls-0.0.4/opyls/load.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      680 2024-04-29 06:07:41.000000 opyls-0.0.4/opyls/paths.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:08:45.356758 opyls-0.0.4/opyls.egg-info/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:08:45.000000 opyls-0.0.4/opyls.egg-info/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      203 2024-04-29 06:08:45.000000 opyls-0.0.4/opyls.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 06:08:45.000000 opyls-0.0.4/opyls.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 06:08:45.000000 opyls-0.0.4/opyls.egg-info/top_level.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 06:08:45.357232 opyls-0.0.4/setup.cfg
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 06:08:43.000000 opyls-0.0.4/setup.py
```

### Comparing `opyls-0.0.3/LICENSE` & `opyls-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opyls-0.0.3/PKG-INFO` & `opyls-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.3
+Version: 0.0.4
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.3/opyls.egg-info/PKG-INFO` & `opyls-0.0.4/opyls.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.3
+Version: 0.0.4
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.3/setup.py` & `opyls-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = "opa_oz's python utils"
 LONG_DESCRIPTION = "Python package with stuff that I'm interested in"
 
 setup(
     name="opyls",
     version=VERSION,
     author="Vladimir Levin",
```

