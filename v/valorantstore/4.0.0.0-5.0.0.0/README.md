# Comparing `tmp/valorantstore-4.0.0.0.tar.gz` & `tmp/valorantstore-5.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valorantstore-4.0.0.0.tar", last modified: Mon Aug 14 14:28:33 2023, max compression
+gzip compressed data, was "valorantstore-5.0.0.0.tar", last modified: Mon Apr 29 19:30:39 2024, max compression
```

## Comparing `valorantstore-4.0.0.0.tar` & `valorantstore-5.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-14 14:28:33.206626 valorantstore-4.0.0.0/
--rw-rw-rw-   0        0        0    18965 2023-08-14 14:28:33.206626 valorantstore-4.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    18457 2023-08-14 14:27:48.000000 valorantstore-4.0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-14 14:28:33.206626 valorantstore-4.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      883 2023-08-14 14:28:15.000000 valorantstore-4.0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-14 14:28:33.190831 valorantstore-4.0.0.0/valorantstore/
--rw-rw-rw-   0        0        0    13780 2023-08-14 14:27:07.000000 valorantstore-4.0.0.0/valorantstore/ValorantStore.py
--rw-rw-rw-   0        0        0      364 2023-08-14 14:17:39.000000 valorantstore-4.0.0.0/valorantstore/ValorantStoreException.py
--rw-rw-rw-   0        0        0      128 2023-08-14 14:17:39.000000 valorantstore-4.0.0.0/valorantstore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-14 14:28:33.206626 valorantstore-4.0.0.0/valorantstore.egg-info/
--rw-rw-rw-   0        0        0    18965 2023-08-14 14:28:33.000000 valorantstore-4.0.0.0/valorantstore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-08-14 14:28:33.000000 valorantstore-4.0.0.0/valorantstore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-14 14:28:33.000000 valorantstore-4.0.0.0/valorantstore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-14 14:28:33.000000 valorantstore-4.0.0.0/valorantstore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-14 14:28:33.000000 valorantstore-4.0.0.0/valorantstore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 19:30:39.085384 valorantstore-5.0.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-08-14 12:55:11.000000 valorantstore-5.0.0.0/LICENSE
+-rw-rw-rw-   0        0        0    19053 2024-04-29 19:30:39.084378 valorantstore-5.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18457 2024-04-29 19:18:21.000000 valorantstore-5.0.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 19:30:39.085384 valorantstore-5.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      912 2024-04-29 19:24:05.000000 valorantstore-5.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:30:39.074818 valorantstore-5.0.0.0/valorantstore/
+-rw-rw-rw-   0        0        0    14421 2024-04-29 19:24:05.000000 valorantstore-5.0.0.0/valorantstore/ValorantStore.py
+-rw-rw-rw-   0        0        0      364 2023-08-14 14:17:39.000000 valorantstore-5.0.0.0/valorantstore/ValorantStoreException.py
+-rw-rw-rw-   0        0        0      128 2023-08-14 14:17:39.000000 valorantstore-5.0.0.0/valorantstore/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:30:39.082882 valorantstore-5.0.0.0/valorantstore.egg-info/
+-rw-rw-rw-   0        0        0    19053 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 19:30:39.000000 valorantstore-5.0.0.0/valorantstore.egg-info/top_level.txt
```

### Comparing `valorantstore-4.0.0.0/PKG-INFO` & `valorantstore-5.0.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: valorantstore
-Version: 4.0.0.0
+Version: 5.0.0.0
 Summary: Python module to display your Valorant store
 Home-page: https://github.com/mahelbir/valorant-store
 Author: Mahmuthan Elbir
 Author-email: me@mahmuthanelbir.com.tr
 License: MIT
 Keywords: valorant store,valorant api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests~=2.28.2
+Requires-Dist: cfscrape~=2.1.1
 
 # Valorant Store
 
 Valorant Store that shows your store without running VALORANT by using unofficial In-game API
 
 ## Requirements
 
