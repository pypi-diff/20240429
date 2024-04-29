# Comparing `tmp/binaryai-0.7.1.tar.gz` & `tmp/binaryai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binaryai-0.7.1.tar", max compression
+gzip compressed data, was "binaryai-0.8.0.tar", max compression
```

## Comparing `binaryai-0.7.1.tar` & `binaryai-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    35149 2023-10-10 09:23:20.437723 binaryai-0.7.1/LICENSE
--rw-r--r--   0        0        0     3308 2023-10-10 09:23:20.437723 binaryai-0.7.1/README.md
--rw-r--r--   0        0        0     1175 2023-10-10 09:23:20.441723 binaryai-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      672 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/__init__.py
--rw-r--r--   0        0        0     5600 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/binaryai_file.py
--rw-r--r--   0        0        0    19881 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client.py
--rw-r--r--   0        0        0     7307 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/__init__.py
--rw-r--r--   0        0        0     1677 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/a_s_c_i_i_string.py
--rw-r--r--   0        0        0     5399 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/base_client.py
--rw-r--r--   0        0        0      660 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/base_model.py
--rw-r--r--   0        0        0      579 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/c_v_e_name.py
--rw-r--r--   0        0        0     1612 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/check_or_upload.py
--rw-r--r--   0        0        0     1385 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/check_state.py
--rw-r--r--   0        0        0    15485 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/client.py
--rw-r--r--   0        0        0     1164 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/compressed_file.py
--rw-r--r--   0        0        0      546 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/create_file.py
--rw-r--r--   0        0        0      418 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/download_link.py
--rw-r--r--   0        0        0     1726 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/enums.py
--rw-r--r--   0        0        0     2366 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/exceptions.py
--rw-r--r--   0        0        0      321 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/file_size.py
--rw-r--r--   0        0        0      333 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/filename.py
--rw-r--r--   0        0        0     1292 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/function_info.py
--rw-r--r--   0        0        0      773 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/function_list.py
--rw-r--r--   0        0        0     1201 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/function_match.py
--rw-r--r--   0        0        0     1325 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/functions_info.py
--rw-r--r--   0        0        0     2574 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/input_types.py
--rw-r--r--   0        0        0     1837 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/license.py
--rw-r--r--   0        0        0      531 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/license_short_name.py
--rw-r--r--   0        0        0      380 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/m_i_m_e_type.py
--rw-r--r--   0        0        0      951 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/overview.py
--rw-r--r--   0        0        0      797 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/reanalyze.py
--rw-r--r--   0        0        0      595 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/s_c_a.py
--rw-r--r--   0        0        0      313 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/client_stub/sha256.py
--rw-r--r--   0        0        0      451 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/component.py
--rw-r--r--   0        0        0      316 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/compressed_file.py
--rw-r--r--   0        0        0      139 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/cve.py
--rw-r--r--   0        0        0      503 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/exceptions.py
--rw-r--r--   0        0        0      928 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/function.py
--rw-r--r--   0        0        0     1360 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/license.py
--rw-r--r--   0        0        0     4760 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/query.graphql
--rw-r--r--   0        0        0     5662 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/upload.py
--rw-r--r--   0        0        0     8839 2023-10-10 09:23:20.441723 binaryai-0.7.1/src/binaryai/utils.py
--rw-r--r--   0        0        0     4152 1970-01-01 00:00:00.000000 binaryai-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 08:35:03.182743 binaryai-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3308 2024-04-29 08:35:03.182743 binaryai-0.8.0/README.md
+-rw-r--r--   0        0        0     1302 2024-04-29 08:35:03.186743 binaryai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      672 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/__init__.py
+-rw-r--r--   0        0        0     5916 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/binaryai_file.py
+-rw-r--r--   0        0        0    20833 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client.py
+-rw-r--r--   0        0        0     7777 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/__init__.py
+-rw-r--r--   0        0        0     1459 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/ascii_string.py
+-rw-r--r--   0        0        0     6659 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/base_client.py
+-rw-r--r--   0        0        0      620 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/base_model.py
+-rw-r--r--   0        0        0     1440 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/check_or_upload.py
+-rw-r--r--   0        0        0     1223 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/check_state.py
+-rw-r--r--   0        0        0    17853 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/client.py
+-rw-r--r--   0        0        0     1042 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/compressed_file.py
+-rw-r--r--   0        0        0      536 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/create_file.py
+-rw-r--r--   0        0        0      520 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/cve_name.py
+-rw-r--r--   0        0        0      365 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/download_link.py
+-rw-r--r--   0        0        0     1978 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/enums.py
+-rw-r--r--   0        0        0     2411 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/exceptions.py
+-rw-r--r--   0        0        0      896 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/file_k_hash.py
+-rw-r--r--   0        0        0      272 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/file_size.py
+-rw-r--r--   0        0        0      284 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/filename.py
+-rw-r--r--   0        0        0     1169 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/function_info.py
+-rw-r--r--   0        0        0      710 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/function_list.py
+-rw-r--r--   0        0        0     1125 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/function_match.py
+-rw-r--r--   0        0        0     1198 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/functions_info.py
+-rw-r--r--   0        0        0     2484 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/input_types.py
+-rw-r--r--   0        0        0     1639 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/license.py
+-rw-r--r--   0        0        0      467 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/license_short_name.py
+-rw-r--r--   0        0        0      331 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/mime_type.py
+-rw-r--r--   0        0        0      892 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/overview.py
+-rw-r--r--   0        0        0      739 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/reanalyze.py
+-rw-r--r--   0        0        0      542 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/sca.py
+-rw-r--r--   0        0        0      319 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/client_stub/sha_256.py
+-rw-r--r--   0        0        0      451 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/component.py
+-rw-r--r--   0        0        0      316 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/compressed_file.py
+-rw-r--r--   0        0        0      139 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/cve.py
+-rw-r--r--   0        0        0      503 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/exceptions.py
+-rw-r--r--   0        0        0      928 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/function.py
+-rw-r--r--   0        0        0     1360 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/license.py
+-rw-r--r--   0        0        0     5980 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/query.graphql
+-rw-r--r--   0        0        0     5663 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/upload.py
+-rw-r--r--   0        0        0     8839 2024-04-29 08:35:03.186743 binaryai-0.8.0/src/binaryai/utils.py
+-rw-r--r--   0        0        0     4152 1970-01-01 00:00:00.000000 binaryai-0.8.0/PKG-INFO
```

### Comparing `binaryai-0.7.1/LICENSE` & `binaryai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binaryai-0.7.1/README.md` & `binaryai-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `binaryai-0.7.1/pyproject.toml` & `binaryai-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "binaryai"
-version = "0.7.1"
+version = "0.8.0"
 description = "BinaryAI-SDK is a library provides an abstracted client module to simplify the procedure of uploading file for analysis."
 license = "GPLv3"
 authors = ["binaryai <binaryai@tencent.com>"]
 readme = "README.md"
 homepage = "https://www.binaryai.cn/"
 documentation = "https://www.binaryai.cn/doc/"
 repository = "https://github.com/binaryai/sdk/"
@@ -18,18 +18,19 @@
 python = "^3.9"
 deprecated = "^1.2.14"
 httpx = "^0.25.0"
 pydantic = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "4.0.1"
-black = "22.6.0"
+black = "24.3.0"
 isort = "5.10.1"
-ariadne-codegen = "^0.9.0"
+ariadne-codegen = "^0.13.0"
 pytest = "^7.4.2"
+scipy = "^1.13.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autoapi = "^2.1.1"
 sphinx-rtd-theme = "^1.3.0"
 sphinx = "^7.2.6"
 myst-parser = "^2.0.0"
 sphinx-intl = "^2.1.0"
@@ -38,7 +39,13 @@
 
 [tool.ariadne-codegen]
 remote_schema_url = "https://api.binaryai.cn/v1/endpoint"
 queries_path = "./src/binaryai/query.graphql"
 target_package_name = "client_stub"
 target_package_path = "./src/binaryai"
 async_client = false
+
+[tool.black]
+exclude = "src/binaryai/client_stub/*"
+
+[tool.isort]
+skip_glob = "src/binaryai/client_stub/*"
```

