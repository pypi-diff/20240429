# Comparing `tmp/pimsclient-2.0.2.tar.gz` & `tmp/pimsclient-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimsclient-2.0.2.tar", max compression
+gzip compressed data, was "pimsclient-2.0.3.tar", max compression
```

## Comparing `pimsclient-2.0.2.tar` & `pimsclient-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2021-07-20 10:36:12.537989 pimsclient-2.0.2/LICENSE
--rw-r--r--   0        0        0      142 2022-11-17 15:55:14.117750 pimsclient-2.0.2/pimsclient/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/auth/__init__.py
--rw-r--r--   0        0        0       83 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/auth/exceptions.py
--rw-r--r--   0        0        0     7484 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/auth/msal.py
--rw-r--r--   0        0        0     1114 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/auth/ntlm.py
--rw-r--r--   0        0        0       84 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/autogen/__init__.py
--rw-r--r--   0        0        0    33589 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/autogen/swagger_models_v0.py
--rw-r--r--   0        0        0     8807 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/client.py
--rw-r--r--   0        0        0     8950 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/core.py
--rw-r--r--   0        0        0      281 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/exceptions.py
--rw-r--r--   0        0        0     6806 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/keyfile.py
--rw-r--r--   0        0        0      138 2024-04-24 09:47:34.483970 pimsclient-2.0.2/pimsclient/logs.py
--rw-r--r--   0        0        0    12729 2024-04-24 13:04:09.246198 pimsclient-2.0.2/pimsclient/server.py
--rw-r--r--   0        0        0     5928 2024-04-24 13:04:09.258198 pimsclient-2.0.2/pimsclient/swagger.py
--rw-r--r--   0        0        0     1042 2024-04-24 13:17:44.708558 pimsclient-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 pimsclient-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-29 09:12:19.496747 pimsclient-2.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-29 09:12:19.496747 pimsclient-2.0.3/pimsclient/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:12:19.496747 pimsclient-2.0.3/pimsclient/auth/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-29 09:12:19.496747 pimsclient-2.0.3/pimsclient/auth/exceptions.py
+-rw-r--r--   0        0        0     7484 2024-04-29 09:12:19.496747 pimsclient-2.0.3/pimsclient/auth/msal.py
+-rw-r--r--   0        0        0     1114 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/auth/ntlm.py
+-rw-r--r--   0        0        0       84 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/autogen/__init__.py
+-rw-r--r--   0        0        0    33589 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/autogen/swagger_models_v0.py
+-rw-r--r--   0        0        0     8807 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/client.py
+-rw-r--r--   0        0        0     8950 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/core.py
+-rw-r--r--   0        0        0      281 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/exceptions.py
+-rw-r--r--   0        0        0     6806 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/keyfile.py
+-rw-r--r--   0        0        0      138 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/logs.py
+-rw-r--r--   0        0        0    12729 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/server.py
+-rw-r--r--   0        0        0     5928 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pimsclient/swagger.py
+-rw-r--r--   0        0        0     1042 2024-04-29 09:12:19.500747 pimsclient-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 pimsclient-2.0.3/PKG-INFO
```

### Comparing `pimsclient-2.0.2/LICENSE` & `pimsclient-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/auth/msal.py` & `pimsclient-2.0.3/pimsclient/auth/msal.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/auth/ntlm.py` & `pimsclient-2.0.3/pimsclient/auth/ntlm.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/autogen/swagger_models_v0.py` & `pimsclient-2.0.3/pimsclient/autogen/swagger_models_v0.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/client.py` & `pimsclient-2.0.3/pimsclient/client.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/core.py` & `pimsclient-2.0.3/pimsclient/core.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/keyfile.py` & `pimsclient-2.0.3/pimsclient/keyfile.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/server.py` & `pimsclient-2.0.3/pimsclient/server.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pimsclient/swagger.py` & `pimsclient-2.0.3/pimsclient/swagger.py`

 * *Files identical despite different names*

### Comparing `pimsclient-2.0.2/pyproject.toml` & `pimsclient-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pimsclient"
-version = "2.0.2"
+version = "2.0.3"
 description = "Client for PIMS key_file management swagger web API"
 authors = ["sjoerdk <sjoerd.kerkstra@radboudumc.nl>"]
 license = "MIT"
 repository = "https://github.com/sjoerdk/pimsclient"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pimsclient-2.0.2/PKG-INFO` & `pimsclient-2.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimsclient
-Version: 2.0.2
+Version: 2.0.3
 Summary: Client for PIMS key_file management swagger web API
 Home-page: https://github.com/sjoerdk/pimsclient
 License: MIT
 Author: sjoerdk
 Author-email: sjoerd.kerkstra@radboudumc.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