@@ -87,8 +90,8 @@
 ## Contributors
 
 Thanks to [@techchrism](https://valapidocs.techchrism.me)
 and [@Valorant-API](https://valorant-api.com), without them many parts of the API would be not available.
 
 ## License
 
-The MIT License (MIT). Please see [License File](LISENCE) for more information.
+The MIT License (MIT). Please see [License File](LICENSE) for more information.
```

### Comparing `valorantstore-4.0.0.0/README.md` & `valorantstore-5.0.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -72,8 +72,8 @@
 ## Contributors
 
 Thanks to [@techchrism](https://valapidocs.techchrism.me)
 and [@Valorant-API](https://valorant-api.com), without them many parts of the API would be not available.
 
 ## License
 
-The MIT License (MIT). Please see [License File](LISENCE) for more information.
+The MIT License (MIT). Please see [License File](LICENSE) for more information.
```

### Comparing `valorantstore-4.0.0.0/setup.py` & `valorantstore-5.0.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 pkg_name = "valorantstore"
 setuptools.setup(
     name=pkg_name,
-    version="4.0.0.0",
+    version="5.0.0.0",
     author="Mahmuthan Elbir",
     author_email="me@mahmuthanelbir.com.tr",
     description="Python module to display your Valorant store",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['valorant store', 'valorant api'],
     license="MIT",
@@ -19,11 +19,12 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=[pkg_name],
     include_package_data=True,
     install_requires=[
+        "requests~=2.28.2",
         "cfscrape~=2.1.1"
     ],
     python_requires=">=3.7"
 )
```

### Comparing `valorantstore-4.0.0.0/valorantstore/ValorantStore.py` & `valorantstore-5.0.0.0/valorantstore/ValorantStore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import base64
+import json
 import pickle
 from os import path, getcwd, remove, mkdir
 from time import time
 
 import cfscrape
 import requests
 
@@ -17,24 +19,33 @@
         self.__region = region
         self.__proxy = proxy
         self.__sess_path = sess_path if sess_path else getcwd()
         if not path.exists(self.__sess_path):
             mkdir(self.__sess_path)
         self.__auth_file = path.join(self.__sess_path, f"riot_auth_{self.__username}.pickle")
         self.__cookie_file = path.join(self.__sess_path, f"riot_cookie_{self.__username}.pickle")
+        self.client_platform = {
+            "platformType": "PC",
+            "platformOS": "Windows",
+            "platformOSVersion": "10.0.19042.1.256.64bit",
+            "platformChipset": "Unknown"
+        }
+        self.client_platform_base64 = base64.b64encode(json.dumps(self.client_platform, indent=4, separators=(',', ': ')).replace('    ', '\t').replace('\n', '\r\n').encode('utf-8')).decode('utf-8')
         if path.isfile(self.__auth_file) and time() - path.getmtime(self.__auth_file) < 3600:
             try:
                 with open(self.__auth_file, "rb") as auth:
                     self.__auth = pickle.load(auth)
             except Exception:
                 remove(self.__auth_file)
                 self.__login()
         else:
             self.__login()
         self.headers = {
+            "X-Riot-ClientPlatform": self.client_platform_base64,
+            "X-Riot-ClientVersion": requests.get("https://valorant-api.com/v1/version").json()['data']['riotClientVersion'],
             "X-Riot-Entitlements-JWT": self.__auth["entitlements_token"],
             "Authorization": "Bearer " + self.__auth["access_token"],
         }
         self.request = requests.session()
 
     @staticmethod
     def __get_access_token(url: str) -> str:
```

### Comparing `valorantstore-4.0.0.0/valorantstore.egg-info/PKG-INFO` & `valorantstore-5.0.0.0/valorantstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: valorantstore
-Version: 4.0.0.0
+Version: 5.0.0.0
 Summary: Python module to display your Valorant store
 Home-page: https://github.com/mahelbir/valorant-store
 Author: Mahmuthan Elbir
 Author-email: me@mahmuthanelbir.com.tr
 License: MIT
 Keywords: valorant store,valorant api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests~=2.28.2
+Requires-Dist: cfscrape~=2.1.1
 
 # Valorant Store
 
 Valorant Store that shows your store without running VALORANT by using unofficial In-game API
 
 ## Requirements
 
@@ -87,8 +90,8 @@
 ## Contributors
 
 Thanks to [@techchrism](https://valapidocs.techchrism.me)
 and [@Valorant-API](https://valorant-api.com), without them many parts of the API would be not available.
 
 ## License
 
-The MIT License (MIT). Please see [License File](LISENCE) for more information.
+The MIT License (MIT). Please see [License File](LICENSE) for more information.
```

