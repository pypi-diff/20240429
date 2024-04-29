# Comparing `tmp/paloalto_panorama_sdk-0.0.2.tar.gz` & `tmp/paloalto_panorama_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paloalto_panorama_sdk-0.0.2.tar", last modified: Mon Apr 29 13:30:35 2024, max compression
+gzip compressed data, was "paloalto_panorama_sdk-0.0.3.tar", last modified: Mon Apr 29 13:33:16 2024, max compression
```

## Comparing `paloalto_panorama_sdk-0.0.2.tar` & `paloalto_panorama_sdk-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.157144 paloalto_panorama_sdk-0.0.2/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.2/LICENSE
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.2/MANIFEST.in
--rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 13:30:35.156736 paloalto_panorama_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:54:18.000000 paloalto_panorama_sdk-0.0.2/README.md
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.138686 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      110 2024-04-29 13:30:30.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/key_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      828 2024-04-29 13:30:14.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/panorama_sdk.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     3515 2024-04-29 05:08:50.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/post_rules_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.148961 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)      708 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/requires.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-04-29 13:30:34.000000 paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/top_level.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-04-29 13:30:35.157235 paloalto_panorama_sdk-0.0.2/setup.cfg
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.2/setup.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.150076 paloalto_panorama_sdk-0.0.2/tests/
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:30:35.156211 paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/panoramaAPIMock.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.2/tests/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.2/tests/test_service.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:33:16.070052 paloalto_panorama_sdk-0.0.3/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.3/LICENSE
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.3/MANIFEST.in
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 13:33:16.069853 paloalto_panorama_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:54:18.000000 paloalto_panorama_sdk-0.0.3/README.md
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:33:16.057223 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      110 2024-04-29 13:33:12.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/address_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/address_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/key_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      847 2024-04-29 13:32:58.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/panorama_sdk.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     3515 2024-04-29 05:08:50.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/post_rules_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/service_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/service_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:33:16.068196 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      344 2024-04-29 13:33:16.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      708 2024-04-29 13:33:16.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-04-29 13:33:16.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-04-29 13:33:16.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/requires.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-04-29 13:33:16.000000 paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/top_level.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-04-29 13:33:16.070091 paloalto_panorama_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.3/setup.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:33:16.068795 paloalto_panorama_sdk-0.0.3/tests/
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-29 13:33:16.069454 paloalto_panorama_sdk-0.0.3/tests/PanoramaAPIMock/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.3/tests/PanoramaAPIMock/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.3/tests/PanoramaAPIMock/panoramaAPIMock.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.3/tests/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.3/tests/test_service.py
```

### Comparing `paloalto_panorama_sdk-0.0.2/LICENSE` & `paloalto_panorama_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_groups_manager.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/address_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/address_manager.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/address_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/key_manager.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/key_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/panorama_sdk.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/panorama_sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.password = password
         self.apikey = KeyManager.get_api_key(
             panorama_url=self.url,
             user=self.username,
             password=self.password,
             verify=verify
         )
-        self.service = ServiceManager(self.url, self.username, self.password)
+        self.service = ServiceManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
 
 
 if __name__ == '__main__':
     panSDK = PanoramaSDK(
         url=os.getenv("url", ""),
         username=os.getenv("user", "test"),
         password=os.getenv("password", "testpass")
```

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/post_rules_manager.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/post_rules_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_groups_manager.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/service_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk/service_manager.py` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk/service_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/SOURCES.txt` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/paloalto_panorama_sdk.egg-info/requires.txt` & `paloalto_panorama_sdk-0.0.3/paloalto_panorama_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/setup.py` & `paloalto_panorama_sdk-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/tests/PanoramaAPIMock/panoramaAPIMock.py` & `paloalto_panorama_sdk-0.0.3/tests/PanoramaAPIMock/panoramaAPIMock.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.2/tests/test_service.py` & `paloalto_panorama_sdk-0.0.3/tests/test_service.py`

 * *Files identical despite different names*

