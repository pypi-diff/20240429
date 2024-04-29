# Comparing `tmp/shipper_shippy-2.36.1.tar.gz` & `tmp/shipper_shippy-2.36.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper_shippy-2.36.1.tar", last modified: Mon Apr 29 21:19:37 2024, max compression
+gzip compressed data, was "shipper_shippy-2.36.2.tar", last modified: Mon Apr 29 21:24:11 2024, max compression
```

## Comparing `shipper_shippy-2.36.1.tar` & `shipper_shippy-2.36.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:37.778579 shipper_shippy-2.36.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 21:19:37.778579 shipper_shippy-2.36.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:19:37.778579 shipper_shippy-2.36.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:37.778579 shipper_shippy-2.36.1/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 21:19:37.000000 shipper_shippy-2.36.1/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 21:19:37.000000 shipper_shippy-2.36.1/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:19:37.000000 shipper_shippy-2.36.1/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 21:19:37.000000 shipper_shippy-2.36.1/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 21:19:37.000000 shipper_shippy-2.36.1/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 21:19:37.000000 shipper_shippy-2.36.1/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:37.774578 shipper_shippy-2.36.1/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 21:19:29.000000 shipper_shippy-2.36.1/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:24:11.523723 shipper_shippy-2.36.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 21:24:11.523723 shipper_shippy-2.36.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:24:11.523723 shipper_shippy-2.36.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:24:11.523723 shipper_shippy-2.36.2/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 21:24:11.000000 shipper_shippy-2.36.2/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 21:24:11.000000 shipper_shippy-2.36.2/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:24:11.000000 shipper_shippy-2.36.2/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 21:24:11.000000 shipper_shippy-2.36.2/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 21:24:11.000000 shipper_shippy-2.36.2/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 21:24:11.000000 shipper_shippy-2.36.2/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:24:11.523723 shipper_shippy-2.36.2/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 21:23:57.000000 shipper_shippy-2.36.2/shippy/version.py
```

### Comparing `shipper_shippy-2.36.1/PKG-INFO` & `shipper_shippy-2.36.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.1
+Version: 2.36.2
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper_shippy-2.36.1/README.md` & `shipper_shippy-2.36.2/README.md`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.1/setup.py` & `shipper_shippy-2.36.2/setup.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.1/shipper_shippy.egg-info/PKG-INFO` & `shipper_shippy-2.36.2/shipper_shippy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.1
+Version: 2.36.2
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper_shippy-2.36.1/shippy/__main__.py` & `shipper_shippy-2.36.2/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.1/shippy/client.py` & `shipper_shippy-2.36.2/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.1/shippy/config.py` & `shipper_shippy-2.36.2/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.1/shippy/constants.py` & `shipper_shippy-2.36.2/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.1/shippy/helper.py` & `shipper_shippy-2.36.2/shippy/helper.py`

 * *Files identical despite different names*
