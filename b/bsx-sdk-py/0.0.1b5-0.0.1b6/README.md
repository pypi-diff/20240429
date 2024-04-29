# Comparing `tmp/bsx_sdk_py-0.0.1b5.tar.gz` & `tmp/bsx_sdk_py-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsx_sdk_py-0.0.1b5.tar", max compression
+gzip compressed data, was "bsx_sdk_py-0.0.1b6.tar", max compression
```

## Comparing `bsx_sdk_py-0.0.1b5.tar` & `bsx_sdk_py-0.0.1b6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2170 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/README.md
--rw-r--r--   0        0        0       89 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/client.py
--rw-r--r--   0        0        0      176 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/types.py
--rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/__init__.py
--rw-r--r--   0        0        0     2453 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/client.py
--rw-r--r--   0        0        0      214 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/types.py
--rw-r--r--   0        0        0     3254 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/base.py
--rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/__init__.py
--rw-r--r--   0        0        0     4250 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/client.py
--rw-r--r--   0        0        0      224 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/types.py
--rw-r--r--   0        0        0       24 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/__init__.py
--rw-r--r--   0        0        0      481 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/acc_info.py
--rw-r--r--   0        0        0     1167 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/exception.py
--rw-r--r--   0        0        0     1882 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/lock.py
--rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/account.py
--rw-r--r--   0        0        0     1470 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/auth.py
--rw-r--r--   0        0        0      234 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/base.py
--rw-r--r--   0        0        0     8455 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/market.py
--rw-r--r--   0        0        0       62 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/__init__.py
--rw-r--r--   0        0        0     1292 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/acc_storage.py
--rw-r--r--   0        0        0     1871 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/api_key_base_manager.py
--rw-r--r--   0        0        0     1563 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/base.py
--rw-r--r--   0        0        0     1417 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/secret_base_manager.py
--rw-r--r--   0        0        0     8631 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/instance.py
--rw-r--r--   0        0        0      556 2024-04-24 10:12:45.800298 bsx_sdk_py-0.0.1b5/pyproject.toml
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 bsx_sdk_py-0.0.1b5/PKG-INFO
+-rw-r--r--   0        0        0     2170 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/README.md
+-rw-r--r--   0        0        0       89 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/client.py
+-rw-r--r--   0        0        0      176 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/types.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/__init__.py
+-rw-r--r--   0        0        0     2453 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/client.py
+-rw-r--r--   0        0        0      214 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/types.py
+-rw-r--r--   0        0        0     3254 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/base.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/__init__.py
+-rw-r--r--   0        0        0     4250 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/client.py
+-rw-r--r--   0        0        0      224 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/types.py
+-rw-r--r--   0        0        0       24 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/acc_info.py
+-rw-r--r--   0        0        0     1167 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/exception.py
+-rw-r--r--   0        0        0     1882 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/lock.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/account.py
+-rw-r--r--   0        0        0     1470 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/auth.py
+-rw-r--r--   0        0        0      234 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/base.py
+-rw-r--r--   0        0        0     8455 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/market.py
+-rw-r--r--   0        0        0       62 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/__init__.py
+-rw-r--r--   0        0        0     1292 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/acc_storage.py
+-rw-r--r--   0        0        0     1871 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/api_key_base_manager.py
+-rw-r--r--   0        0        0     1563 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/base.py
+-rw-r--r--   0        0        0     1417 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/secret_base_manager.py
+-rw-r--r--   0        0        0     8789 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/instance.py
+-rw-r--r--   0        0        0      556 2024-04-29 06:31:42.044713 bsx_sdk_py-0.0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 bsx_sdk_py-0.0.1b6/PKG-INFO
```

### Comparing `bsx_sdk_py-0.0.1b5/README.md` & `bsx_sdk_py-0.0.1b6/README.md`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/client.py` & `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/client.py` & `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/base.py` & `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/base.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/client.py` & `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/common/exception.py` & `bsx_sdk_py-0.0.1b6/bsx_py/common/exception.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/common/lock.py` & `bsx_sdk_py-0.0.1b6/bsx_py/common/lock.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/common/types/account.py` & `bsx_sdk_py-0.0.1b6/bsx_py/common/types/account.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/common/types/auth.py` & `bsx_sdk_py-0.0.1b6/bsx_py/common/types/auth.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/common/types/market.py` & `bsx_sdk_py-0.0.1b6/bsx_py/common/types/market.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/helper/acc_storage.py` & `bsx_sdk_py-0.0.1b6/bsx_py/helper/acc_storage.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/helper/api_key_base_manager.py` & `bsx_sdk_py-0.0.1b6/bsx_py/helper/api_key_base_manager.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/helper/base.py` & `bsx_sdk_py-0.0.1b6/bsx_py/helper/base.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/helper/secret_base_manager.py` & `bsx_sdk_py-0.0.1b6/bsx_py/helper/secret_base_manager.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b5/bsx_py/instance.py` & `bsx_sdk_py-0.0.1b6/bsx_py/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,62 +38,62 @@
 
     BSXInstance will handle signing, authenticating, API key renewal internally.
 
     Each BSXInstance works with only one wallet. If you want to use multiple wallets, just create multiple instances.
     """
 
     @staticmethod
-    def from_api_key(api_key: str, api_secret: str, signer: LocalAccount, env: Environment) -> 'BSXInstance':
+    def from_api_key(api_key: str, api_secret: str, signer: LocalAccount, env: Environment | str) -> 'BSXInstance':
         """
         Initialize a new BSXInstance object using an active API key.
 
         The BSXInstance returned by this method will not be able to submit withdrawal requests
 
         Attributes:
             api_key (str): BSX API key
 
             api_secret (str): BSX secret
 
             signer (LocalAccount): signer wallet used to sign requests
 
-            env (Environment): environment to use (Testnet or mainnet)
+            env (Environment|str): environment to use (Testnet or mainnet) or the domain in plain text
 
         Raises:
             BSXRequestException: If the response status is not "success".
         """
         instance = BSXInstance.__new__(BSXInstance)
-        domain = env.value
+        domain = env.value if isinstance(env, Environment) else env
         config = instance._get_chain_config(domain)
         eip712_domain = instance._build_eip712_domain(config)
 
         instance._acc_manager = AccountManager.from_api_key(api_key, api_secret, signer.key, domain, eip712_domain)
         instance._account_client = AccountClient(
             domain=domain, domain_signature=eip712_domain, config=config, acc_info=instance._acc_manager
         )
         instance._market_client = MarketClient(
             domain=domain, domain_signature=eip712_domain, acc_info=instance._acc_manager
         )
 
         return instance
 
-    def __init__(self, env: Environment, wallet: LocalAccount, signer: LocalAccount):
+    def __init__(self, env: Environment | str, wallet: LocalAccount, signer: LocalAccount):
         """
         Initialize a new BSXInstance object using main wallet's private key
 
         Attributes:
-            env (Environment): environment to use (Testnet or mainnet)
+            env (Environment|str): environment to use (Testnet or mainnet) or the domain in plain text
 
             wallet (LocalAccount): main wallet
 
             signer (LocalAccount): signer wallet used to sign requests
 
         Raises:
             BSXRequestException: If the response status is not "success".
         """
-        domain = env.value
+        domain = env.value if isinstance(env, Environment) else env
         config = self._get_chain_config(domain)
         eip712_domain = self._build_eip712_domain(config)
 
         self._acc_manager = AccountManager.from_secret(wallet.key, signer.key, domain, eip712_domain)
         self._account_client = AccountClient(
             domain=domain, domain_signature=eip712_domain, config=config, acc_info=self._acc_manager
         )
```

### Comparing `bsx_sdk_py-0.0.1b5/pyproject.toml` & `bsx_sdk_py-0.0.1b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bsx-sdk-py"
-version = "0.0.1beta5"
+version = "0.0.1beta6"
 description = ""
 authors = ["bsx-engineering <dev@bsx.exchange>"]
 readme = "README.md"
 packages = [
     { include = "bsx_py" }
 ]
```

### Comparing `bsx_sdk_py-0.0.1b5/PKG-INFO` & `bsx_sdk_py-0.0.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsx-sdk-py
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: 
 Author: bsx-engineering
 Author-email: dev@bsx.exchange
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

