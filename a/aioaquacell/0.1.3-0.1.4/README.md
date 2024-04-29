# Comparing `tmp/aioaquacell-0.1.3.tar.gz` & `tmp/aioaquacell-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aioaquacell-0.1.3.tar", last modified: Tue Apr 23 18:43:43 2024, max compression
+gzip compressed data, was "dist\aioaquacell-0.1.4.tar", last modified: Mon Apr 29 20:31:41 2024, max compression
```

## Comparing `aioaquacell-0.1.3.tar` & `aioaquacell-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:43.353253 aioaquacell-0.1.3/
--rw-rw-rw-   0        0        0    11542 2023-09-29 19:48:26.000000 aioaquacell-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1262 2024-04-23 18:43:43.354253 aioaquacell-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-10-12 20:07:12.000000 aioaquacell-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:43.347254 aioaquacell-0.1.3/aioaquacell/
--rw-rw-rw-   0        0        0      149 2024-02-05 17:27:05.000000 aioaquacell-0.1.3/aioaquacell/__init__.py
--rw-rw-rw-   0        0        0     2934 2024-02-05 18:04:16.000000 aioaquacell-0.1.3/aioaquacell/aquacell_api.py
--rw-rw-rw-   0        0        0      297 2024-02-05 14:02:18.000000 aioaquacell-0.1.3/aioaquacell/authentication_tokens.py
--rw-rw-rw-   0        0        0     3465 2023-10-12 18:10:05.000000 aioaquacell-0.1.3/aioaquacell/aws_cognito_authenticator.py
--rw-rw-rw-   0        0        0      289 2023-09-27 20:13:49.000000 aioaquacell-0.1.3/aioaquacell/aws_credentials.py
--rw-rw-rw-   0        0        0     1106 2023-10-04 17:49:18.000000 aioaquacell-0.1.3/aioaquacell/aws_signature_request.py
--rw-rw-rw-   0        0        0      340 2024-02-05 14:20:59.000000 aioaquacell-0.1.3/aioaquacell/exceptions.py
--rw-rw-rw-   0        0        0     1771 2024-03-09 22:46:27.000000 aioaquacell-0.1.3/aioaquacell/softener.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:43.353253 aioaquacell-0.1.3/aioaquacell.egg-info/
--rw-rw-rw-   0        0        0     1262 2024-04-23 18:43:43.000000 aioaquacell-0.1.3/aioaquacell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2024-04-23 18:43:43.000000 aioaquacell-0.1.3/aioaquacell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:43:43.000000 aioaquacell-0.1.3/aioaquacell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-23 18:43:43.000000 aioaquacell-0.1.3/aioaquacell.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-23 18:43:43.000000 aioaquacell-0.1.3/aioaquacell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-23 18:43:43.355255 aioaquacell-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-04-23 18:43:31.000000 aioaquacell-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 20:31:41.201890 aioaquacell-0.1.4/
+-rw-rw-rw-   0        0        0    11542 2023-09-29 19:48:26.000000 aioaquacell-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1262 2024-04-29 20:31:41.201890 aioaquacell-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-10-12 20:07:12.000000 aioaquacell-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 20:31:41.196891 aioaquacell-0.1.4/aioaquacell/
+-rw-rw-rw-   0        0        0      149 2024-02-05 17:27:05.000000 aioaquacell-0.1.4/aioaquacell/__init__.py
+-rw-rw-rw-   0        0        0     2916 2024-04-29 20:30:36.000000 aioaquacell-0.1.4/aioaquacell/aquacell_api.py
+-rw-rw-rw-   0        0        0      297 2024-02-05 14:02:18.000000 aioaquacell-0.1.4/aioaquacell/authentication_tokens.py
+-rw-rw-rw-   0        0        0     3465 2023-10-12 18:10:05.000000 aioaquacell-0.1.4/aioaquacell/aws_cognito_authenticator.py
+-rw-rw-rw-   0        0        0      289 2023-09-27 20:13:49.000000 aioaquacell-0.1.4/aioaquacell/aws_credentials.py
+-rw-rw-rw-   0        0        0     1106 2023-10-04 17:49:18.000000 aioaquacell-0.1.4/aioaquacell/aws_signature_request.py
+-rw-rw-rw-   0        0        0      340 2024-02-05 14:20:59.000000 aioaquacell-0.1.4/aioaquacell/exceptions.py
+-rw-rw-rw-   0        0        0     1771 2024-03-09 22:46:27.000000 aioaquacell-0.1.4/aioaquacell/softener.py
+drwxrwxrwx   0        0        0        0 2024-04-29 20:31:41.201890 aioaquacell-0.1.4/aioaquacell.egg-info/
+-rw-rw-rw-   0        0        0     1262 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 20:31:41.000000 aioaquacell-0.1.4/aioaquacell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-29 20:31:41.202891 aioaquacell-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-04-29 20:30:49.000000 aioaquacell-0.1.4/setup.py
```

### Comparing `aioaquacell-0.1.3/LICENSE` & `aioaquacell-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.3/PKG-INFO` & `aioaquacell-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aioaquacell
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronous library to retrieve details of your Aquacell water softener device
 Home-page: https://github.com/Jordi1990/aioaquacell
-Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.4.tar.gz
 Author: Jordi Epema
 Author-email: jordi.epema@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aioaquacell
```

### Comparing `aioaquacell-0.1.3/README.md` & `aioaquacell-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.3/aioaquacell/aquacell_api.py` & `aioaquacell-0.1.4/aioaquacell/aquacell_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Parses data from the Aquacell API. """
 import json
+import string
 
 import botocore
 from aiohttp import ClientSession
 
 from aioaquacell.aws_cognito_authenticator import AwsCognitoAuthenticator
 from aioaquacell.aws_signature_request import AwsSignatureRequest
 from aioaquacell.exceptions import NotAuthenticated, ApiException, AuthenticationFailed
@@ -17,36 +18,35 @@
     client_id = "64kp67l1jo9toeesan7s1sdpae"
     pool_id = "eu-west-1_noZbcE2Av"
     identity_pool_id = "eu-west-1:f44120d5-bd20-4461-b282-1ed637861951"
 
     def __init__(self, session: ClientSession):
         self.session = session
         self.id_token = None
-        self.refresh_token = None
         self.authenticator = AwsCognitoAuthenticator(
             self.region_name, self.client_id, self.pool_id, self.identity_pool_id
         )
 
     """ Authenticate using a previous obtained refresh token. """
-    async def authenticate_refresh(self, refresh_token) -> None:
-        await self.__authenticate(None, None, refresh_token)
+    async def authenticate_refresh(self, refresh_token) -> string:
+        return await self.__authenticate(None, None, refresh_token)
 
     """" Authenticate using username and password. """
-    async def authenticate(self, user_name, password) -> None:
-        await self.__authenticate(user_name, password, None)
+    async def authenticate(self, user_name, password) -> string:
+        return await self.__authenticate(user_name, password, None)
 
-    async def __authenticate(self, user_name, password, refresh_token) -> None:
+    async def __authenticate(self, user_name, password, refresh_token) -> string:
         try:
             if refresh_token is None:
                 token = await self.authenticator.get_new_token(user_name, password)
-                self.refresh_token = token.refresh_token
             else:
                 token = await self.authenticator.refresh_token(refresh_token)
 
             self.id_token = token.id_token
+            return token.refresh_token
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == 'NotAuthorizedException':
                 raise AuthenticationFailed(e)
             else:
                 raise ApiException(e)
 
     async def get_all_softeners(self) -> list[Softener]:
```

### Comparing `aioaquacell-0.1.3/aioaquacell/aws_cognito_authenticator.py` & `aioaquacell-0.1.4/aioaquacell/aws_cognito_authenticator.py`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.3/aioaquacell/aws_signature_request.py` & `aioaquacell-0.1.4/aioaquacell/aws_signature_request.py`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.3/aioaquacell/softener.py` & `aioaquacell-0.1.4/aioaquacell/softener.py`

 * *Files identical despite different names*

### Comparing `aioaquacell-0.1.3/aioaquacell.egg-info/PKG-INFO` & `aioaquacell-0.1.4/aioaquacell.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aioaquacell
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronous library to retrieve details of your Aquacell water softener device
 Home-page: https://github.com/Jordi1990/aioaquacell
-Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.4.tar.gz
 Author: Jordi Epema
 Author-email: jordi.epema@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Aioaquacell
```

### Comparing `aioaquacell-0.1.3/setup.py` & `aioaquacell-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 setup(
     name="aioaquacell",
     version=VERSION,
     packages=["aioaquacell"],
     install_requires=[
         "aiohttp",
@@ -20,9 +20,9 @@
     url="https://github.com/Jordi1990/aioaquacell",
     license="Apache License 2.0",
     author="Jordi Epema",
     author_email="jordi.epema@gmail.com",
     description="Asynchronous library to retrieve details of your Aquacell water softener device",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
-    download_url="https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.3.tar.gz",
+    download_url="https://github.com/Jordi1990/aioaquacell/archive/refs/tags/v0.1.4.tar.gz",
 )
```