### Comparing `binaryai-0.7.1/src/binaryai/__init__.py` & `binaryai-0.8.0/src/binaryai/__init__.py`

 * *Files identical despite different names*

### Comparing `binaryai-0.7.1/src/binaryai/binaryai_file.py` & `binaryai-0.8.0/src/binaryai/binaryai_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,7 +167,15 @@
 
         Returns:
             List[MatchedFunction]: a List containing 10 match results,
             every result is a Dict the contains score and pseudocode.
             The List is sorted by score from high to low.
         """
         return self._bai.get_func_match(self.sha256, offset)
+
+    def get_khash_info(self) -> tuple[bytes, str]:
+        """Return the KHash of this file. See website for detailed introduction on KHash.
+
+        Returns:
+            Tuple[bytes, str]: KHash's value and version. Only compare if version is same.
+        """
+        return self._bai.get_khash_info(self.sha256)
```

### Comparing `binaryai-0.7.1/src/binaryai/client.py` & `binaryai-0.8.0/src/binaryai/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+import binascii
 import logging
 import os
 import threading
 import time
 from importlib.metadata import version
 from typing import Dict, Iterator, List, Optional, Union
 from urllib.parse import urlparse
@@ -53,19 +54,21 @@
     """
 
     def __init__(
         self,
         *,
         secret_id: Optional[str] = os.environ.get("BINARYAI_SECRET_ID"),
         secret_key: Optional[str] = os.environ.get("BINARYAI_SECRET_KEY"),
-        endpoint: str = os.environ.get("BINARYAI_ENDPOINT", DEFAULT_ENDPOINT),
+        endpoint: str = os.environ.get("BINARYAI_ENDPOINT") or DEFAULT_ENDPOINT,
     ) -> None:
         super().__init__()
-        if secret_id is None or secret_key is None:
+        if not (secret_id and secret_key):
             raise ValueError("Please set secret id and key in your code or environ")
