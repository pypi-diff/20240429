# Comparing `tmp/gdata_vaas-4.4.0.tar.gz` & `tmp/gdata_vaas-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata_vaas-4.4.0.tar", last modified: Wed Apr 24 12:12:05 2024, max compression
+gzip compressed data, was "gdata_vaas-5.0.0.tar", last modified: Mon Apr 29 08:48:58 2024, max compression
```

## Comparing `gdata_vaas-4.4.0.tar` & `gdata_vaas-5.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 12:12:05.148325 gdata_vaas-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.140325 gdata_vaas-4.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/resource_owner_password_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14646 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/tests/test_resource_owner_password_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:48:57.999978 gdata_vaas-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-29 08:48:57.999978 gdata_vaas-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 08:48:57.999978 gdata_vaas-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:48:57.995978 gdata_vaas-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:48:57.999978 gdata_vaas-5.0.0/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-29 08:48:57.000000 gdata_vaas-5.0.0/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 08:48:57.000000 gdata_vaas-5.0.0/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:48:57.000000 gdata_vaas-5.0.0/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 08:48:57.000000 gdata_vaas-5.0.0/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 08:48:57.000000 gdata_vaas-5.0.0/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:48:57.999978 gdata_vaas-5.0.0/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/src/vaas/resource_owner_password_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:48:57.999978 gdata_vaas-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/tests/test_resource_owner_password_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-29 08:48:16.000000 gdata_vaas-5.0.0/tests/test_vaas.py
```

### Comparing `gdata_vaas-4.4.0/LICENSE` & `gdata_vaas-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/PKG-INFO` & `gdata_vaas-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 4.4.0
+Version: 5.0.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata_vaas-4.4.0/README.md` & `gdata_vaas-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/setup.cfg` & `gdata_vaas-5.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 4.4.0
+version = 5.0.0
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls =
```

### Comparing `gdata_vaas-4.4.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata_vaas-5.0.0/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 4.4.0
+Version: 5.0.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata_vaas-4.4.0/src/gdata_vaas.egg-info/SOURCES.txt` & `gdata_vaas-5.0.0/src/gdata_vaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/src/vaas/__init__.py` & `gdata_vaas-5.0.0/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata_vaas-5.0.0/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/src/vaas/resource_owner_password_grant_authenticator.py` & `gdata_vaas-5.0.0/src/vaas/resource_owner_password_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/src/vaas/vaas.py` & `gdata_vaas-5.0.0/src/vaas/vaas.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,16 +95,17 @@
 
 
 def map_response(verdict_response):
     return {
         "Sha256": verdict_response.get("sha256"),
         "Guid": verdict_response.get("guid"),
         "Verdict": verdict_response.get("verdict"),
-        "LibMagic": verdict_response.get("lib_magic"),
-        "Detections": verdict_response.get("detections"),
+        "Detection": verdict_response.get("detection"),
+        "FileType": verdict_response.get("file_type"),
+        "MimeType": verdict_response.get("mime_type")
     }
 
 
 class Vaas:
     """Verdict-as-a-Service client"""
 
     def __init__(
```

### Comparing `gdata_vaas-4.4.0/src/vaas/vaas_errors.py` & `gdata_vaas-5.0.0/src/vaas/vaas_errors.py`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/tests/test_client_credentials_grant_authenticator.py` & `gdata_vaas-5.0.0/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/tests/test_resource_owner_password_grant_authenticator.py` & `gdata_vaas-5.0.0/tests/test_resource_owner_password_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata_vaas-4.4.0/tests/test_vaas.py` & `gdata_vaas-5.0.0/tests/test_vaas.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,27 +115,27 @@
             self.assertEqual(verdict["Verdict"], "Malicious")
             self.assertEqual(
                 verdict["Sha256"].casefold(),
                 "275a021bbfb6489e54d471899f7db9d1663fc695ec2fe2a2c4538aabf651fd0f".casefold(),
             self.assertEqual(verdict["Guid"].casefold(), guid)
             )
 
-    # async def test_for_sha256_returns_pup_for_amtso(self):
-    #     async with await create_and_connect() as vaas:
-    #         guid = str(uuid.uuid4())
-    #         verdict = await vaas.for_sha256(
-    #             "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad",
-    #             guid=guid
-    #         )
-    #         self.assertEqual(verdict["Verdict"], "Pup")
-    #         self.assertEqual(
-    #             verdict["Sha256"].casefold(),
-    #             "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad".casefold(),
-    #         )
-    #         self.assertEqual(verdict["Guid"].casefold(), guid)
+    async def test_for_sha256_returns_pup_for_amtso(self):
+        async with await create_and_connect() as vaas:
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_sha256(
+                "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad",
+                guid=guid
+            )
+            self.assertEqual(verdict["Verdict"], "Pup")
+            self.assertEqual(
+                verdict["Sha256"].casefold(),
+                "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad".casefold(),
+            )
+            self.assertEqual(verdict["Guid"].casefold(), guid)
 
     async def test_for_buffer_returns_malicious_for_eicar(self):
         async with await create_and_connect() as vaas:
             buffer = base64.b64decode(EICAR_BASE64)
             sha256 = hashlib.sha256(buffer).hexdigest()
             guid = str(uuid.uuid4())
             verdict = await vaas.for_buffer(buffer, guid=guid)
@@ -245,14 +245,14 @@
 
     async def test_for_url_returns_detections_and_mime_type(self):
         options = get_disabled_options()
         async with await create_and_connect(options=options) as vaas:
             guid = str(uuid.uuid4())
             verdict = await vaas.for_url("https://secure.eicar.org/eicar.com.txt", guid=guid)
             self.assertEqual(verdict["Verdict"], "Malicious")
-            self.assertIsNotNone(verdict["Detections"])
-            self.assertEqual(verdict["LibMagic"]['file_type'], "EICAR virus test files")
-            self.assertEqual(verdict["LibMagic"]['mime_type'], "text/plain")
+            self.assertIsNotNone(verdict["Detection"])
+            self.assertEqual(verdict['FileType'], "EICAR virus test files")
+            self.assertEqual(verdict['MimeType'], "text/plain")
 
 
 if __name__ == "__main__":
     unittest.main()
```

