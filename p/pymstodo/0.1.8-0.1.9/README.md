# Comparing `tmp/pymstodo-0.1.8.tar.gz` & `tmp/pymstodo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymstodo-0.1.8.tar", last modified: Sun Apr 28 20:10:47 2024, max compression
+gzip compressed data, was "pymstodo-0.1.9.tar", last modified: Sun Apr 28 20:25:43 2024, max compression
```

## Comparing `pymstodo-0.1.8.tar` & `pymstodo-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:10:47.767568 pymstodo-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 20:10:41.000000 pymstodo-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-28 20:10:47.767568 pymstodo-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-28 20:10:41.000000 pymstodo-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:10:47.767568 pymstodo-0.1.8/pymstodo/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/windows_zones_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-28 20:10:41.000000 pymstodo-0.1.8/pymstodo/windows_zones_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:10:47.767568 pymstodo-0.1.8/pymstodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 20:10:47.000000 pymstodo-0.1.8/pymstodo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:10:47.767568 pymstodo-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-28 20:10:41.000000 pymstodo-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:25:43.730156 pymstodo-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 20:25:40.000000 pymstodo-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-28 20:25:43.726156 pymstodo-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-28 20:25:40.000000 pymstodo-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:25:43.726156 pymstodo-0.1.9/pymstodo/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 20:25:40.000000 pymstodo-0.1.9/pymstodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-04-28 20:25:40.000000 pymstodo-0.1.9/pymstodo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-28 20:25:40.000000 pymstodo-0.1.9/pymstodo/windows_zones_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-28 20:25:40.000000 pymstodo-0.1.9/pymstodo/windows_zones_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:25:43.726156 pymstodo-0.1.9/pymstodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-28 20:25:43.000000 pymstodo-0.1.9/pymstodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-28 20:25:43.000000 pymstodo-0.1.9/pymstodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:25:43.000000 pymstodo-0.1.9/pymstodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-28 20:25:43.000000 pymstodo-0.1.9/pymstodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 20:25:43.000000 pymstodo-0.1.9/pymstodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:25:43.730156 pymstodo-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-28 20:25:40.000000 pymstodo-0.1.9/setup.py
```

### Comparing `pymstodo-0.1.8/LICENSE` & `pymstodo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.8/PKG-INFO` & `pymstodo-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.8
+Version: 0.1.9
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Serhiy Shliapuhin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pymstodo-0.1.8/README.md` & `pymstodo-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.8/pymstodo/client.py` & `pymstodo-0.1.9/pymstodo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
     Args:
         client_id: API client ID
         client_secret: API client secret
         token: Token obtained by method `get_token`
     '''
     _redirect: str = 'https://localhost/login/authorized'
-    _scope: str = 'openid Tasks.ReadWrite offline_access'
+    _scope: str = 'openid Tasks.ReadWrite email profile'
     _authority: str = 'https://login.microsoftonline.com/common'
     _authorize_endpoint: str = '/oauth2/v2.0/authorize'
     _token_endpoint: str = '/oauth2/v2.0/token'
     _base_api_url: str = 'https://graph.microsoft.com/v1.0/me/todo/'
 
     def __init__(self, client_id: str, client_secret: str, token: Token) -> None:
         self.client_id: str = client_id
```

### Comparing `pymstodo-0.1.8/pymstodo/windows_zones_data.py` & `pymstodo-0.1.9/pymstodo/windows_zones_data.py`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.8/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.1.9/pymstodo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.8
+Version: 0.1.9
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Serhiy Shliapuhin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pymstodo-0.1.8/setup.py` & `pymstodo-0.1.9/setup.py`

 * *Files identical despite different names*

