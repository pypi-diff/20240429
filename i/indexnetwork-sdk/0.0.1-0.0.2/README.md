# Comparing `tmp/indexnetwork_sdk-0.0.1.tar.gz` & `tmp/indexnetwork_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexnetwork_sdk-0.0.1.tar", last modified: Mon Apr 29 15:45:50 2024, max compression
+gzip compressed data, was "indexnetwork_sdk-0.0.2.tar", last modified: Mon Apr 29 15:50:13 2024, max compression
```

## Comparing `indexnetwork_sdk-0.0.1.tar` & `indexnetwork_sdk-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:45:50.581142 indexnetwork_sdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 15:45:50.581142 indexnetwork_sdk-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:45:50.581142 indexnetwork_sdk-0.0.1/indexclient/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 15:45:36.000000 indexnetwork_sdk-0.0.1/indexclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-29 15:45:36.000000 indexnetwork_sdk-0.0.1/indexclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 15:45:36.000000 indexnetwork_sdk-0.0.1/indexclient/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 15:45:36.000000 indexnetwork_sdk-0.0.1/indexclient/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-29 15:45:36.000000 indexnetwork_sdk-0.0.1/indexclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:45:50.581142 indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 15:45:50.000000 indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 15:45:50.000000 indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:45:50.000000 indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 15:45:50.000000 indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 15:45:50.000000 indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:45:50.581142 indexnetwork_sdk-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-29 15:45:36.000000 indexnetwork_sdk-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:13.493396 indexnetwork_sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 15:50:13.493396 indexnetwork_sdk-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:13.493396 indexnetwork_sdk-0.0.2/indexclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 15:50:02.000000 indexnetwork_sdk-0.0.2/indexclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-29 15:50:02.000000 indexnetwork_sdk-0.0.2/indexclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 15:50:02.000000 indexnetwork_sdk-0.0.2/indexclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 15:50:02.000000 indexnetwork_sdk-0.0.2/indexclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-29 15:50:02.000000 indexnetwork_sdk-0.0.2/indexclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:13.493396 indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 15:50:13.000000 indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 15:50:13.000000 indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:50:13.000000 indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 15:50:13.000000 indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 15:50:13.000000 indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:50:13.493396 indexnetwork_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-29 15:50:02.000000 indexnetwork_sdk-0.0.2/setup.py
```

### Comparing `indexnetwork_sdk-0.0.1/PKG-INFO` & `indexnetwork_sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexnetwork-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Index Network SDK
 Home-page: https://github.com/indexnetwork/index
 Author: Index
 Author-email: accounts@index.network
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Requires-Dist: abnf
```

### Comparing `indexnetwork_sdk-0.0.1/indexclient/client.py` & `indexnetwork_sdk-0.0.2/indexclient/client.py`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.1/indexclient/types.py` & `indexnetwork_sdk-0.0.2/indexclient/types.py`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.1/indexclient/utils.py` & `indexnetwork_sdk-0.0.2/indexclient/utils.py`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/PKG-INFO` & `indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexnetwork-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Index Network SDK
 Home-page: https://github.com/indexnetwork/index
 Author: Index
 Author-email: accounts@index.network
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Requires-Dist: abnf
```

### Comparing `indexnetwork_sdk-0.0.1/indexnetwork_sdk.egg-info/requires.txt` & `indexnetwork_sdk-0.0.2/indexnetwork_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `indexnetwork_sdk-0.0.1/setup.py` & `indexnetwork_sdk-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
   name='indexnetwork-sdk',
-  version='0.0.1',
+  version='0.0.2',
   description='Index Network SDK',
   long_description="Index Network Client SDK",
   long_description_content_type='text/markdown',
   author='Index',
   author_email='accounts@index.network',
   url='https://github.com/indexnetwork/index',
   packages=find_packages(),
```

