# Comparing `tmp/paloalto_panorama_sdk-0.0.1.tar.gz` & `tmp/paloalto_panorama_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paloalto_panorama_sdk-0.0.1.tar", last modified: Mon Apr 29 08:39:00 2024, max compression
+gzip compressed data, was "paloalto_panorama_sdk-0.0.2.tar", last modified: Mon Apr 29 13:30:35 2024, max compression
```

## Comparing `paloalto_panorama_sdk-0.0.1.tar` & `paloalto_panorama_sdk-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 08:39:00.683831 paloalto_panorama_sdk-0.0.1/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.1/LICENSE
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.1/MANIFEST.in
--rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 08:39:00.683552 paloalto_panorama_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:54:18.000000 paloalto_panorama_sdk-0.0.1/README.md
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 08:39:00.668034 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      110 2024-04-29 08:38:23.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/address_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/address_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      994 2024-04-29 05:06:19.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/key_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      788 2024-04-29 08:38:23.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/panorama_sdk.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     3515 2024-04-29 05:08:50.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/post_rules_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/service_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/service_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 08:39:00.681082 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 08:39:00.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)      708 2024-04-29 08:39:00.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-04-29 08:39:00.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-04-29 08:39:00.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/requires.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-04-29 08:39:00.000000 paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/top_level.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-04-29 08:39:00.683877 paloalto_panorama_sdk-0.0.1/setup.cfg
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.1/setup.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 08:39:00.682164 paloalto_panorama_sdk-0.0.1/tests/
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 08:39:00.683084 paloalto_panorama_sdk-0.0.1/tests/PanoramaAPIMock/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.1/tests/PanoramaAPIMock/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.1/tests/PanoramaAPIMock/panoramaAPIMock.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.1/tests/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:38:23.000000 paloalto_panorama_sdk-0.0.1/tests/test_service.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.157144 paloalto_panorama_sdk-0.0.2/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.2/LICENSE
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.2/MANIFEST.in
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 13:30:35.156736 paloalto_panorama_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:54:18.000000 paloalto_panorama_sdk-0.0.2/README.md
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.138686 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      110 2024-04-29 13:30:30.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/key_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      828 2024-04-29 13:30:14.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/panorama_sdk.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     3515 2024-04-29 05:08:50.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/post_rules_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.148961 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      708 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/requires.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/top_level.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-04-29 13:30:35.157235 paloalto_panorama_sdk-0.0.2/setup.cfg
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.2/setup.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.150076 paloalto_panorama_sdk-0.0.2/tests/
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.156211 paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/panoramaAPIMock.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.2/tests/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.2/tests/test_service.py
```

### Comparing `paloalto_panorama_sdk-0.0.1/LICENSE` & `paloalto_panorama_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/address_groups_manager.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/address_manager.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/key_manager.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/key_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import requests
 
 
 class KeyManager:
 
     @staticmethod
-    def get_api_key(panorama_url, user, password) -> str:
+    def get_api_key(panorama_url, user, password, verify=True) -> str:
         user = user
         password = password
         key_response = requests.get(url=f"{panorama_url}/api/?type=keygen&user={user}&password={password}",
-                                    verify=False)
+                                    verify=verify)
         xml_key = key_response.content.decode('utf-8')
         root = ElementTree.fromstring(xml_key)
         try:
             api_key = root.find(".//key").text
             return api_key
         except AttributeError:
             return "Invalid Credentials"
 
     @staticmethod
-    def check_valid_key(panorama_url, api_key) -> bool:
+    def check_valid_key(panorama_url, api_key, verify=True) -> bool:
         url = f"{panorama_url}/restapi/v10.2/Panorama/Templates"
         headers = {"Content-Type": "application/json", 'X-PAN-KEY': f"{api_key}"}
-        response = requests.get(url=url, headers=headers, verify=False)
+        response = requests.get(url=url, headers=headers, verify=verify)
         if response.status_code == 200:
             return True
         return False
```

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/panorama_sdk.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/panorama_sdk.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from paloalto_panorama_sdk.service_manager import ServiceManager
 from dotenv import load_dotenv
 
 load_dotenv()
 
 
 class PanoramaSDK:
-    def __init__(self, url, username, password):
+    def __init__(self, url, username, password, verify=True):
         self.url = url
         self.username = username
         self.password = password
         self.apikey = KeyManager.get_api_key(
             panorama_url=self.url,
             user=self.username,
-            password=self.password
+            password=self.password,
+            verify=verify
         )
         self.service = ServiceManager(self.url, self.username, self.password)
 
 
 if __name__ == '__main__':
     panSDK = PanoramaSDK(
         url=os.getenv("url", ""),
```

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/post_rules_manager.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/post_rules_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/service_groups_manager.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk/service_manager.py` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/SOURCES.txt` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/paloalto_panorama_sdk.egg-info/requires.txt` & `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/setup.py` & `paloalto_panorama_sdk-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/tests/PanoramaAPIMock/panoramaAPIMock.py` & `paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/panoramaAPIMock.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.1/tests/test_service.py` & `paloalto_panorama_sdk-0.0.2/tests/test_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     @classmethod
     def tearDownClass(cls):
         logging.debug("Stopping PanoramaSDKService thread")
         cls.server_thread.join()
 
     def setUp(self):
         logging.debug("Starting PanoramaSDKService setUp")
-        self.panSDK = PanoramaSDK(url="https://127.17.90.2", username="testuser", password="testpassword")
+        self.panSDK = PanoramaSDK(url="https://172.17.90.2", username="testuser", password="testpassword")
 
     def test_panorama_get_apikey(self):
         logging.debug(f"Erwarteter apikey: 'mock_apikey_12345'")
         logging.debug(f"Tatsächlicher apikey: '{self.panSDK.apikey}'")
         self.assertEqual(self.panSDK.apikey, "mock_apikey_12345")
```

