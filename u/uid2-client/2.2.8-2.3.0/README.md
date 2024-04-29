# Comparing `tmp/uid2_client-2.2.8.tar.gz` & `tmp/uid2_client-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-2.2.8.tar", last modified: Mon Mar 11 23:07:55 2024, max compression
+gzip compressed data, was "uid2_client-2.3.0.tar", last modified: Mon Apr 29 21:20:17 2024, max compression
```

## Comparing `uid2_client-2.2.8.tar` & `uid2_client-2.3.0.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:07:55.076869 uid2_client-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-03-11 23:07:32.000000 uid2_client-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-11 23:07:55.076869 uid2_client-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-11 23:07:32.000000 uid2_client-2.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-11 23:07:49.000000 uid2_client-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-11 23:07:55.080869 uid2_client-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-11 23:07:32.000000 uid2_client-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:07:55.072869 uid2_client-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29296 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_key_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_publisher_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-11 23:07:32.000000 uid2_client-2.2.8/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:07:55.076869 uid2_client-2.2.8/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17717 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/euid_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/identity_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/input_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/publisher_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/request_response_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/token_generate_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/token_generate_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/token_refresh_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/uid2_base64_url_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-11 23:07:32.000000 uid2_client-2.2.8/uid2_client/uid2_client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:07:55.076869 uid2_client-2.2.8/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-11 23:07:55.000000 uid2_client-2.2.8/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-11 23:07:55.000000 uid2_client-2.2.8/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 23:07:55.000000 uid2_client-2.2.8/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-11 23:07:55.000000 uid2_client-2.2.8/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-11 23:07:55.000000 uid2_client-2.2.8/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 23:07:54.000000 uid2_client-2.2.8/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.123012 uid2_client-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-29 21:19:55.000000 uid2_client-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 21:20:17.123012 uid2_client-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-29 21:19:55.000000 uid2_client-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-29 21:20:11.000000 uid2_client-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-29 21:20:17.123012 uid2_client-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 21:19:55.000000 uid2_client-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.115012 uid2_client-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_bidstream_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_publisher_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_refresh_keys_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_sharing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.119012 uid2_client-2.3.0/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/bidstream_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/client_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/decryption_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/encryption_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/encryption_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/euid_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/identity_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/input_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/publisher_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/refresh_keys_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/request_response_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/sharing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/token_generate_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/token_generate_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/token_refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/uid2_base64_url_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/uid2_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/uid2_token_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.123012 uid2_client-2.3.0/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:20:16.000000 uid2_client-2.3.0/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-2.2.8/LICENSE` & `uid2_client-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/PKG-INFO` & `uid2_client-2.3.0/uid2_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uid2_client
-Version: 2.2.8
+Name: uid2-client
+Version: 2.3.0
 Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
@@ -83,15 +83,16 @@
 ### Example Usage
 
 To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A== \
-	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE=
+	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE= \
+	DOMAIN=example.com
 ```
 
 Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
```

### Comparing `uid2_client-2.2.8/README.md` & `uid2_client-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 ### Example Usage
 
 To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A== \
-	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE=
+	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE= \
+	DOMAIN=example.com
 ```
 
 Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
```

### Comparing `uid2_client-2.2.8/pyproject.toml` & `uid2_client-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools == 68.2.2",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "2.2.8"
+version = "2.3.0"
 authors = [
     { name = "UID2 team", email = "unifiedid-admin@thetradedesk.com" }
 ]
 description = "UID2 SDK for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `uid2_client-2.2.8/setup.cfg` & `uid2_client-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/tests/test_encryption.py` & `uid2_client-2.3.0/tests/test_encryption.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import unittest
 
-from tests.uid2_token_generator import UID2TokenGenerator, Params
+from test_utils import *
 from uid2_client import *
