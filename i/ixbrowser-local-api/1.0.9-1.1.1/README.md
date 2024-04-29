# Comparing `tmp/ixbrowser-local-api-1.0.9.tar.gz` & `tmp/ixbrowser_local_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrowser-local-api-1.0.9.tar", last modified: Tue Jan  2 13:18:55 2024, max compression
+gzip compressed data, was "ixbrowser_local_api-1.1.1.tar", last modified: Mon Apr 29 06:14:32 2024, max compression
```

## Comparing `ixbrowser-local-api-1.0.9.tar` & `ixbrowser_local_api-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:18:55.113593 ixbrowser-local-api-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-02 13:18:55.113593 ixbrowser-local-api-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:18:55.113593 ixbrowser-local-api-1.0.9/ixbrowser_local_api/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31854 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 13:18:55.113593 ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-02 13:18:55.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-02 13:18:55.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 13:18:55.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-02 13:18:55.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-02 13:18:55.000000 ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 13:18:55.113593 ixbrowser-local-api-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-02 13:18:44.000000 ixbrowser-local-api-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:32.838344 ixbrowser_local_api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-29 06:14:32.838344 ixbrowser_local_api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:32.838344 ixbrowser_local_api-1.1.1/ixbrowser_local_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32821 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:32.838344 ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-29 06:14:32.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-29 06:14:32.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 06:14:32.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 06:14:32.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 06:14:32.000000 ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 06:14:32.838344 ixbrowser_local_api-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 06:14:25.000000 ixbrowser_local_api-1.1.1/setup.py
```

### Comparing `ixbrowser-local-api-1.0.9/LICENSE` & `ixbrowser_local_api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrowser-local-api-1.0.9/PKG-INFO` & `ixbrowser_local_api-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrowser-local-api
-Version: 1.0.9
+Version: 1.1.1
 Summary: A client of ixBrowser local api
 Home-page: https://github.com/ixspyinc/ixbrowser-local-api-python
 Author: ixBrowser Team
 Author-email: tech@ixborwser.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ixbrowser-local-api-1.0.9/README.md` & `ixbrowser_local_api-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ixbrowser-local-api-1.0.9/ixbrowser_local_api/client.py` & `ixbrowser_local_api-1.1.1/ixbrowser_local_api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from .errors import UnexpectedError, HttpError, ResponseError, BaseError
 from .utils import Utils
 from .consts import Consts
 from .entities import Profile, Proxy, Preference, Fingerprint
 
-
 class IXBrowserClient(object):
     def __init__(self, target=Consts.DEFAULT_API_TARGET, port=Consts.DEFAULT_API_PORT):
         """
 
         :param target:
         :param port:
         """
@@ -73,15 +72,19 @@
         """
         url = self.base_url + Consts.ACTION_FOR_PROFILE_OPEN
         params = dict()
         params['profile_id'] = profile_id
         params['load_extensions'] = load_extensions
         params['load_profile_info_page'] = load_profile_info_page
         params['cookies_backup'] = cookies_backup
-        params['cookie'] = cookie
+        
+        # None appears as null in json, which will cause cookie loading to fail.
+        if cookie is not None:
+            params['cookie'] = cookie
+
         if startup_args is None:
             startup_args = []
         if disable_extension_welcome_page:
             startup_args.append('--disable-extension-welcome-page')
         params['args'] = startup_args
 
         try:
@@ -95,41 +98,49 @@
         if self.code is not None:
             return None
         else:
             return True
 
     def open_profile_with_random_fingerprint(self, profile_id, load_extensions=True, load_profile_info_page=False,
                                              cookie=None, disable_extension_welcome_page=True, startup_args=[],
-                                             proxy_config: Proxy = None):
+                                             proxy_config: Proxy = None, fingerprint_config: Fingerprint = None):
         """
         open profile with random fingerprint
         :param profile_id:
         :param load_extensions:
         :param load_profile_info_page:
         :param cookie:
         :param disable_extension_welcome_page:
         :param startup_args:
         :param proxy_config:
+        :param fingerprint_config:
         :return:
         """
         url = self.base_url + Consts.ACTION_FOR_PROFILE_OPEN_WITH_FINGERPRINT
         params = dict()
         params['profile_id'] = profile_id
         params['load_extensions'] = load_extensions
         params['load_profile_info_page'] = load_profile_info_page
-        params['cookie'] = cookie
+
+        # None appears as null in json, which will cause cookie loading to fail.
+        if cookie is not None:
+            params['cookie'] = cookie
+
         if startup_args is None:
             startup_args = []
         if disable_extension_welcome_page:
             startup_args.append('--disable-extension-welcome-page')
         params['args'] = startup_args
 
         if proxy_config is not None:
             params['proxy_config'] = proxy_config.dump_to_dict()
 
+        if fingerprint_config is not None:
+            params['fingerprint_config'] = fingerprint_config.dump_to_dict()
+
         try:
             self.code = None
             Utils.show_request_log = self.show_request_log
             result = Utils.get_api_response(url, params)
             return result
         except BaseError as e:
             self.code = e.code
@@ -138,17 +149,14 @@
             return None
         else:
             return True
 
     def close_profile(self, profile_id):
         """
         close profile
