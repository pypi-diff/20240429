# Comparing `tmp/cesm-0.0.7.tar.gz` & `tmp/cesm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesm-0.0.7.tar", last modified: Mon Apr 29 08:44:44 2024, max compression
+gzip compressed data, was "cesm-0.0.8.tar", last modified: Mon Apr 29 11:25:31 2024, max compression
```

## Comparing `cesm-0.0.7.tar` & `cesm-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:44:44.014236 cesm-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:44:44.014236 cesm-0.0.7/Core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:44:34.000000 cesm-0.0.7/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-04-29 08:44:34.000000 cesm-0.0.7/Core/data_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-29 08:44:34.000000 cesm-0.0.7/Core/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    19226 2024-04-29 08:44:34.000000 cesm-0.0.7/Core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-29 08:44:34.000000 cesm-0.0.7/Core/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-04-29 08:44:34.000000 cesm-0.0.7/Core/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 08:44:34.000000 cesm-0.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 08:44:44.014236 cesm-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-29 08:44:34.000000 cesm-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:44:44.014236 cesm-0.0.7/cesm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 08:44:43.000000 cesm-0.0.7/cesm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-29 08:44:43.000000 cesm-0.0.7/cesm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:44:43.000000 cesm-0.0.7/cesm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 08:44:43.000000 cesm-0.0.7/cesm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 08:44:43.000000 cesm-0.0.7/cesm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 08:44:43.000000 cesm-0.0.7/cesm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-29 08:44:34.000000 cesm-0.0.7/cesm.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:44:44.014236 cesm-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-29 08:44:34.000000 cesm-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:25:31.046270 cesm-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 11:25:21.000000 cesm-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 11:25:31.046270 cesm-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-29 11:25:21.000000 cesm-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:25:31.046270 cesm-0.0.8/cesm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 11:25:31.000000 cesm-0.0.8/cesm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-29 11:25:31.000000 cesm-0.0.8/cesm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:25:31.000000 cesm-0.0.8/cesm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 11:25:31.000000 cesm-0.0.8/cesm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 11:25:31.000000 cesm-0.0.8/cesm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 11:25:31.000000 cesm-0.0.8/cesm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-29 11:25:21.000000 cesm-0.0.8/cesm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:25:31.046270 cesm-0.0.8/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:25:21.000000 cesm-0.0.8/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-04-29 11:25:21.000000 cesm-0.0.8/core/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-29 11:25:21.000000 cesm-0.0.8/core/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19226 2024-04-29 11:25:21.000000 cesm-0.0.8/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-29 11:25:21.000000 cesm-0.0.8/core/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11846 2024-04-29 11:25:21.000000 cesm-0.0.8/core/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:25:31.046270 cesm-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-29 11:25:21.000000 cesm-0.0.8/setup.py
```

### Comparing `cesm-0.0.7/Core/data_access.py` & `cesm-0.0.8/core/data_access.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/Core/input_parser.py` & `cesm-0.0.8/core/input_parser.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/Core/model.py` & `cesm-0.0.8/core/model.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/Core/params.py` & `cesm-0.0.8/core/params.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/Core/plotter.py` & `cesm-0.0.8/core/plotter.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/LICENSE.md` & `cesm-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/PKG-INFO` & `cesm-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Compact Energy System Modeling Tool (CESM)
 Home-page: https://github.com/EINS-TUDa/CESM
 Author: ['Sina Hajikazemi', 'Julia Barbosa']
 Author-email: sina.hkazemi@email.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `cesm-0.0.7/README.md` & `cesm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/cesm.egg-info/PKG-INFO` & `cesm-0.0.8/cesm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Compact Energy System Modeling Tool (CESM)
 Home-page: https://github.com/EINS-TUDa/CESM
 Author: ['Sina Hajikazemi', 'Julia Barbosa']
 Author-email: sina.hkazemi@email.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `cesm-0.0.7/cesm.py` & `cesm-0.0.8/cesm.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.7/setup.py` & `cesm-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cesm',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     description='Compact Energy System Modeling Tool (CESM)',
     long_description="""
 Compact Energy System Modeling Tool (CESM)
 This is a compact energy system modeling tool that can model different forms of energy carriers and the conversion processes that convert them to each other. 
 The optimal output of the model determines how much should be invested in each part of the energy system to meet the energy demand and minimize costs.
```