-from uid2_client.encryption import _encrypt_token
-from uid2_client.identity_scope import IdentityScope
-from uid2_client.identity_type import IdentityType
-from uid2_client.keys import *
 
 _master_secret = bytes([139, 37, 241, 173, 18, 92, 36, 232, 165, 168, 23, 18, 38, 195, 123, 92, 160, 136, 185, 40, 91, 173, 165, 221, 168, 16, 169, 164, 38, 139, 8, 155])
 _site_secret =   bytes([32, 251, 7, 194, 132, 154, 250, 86, 202, 116, 104, 29, 131, 192, 139, 215, 48, 164, 11, 65, 226, 110, 167, 14, 108, 51, 254, 125, 65, 24, 23, 133])
 _master_key_id = 164
 _site_key_id = 165
 _test_site_key_id = 166
 _site_id = 9000
@@ -18,14 +14,15 @@
 _example_id = 'ywsvDNINiZOVSsfkHpLpSJzXzhr6Jx9Z/4Q0+lsEUvM='
 _now = dt.datetime.now(tz=timezone.utc)
 _master_key = EncryptionKey(_master_key_id, -1, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _master_secret, keyset_id=9999)
 _site_key = EncryptionKey(_site_key_id, _site_id, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _site_secret)
 _keyset_key = EncryptionKey(_site_key_id, _site_id, _now - dt.timedelta(days=-1), _now, _now + dt.timedelta(days=1), _site_secret, keyset_id=20)
 _test_site_key = EncryptionKey(_test_site_key_id, _site_id, dt.datetime(2020, 1, 1, tzinfo=timezone.utc), dt.datetime(2020, 1, 1, tzinfo=timezone.utc), _now + dt.timedelta(days=1), encryption_block_size * b'9')
 
+
 class TestEncryptionFunctions(unittest.TestCase):
 
     def test_cross_platform_consistency_check_base64_url_test_cases(self):
         case1 = bytes([ 0xff, 0xE0, 0x88, 0xFF, 0xEE, 0x99, 0x99])
         # the Base64 equivalent is "/+CI/+6ZmQ=="
         # and we want the Base64URL encoded to remove 2 '=' paddings at the back
         self.cross_platform_consistency_check_base64_url_test(case1, "_-CI_-6ZmQ")
@@ -42,31 +39,43 @@
     def cross_platform_consistency_check_base64_url_test(self, raw_input, expected_base64_url_str):
         base64_url_encoded_str = Uid2Base64UrlCoder.encode(raw_input)
         self.assertEqual(expected_base64_url_str, base64_url_encoded_str)
 
         decoded = Uid2Base64UrlCoder.decode(base64_url_encoded_str)
         self.assertEqual(decoded, raw_input)
 
-    def validate_advertising_token(self, advertising_token_string, identity_scope, identity_type):
+    def validate_advertising_token(self, advertising_token_string, identity_scope, identity_type,
+                                   token_version=AdvertisingTokenVersion.ADVERTISING_TOKEN_V4):
+
+        if token_version == AdvertisingTokenVersion.ADVERTISING_TOKEN_V2:
+            self.assertEqual("A", advertising_token_string[0])
+            self.assertEqual("g", advertising_token_string[1])
+            return
+
         first_char = advertising_token_string[0]
         if identity_scope == IdentityScope.UID2:
             self.assertEqual("A" if identity_type == IdentityType.Email.value else "B", first_char)
         else:
             self.assertEqual("E" if identity_type == IdentityType.Email.value else "F", first_char)
 
         second_char = advertising_token_string[1]
-        self.assertEqual("4", second_char)
-
-        # No URL-unfriendly characters allowed
-        self.assertEqual(-1, advertising_token_string.find("="))
-        self.assertEqual(-1, advertising_token_string.find("+"))
-        self.assertEqual(-1, advertising_token_string.find("/"))
+        if token_version == AdvertisingTokenVersion.ADVERTISING_TOKEN_V3:
+            self.assertEqual("3", second_char)
+            return
+        else:
+            self.assertEqual("4", second_char)
 
+            # No URL-unfriendly characters allowed
+            self.assertEqual(-1, advertising_token_string.find("="))
+            self.assertEqual(-1, advertising_token_string.find("+"))
+            self.assertEqual(-1, advertising_token_string.find("/"))
 
     def generate_uid2_token_v4(self, uid, master_key, site_id, site_key, params = Params(), identity_type = IdentityType.Email, identity_scope = IdentityScope.UID2):