+        if not endpoint:
+            raise ValueError("Please set endpoint, or leave it as empty if you have no idea")
         transport = httpx.HTTPTransport(
             verify=True,
             retries=3,
         )
         auth = QCloudHttpxAuth(
             secret_id,
             secret_key,
@@ -193,18 +196,18 @@
 
         Args:
             md5: File md5 hash.
 
         Returns:
             str: File sha256sum.
         """
-        f = self._client.sha256(md5).file
+        f = self._client.sha_256(md5).file
         if not f:
             raise FileNotExistError("File not exists or no permission")
-        return f.sha256
+        return f.sha_256
 
     def get_filenames(self, sha256: str) -> List[str]:
         """Get all uploaded filenames for a given file.
 
         Args:
             sha256: File sha256sum.
 
@@ -221,15 +224,15 @@
 
         Args:
             sha256: File sha256sum.
 
         Returns:
             str: MIME type string.
         """
-        f = self._client.m_i_m_e_type(sha256).file
+        f = self._client.mime_type(sha256).file
         if not f:
             raise FileNotExistError("File not exists or no permission")
         return f.mime_type
 
     def get_size(self, sha256: str) -> int:
         """Get size in bytes of a given file.
 
@@ -259,26 +262,26 @@
 
         file_list = []
         for compressed_file in f.decompressed or []:
             if compressed_file:
                 file_list.append(
                     CompressedFile(
                         path=compressed_file.path,
-                        sha256=compressed_file.sha256,
+                        sha256=compressed_file.sha_256,
                     )
                 )
         return file_list
 
     def get_all_cve_names(self, sha256: str) -> List[str]:
         """Get all CVE names for a given file.
 
         Args:
             sha256: File sha256sum.
         """
-        f = self._client.c_v_e_name(sha256).file
+        f = self._client.cve_name(sha256).file
         if not f:
             raise FileNotExistError("File not exists or no permission")
 
         cve_list = []
         for elem in f.scainfo or []:
             for mapping in elem.cves or []:
                 cve_list.append(mapping.name)
@@ -341,15 +344,15 @@
 
         Args:
             sha256: File sha256sum.
 
         Returns:
             List[str]: A list of ASCII strings.
         """
-        f = self._client.a_s_c_i_i_string(sha256).file
+        f = self._client.ascii_string(sha256).file
         if not f:
             raise FileNotExistError("File not exists or no permission")
 
         if f.executable and f.executable.ascii_strings:
             return f.executable.ascii_strings
         else:
             return []
@@ -359,26 +362,26 @@
 
         Args:
             sha256: File sha256sum.
 
         Returns:
             List[Component]: A list of software components.
         """
-        f = self._client.s_c_a(sha256).file
+        f = self._client.sca(sha256).file
         if not f:
             raise FileNotExistError("File not exists or no permission")
 
         component_list = []
         for elem in f.scainfo or []:
             component_list.append(
                 Component(
                     name=elem.name,
                     version=elem.version,
                     description=elem.description,
-                    source_code_url=elem.source_code_u_r_l,
+                    source_code_url=elem.source_code_url,
                     summary=elem.summary,
                 )
             )
         return component_list
 
     def get_overview(self, sha256: str) -> Dict[str, Union[str, int]]:
         """Fetch analysis overview from BinaryAI Beat server by file's sha256.
@@ -558,7 +561,27 @@
         for item in func.match:
             matched_func = MatchedFunction(
                 score=item.score,
                 code=(None if not item.function else item.function.code),
             )
             matched_func_list.append(matched_func)
         return matched_func_list
+
+    def get_khash_info(self, sha256: str) -> Optional[tuple[bytes, str]]:
+        """Return the KHash of this file. See website for detailed introduction on KHash.
+
+        Returns:
+            Optional[Tuple[bytes, str]]: KHash's value and version. Only compare if version is same.
+                                         You are not expected to parse version.
+        """
+        m = self._client.file_k_hash(sha256)
+        if not m.file:
+            return None
+        if not m.file.decompile_result:
+            return None
+        if not m.file.decompile_result.k_hash_info:
+            return None
+        # wiring protocol of hash value is a hex sequence
+        return (
+            binascii.unhexlify(m.file.decompile_result.k_hash_info.hash.hash),
+            m.file.decompile_result.k_hash_info.hash.version,
+        )
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/__init__.py` & `binaryai-0.8.0/src/binaryai/client_stub/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 
-from .a_s_c_i_i_string import (
+from .ascii_string import (
     ASCIIString,
     ASCIIStringFile,
     ASCIIStringFileExecutableCOFFInfo,
     ASCIIStringFileExecutableELFInfo,
     ASCIIStringFileExecutableMachoInfo,
     ASCIIStringFileExecutablePEInfo,
 )
 from .base_client import BaseClient
 from .base_model import BaseModel, Upload
-from .c_v_e_name import CVEName, CVENameFile, CVENameFileScainfo, CVENameFileScainfoCves
 from .check_or_upload import (
     CheckOrUpload,
     CheckOrUploadCreateUploadTicketFile,
     CheckOrUploadCreateUploadTicketOwnershipTicket,
     CheckOrUploadCreateUploadTicketUploadTicket,
     CheckOrUploadCreateUploadTicketUploadTicketRequestHeaders,
 )
@@ -31,16 +30,18 @@
 from .compressed_file import (
     CompressedFile,
     CompressedFileFile,
     CompressedFileFileDecompressedCompressedDirectory,
     CompressedFileFileDecompressedCompressedFile,
 )
 from .create_file import CreateFile, CreateFileCreateFile
+from .cve_name import CVEName, CVENameFile, CVENameFileScainfo, CVENameFileScainfoCves
 from .download_link import DownloadLink, DownloadLinkFile
 from .enums import (
+    AnalyzeProgressStep,
     AntivirusSafeLevel,
     ExecuteType,
     FileType,
     MatchAlgorithm,
     NoopReason,
     PseudoCodeAnnotationType,
     RelroLevel,
@@ -51,15 +52,22 @@
     XRefType,
 )
 from .exceptions import (
     GraphQLClientError,
     GraphQLClientGraphQLError,
     GraphQLClientGraphQLMultiError,
     GraphQLClientHttpError,
-    GraphQlClientInvalidResponseError,
+    GraphQLClientInvalidResponseError,
+)
+from .file_k_hash import (
+    FileKHash,
+    FileKHashFile,
+    FileKHashFileDecompileResult,
+    FileKHashFileDecompileResultKHashInfo,
+    FileKHashFileDecompileResultKHashInfoHash,
 )
 from .file_size import FileSize, FileSizeFile
 from .filename import Filename, FilenameFile
 from .function_info import (
     FunctionInfo,
     FunctionInfoFile,
     FunctionInfoFileDecompileResult,
@@ -90,14 +98,15 @@
     FunctionsInfoFileDecompileResultFunctionsPseudoCode,
 )
 from .input_types import (
     BindiffMatchInput,
     CreateFileInput,
     CreateMatchInput,
     CreateUploadTicketInput,
+    KHashInput,
     MatchTargetInput,
     OSSMatchInput,
     ReanalyzeInput,
     SearchBinaryInput,
     SearchBinaryStatisticInput,
     SearchCVESec,
     SearchFileInput,
@@ -110,28 +119,43 @@
     LicenseFileScainfo,
     LicenseFileScainfoLicenselist,
     LicenseFileScainfoLicenselistTags,
     LicenseFileScainfoLicenselistTagsCondition,
     LicenseFileScainfoLicenselistTagsForbidden,
     LicenseFileScainfoLicenselistTagsPermission,
 )
-from .license_short_name import LicenseShortName, LicenseShortNameFile, LicenseShortNameFileScainfo
-from .m_i_m_e_type import MIMEType, MIMETypeFile
-from .overview import Overview, OverviewFile, OverviewFileDecompileResult, OverviewFileDecompileResultBasicInfo
-from .reanalyze import Reanalyze, ReanalyzeReanalyze, ReanalyzeReanalyzeFile, ReanalyzeReanalyzeFileAnalyzeStatus
-from .s_c_a import SCA, SCAFile, SCAFileScainfo
-from .sha256 import Sha256, Sha256File
+from .license_short_name import (
+    LicenseShortName,
+    LicenseShortNameFile,
+    LicenseShortNameFileScainfo,
+)
+from .mime_type import MIMEType, MIMETypeFile
+from .overview import (
+    Overview,
+    OverviewFile,
+    OverviewFileDecompileResult,
+    OverviewFileDecompileResultBasicInfo,
+)
+from .reanalyze import (
+    Reanalyze,
+    ReanalyzeReanalyze,
+    ReanalyzeReanalyzeFile,
+    ReanalyzeReanalyzeFileAnalyzeStatus,
+)
+from .sca import SCA, SCAFile, SCAFileScainfo
+from .sha_256 import Sha256, Sha256File
 
 __all__ = [
     "ASCIIString",
     "ASCIIStringFile",
     "ASCIIStringFileExecutableCOFFInfo",
     "ASCIIStringFileExecutableELFInfo",
     "ASCIIStringFileExecutableMachoInfo",
     "ASCIIStringFileExecutablePEInfo",
+    "AnalyzeProgressStep",
     "AntivirusSafeLevel",
     "BaseClient",
     "BaseModel",
     "BindiffMatchInput",
     "CVEName",
     "CVENameFile",
     "CVENameFileScainfo",
@@ -157,14 +181,19 @@
     "CreateFileCreateFile",
     "CreateFileInput",
     "CreateMatchInput",
     "CreateUploadTicketInput",
     "DownloadLink",
     "DownloadLinkFile",
     "ExecuteType",
+    "FileKHash",
+    "FileKHashFile",
+    "FileKHashFileDecompileResult",
+    "FileKHashFileDecompileResultKHashInfo",
+    "FileKHashFileDecompileResultKHashInfoHash",
     "FileSize",
     "FileSizeFile",
     "FileType",
     "Filename",
     "FilenameFile",
     "FunctionInfo",
     "FunctionInfoFile",
@@ -188,15 +217,16 @@
     "FunctionsInfoFileDecompileResultFunctions",
     "FunctionsInfoFileDecompileResultFunctionsEmbedding",
     "FunctionsInfoFileDecompileResultFunctionsPseudoCode",
     "GraphQLClientError",
     "GraphQLClientGraphQLError",
     "GraphQLClientGraphQLMultiError",
     "GraphQLClientHttpError",
-    "GraphQlClientInvalidResponseError",
+    "GraphQLClientInvalidResponseError",
+    "KHashInput",
     "License",
     "LicenseFile",
     "LicenseFileScainfo",
     "LicenseFileScainfoLicenselist",
     "LicenseFileScainfoLicenselistTags",
     "LicenseFileScainfoLicenselistTagsCondition",
     "LicenseFileScainfoLicenselistTagsForbidden",
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/a_s_c_i_i_string.py` & `binaryai-0.8.0/src/binaryai/client_stub/ascii_string.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Annotated, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -12,43 +12,39 @@
     file: Optional["ASCIIStringFile"]
 
 
 class ASCIIStringFile(BaseModel):
     executable: Optional[
         Annotated[
             Union[
-                "ASCIIStringFileExecutableCOFFInfo",
                 "ASCIIStringFileExecutableELFInfo",
-                "ASCIIStringFileExecutableMachoInfo",
                 "ASCIIStringFileExecutablePEInfo",
+                "ASCIIStringFileExecutableMachoInfo",
+                "ASCIIStringFileExecutableCOFFInfo",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
-class ASCIIStringFileExecutableCOFFInfo(BaseModel):
-    typename__: Literal["COFFInfo"] = Field(alias="__typename")
+class ASCIIStringFileExecutableELFInfo(BaseModel):
+    typename__: Literal["ELFInfo"] = Field(alias="__typename")
     ascii_strings: Optional[List[str]] = Field(alias="asciiStrings")
 
 
-class ASCIIStringFileExecutableELFInfo(BaseModel):
-    typename__: Literal["ELFInfo"] = Field(alias="__typename")
+class ASCIIStringFileExecutablePEInfo(BaseModel):
+    typename__: Literal["PEInfo"] = Field(alias="__typename")
     ascii_strings: Optional[List[str]] = Field(alias="asciiStrings")
 
 
 class ASCIIStringFileExecutableMachoInfo(BaseModel):
     typename__: Literal["MachoInfo"] = Field(alias="__typename")
     ascii_strings: Optional[List[str]] = Field(alias="asciiStrings")
 
 
-class ASCIIStringFileExecutablePEInfo(BaseModel):
-    typename__: Literal["PEInfo"] = Field(alias="__typename")
+class ASCIIStringFileExecutableCOFFInfo(BaseModel):
+    typename__: Literal["COFFInfo"] = Field(alias="__typename")
     ascii_strings: Optional[List[str]] = Field(alias="asciiStrings")
 
 
 ASCIIString.model_rebuild()
 ASCIIStringFile.model_rebuild()
-ASCIIStringFileExecutableCOFFInfo.model_rebuild()
-ASCIIStringFileExecutableELFInfo.model_rebuild()
-ASCIIStringFileExecutableMachoInfo.model_rebuild()
-ASCIIStringFileExecutablePEInfo.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/base_client.py` & `binaryai-0.8.0/src/binaryai/client_stub/base_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 
 import json
 from typing import IO, Any, Dict, List, Optional, Tuple, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic_core import to_jsonable_python
 
 from .base_model import UNSET, Upload
-from .exceptions import GraphQLClientGraphQLMultiError, GraphQLClientHttpError, GraphQlClientInvalidResponseError
+from .exceptions import (
+    GraphQLClientGraphQLMultiError,
+    GraphQLClientHttpError,
+    GraphQLClientInvalidResponseError,
+)
 
 Self = TypeVar("Self", bound="BaseClient")
 
 
 class BaseClient:
     def __init__(
         self,
@@ -32,69 +36,98 @@
         self,
         exc_type: object,
         exc_val: object,
         exc_tb: object,
     ) -> None:
         self.http_client.close()
 
-    def execute(self, query: str, variables: Optional[Dict[str, Any]] = None) -> httpx.Response:
+    def execute(
+        self,
+        query: str,
+        operation_name: Optional[str] = None,
+        variables: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
+    ) -> httpx.Response:
         processed_variables, files, files_map = self._process_variables(variables)
-        payload: Dict[str, Any] = {"query": query, "variables": processed_variables}
 
         if files and files_map:
             return self._execute_multipart(
-                payload=payload,
+                query=query,
+                operation_name=operation_name,
+                variables=processed_variables,
                 files=files,
                 files_map=files_map,
+                **kwargs,
             )
 
-        return self._execute_json(payload=payload)
+        return self._execute_json(
+            query=query,
+            operation_name=operation_name,
+            variables=processed_variables,
+            **kwargs,
+        )
 
-    def get_data(self, response: httpx.Response) -> dict[str, Any]:
+    def get_data(self, response: httpx.Response) -> Dict[str, Any]:
         if not response.is_success:
-            raise GraphQLClientHttpError(status_code=response.status_code, response=response)
+            raise GraphQLClientHttpError(
+                status_code=response.status_code, response=response
+            )
 
         try:
             response_json = response.json()
         except ValueError as exc:
-            raise GraphQlClientInvalidResponseError(response=response) from exc
+            raise GraphQLClientInvalidResponseError(response=response) from exc
 
-        if (not isinstance(response_json, dict)) or ("data" not in response_json):
-            raise GraphQlClientInvalidResponseError(response=response)
+        if (not isinstance(response_json, dict)) or (
+            "data" not in response_json and "errors" not in response_json
+        ):
+            raise GraphQLClientInvalidResponseError(response=response)
 
-        data = response_json["data"]
+        data = response_json.get("data")
         errors = response_json.get("errors")
 
         if errors:
-            raise GraphQLClientGraphQLMultiError.from_errors_dicts(errors_dicts=errors, data=data)
+            raise GraphQLClientGraphQLMultiError.from_errors_dicts(
+                errors_dicts=errors, data=data
+            )
 
-        return cast(dict[str, Any], data)
+        return cast(Dict[str, Any], data)
 
     def _process_variables(
         self, variables: Optional[Dict[str, Any]]
-    ) -> Tuple[Dict[str, Any], Dict[str, Tuple[str, IO[bytes], str]], Dict[str, List[str]]]:
+    ) -> Tuple[
+        Dict[str, Any], Dict[str, Tuple[str, IO[bytes], str]], Dict[str, List[str]]
+    ]:
         if not variables:
             return {}, {}, {}
 
         serializable_variables = self._convert_dict_to_json_serializable(variables)
         return self._get_files_from_variables(serializable_variables)
 
-    def _convert_dict_to_json_serializable(self, dict_: Dict[str, Any]) -> Dict[str, Any]:
-        return {key: self._convert_value(value) for key, value in dict_.items() if value is not UNSET}
+    def _convert_dict_to_json_serializable(
+        self, dict_: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        return {
+            key: self._convert_value(value)
+            for key, value in dict_.items()
+            if value is not UNSET
+        }
 
     def _convert_value(self, value: Any) -> Any:
         if isinstance(value, BaseModel):
             return value.model_dump(by_alias=True, exclude_unset=True)
         if isinstance(value, list):
             return [self._convert_value(item) for item in value]
         return value
 
     def _get_files_from_variables(
         self, variables: Dict[str, Any]
-    ) -> Tuple[Dict[str, Any], Dict[str, Tuple[str, IO[bytes], str]], Dict[str, List[str]]]:
+    ) -> Tuple[
+        Dict[str, Any], Dict[str, Tuple[str, IO[bytes], str]], Dict[str, List[str]]
+    ]:
         files_map: Dict[str, List[str]] = {}
         files_list: List[Upload] = []
 
         def separate_files(path: str, obj: Any) -> Any:
             if isinstance(obj, list):
                 nulled_list = []
                 for index, value in enumerate(obj):
@@ -126,21 +159,53 @@
             str(i): (file_.filename, cast(IO[bytes], file_.content), file_.content_type)
             for i, file_ in enumerate(files_list)
         }
         return nulled_variables, files, files_map
 
     def _execute_multipart(
         self,
-        payload: Dict[str, Any],
+        query: str,
+        operation_name: Optional[str],
+        variables: Dict[str, Any],
         files: Dict[str, Tuple[str, IO[bytes], str]],
         files_map: Dict[str, List[str]],
+        **kwargs: Any,
     ) -> httpx.Response:
         data = {
-            "operations": json.dumps(payload, default=to_jsonable_python),
+            "operations": json.dumps(
+                {
+                    "query": query,
+                    "operationName": operation_name,
+                    "variables": variables,
+                },
+                default=to_jsonable_python,
+            ),
             "map": json.dumps(files_map, default=to_jsonable_python),
         }
 
-        return self.http_client.post(url=self.url, data=data, files=files)
+        return self.http_client.post(url=self.url, data=data, files=files, **kwargs)
+
+    def _execute_json(
+        self,
+        query: str,
+        operation_name: Optional[str],
+        variables: Dict[str, Any],
+        **kwargs: Any,
+    ) -> httpx.Response:
+        headers: Dict[str, str] = {"Content-Type": "application/json"}
+        headers.update(kwargs.get("headers", {}))
+
+        merged_kwargs: Dict[str, Any] = kwargs.copy()
+        merged_kwargs["headers"] = headers
 
-    def _execute_json(self, payload: Dict[str, Any]) -> httpx.Response:
-        content = json.dumps(payload, default=to_jsonable_python)
-        return self.http_client.post(url=self.url, content=content, headers={"Content-Type": "application/json"})
+        return self.http_client.post(
+            url=self.url,
+            content=json.dumps(
+                {
+                    "query": query,
+                    "operationName": operation_name,
+                    "variables": variables,
+                },
+                default=to_jsonable_python,
+            ),
+            **merged_kwargs,
+        )
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/base_model.py` & `binaryai-0.8.0/src/binaryai/client_stub/base_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 
 from io import IOBase
 
-from pydantic import BaseModel as PydanticBaseModel
-from pydantic import ConfigDict
+from pydantic import BaseModel as PydanticBaseModel, ConfigDict
 
 
 class UnsetType:
     def __bool__(self) -> bool:
         return False
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/c_v_e_name.py` & `binaryai-0.8.0/src/binaryai/client_stub/cve_name.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import List, Optional
 
 from .base_model import BaseModel
 
 
@@ -21,8 +21,7 @@
 class CVENameFileScainfoCves(BaseModel):
     name: str
 
 
 CVEName.model_rebuild()
 CVENameFile.model_rebuild()
 CVENameFileScainfo.model_rebuild()
-CVENameFileScainfoCves.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/check_or_upload.py` & `binaryai-0.8.0/src/binaryai/client_stub/check_or_upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import List, Literal, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class CheckOrUpload(BaseModel):
     create_upload_ticket: Union[
-        "CheckOrUploadCreateUploadTicketFile",
-        "CheckOrUploadCreateUploadTicketOwnershipTicket",
         "CheckOrUploadCreateUploadTicketUploadTicket",
+        "CheckOrUploadCreateUploadTicketOwnershipTicket",
+        "CheckOrUploadCreateUploadTicketFile",
     ] = Field(alias="createUploadTicket", discriminator="typename__")
 
 
-class CheckOrUploadCreateUploadTicketFile(BaseModel):
-    typename__: Literal["File"] = Field(alias="__typename")
-    sha256: str
-
-
-class CheckOrUploadCreateUploadTicketOwnershipTicket(BaseModel):
-    typename__: Literal["OwnershipTicket"] = Field(alias="__typename")
-    ticket_i_d: str = Field(alias="ticketID")
-    secret_prepend: str = Field(alias="secretPrepend")
-    secret_append: str = Field(alias="secretAppend")
-
-
 class CheckOrUploadCreateUploadTicketUploadTicket(BaseModel):
     typename__: Literal["UploadTicket"] = Field(alias="__typename")
-    ticket_i_d: str = Field(alias="ticketID")
+    ticket_id: str = Field(alias="ticketID")
     url: str
-    request_headers: List["CheckOrUploadCreateUploadTicketUploadTicketRequestHeaders"] = Field(alias="requestHeaders")
+    request_headers: List[
+        "CheckOrUploadCreateUploadTicketUploadTicketRequestHeaders"
+    ] = Field(alias="requestHeaders")
 
 
 class CheckOrUploadCreateUploadTicketUploadTicketRequestHeaders(BaseModel):
     key: str
     value: str
 
 
+class CheckOrUploadCreateUploadTicketOwnershipTicket(BaseModel):
+    typename__: Literal["OwnershipTicket"] = Field(alias="__typename")
+    ticket_id: str = Field(alias="ticketID")
+    secret_prepend: str = Field(alias="secretPrepend")
+    secret_append: str = Field(alias="secretAppend")
+
+
+class CheckOrUploadCreateUploadTicketFile(BaseModel):
+    typename__: Literal["File"] = Field(alias="__typename")
+    sha_256: str = Field(alias="sha256")
+
+
 CheckOrUpload.model_rebuild()
-CheckOrUploadCreateUploadTicketFile.model_rebuild()
-CheckOrUploadCreateUploadTicketOwnershipTicket.model_rebuild()
 CheckOrUploadCreateUploadTicketUploadTicket.model_rebuild()
-CheckOrUploadCreateUploadTicketUploadTicketRequestHeaders.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/check_state.py` & `binaryai-0.8.0/src/binaryai/client_stub/check_state.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -10,18 +10,24 @@
 
 
 class CheckState(BaseModel):
     file: Optional["CheckStateFile"]
 
 
 class CheckStateFile(BaseModel):
-    smart_binary_status: Optional["CheckStateFileSmartBinaryStatus"] = Field(alias="smartBinaryStatus")
-    smart_beat_status: Optional["CheckStateFileSmartBeatStatus"] = Field(alias="smartBeatStatus")
+    smart_binary_status: Optional["CheckStateFileSmartBinaryStatus"] = Field(
+        alias="smartBinaryStatus"
+    )
+    smart_beat_status: Optional["CheckStateFileSmartBeatStatus"] = Field(
+        alias="smartBeatStatus"
+    )
     text: Optional["CheckStateFileText"]
-    decompile_result: Optional["CheckStateFileDecompileResult"] = Field(alias="decompileResult")
+    decompile_result: Optional["CheckStateFileDecompileResult"] = Field(
+        alias="decompileResult"
+    )
 
 
 class CheckStateFileSmartBinaryStatus(BaseModel):
     status: Status
 
 
 class CheckStateFileSmartBeatStatus(BaseModel):
@@ -38,12 +44,8 @@
 
 class CheckStateFileDecompileResultBasicInfo(BaseModel):
     file_type: str = Field(alias="fileType")
 
 
 CheckState.model_rebuild()
 CheckStateFile.model_rebuild()
-CheckStateFileSmartBinaryStatus.model_rebuild()
-CheckStateFileSmartBeatStatus.model_rebuild()
-CheckStateFileText.model_rebuild()
 CheckStateFileDecompileResult.model_rebuild()
-CheckStateFileDecompileResultBasicInfo.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/compressed_file.py` & `binaryai-0.8.0/src/binaryai/client_stub/compressed_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Annotated, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -13,30 +13,28 @@
 
 
 class CompressedFileFile(BaseModel):
     decompressed: Optional[
         List[
             Annotated[
                 Union[
-                    "CompressedFileFileDecompressedCompressedDirectory",
                     "CompressedFileFileDecompressedCompressedFile",
+                    "CompressedFileFileDecompressedCompressedDirectory",
                 ],
                 Field(discriminator="typename__"),
             ]
         ]
     ]
 
 
-class CompressedFileFileDecompressedCompressedDirectory(BaseModel):
-    typename__: Literal["CompressedDirectory"] = Field(alias="__typename")
-
-
 class CompressedFileFileDecompressedCompressedFile(BaseModel):
     typename__: Literal["CompressedFile"] = Field(alias="__typename")
     path: str
-    sha256: str
+    sha_256: str = Field(alias="sha256")
+
+
+class CompressedFileFileDecompressedCompressedDirectory(BaseModel):
+    typename__: Literal["CompressedDirectory"] = Field(alias="__typename")
 
 
 CompressedFile.model_rebuild()
 CompressedFileFile.model_rebuild()
-CompressedFileFileDecompressedCompressedDirectory.model_rebuild()
-CompressedFileFileDecompressedCompressedFile.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/create_file.py` & `binaryai-0.8.0/src/binaryai/client_stub/create_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Any, List
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class CreateFile(BaseModel):
     create_file: "CreateFileCreateFile" = Field(alias="createFile")
 
 
 class CreateFileCreateFile(BaseModel):
-    sha256: str
-    md5: str
+    sha_256: str = Field(alias="sha256")
+    md_5: str = Field(alias="md5")
     name: List[str]
     size: int
     mime_type: str = Field(alias="mimeType")
     create_time: Any = Field(alias="createTime")
 
 
 CreateFile.model_rebuild()
-CreateFileCreateFile.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/enums.py` & `binaryai-0.8.0/src/binaryai/client_stub/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: https://api.binaryai.cn/v1/endpoint
 
 from enum import Enum
 
 
+class AnalyzeProgressStep(str, Enum):
+    Begin = "Begin"
+    Done = "Done"
+    AutoAnalysis = "AutoAnalysis"
+    Decompile = "Decompile"
+    FeatureForward = "FeatureForward"
+    EmbedRecall = "EmbedRecall"
+    EmbedRank = "EmbedRank"
+    ResultUpload = "ResultUpload"
+
+
 class AntivirusSafeLevel(str, Enum):
-    INFECTED = "INFECTED"
-    MALICIOUS = "MALICIOUS"
-    MALICIOUS_FORCE = "MALICIOUS_FORCE"
-    MALICIOUS_WEAK = "MALICIOUS_WEAK"
-    SAFE = "SAFE"
+    UNKNOWN = "UNKNOWN"
     SAFE_FORCE = "SAFE_FORCE"
+    SAFE = "SAFE"
     SAFE_WEAK = "SAFE_WEAK"
     UNDETECTED = "UNDETECTED"
-    UNKNOWN = "UNKNOWN"
+    MALICIOUS_WEAK = "MALICIOUS_WEAK"
+    MALICIOUS = "MALICIOUS"
+    MALICIOUS_FORCE = "MALICIOUS_FORCE"
+    INFECTED = "INFECTED"
 
 
 class ExecuteType(str, Enum):
-    FileMeta = "FileMeta"
-    SmartBeat = "SmartBeat"
     SmartBinary = "SmartBinary"
     SmartExtractor = "SmartExtractor"
+    FileMeta = "FileMeta"
+    SmartBeat = "SmartBeat"
 
 
 class FileType(str, Enum):
-    COFF = "COFF"
     ELF = "ELF"
-    Macho = "Macho"
     PE = "PE"
+    Macho = "Macho"
+    COFF = "COFF"
 
 
 class MatchAlgorithm(str, Enum):
     Normal = "Normal"
     Professional = "Professional"
 
 
 class NoopReason(str, Enum):
     AlreadyRunning = "AlreadyRunning"
-    RateLimited = "RateLimited"
     WouldNotChange = "WouldNotChange"
+    RateLimited = "RateLimited"
 
 
 class PseudoCodeAnnotationType(str, Enum):
     HAS_FUNC_DEF = "HAS_FUNC_DEF"
     HAS_XREF = "HAS_XREF"
 
 
 class RelroLevel(str, Enum):
-    Full = "Full"
     No = "No"
+    Full = "Full"
     Partial = "Partial"
 
 
 class SCAAlgo(str, Enum):
     NORMAL = "NORMAL"
     PROFESSIONAL = "PROFESSIONAL"
 
 
 class SearchBinaryStatisticKey(str, Enum):
-    THIRD_LIB_CVE_NAME = "THIRD_LIB_CVE_NAME"
     THIRD_LIB_NAME = "THIRD_LIB_NAME"
     THIRD_LIB_VERSION = "THIRD_LIB_VERSION"
+    THIRD_LIB_CVE_NAME = "THIRD_LIB_CVE_NAME"
 
 
 class Status(str, Enum):
-    Fail = "Fail"
     Ready = "Ready"
+    Waiting = "Waiting"
     Running = "Running"
     Success = "Success"
+    Fail = "Fail"
     Timeout = "Timeout"
-    Waiting = "Waiting"
 
 
 class SymbolType(str, Enum):
-    DATA_LABEL = "DATA_LABEL"
     FUNCTION = "FUNCTION"
     THUNK_FUNCTION = "THUNK_FUNCTION"
+    DATA_LABEL = "DATA_LABEL"
 
 
 class XRefType(str, Enum):
     CALL = "CALL"
     DATA = "DATA"
     STRING = "STRING"
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/exceptions.py` & `binaryai-0.8.0/src/binaryai/client_stub/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
@@ -14,15 +14,15 @@
         self.status_code = status_code
         self.response = response
 
     def __str__(self) -> str:
         return f"HTTP status code: {self.status_code}"
 
 
-class GraphQlClientInvalidResponseError(GraphQLClientError):
+class GraphQLClientInvalidResponseError(GraphQLClientError):
     def __init__(self, response: httpx.Response) -> None:
         self.response = response
 
     def __str__(self) -> str:
         return "Invalid response format."
 
 
@@ -52,24 +52,28 @@
             path=error.get("path"),
             extensions=error.get("extensions"),
             orginal=error,
         )
 
 
 class GraphQLClientGraphQLMultiError(GraphQLClientError):
-    def __init__(self, errors: List[GraphQLClientGraphQLError], data: Dict[str, Any]):
+    def __init__(
+        self,
+        errors: List[GraphQLClientGraphQLError],
+        data: Optional[Dict[str, Any]] = None,
+    ):
         self.errors = errors
         self.data = data
 
     def __str__(self) -> str:
         return "; ".join(str(e) for e in self.errors)
 
     @classmethod
     def from_errors_dicts(
-        cls, errors_dicts: List[Dict[str, Any]], data: Dict[str, Any]
+        cls, errors_dicts: List[Dict[str, Any]], data: Optional[Dict[str, Any]] = None
     ) -> "GraphQLClientGraphQLMultiError":
         return cls(
             errors=[GraphQLClientGraphQLError.from_dict(e) for e in errors_dicts],
             data=data,
         )
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/function_info.py` & `binaryai-0.8.0/src/binaryai/client_stub/function_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class FunctionInfo(BaseModel):
     file: Optional["FunctionInfoFile"]
 
 
 class FunctionInfoFile(BaseModel):
-    decompile_result: Optional["FunctionInfoFileDecompileResult"] = Field(alias="decompileResult")
+    decompile_result: Optional["FunctionInfoFileDecompileResult"] = Field(
+        alias="decompileResult"
+    )
 
 
 class FunctionInfoFileDecompileResult(BaseModel):
     function: Optional["FunctionInfoFileDecompileResultFunction"]
 
 
 class FunctionInfoFileDecompileResultFunction(BaseModel):
     offset: Any
     name: str
     embedding: Optional["FunctionInfoFileDecompileResultFunctionEmbedding"] = None
-    pseudo_code: Optional["FunctionInfoFileDecompileResultFunctionPseudoCode"] = Field(alias="pseudoCode")
+    pseudo_code: Optional["FunctionInfoFileDecompileResultFunctionPseudoCode"] = Field(
+        alias="pseudoCode"
+    )
 
 
 class FunctionInfoFileDecompileResultFunctionEmbedding(BaseModel):
     vector: List[float]
     version: str
 
 
@@ -36,9 +40,7 @@
     code: str
 
 
 FunctionInfo.model_rebuild()
 FunctionInfoFile.model_rebuild()
 FunctionInfoFileDecompileResult.model_rebuild()
 FunctionInfoFileDecompileResultFunction.model_rebuild()
-FunctionInfoFileDecompileResultFunctionEmbedding.model_rebuild()
-FunctionInfoFileDecompileResultFunctionPseudoCode.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/function_list.py` & `binaryai-0.8.0/src/binaryai/client_stub/function_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class FunctionList(BaseModel):
     file: Optional["FunctionListFile"]
 
 
 class FunctionListFile(BaseModel):
-    decompile_result: Optional["FunctionListFileDecompileResult"] = Field(alias="decompileResult")
+    decompile_result: Optional["FunctionListFileDecompileResult"] = Field(
+        alias="decompileResult"
+    )
 
 
 class FunctionListFileDecompileResult(BaseModel):
     functions: Optional[List["FunctionListFileDecompileResultFunctions"]]
 
 
 class FunctionListFileDecompileResultFunctions(BaseModel):
     offset: Any
 
 
 FunctionList.model_rebuild()
 FunctionListFile.model_rebuild()
 FunctionListFileDecompileResult.model_rebuild()
-FunctionListFileDecompileResultFunctions.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/function_match.py` & `binaryai-0.8.0/src/binaryai/client_stub/function_match.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class FunctionMatch(BaseModel):
     file: Optional["FunctionMatchFile"]
 
 
 class FunctionMatchFile(BaseModel):
-    decompile_result: Optional["FunctionMatchFileDecompileResult"] = Field(alias="decompileResult")
+    decompile_result: Optional["FunctionMatchFileDecompileResult"] = Field(
+        alias="decompileResult"
+    )
 
 
 class FunctionMatchFileDecompileResult(BaseModel):
     function: Optional["FunctionMatchFileDecompileResultFunction"]
 
 
 class FunctionMatchFileDecompileResultFunction(BaseModel):
@@ -34,8 +36,7 @@
 
 
 FunctionMatch.model_rebuild()
 FunctionMatchFile.model_rebuild()
 FunctionMatchFileDecompileResult.model_rebuild()
 FunctionMatchFileDecompileResultFunction.model_rebuild()
 FunctionMatchFileDecompileResultFunctionMatch.model_rebuild()
-FunctionMatchFileDecompileResultFunctionMatchFunction.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/functions_info.py` & `binaryai-0.8.0/src/binaryai/client_stub/functions_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class FunctionsInfo(BaseModel):
     file: Optional["FunctionsInfoFile"]
 
 
 class FunctionsInfoFile(BaseModel):
-    decompile_result: Optional["FunctionsInfoFileDecompileResult"] = Field(alias="decompileResult")
+    decompile_result: Optional["FunctionsInfoFileDecompileResult"] = Field(
+        alias="decompileResult"
+    )
 
 
 class FunctionsInfoFileDecompileResult(BaseModel):
     functions: Optional[List["FunctionsInfoFileDecompileResultFunctions"]]
 
 
 class FunctionsInfoFileDecompileResultFunctions(BaseModel):
     offset: Any
     name: str
     embedding: Optional["FunctionsInfoFileDecompileResultFunctionsEmbedding"] = None
-    pseudo_code: Optional["FunctionsInfoFileDecompileResultFunctionsPseudoCode"] = Field(alias="pseudoCode")
+    pseudo_code: Optional[
+        "FunctionsInfoFileDecompileResultFunctionsPseudoCode"
+    ] = Field(alias="pseudoCode")
 
 
 class FunctionsInfoFileDecompileResultFunctionsEmbedding(BaseModel):
     vector: List[float]
     version: str
 
 
@@ -36,9 +40,7 @@
     code: str
 
 
 FunctionsInfo.model_rebuild()
 FunctionsInfoFile.model_rebuild()
 FunctionsInfoFileDecompileResult.model_rebuild()
 FunctionsInfoFileDecompileResultFunctions.model_rebuild()
-FunctionsInfoFileDecompileResultFunctionsEmbedding.model_rebuild()
-FunctionsInfoFileDecompileResultFunctionsPseudoCode.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/input_types.py` & `binaryai-0.8.0/src/binaryai/client_stub/input_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,85 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: https://api.binaryai.cn/v1/endpoint
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import FileType, SearchBinaryStatisticKey, SymbolType
 
 
 class BindiffMatchInput(BaseModel):
-    sha256: str
+    sha_256: str = Field(alias="sha256")
 
 
 class CreateFileInput(BaseModel):
+    ticket_id: str = Field(alias="ticketID")
     ownership_po_s: Optional[str] = Field(alias="ownershipPoS", default=None)
-    ticket_i_d: str = Field(alias="ticketID")
 
 
 class CreateMatchInput(BaseModel):
-    sha256: str
+    sha_256: str = Field(alias="sha256")
     target: "MatchTargetInput"
 
 
 class CreateUploadTicketInput(BaseModel):
-    captcha_random_string: Optional[str] = Field(alias="captchaRandomString", default=None)
-    captcha_ticket: Optional[str] = Field(alias="captchaTicket", default=None)
-    md5: Optional[str] = None
+    sha_256: Optional[str] = Field(alias="sha256", default=None)
+    md_5: Optional[str] = Field(alias="md5", default=None)
     name: Optional[str] = None
-    sha256: Optional[str] = None
+    captcha_ticket: Optional[str] = Field(alias="captchaTicket", default=None)
+    captcha_random_string: Optional[str] = Field(
+        alias="captchaRandomString", default=None
+    )
+
+
+class KHashInput(BaseModel):
+    hash_hexlified_string: str = Field(alias="hashHexlifiedString")
+    version: str
+    bit_size: int = Field(alias="bitSize")
 
 
 class MatchTargetInput(BaseModel):
     bindiff: Optional["BindiffMatchInput"] = None
     oss: Optional["OSSMatchInput"] = None
 
 
 class OSSMatchInput(BaseModel):
-    repo_u_r_ls: Optional[List[str]] = Field(alias="repoURLs", default=None)
+    repo_ur_ls: Optional[List[str]] = Field(alias="repoURLs", default=None)
 
 
 class ReanalyzeInput(BaseModel):
-    sha256: str
+    sha_256: str = Field(alias="sha256")
     skip_version_check: Optional[bool] = Field(alias="skipVersionCheck", default=None)
 
 
 class SearchBinaryInput(BaseModel):
-    include_type: Optional[List[FileType]] = Field(alias="includeType", default=None)
-    keyword: Optional[str] = None
-    limit: Optional[int] = None
     offset: Optional[int] = None
-    statistic: Optional[List["SearchBinaryStatisticInput"]] = None
+    limit: Optional[int] = None
+    keyword: Optional[str] = None
+    include_type: Optional[List[FileType]] = Field(alias="includeType", default=None)
     third_lib: Optional[List["SearchThirdLib"]] = Field(alias="thirdLib", default=None)
+    statistic: Optional[List["SearchBinaryStatisticInput"]] = None
 
 
 class SearchBinaryStatisticInput(BaseModel):
     keys: List[SearchBinaryStatisticKey]
 
 
 class SearchCVESec(BaseModel):
     name: str
 
 
 class SearchFileInput(BaseModel):
-    md5: Optional[str] = None
-    sha256: Optional[str] = None
+    sha_256: Optional[str] = Field(alias="sha256", default=None)
+    md_5: Optional[str] = Field(alias="md5", default=None)
 
 
 class SearchThirdLib(BaseModel):
-    cves: Optional[List["SearchCVESec"]] = None
     name: Optional[str] = None
     version: Optional[List[str]] = None
+    cves: Optional[List["SearchCVESec"]] = None
 
 
 class SymbolTableFilter(BaseModel):
     symbol_type: Optional[List[SymbolType]] = Field(alias="symbolType", default=None)
-
-
-BindiffMatchInput.model_rebuild()
-CreateFileInput.model_rebuild()
-CreateMatchInput.model_rebuild()
-CreateUploadTicketInput.model_rebuild()
-MatchTargetInput.model_rebuild()
-OSSMatchInput.model_rebuild()
-ReanalyzeInput.model_rebuild()
-SearchBinaryInput.model_rebuild()
-SearchBinaryStatisticInput.model_rebuild()
-SearchCVESec.model_rebuild()
-SearchFileInput.model_rebuild()
-SearchThirdLib.model_rebuild()
-SymbolTableFilter.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/license.py` & `binaryai-0.8.0/src/binaryai/client_stub/license.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -55,10 +55,7 @@
 
 
 License.model_rebuild()
 LicenseFile.model_rebuild()
 LicenseFileScainfo.model_rebuild()
 LicenseFileScainfoLicenselist.model_rebuild()
 LicenseFileScainfoLicenselistTags.model_rebuild()
-LicenseFileScainfoLicenselistTagsPermission.model_rebuild()
-LicenseFileScainfoLicenselistTagsCondition.model_rebuild()
-LicenseFileScainfoLicenselistTagsForbidden.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/overview.py` & `binaryai-0.8.0/src/binaryai/client_stub/overview.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
 class Overview(BaseModel):
     file: Optional["OverviewFile"]
 
 
 class OverviewFile(BaseModel):
-    decompile_result: Optional["OverviewFileDecompileResult"] = Field(alias="decompileResult")
+    decompile_result: Optional["OverviewFileDecompileResult"] = Field(
+        alias="decompileResult"
+    )
 
 
 class OverviewFileDecompileResult(BaseModel):
     basic_info: "OverviewFileDecompileResultBasicInfo" = Field(alias="basicInfo")
 
 
 class OverviewFileDecompileResultBasicInfo(BaseModel):
@@ -29,8 +31,7 @@
     entry_point: Optional[Any] = Field(alias="entryPoint")
     base_address: Optional[Any] = Field(alias="baseAddress")
 
 
 Overview.model_rebuild()
 OverviewFile.model_rebuild()
 OverviewFileDecompileResult.model_rebuild()
-OverviewFileDecompileResultBasicInfo.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/client_stub/reanalyze.py` & `binaryai-0.8.0/src/binaryai/client_stub/reanalyze.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-09-18 11:53
+# Generated by ariadne-codegen
 # Source: ./src/binaryai/query.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -15,18 +15,19 @@
 
 class ReanalyzeReanalyze(BaseModel):
     noop_reason: Optional[NoopReason] = Field(alias="noopReason")
     file: "ReanalyzeReanalyzeFile"
 
 
 class ReanalyzeReanalyzeFile(BaseModel):
-    analyze_status: Optional["ReanalyzeReanalyzeFileAnalyzeStatus"] = Field(alias="analyzeStatus")
+    analyze_status: Optional["ReanalyzeReanalyzeFileAnalyzeStatus"] = Field(
+        alias="analyzeStatus"
+    )
 
 
 class ReanalyzeReanalyzeFileAnalyzeStatus(BaseModel):
     status: Status
 
 
 Reanalyze.model_rebuild()
 ReanalyzeReanalyze.model_rebuild()
 ReanalyzeReanalyzeFile.model_rebuild()
-ReanalyzeReanalyzeFileAnalyzeStatus.model_rebuild()
```

### Comparing `binaryai-0.7.1/src/binaryai/function.py` & `binaryai-0.8.0/src/binaryai/function.py`

 * *Files identical despite different names*

### Comparing `binaryai-0.7.1/src/binaryai/license.py` & `binaryai-0.8.0/src/binaryai/license.py`

 * *Files identical despite different names*

### Comparing `binaryai-0.7.1/src/binaryai/query.graphql` & `binaryai-0.8.0/src/binaryai/query.graphql`

 * *Files 19% similar despite different names*

```diff
@@ -1,178 +1,169 @@
 query Sha256($md5: String!) {
-  file: fileByHash(input: {md5: $md5}) {
-    sha256
-  }
+    file: fileByHash(input: { md5: $md5 }) {
+        sha256
+    }
 }
 
-
 query Filename($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    name
-  }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        name
+    }
 }
 
-
 query MIMEType($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    mimeType
-  }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        mimeType
+    }
 }
 
-
 query FileSize($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    size
-  }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        size
+    }
 }
 
-
 query CVEName($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    scainfo {
-      cves {
-        name
-      }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        scainfo {
+            cves {
+                name
+            }
+        }
     }
-  }
 }
 
-
 query LicenseShortName($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    scainfo {
-      license
+    file: fileByHash(input: { sha256: $sha256 }) {
+        scainfo {
+            license
+        }
     }
-  }
 }
 
-
 query License($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    scainfo {
-      licenselist {
-        checkreason
-        content
-        extra
-        fullName
-        pass
-        risk
-        shortName
-        source
-        url
-        tags {
-          permission {
-            tagName
-            description
-          }
-          condition {
-            tagName
-            description
-          }
-          forbidden {
-            tagName
-            description
-          }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        scainfo {
+            licenselist {
+                checkreason
+                content
+                extra
+                fullName
+                pass
+                risk
+                shortName
+                source
+                url
+                tags {
+                    permission {
+                        tagName
+                        description
+                    }
+                    condition {
+                        tagName
+                        description
+                    }
+                    forbidden {
+                        tagName
+                        description
+                    }
+                }
+            }
         }
-      }
     }
-  }
 }
 
-
 query ASCIIString($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    executable {
-      ... on COFFInfo {
-        asciiStrings
-      }
-      ... on ELFInfo {
-        asciiStrings
-      }
-      ... on MachoInfo {
-        asciiStrings
-      }
-      ... on PEInfo {
-        asciiStrings
-      }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        executable {
+            ... on COFFInfo {
+                asciiStrings
+            }
+            ... on ELFInfo {
+                asciiStrings
+            }
+            ... on MachoInfo {
+                asciiStrings
+            }
+            ... on PEInfo {
+                asciiStrings
+            }
+        }
     }
-  }
 }
 
-
 query SCA($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    scainfo {
-      name
-      version
-      description
-      sourceCodeURL
-      summary
+    file: fileByHash(input: { sha256: $sha256 }) {
+        scainfo {
+            name
+            version
+            description
+            sourceCodeURL
+            summary
+        }
     }
-  }
 }
 
-
 query Overview($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    decompileResult {
-      basicInfo {
-        fileType
-        machine
-        platform
-        endian
-        loader
-        entryPoint
-        baseAddress
-      }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        decompileResult {
+            basicInfo {
+                fileType
+                machine
+                platform
+                endian
+                loader
+                entryPoint
+                baseAddress
+            }
+        }
     }
-  }
 }
 
-
 query DownloadLink($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    downloadLink
-  }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        downloadLink
+    }
 }
 
-
 query CheckState($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    smartBinaryStatus : analyzeStatus(analyzer: SmartBinary) {
-      status
-    }
-    smartBeatStatus : analyzeStatus(analyzer: SmartBeat) {
-      status
-    }
-    text {
-      content           # trigger smartBinary
-    }
-    decompileResult {
-      basicInfo {
-        fileType        # trigger smartBeat
-      }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        smartBinaryStatus: analyzeStatus(analyzer: SmartBinary) {
+            status
+        }
+        smartBeatStatus: analyzeStatus(analyzer: SmartBeat) {
+            status
+        }
+        text {
+            content # trigger smartBinary
+        }
+        decompileResult {
+            basicInfo {
+                fileType # trigger smartBeat
+            }
+        }
     }
-  }
 }
 
-
 query FunctionList($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    decompileResult {
-      functions {
-        offset
-      }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        decompileResult {
+            functions {
+                offset
+            }
+        }
     }
-  }
 }
 
-
-query FunctionInfo($sha256: String!, $offset: BigInt!, $withEmbedding: Boolean!) {
-    file: fileByHash(input: {sha256: $sha256}) {
+query FunctionInfo(
+    $sha256: String!
+    $offset: BigInt!
+    $withEmbedding: Boolean!
+) {
+    file: fileByHash(input: { sha256: $sha256 }) {
         decompileResult {
             function(offset: $offset) {
                 offset
                 name
                 embedding @include(if: $withEmbedding) {
                     vector
                     version
@@ -181,17 +172,20 @@
                     code
                 }
             }
         }
     }
 }
 
-
-query FunctionsInfo($sha256: String!, $offset: [BigInt!], $withEmbedding: Boolean!) {
-    file: fileByHash(input: {sha256: $sha256}) {
+query FunctionsInfo(
+    $sha256: String!
+    $offset: [BigInt!]
+    $withEmbedding: Boolean!
+) {
+    file: fileByHash(input: { sha256: $sha256 }) {
         decompileResult {
             functions(offset: $offset) {
                 offset
                 name
                 embedding @include(if: $withEmbedding) {
                     vector
                     version
@@ -200,81 +194,89 @@
                     code
                 }
             }
         }
     }
 }
 
-
 query FunctionMatch($sha256: String!, $offset: BigInt!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    decompileResult {
-      function(offset: $offset) {
-        match(topK: 10) {
-          score
-          function {
-            code
-          }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        decompileResult {
+            function(offset: $offset) {
+                match(topK: 10) {
+                    score
+                    function {
+                        code
+                    }
+                }
+            }
         }
-      }
     }
-  }
 }
 
+query FileKHash($sha256: String!) {
+    file: fileByHash(input: { sha256: $sha256 }) {
+        decompileResult {
+            kHashInfo {
+                hash {
+                    hash
+                    version
+                }
+            }
+        }
+    }
+}
 
 query CompressedFile($sha256: String!) {
-  file: fileByHash(input: {sha256: $sha256}) {
-    decompressed {
-      ... on CompressedFile {
-        path
-        sha256
-      }
+    file: fileByHash(input: { sha256: $sha256 }) {
+        decompressed {
+            ... on CompressedFile {
+                path
+                sha256
+            }
+        }
     }
-  }
 }
 
-
 mutation Reanalyze($input: ReanalyzeInput!) {
-  reanalyze(input: $input) {
-    noopReason
-    file {
-      analyzeStatus {
-        status
-      }
+    reanalyze(input: $input) {
+        noopReason
+        file {
+            analyzeStatus {
+                status
+            }
+        }
     }
-  }
 }
 
 mutation CheckOrUpload($input: CreateUploadTicketInput!) {
-  createUploadTicket(input: $input) {
-    __typename
-    ... on File {
-      sha256
-    }
-    ... on UploadTicket {
-      ticketID
-      url
-      requestHeaders {
-        key
-        value
-      }
-    }
-    ... on OwnershipTicket {
-      ticketID
-      secretPrepend
-      secretAppend
+    createUploadTicket(input: $input) {
+        __typename
+        ... on File {
+            sha256
+        }
+        ... on UploadTicket {
+            ticketID
+            url
+            requestHeaders {
+                key
+                value
+            }
+        }
+        ... on OwnershipTicket {
+            ticketID
+            secretPrepend
+            secretAppend
+        }
     }
-  }
 }
 
-
 mutation CreateFile($input: CreateFileInput!) {
-  createFile(input: $input) {
-    sha256
-    md5
-    name
-    size
-    mimeType
-    createTime
-  }
+    createFile(input: $input) {
+        sha256
+        md5
+        name
+        size
+        mimeType
+        createTime
+    }
 }
-
```

### Comparing `binaryai-0.7.1/src/binaryai/upload.py` & `binaryai-0.8.0/src/binaryai/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,33 +62,33 @@
         """
         Starts the upload sequence.
         """
         ticket = self.__create_ticket(filename=self._filename, sha256=self._sha256, md5=self._md5)
         ticket_type = ticket.typename__
 
         if ticket_type == "File":
-            return ticket.sha256
+            return ticket.sha_256
 
         reply_pos = None
 
         if ticket_type == "OwnershipTicket":
             logger.info("calculate pos")
             reply_pos = self.__reply_ticket_pos(ticket)
         elif ticket_type == "UploadTicket":
             logger.info("uploading file")
             self.__reply_ticket_upload(ticket)
         else:
             raise ValueError("unknown upload type, upgrade SDK or contact developers")
 
-        ticket_id = ticket.ticket_i_d
+        ticket_id = ticket.ticket_id
         logger.info("creating file")
         req = client_stub.CreateFileInput(ticketID=ticket_id, ownershipPoS=reply_pos)
         verify_response = self._client.create_file(req)
 
-        return verify_response.create_file.sha256
+        return verify_response.create_file.sha_256
 
     def __create_ticket(
         self, *, filename: Optional[str] = None, sha256: Optional[str] = None, md5: Optional[str] = None
     ):
         """
         Checks if file exists on FileManager with filename and file's hashsum.
         """
```

### Comparing `binaryai-0.7.1/src/binaryai/utils.py` & `binaryai-0.8.0/src/binaryai/utils.py`

 * *Files identical despite different names*

### Comparing `binaryai-0.7.1/PKG-INFO` & `binaryai-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binaryai
-Version: 0.7.1
+Version: 0.8.0
 Summary: BinaryAI-SDK is a library provides an abstracted client module to simplify the procedure of uploading file for analysis.
 Home-page: https://www.binaryai.cn/
 License: GPLv3
 Author: binaryai
 Author-email: binaryai@tencent.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

