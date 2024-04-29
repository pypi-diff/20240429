# Comparing `tmp/exponent_server_sdk_async-2.1.2.tar.gz` & `tmp/exponent_server_sdk_async-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponent_server_sdk_async-2.1.2.tar", last modified: Mon Apr 29 12:30:34 2024, max compression
+gzip compressed data, was "exponent_server_sdk_async-2.1.3.tar", last modified: Mon Apr 29 12:56:27 2024, max compression
```

## Comparing `exponent_server_sdk_async-2.1.2.tar` & `exponent_server_sdk_async-2.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-04-29 10:49:11.229618 exponent_server_sdk_async-2.1.2/LICENSE
--rw-r--r--   0        0        0     2291 2024-04-29 12:28:48.734311 exponent_server_sdk_async-2.1.2/README.md
--rw-r--r--   0        0        0    15289 2024-04-29 11:13:38.470683 exponent_server_sdk_async-2.1.2/exponent_server_sdk_async/__init__.py
--rw-r--r--   0        0        0     6324 2024-04-29 12:29:26.655397 exponent_server_sdk_async-2.1.2/exponent_server_sdk_async/debug.log
--rw-r--r--   0        0        0     1654 2024-04-29 12:29:26.451811 exponent_server_sdk_async-2.1.2/exponent_server_sdk_async/main.py
--rw-r--r--   0        0        0      724 2024-04-29 12:30:34.955946 exponent_server_sdk_async-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 exponent_server_sdk_async-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-29 10:49:11.229618 exponent_server_sdk_async-2.1.3/LICENSE
+-rw-r--r--   0        0        0     2195 2024-04-29 12:51:36.626710 exponent_server_sdk_async-2.1.3/README.md
+-rw-r--r--   0        0        0    15289 2024-04-29 11:13:38.470683 exponent_server_sdk_async-2.1.3/exponent_server_sdk_async/__init__.py
+-rw-r--r--   0        0        0     6324 2024-04-29 12:29:26.655397 exponent_server_sdk_async-2.1.3/exponent_server_sdk_async/debug.log
+-rw-r--r--   0        0        0     1654 2024-04-29 12:29:26.451811 exponent_server_sdk_async-2.1.3/exponent_server_sdk_async/main.py
+-rw-r--r--   0        0        0      724 2024-04-29 12:56:27.012509 exponent_server_sdk_async-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 exponent_server_sdk_async-2.1.3/PKG-INFO
```

### Comparing `exponent_server_sdk_async-2.1.2/LICENSE` & `exponent_server_sdk_async-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.2/README.md` & `exponent_server_sdk_async-2.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-# exponent-server-sdk-python
+# exponent-server-sdk-python-async
 
-This repo is maintained by Expo's awesome community :heart_eyes:! So, if you have problems with the code in this repository, please feel free to open an issue, and make a PR. Thanks!
+This repo is made for the async version of the [exponent-server-sdk-python](https://github.com/expo-community/expo-server-sdk-python) made by [Bahadır Araz](https://github.com/bahadiraraz).
 
 ## Installation
 
 ```
-pip install exponent_server_sdk
+pip install exponent-server-sdk-async==2.1.2
 ```
 
 ## Usage
-
 Use to send push notifications to Exponent Experiences from a Python server.
-
 [Full documentation](https://docs.expo.dev/push-notifications/sending-notifications/#http2-api) on the API is available if you want to dive into the details.
-
-Here's an example on how to use this with retries and reporting via [pyrollbar](https://github.com/rollbar/pyrollbar).
-
 ```python
 import os
 import httpx
 from httpx import HTTPError, NetworkError
 from loguru import logger
 from dotenv import load_dotenv
 from exponent_server_sdk_async import (
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exponent_server_sdk_async-2.1.2/exponent_server_sdk_async/__init__.py` & `exponent_server_sdk_async-2.1.3/exponent_server_sdk_async/__init__.py`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.2/exponent_server_sdk_async/debug.log` & `exponent_server_sdk_async-2.1.3/exponent_server_sdk_async/debug.log`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.2/exponent_server_sdk_async/main.py` & `exponent_server_sdk_async-2.1.3/exponent_server_sdk_async/main.py`

 * *Files identical despite different names*

### Comparing `exponent_server_sdk_async-2.1.2/pyproject.toml` & `exponent_server_sdk_async-2.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "exponent_server_sdk_async"
-version = "2.1.2"
+version = "2.1.3"
 description = "Expo Server SDK for Python async"
 authors = [
     { name = "Bahadır Araz", email = "bahadiraraz@protonmail.com" },
     { name = "Expo Team", email = "exponent.team@gmail.com" },
 ]
 dependencies = [
     "setuptools>=69.5.1",
```

### Comparing `exponent_server_sdk_async-2.1.2/PKG-INFO` & `exponent_server_sdk_async-2.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponent_server_sdk_async
-Version: 2.1.2
+Version: 2.1.3
 Summary: Expo Server SDK for Python async
 Author-Email: =?utf-8?q?Bahad=C4=B1r_Araz?= <bahadiraraz@protonmail.com>, Expo Team <exponent.team@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/expo/exponent-server-sdk-python
 Requires-Python: >=3.12
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: requests
@@ -12,32 +12,27 @@
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: pytest>=8.2.0
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: pytest-asyncio>=0.23.6
 Description-Content-Type: text/markdown
 
-# exponent-server-sdk-python
+# exponent-server-sdk-python-async
 
-This repo is maintained by Expo's awesome community :heart_eyes:! So, if you have problems with the code in this repository, please feel free to open an issue, and make a PR. Thanks!
+This repo is made for the async version of the [exponent-server-sdk-python](https://github.com/expo-community/expo-server-sdk-python) made by [Bahadır Araz](https://github.com/bahadiraraz).
 
 ## Installation
 
 ```
-pip install exponent_server_sdk
+pip install exponent-server-sdk-async==2.1.2
 ```
 
 ## Usage
-
 Use to send push notifications to Exponent Experiences from a Python server.
-
 [Full documentation](https://docs.expo.dev/push-notifications/sending-notifications/#http2-api) on the API is available if you want to dive into the details.
-
-Here's an example on how to use this with retries and reporting via [pyrollbar](https://github.com/rollbar/pyrollbar).
-
 ```python
 import os
 import httpx
 from httpx import HTTPError, NetworkError
 from loguru import logger
 from dotenv import load_dotenv
 from exponent_server_sdk_async import (
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