+        if not isinstance(params.token_expiry, dt.datetime):
+            params.token_expiry = dt.datetime.now(tz=timezone.utc) + params.token_expiry
         advertising_token = UID2TokenGenerator.generate_uid2_token_v4(uid, master_key, site_id, site_key, params)
         self.validate_advertising_token(advertising_token, identity_scope, identity_type)
         return advertising_token
 
 
     def test_cross_platform_consistency_decrypt(self):
         crossPlatformAdvertisingToken = "AIAAAACkOqJj9VoxXJNnuX3v-ymceRf8_Av0vA5asOj9YBZJc1kV1vHdmb0AIjlzWnFF-gxIlgXqhRFhPo3iXpugPBl3gv4GKnGkw-Zgm2QqMsDPPLpMCYiWrIUqHPm8hQiq9PuTU-Ba9xecRsSIAN0WCwKLwA_EDVdzmnLJu64dQoeYmuu3u1G2EuTkuMrevmP98tJqSUePKwnfK73-0Zdshw";
@@ -101,28 +110,28 @@
         runtime_advertising_token = self.generate_uid2_token_v4(_example_id, master_key, _site_id, site_key, params)
         # best effort check as the token might simply just not require padding
         self.assertEqual(-1, runtime_advertising_token.find('='))
         self.assertEqual(-1, runtime_advertising_token.find('+'))
         self.assertEqual(-1, runtime_advertising_token.find('/'))
 
         result = decrypt(runtime_advertising_token, EncryptionKeysCollection([_master_key, _site_key]))
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
         # can also decrypt a known token generated from other SDK
         result = decrypt(crossPlatformAdvertisingToken, EncryptionKeysCollection([_master_key, _site_key]))
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
 
     def test_decrypt_token_v4(self):
         token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
         result = decrypt(token, keys)
 
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
 
     def test_decrypt_token_v4_empty_keys(self):
         token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
