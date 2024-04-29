# Comparing `tmp/glpic-99.0.202404260959.tar.gz` & `tmp/glpic-99.0.202404290910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404260959.tar", last modified: Fri Apr 26 09:59:05 2024, max compression
+gzip compressed data, was "glpic-99.0.202404290910.tar", last modified: Mon Apr 29 09:10:42 2024, max compression
```

## Comparing `glpic-99.0.202404260959.tar` & `glpic-99.0.202404290910.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:59:05.495205 glpic-99.0.202404260959/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 09:59:05.495205 glpic-99.0.202404260959/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 09:58:50.000000 glpic-99.0.202404260959/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:59:05.495205 glpic-99.0.202404260959/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-26 09:58:50.000000 glpic-99.0.202404260959/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-26 09:58:50.000000 glpic-99.0.202404260959/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:59:05.495205 glpic-99.0.202404260959/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:59:05.495205 glpic-99.0.202404260959/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 09:59:05.000000 glpic-99.0.202404260959/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:10:42.700272 glpic-99.0.202404290910/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 09:10:42.700272 glpic-99.0.202404290910/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-29 09:10:22.000000 glpic-99.0.202404290910/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:10:42.700272 glpic-99.0.202404290910/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-29 09:10:22.000000 glpic-99.0.202404290910/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-29 09:10:22.000000 glpic-99.0.202404290910/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:10:42.700272 glpic-99.0.202404290910/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:10:42.700272 glpic-99.0.202404290910/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-29 09:10:42.000000 glpic-99.0.202404290910/setup.py
```

### Comparing `glpic-99.0.202404260959/README.md` & `glpic-99.0.202404290910/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 - valid user and API token
 - prettytable python library
 
 ## env variables
 
 store your creds in any env file such as [glpic.env.sample](glpic.env.sample) and set data accordingly
 
+# Installation
+
+```
+pip3 install glpic
+```
+
 # How to use
 
 ```
 glpic list computers
 ```
 
 ```
```

### Comparing `glpic-99.0.202404260959/glpic/__init__.py` & `glpic-99.0.202404290910/glpic/__init__.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404260959/glpic/cli.py` & `glpic-99.0.202404290910/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404260959/setup.py` & `glpic-99.0.202404290910/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404260959',
+    version='99.0.202404290910',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

