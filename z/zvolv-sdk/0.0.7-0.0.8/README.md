# Comparing `tmp/zvolv_sdk-0.0.7.tar.gz` & `tmp/zvolv_sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zvolv_sdk-0.0.7.tar", last modified: Fri Apr 19 07:16:22 2024, max compression
+gzip compressed data, was "zvolv_sdk-0.0.8.tar", last modified: Fri Apr 19 07:51:44 2024, max compression
```

## Comparing `zvolv_sdk-0.0.7.tar` & `zvolv_sdk-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/tests/test_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/zvolv_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/zvolv_sdk/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/modules/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/modules/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/zvolv_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:44.028259 zvolv_sdk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-19 07:51:44.028259 zvolv_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 07:51:44.028259 zvolv_sdk-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:44.024259 zvolv_sdk-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/tests/test_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:44.024259 zvolv_sdk-0.0.8/zvolv_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:44.028259 zvolv_sdk-0.0.8/zvolv_sdk/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/modules/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/modules/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/modules/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-19 07:51:39.000000 zvolv_sdk-0.0.8/zvolv_sdk/zvolv_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:44.028259 zvolv_sdk-0.0.8/zvolv_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-19 07:51:44.000000 zvolv_sdk-0.0.8/zvolv_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 07:51:44.000000 zvolv_sdk-0.0.8/zvolv_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:51:44.000000 zvolv_sdk-0.0.8/zvolv_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 07:51:44.000000 zvolv_sdk-0.0.8/zvolv_sdk.egg-info/top_level.txt
```

### Comparing `zvolv_sdk-0.0.7/LICENSE` & `zvolv_sdk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.7/PKG-INFO` & `zvolv_sdk-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zvolv_sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Zvolv API Platform SDK for Python
 Home-page: https://github.com/zvolvapi/python-zvolv-sdk
 Download-URL: https://github.com/zvolvapi/python-zvolv-sdk/archive/v_01.tar.gz
 Author: Akshay Jadhav
 Author-email: support@zvolv.com
 License: MIT
 Keywords: zvolv,zvolv-api,web-api,sdk,rest-api-client
@@ -64,30 +64,39 @@
 ## Initialize Workspace
 
 methods for interacting with workspaces.
 
 ```bash
 
 try:
-    workspace = client.workspace.init('kapilwf');
+    workspace = client.workspace.init('kapilwf')
 except Error:
     print(Error)
 
 ```
 ## Perform Authentication
 
 methods for authentication.
 
 ```bash
 try:
-    login = client.auth.login('email', 'pass');
+    login = client.auth.login('email', 'pass')
 except Error:
     print(Error)
 ```
+## Perform Analytics Search
+methods for performing analytics-related operations.
 
+```bash
+try:
+    analytics = client.analytics.search('65c470f6dab3102c930725ca', { query: { match_all: {} }, from: 0, size: 20, track_total_hits: True })
+except Error:
+    print(Error)
+
+```
 
 ### Feedback
 
 ---
 
 If you get stuck, we’re here to help. The following are the best ways to get assistance working through your issue:
```

### Comparing `zvolv_sdk-0.0.7/README.md` & `zvolv_sdk-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,30 +38,39 @@
 ## Initialize Workspace
 
 methods for interacting with workspaces.
 
 ```bash
 
 try:
-    workspace = client.workspace.init('kapilwf');
+    workspace = client.workspace.init('kapilwf')
 except Error:
     print(Error)
 
 ```
 ## Perform Authentication
 
 methods for authentication.
 
 ```bash
 try:
-    login = client.auth.login('email', 'pass');
+    login = client.auth.login('email', 'pass')
 except Error:
     print(Error)
 ```
+## Perform Analytics Search
+methods for performing analytics-related operations.
 
+```bash
+try:
+    analytics = client.analytics.search('65c470f6dab3102c930725ca', { query: { match_all: {} }, from: 0, size: 20, track_total_hits: True })
+except Error:
+    print(Error)
+
+```
 
 ### Feedback
 
 ---
 
 If you get stuck, we’re here to help. The following are the best ways to get assistance working through your issue:
