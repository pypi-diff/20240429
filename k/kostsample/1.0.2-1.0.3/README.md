# Comparing `tmp/kostsample-1.0.2.tar.gz` & `tmp/kostsample-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kostsample-1.0.2.tar", last modified: Mon Apr 29 09:36:22 2024, max compression
+gzip compressed data, was "kostsample-1.0.3.tar", last modified: Mon Apr 29 09:37:20 2024, max compression
```

## Comparing `kostsample-1.0.2.tar` & `kostsample-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-29 09:36:22.424392 kostsample-1.0.2/
--rw-r--r--   0 jenkins    (117) jenkins    (123)     5189 2024-04-29 09:36:22.424392 kostsample-1.0.2/PKG-INFO
--rw-r--r--   0 jenkins    (117) jenkins    (123)     3866 2024-04-27 19:40:14.000000 kostsample-1.0.2/README.md
-drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-29 09:36:22.420392 kostsample-1.0.2/kostsample/
--rw-r--r--   0 jenkins    (117) jenkins    (123)        0 2024-04-27 19:40:14.000000 kostsample-1.0.2/kostsample/__init__.py
--rw-r--r--   0 jenkins    (117) jenkins    (123)       38 2024-04-27 19:40:14.000000 kostsample-1.0.2/kostsample/main.py
-drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-29 09:36:22.420392 kostsample-1.0.2/kostsample.egg-info/
--rw-r--r--   0 jenkins    (117) jenkins    (123)     5189 2024-04-29 09:36:22.000000 kostsample-1.0.2/kostsample.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (117) jenkins    (123)      233 2024-04-29 09:36:22.000000 kostsample-1.0.2/kostsample.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (117) jenkins    (123)        1 2024-04-29 09:36:22.000000 kostsample-1.0.2/kostsample.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (117) jenkins    (123)       49 2024-04-29 09:36:22.000000 kostsample-1.0.2/kostsample.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (117) jenkins    (123)       11 2024-04-29 09:36:22.000000 kostsample-1.0.2/kostsample.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (117) jenkins    (123)       38 2024-04-29 09:36:22.424392 kostsample-1.0.2/setup.cfg
--rw-r--r--   0 jenkins    (117) jenkins    (123)      775 2024-04-29 09:10:56.000000 kostsample-1.0.2/setup.py
+drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-29 09:37:20.932059 kostsample-1.0.3/
+-rw-r--r--   0 jenkins    (117) jenkins    (123)     5189 2024-04-29 09:37:20.932059 kostsample-1.0.3/PKG-INFO
+-rw-r--r--   0 jenkins    (117) jenkins    (123)     3866 2024-04-27 19:40:14.000000 kostsample-1.0.3/README.md
+drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-29 09:37:20.932059 kostsample-1.0.3/kostsample/
+-rw-r--r--   0 jenkins    (117) jenkins    (123)        0 2024-04-27 19:40:14.000000 kostsample-1.0.3/kostsample/__init__.py
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       38 2024-04-27 19:40:14.000000 kostsample-1.0.3/kostsample/main.py
+drwxr-xr-x   0 jenkins    (117) jenkins    (123)        0 2024-04-29 09:37:20.932059 kostsample-1.0.3/kostsample.egg-info/
+-rw-r--r--   0 jenkins    (117) jenkins    (123)     5189 2024-04-29 09:37:20.000000 kostsample-1.0.3/kostsample.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (117) jenkins    (123)      233 2024-04-29 09:37:20.000000 kostsample-1.0.3/kostsample.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)        1 2024-04-29 09:37:20.000000 kostsample-1.0.3/kostsample.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       49 2024-04-29 09:37:20.000000 kostsample-1.0.3/kostsample.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       11 2024-04-29 09:37:20.000000 kostsample-1.0.3/kostsample.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (117) jenkins    (123)       38 2024-04-29 09:37:20.932059 kostsample-1.0.3/setup.cfg
+-rw-r--r--   0 jenkins    (117) jenkins    (123)      775 2024-04-29 09:37:17.000000 kostsample-1.0.3/setup.py
```

### Comparing `kostsample-1.0.2/PKG-INFO` & `kostsample-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kostsample
-Version: 1.0.2
+Version: 1.0.3
 Summary: python-sample-app is a starter template for new python applications
 Home-page: https://github.com/becosta/python-sample-app
 Author: Benjamin Costa & Vitalii Kostyreva
 Author-email: kostyreva-09876@gmail.com
 License: MIT
 Description: # Python Sample App
```

### Comparing `kostsample-1.0.2/README.md` & `kostsample-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kostsample-1.0.2/kostsample.egg-info/PKG-INFO` & `kostsample-1.0.3/kostsample.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kostsample
-Version: 1.0.2
+Version: 1.0.3
 Summary: python-sample-app is a starter template for new python applications
 Home-page: https://github.com/becosta/python-sample-app
 Author: Benjamin Costa & Vitalii Kostyreva
 Author-email: kostyreva-09876@gmail.com
 License: MIT
 Description: # Python Sample App
```

### Comparing `kostsample-1.0.2/setup.py` & `kostsample-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Used in pypi.org as the README description of your package
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
         name='kostsample',
-        version='1.0.2',
+        version='1.0.3',
         description='python-sample-app is a starter template for new python applications',
         author='Benjamin Costa & Vitalii Kostyreva',
         author_email='kostyreva-09876@gmail.com',
         license="MIT",
         url="https://github.com/becosta/python-sample-app",
         packages=['kostsample'],
         entry_points={
```