-        The window is currently closed by killing the process, so it is not recommended at this time.
-        It is recommended to use selenium's close method to close the profile.
-        For example IXBrowserClient.close_profile_via_selenium
         :param profile_id:
         :return:
         """
         url = self.base_url + Consts.ACTION_FOR_PROFILE_CLOSE
         params = dict()
 
         params['profile_id'] = profile_id
@@ -162,19 +170,21 @@
             self.code = e.code
             self.message = e.message
 
         if self.code is not None:
             return None
         else:
             return True
-
+        
     @staticmethod
     def close_profile_via_selenium(obj):
         """
-        Alias method of close_profile
+        close_profile will no longer have a shutdown exception prompt, and selenium-specific methods are no longer needed.
+        
+        Alias method of close_profile, will be deprecated in the future
         :param obj: selenium.webdriver.chrome instance
         :return:
         """
         whs = obj.window_handles
         for handle in whs:
             # Compatible with selenium 3 and selenium 4 methods
             try:
@@ -547,15 +557,14 @@
             self.message = e.message
 
         if self.code is not None:
             return None
         else:
             return True
 
-
     def update_profile_groups_in_batches(self, profile_id, group_id):
         """
         update profile groups in batches
         :param profile_id: integer or list
         :param group_id: integer
         :return:
         """
@@ -592,14 +601,35 @@
         try:
             self.code = None
             Utils.show_request_log = self.show_request_log
             result = Utils.get_api_response(url, params)
             return result
         except BaseError as e:
             self.code = e.code
+            self.message = e.message
+
+        if self.code is not None:
+            return None
+        else:
+            return True
+
+    def empty_recycle_bin(self):
+        """
+        Empty all Profiles in the Recycle Bin
+        :return:
+        """
+        url = self.base_url + Consts.ACTION_FOR_PROFILE_EMPTY_RECYCLE_BIN
+        params = dict()
+        try:
+            self.code = None
+            Utils.show_request_log = self.show_request_log
+            result = Utils.get_api_response(url, params)
+            return result
+        except BaseError as e:
+            self.code = e.code
             self.message = e.message
 
         if self.code is not None:
             return None
         else:
             return True
```

### Comparing `ixbrowser-local-api-1.0.9/ixbrowser_local_api/consts.py` & `ixbrowser_local_api-1.1.1/ixbrowser_local_api/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     ACTION_FOR_PROFILE_DELETE = 'profile-delete'
 
     ACTION_FOR_PROFILE_COPY = 'profile-copy'
 
     ACTION_FOR_PROFILE_CLEAR_CACHE = 'profile-clear-cache'
     ACTION_FOR_PROFILE_GET_COOKIES = 'profile-get-cookies'
     ACTION_FOR_PROFILE_UPDATE_COOKIES = 'profile-update-cookies'
+    ACTION_FOR_PROFILE_EMPTY_RECYCLE_BIN = "empty-recycle-bin"
 
     ACTION_FOR_PROFILE_UPDATE_GROUPS_IN_BATCHES = 'profile-update-groups-in-batches'
 
     ACTION_FOR_PROFILE_UPDATE_PROXY_TO_TRAFFIC_PACKAGE_MODE = 'profile-update-proxy-for-purchased-traffic-package'
     ACTION_FOR_PROFILE_UPDATE_PROXY_TO_PURCHASED_MODE = 'profile-update-proxy-for-purchased-proxy'
     ACTION_FOR_PROFILE_UPDATE_PROXY_TO_CUSTOM_MODE = 'profile-update-proxy-for-custom-proxy'
```

### Comparing `ixbrowser-local-api-1.0.9/ixbrowser_local_api/entities.py` & `ixbrowser_local_api-1.1.1/ixbrowser_local_api/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,14 +368,15 @@
         self.resolving_power = None
 
         self.fonts_type = None
         self.fonts = None
 
         self.webrtc = None
 
+        # 1: Random, 2: Customized, 3: Close
         self.webgl_data_type = None
         self.webgl_image = None
         self.webgl_factory = None
         self.webgl_info = None
 
         self.canvas_type = None
         self.audio_context = None
```

### Comparing `ixbrowser-local-api-1.0.9/ixbrowser_local_api/errors.py` & `ixbrowser_local_api-1.1.1/ixbrowser_local_api/errors.py`

 * *Files identical despite different names*

### Comparing `ixbrowser-local-api-1.0.9/ixbrowser_local_api/utils.py` & `ixbrowser_local_api-1.1.1/ixbrowser_local_api/utils.py`

 * *Files identical despite different names*

### Comparing `ixbrowser-local-api-1.0.9/ixbrowser_local_api.egg-info/PKG-INFO` & `ixbrowser_local_api-1.1.1/ixbrowser_local_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrowser-local-api
-Version: 1.0.9
+Version: 1.1.1
 Summary: A client of ixBrowser local api
 Home-page: https://github.com/ixspyinc/ixbrowser-local-api-python
 Author: ixBrowser Team
 Author-email: tech@ixborwser.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ixbrowser-local-api-1.0.9/setup.py` & `ixbrowser_local_api-1.1.1/setup.py`

 * *Files identical despite different names*