@@ -144,15 +153,15 @@
 
         keys = EncryptionKeysCollection([_master_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
     def test_decrypt_token_v4_invalid_version(self):
-        params = Params(dt.timedelta(hours=1))
+        params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(hours=1))
         token = UID2TokenGenerator.generate_uid2_token_with_debug_info(_example_id, _master_key, _site_id, _site_key, params, 1)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
@@ -162,27 +171,91 @@
         token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
+    def _generate_v2_token(self, expires_in_seconds):
+        return UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key,
+                                                         Params(dt.datetime.now(tz=timezone.utc) + expires_in_seconds))
+
+    def _generate_v4_token(self, expires_in_seconds):
+        return self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, Params(expires_in_seconds))
+
+    def test_decrypt_token_2_invalid_lifetime_exception(self):
+        test_cases = [
+            # expires 30s AFTER max
+            [self._generate_v2_token(dt.timedelta(seconds=60)), 30, 3600, ClientType.BIDSTREAM],
+            [self._generate_v4_token(dt.timedelta(seconds=60)), 30, 3600, ClientType.BIDSTREAM],
+            [self._generate_v2_token(dt.timedelta(seconds=60)), 3600, 30, ClientType.SHARING],
+            [self._generate_v4_token(dt.timedelta(seconds=60)), 3600, 30, ClientType.SHARING],
+            # expires 1s AFTER max
+            [self._generate_v2_token(dt.timedelta(seconds=60)), 59, 3600, ClientType.BIDSTREAM],
+            [self._generate_v4_token(dt.timedelta(seconds=60)), 59, 3600, ClientType.BIDSTREAM],
+            [self._generate_v2_token(dt.timedelta(seconds=60)), 3600, 59, ClientType.SHARING],
+            [self._generate_v4_token(dt.timedelta(seconds=60)), 3600, 59, ClientType.SHARING],
+            # expires 1 day AFTER max
+            [self._generate_v2_token(dt.timedelta(days=3)), dt.timedelta(days=2).seconds, dt.timedelta(days=4).seconds,
+             ClientType.BIDSTREAM],
+            [self._generate_v4_token(dt.timedelta(days=3)), dt.timedelta(days=2).seconds,
+             dt.timedelta(days=4).seconds, ClientType.BIDSTREAM],
+            [self._generate_v2_token(dt.timedelta(days=3)), dt.timedelta(days=4).seconds, dt.timedelta(days=2).seconds,
+             ClientType.SHARING],
+            [self._generate_v4_token(dt.timedelta(days=3)), dt.timedelta(days=4).seconds,
+             dt.timedelta(days=2).seconds, ClientType.SHARING]
+        ]
+        for token, max_bidstream_lifetime_seconds, max_sharing_lifetime_seconds, client_type in test_cases:
+            with self.subTest(token=token,
+                              max_bidstream_lifetime_seconds=max_bidstream_lifetime_seconds,
+                              max_sharing_lifetime_seconds=max_sharing_lifetime_seconds, client_type=client_type):
+                key_collection = EncryptionKeysCollection([_master_key, _site_key], IdentityScope.UID2, None, None,
+                                                          None, None,
+                                                          max_sharing_lifetime_seconds, max_bidstream_lifetime_seconds,
+                                                          None)
+                decrypted_token = decrypt_token(token, key_collection, "", client_type)
+                self.assertEqual(decrypted_token.status, DecryptionStatus.INVALID_TOKEN_LIFETIME)
+
+    def test_decrypt_token_invalid_lifetime_pass(self):
+        seconds_since_established = 3600  # from UID2TokenGenerator.generate_uid2_token_v4
+        test_cases = [
+            # expires 30s before max
+            [self._generate_v2_token(dt.timedelta(seconds=30)), seconds_since_established + 60, 60, ClientType.BIDSTREAM],
+            [self._generate_v4_token(dt.timedelta(seconds=30)), seconds_since_established + 60, 60, ClientType.BIDSTREAM],
+            [self._generate_v2_token(dt.timedelta(seconds=30)), 30, seconds_since_established + 30, ClientType.SHARING],
+            [self._generate_v4_token(dt.timedelta(seconds=30)), 30, seconds_since_established + 30, ClientType.SHARING],
+            # expires exactly at max
+            [self._generate_v2_token(dt.timedelta(seconds=30)), seconds_since_established + 30, 30, ClientType.BIDSTREAM],
+            [self._generate_v4_token(dt.timedelta(seconds=30)), seconds_since_established + 30, 30, ClientType.BIDSTREAM],
+            [self._generate_v2_token(dt.timedelta(seconds=30)), 60, seconds_since_established + 60, ClientType.SHARING],
+            [self._generate_v4_token(dt.timedelta(seconds=30)), 60, seconds_since_established + 60, ClientType.SHARING]
+        ]
+        for token, max_bidstream_lifetime_seconds, max_sharing_lifetime_seconds, client_type in test_cases:
+            with self.subTest(token=token,
+                              max_bidstream_lifetime_seconds=max_bidstream_lifetime_seconds,
+                              max_sharing_lifetime_seconds=max_sharing_lifetime_seconds, client_type=client_type):
+
+                key_collection = EncryptionKeysCollection([_master_key, _site_key], IdentityScope.UID2, None, None,
+                                                          None, None,
+                                                          max_sharing_lifetime_seconds, max_bidstream_lifetime_seconds,
+                                                          None)
+                decrypt_token(token, key_collection, "", client_type)
 
     def test_decrypt_token_v4_custom_now(self):
         expiry = dt.datetime(2021, 3, 22, 9, 1, 2, tzinfo=timezone.utc)
         params = Params(expiry)
         token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
         result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
 
     def test_decrypt_token_v4_invalid_payload(self):
         params = Params(dt.timedelta(seconds=-1))
         token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