```

### Comparing `zvolv_sdk-0.0.7/setup.py` & `zvolv_sdk-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.7/zvolv_sdk/modules/auth.py` & `zvolv_sdk-0.0.8/zvolv_sdk/modules/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import requests
 import hashlib
 
 class Auth:
-    def __init__(self, session, base_url):
+    def __init__(self, session, base_url, workspace_instance):
         self.session = session
         self.base_url = base_url
+        self.workspace_instance = workspace_instance
+        self.user_instance = None
 
     def login(self, email, password):
         """Authenticate a user and store their auth token."""
         url = f"{self.base_url}/rest/v17/user/login"
+        headers = {
+            'Content-Type': 'application/json',
+            'jwt': 'true',
+            'businessDomain': self.workspace_instance['BUSINESS_DOMAIN'],
+            'businessTagId': self.workspace_instance['BUSINESS_TAG_ID'],
+        }
         sha512pwd = hashlib.sha512(password.encode('utf-8')).hexdigest()
         data = {'email': email, 'password': sha512pwd}
-        response = self.session.post(url, json=data, headers={'Content-Type': 'application/json', 'jwt': True,
-        'businessDomain': 'kapilwf', 'businessTagId' : '449VZ2DY54AF3'})
+        response = self.session.post(url, json=data, headers=headers)
         if response.status_code == 200:
             resp = response.json()
             if resp.get('error') == False:
+                print("Login Success")
                 token = resp['loginToken']
                 self.session.headers.update({'Authorization': f"Bearer {token}"})
-                print(self.session.headers)
+                self.user_instance = resp
             else:
                 print("Login Failed")
                 print(response.json())
 
         return response.json()
```

### Comparing `zvolv_sdk-0.0.7/zvolv_sdk/modules/workspace.py` & `zvolv_sdk-0.0.8/zvolv_sdk/modules/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import requests
-import hashlib
 
 class Workspace:
-    workspaceInstance = None
     def __init__(self, session, base_url):
         self.session = session
         self.base_url = base_url
+        self.workspace_instance = None
     
     def init(self, domain):
         """Set the domain for the workspace."""
         self.session.headers.update({'domain': domain})
         """Fetch workspace details from domain."""
         url = f"{self.base_url}/rest/v17/organisation/web/config/{domain}"
         response = self.session.get(url)
         if response.status_code == 200:
             resp = response.json()
             if resp.get('error') == False:
-                self.workspaceInstance = resp['data']
+                self.workspace_instance = resp['data']
                 print("Init Success")
                 print(response.json())
             else:
                 print("Init Failed")
                 print(response.json())
 
         return response.json()
```

### Comparing `zvolv_sdk-0.0.7/zvolv_sdk/server_configuration.py` & `zvolv_sdk-0.0.8/zvolv_sdk/server_configuration.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.7/zvolv_sdk.egg-info/PKG-INFO` & `zvolv_sdk-0.0.8/zvolv_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zvolv_sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Zvolv API Platform SDK for Python
 Home-page: https://github.com/zvolvapi/python-zvolv-sdk
 Download-URL: https://github.com/zvolvapi/python-zvolv-sdk/archive/v_01.tar.gz
 Author: Akshay Jadhav
 Author-email: support@zvolv.com
 License: MIT
 Keywords: zvolv,zvolv-api,web-api,sdk,rest-api-client
@@ -64,30 +64,39 @@
 ## Initialize Workspace
 
 methods for interacting with workspaces.
 
 ```bash
 
 try:
-    workspace = client.workspace.init('kapilwf');
+    workspace = client.workspace.init('kapilwf')
 except Error:
     print(Error)
 
 ```
 ## Perform Authentication
 
 methods for authentication.
 
 ```bash
 try:
-    login = client.auth.login('email', 'pass');
+    login = client.auth.login('email', 'pass')
 except Error:
     print(Error)
 ```
+## Perform Analytics Search
+methods for performing analytics-related operations.
 
+```bash
+try:
+    analytics = client.analytics.search('65c470f6dab3102c930725ca', { query: { match_all: {} }, from: 0, size: 20, track_total_hits: True })
+except Error:
+    print(Error)
+
+```
 
 ### Feedback
 
 ---
 
 If you get stuck, we’re here to help. The following are the best ways to get assistance working through your issue:
```