@@ -193,15 +266,15 @@
 
     def test_decrypt_token_v3(self):
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
         result = decrypt(token, keys)
 
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
 
     def test_decrypt_token_v3_empty_keys(self):
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
@@ -223,25 +296,25 @@
 
         keys = EncryptionKeysCollection([_master_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
     def test_decrypt_token_v3_invalid_version(self):
-        params = Params(dt.timedelta(hours=1))
+        params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(hours=1))
         token = UID2TokenGenerator.generate_uid2_token_with_debug_info(_example_id, _master_key, _site_id, _site_key, params, 1)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
 
     def test_decrypt_token_v3_expired(self):
-        params = Params(dt.timedelta(seconds=-1))
+        params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
@@ -253,34 +326,34 @@
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
         result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
 
     def test_decrypt_token_v3_invalid_payload(self):
-        params = Params(dt.timedelta(seconds=-1))
+        params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v3(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token[:-3], keys)
 
 
     def test_decrypt_token_v2(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
         result = decrypt(token, keys)
 
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
 
     def test_decrypt_token_v2_empty_keys(self):
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
@@ -332,44 +405,43 @@
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
         result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
-        self.assertEqual(_example_id, result.uid2)
+        self.assertEqual(_example_id, result.uid)
 
     def test_smoke_token_v3(self):
         uid2 = _example_id
         identity_scope = IdentityScope.UID2
         now = dt.datetime.now(tz=timezone.utc)
 
         keys = EncryptionKeysCollection([_master_key, _site_key, _keyset_key], default_keyset_id=20,
                                         master_keyset_id=9999, caller_site_id=20)
-
-        result = _encrypt_token(uid2, identity_scope, _master_key, _site_key, _site_id, now=now,
-                                token_expiry=now + dt.timedelta(days=30) if keys.get_token_expiry_seconds() is None \
-                                    else now + dt.timedelta(seconds=int(keys.get_token_expiry_seconds())),
-                         ad_token_version=AdvertisingTokenVersion.ADVERTISING_TOKEN_V3)
+        token_expiry = now + dt.timedelta(days=30) if keys.get_token_expiry_seconds() is None \
+            else now + dt.timedelta(seconds=int(keys.get_token_expiry_seconds()))
+        result = UID2TokenGenerator.generate_uid2_token_v3(uid2, _master_key, _site_id, _site_key,
+                                                           Params(expiry=token_expiry, token_generated=now))
         final = decrypt(result, keys, now=now)
 
-        self.assertEqual(uid2, final.uid2)
+        self.assertEqual(uid2, final.uid)
 
     def test_smoke_token_v4(self):
         uid2 = _example_id
         identity_scope = IdentityScope.UID2
         now = dt.datetime.now(tz=timezone.utc)
 
         keys = EncryptionKeysCollection([_master_key, _site_key, _keyset_key], default_keyset_id=20,
                                         master_keyset_id=9999, caller_site_id=20)
 
         result = encrypt(uid2, identity_scope, keys, now=now)
-        final = decrypt(result, keys, now=now)
+        final = decrypt(result.encrypted_data, keys, now=now)
 
-        self.assertEqual(uid2, final.uid2)
+        self.assertEqual(uid2, final.uid)
 
     def test_decrypt_token_v2_invalid_payload(self):
         params = Params(dt.datetime.now(tz=timezone.utc) + dt.timedelta(seconds=-1))
         token = UID2TokenGenerator.generate_uid2_token_v2(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
@@ -634,23 +706,14 @@
         self.verify_identity_type("EKCoNGWPYng/whjBIwANJHKvvGlGyzARtDIAk95FlJyb",
                                                       IdentityType.Email.value) #v3 EUID test@example.com
 
     def verify_identity_type(self, raw_uid, expected_identity_type):
         token = self.generate_uid2_token_v4(raw_uid, _master_key, _site_id, _site_key, Params(), expected_identity_type)
         keys = EncryptionKeysCollection([_master_key, _site_key])
         result = decrypt(token, keys)
-        self.assertEqual(raw_uid, result.uid2)
-        self.assertEqual(expected_identity_type, get_token_identity_type(token))
-
-
-def get_token_identity_type(id):
-    firstChar = id[0]
-    if 'A' == firstChar or 'E' == firstChar: #from UID2-79+Token+ and +ID+format+v3
-        return IdentityType.Email.value
-    elif 'F' == firstChar or 'B' == firstChar:
-        return IdentityType.Phone.value
+        self.assertEqual(raw_uid, result.uid)
+        self.assertEqual(expected_identity_type, get_identity_type(token))
 
-    raise Exception("unknown IdentityType")
 
 def format_time(t):
     s = t.strftime('%Y-%m-%d %H:%M:%S.%f')
     return s[:-3]
```

### Comparing `uid2_client-2.2.8/tests/test_key_parse.py` & `uid2_client-2.3.0/tests/test_key_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def _make_dt(timestamp):
     return dt.datetime.fromtimestamp(timestamp, tz=dt.timezone.utc)
 
 
 class TestKeyParse(unittest.TestCase):
     def test_key_parse(self):
         s = "{ \"body\": { " + \
+            "\"identity_scope\": \"UID2\", " + \
             "\"caller_site_id\": 11, " + \
             "\"master_keyset_id\": 1, " + \
             "\"default_keyset_id\": 99999, " + \
             "\"token_expiry_seconds\": 1728000, " + \
             "\"keys\": [ " + \
             "{ " + \
             "\"id\": 3, " + \
```

### Comparing `uid2_client-2.2.8/tests/test_keys.py` & `uid2_client-2.3.0/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/tests/test_normalization.py` & `uid2_client-2.3.0/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/tests/test_publisher_client.py` & `uid2_client-2.3.0/tests/test_publisher_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/__init__.py` & `uid2_client-2.3.0/uid2_client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,9 +13,16 @@
 from .encryption import *
 from .keys import *
 from .euid_client_factory import *
 from .uid2_client_factory import *
 from .token_generate_input import *
 from .token_generate_response import *
 from .publisher_client import *
+from .bidstream_client import *
+from .sharing_client import *
+from .decryption_status import *
+from .encryption_status import *
+from .encryption_data_response import *
+from .refresh_response import *
+from .uid2_token_generator import *
```

### Comparing `uid2_client-2.2.8/uid2_client/auto_refresh.py` & `uid2_client-2.3.0/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/identity_tokens.py` & `uid2_client-2.3.0/uid2_client/identity_tokens.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/input_util.py` & `uid2_client-2.3.0/uid2_client/input_util.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/keys.py` & `uid2_client-2.3.0/uid2_client/keys.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 Do not use this module directly, import from uid2_client instead, e.g.
 >>> from uid2_client import EncryptionKeysCollection
 """
 
 
 import datetime as dt
+import sys
 from bisect import bisect_right, bisect_left
+from .identity_scope import IdentityScope
 
 
 class EncryptionKey:
     """Wrapper class for keeping data about an encryption key.
 
     Attrs:
         key_id (int): identifier of the key
@@ -96,24 +98,37 @@
 class EncryptionKeysCollection:
     """A collection of EncryptionKey objects.
 
     This is a dictionary like immutable collection object containing encryption keys
     used for decoding UID2 advertising tokens.
     """
 
-    def __init__(self, keys, caller_site_id=None, master_keyset_id=None, default_keyset_id=None, token_expiry_seconds=None):
+    def __init__(self, keys, identity_scope=IdentityScope.UID2, caller_site_id=None, master_keyset_id=None, default_keyset_id=None, token_expiry_seconds=None, max_sharing_lifetime_seconds=None, max_bidstream_lifetime_seconds=None, allow_clock_skew_seconds=None):
         self._latest_expires = None
         self._keys = dict()
+        self._identity_scope = identity_scope
         self._keys_by_site = dict()
         self._keys_by_keyset = dict()
         self.set_keys(keys)
         self._caller_site_id = caller_site_id
         self._master_keyset_id = master_keyset_id
         self._default_keyset_id = default_keyset_id
         self._token_expiry_seconds = token_expiry_seconds
+        if max_sharing_lifetime_seconds is None:
+            self._max_sharing_lifetime_seconds = sys.maxsize
+        else:
+            self._max_sharing_lifetime_seconds = max_sharing_lifetime_seconds
+        if max_bidstream_lifetime_seconds is None:
+            self._max_bidstream_lifetime_seconds = sys.maxsize
+        else:
+            self._max_bidstream_lifetime_seconds = max_bidstream_lifetime_seconds
+        if allow_clock_skew_seconds is None:
+            self._allow_clock_skew_seconds = 60 * 30  # 30 minutes
+        else:
+            self._allow_clock_skew_seconds = allow_clock_skew_seconds
 
     def set_keys(self, keys):
         for key in keys:
             self._keys[key.key_id] = key
             if key.site_id > 0:
                 self._keys_by_site.setdefault(key.site_id, []).append(key)
             if key.keyset_id is not None:
@@ -130,26 +145,37 @@
     def __contains__(self, key_id):
         return key_id in self._keys.keys()
 
 
     def __getitem__(self, key_id):
         return self._keys[key_id]
 
+    def get_identity_scope(self):
+        return self._identity_scope
+
     def get_caller_site_id(self):
         return self._caller_site_id
 
     def get_master_keyset_id(self):
         return self._master_keyset_id
 
     def get_default_keyset_id(self):
         return self._default_keyset_id
 
     def get_token_expiry_seconds(self):
         return self._token_expiry_seconds
 
+    def get_max_bidstream_lifetime_seconds(self):
+        return self._max_bidstream_lifetime_seconds
+
+    def get_max_sharing_lifetime_seconds(self):
+        return self._max_sharing_lifetime_seconds
+
+    def get_allow_clock_skew_seconds(self):
+        return self._allow_clock_skew_seconds
 
     def get(self, key_id, default=None):
         """Get encryption key with the specified id, else default."""
         return self._keys.get(key_id, default)
 
 
     def key_ids(self):
```

### Comparing `uid2_client-2.2.8/uid2_client/publisher_client.py` & `uid2_client-2.3.0/uid2_client/publisher_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""Internal module for holding the Uid2Client class.
-
-Do not use this module directly, import through uid2_client module instead, e.g.
-
+"""Usage
 >>> from uid2_client import Uid2PublisherClient
 """
 
 import datetime as dt
 from datetime import timezone
```

### Comparing `uid2_client-2.2.8/uid2_client/request_response_util.py` & `uid2_client-2.3.0/uid2_client/request_response_util.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/token_generate_input.py` & `uid2_client-2.3.0/uid2_client/token_generate_input.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/token_generate_response.py` & `uid2_client-2.3.0/uid2_client/token_generate_response.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/token_refresh_response.py` & `uid2_client-2.3.0/uid2_client/token_refresh_response.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.3.0/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.2.8/uid2_client.egg-info/PKG-INFO` & `uid2_client-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uid2-client
-Version: 2.2.8
+Name: uid2_client
+Version: 2.3.0
 Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
 Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
@@ -83,15 +83,16 @@
 ### Example Usage
 
 To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A== \
-	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE=
+	RAW_UID=JCqmlLXpbbu/jTdpB2a1cNAVs8O72eMXPaQzC9Ic9mE= \
+	DOMAIN=example.com
 ```
 
 Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
```

### Comparing `uid2_client-2.2.8/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.3.0/uid2_client.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_bidstream_client.py
 tests/test_client.py
 tests/test_encryption.py
 tests/test_key_parse.py
 tests/test_keys.py
 tests/test_normalization.py
 tests/test_publisher_client.py
+tests/test_refresh_keys_util.py
 tests/test_sharing.py
+tests/test_sharing_client.py
 tests/test_utils.py
 uid2_client/__init__.py
 uid2_client/advertising_token_version.py
 uid2_client/auto_refresh.py
+uid2_client/bidstream_client.py
 uid2_client/client.py
+uid2_client/client_type.py
+uid2_client/decryption_status.py
 uid2_client/encryption.py
+uid2_client/encryption_data_response.py
+uid2_client/encryption_status.py
 uid2_client/euid_client_factory.py
 uid2_client/identity_scope.py
 uid2_client/identity_tokens.py
 uid2_client/identity_type.py
 uid2_client/input_util.py
 uid2_client/keys.py
 uid2_client/publisher_client.py
+uid2_client/refresh_keys_util.py
+uid2_client/refresh_response.py
 uid2_client/request_response_util.py
+uid2_client/sharing_client.py
 uid2_client/token_generate_input.py
 uid2_client/token_generate_response.py
 uid2_client/token_refresh_response.py
 uid2_client/uid2_base64_url_coder.py
 uid2_client/uid2_client_factory.py
+uid2_client/uid2_token_generator.py
 uid2_client.egg-info/PKG-INFO
 uid2_client.egg-info/SOURCES.txt
 uid2_client.egg-info/dependency_links.txt
 uid2_client.egg-info/requires.txt
 uid2_client.egg-info/top_level.txt
 uid2_client.egg-info/zip-safe
```

