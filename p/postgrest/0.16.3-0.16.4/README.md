# Comparing `tmp/postgrest-0.16.3.tar.gz` & `tmp/postgrest-0.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgrest-0.16.3.tar", max compression
+gzip compressed data, was "postgrest-0.16.4.tar", max compression
```

## Comparing `postgrest-0.16.3.tar` & `postgrest-0.16.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2024-04-13 09:57:42.465729 postgrest-0.16.3/LICENSE
--rw-r--r--   0        0        0     4078 2024-04-13 09:57:42.465729 postgrest-0.16.3/README.md
--rw-r--r--   0        0        0      941 2024-04-13 09:57:44.333740 postgrest-0.16.3/postgrest/__init__.py
--rw-r--r--   0        0        0       35 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_async/__init__.py
--rw-r--r--   0        0        0     3263 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_async/client.py
--rw-r--r--   0        0        0    14157 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_async/request_builder.py
--rw-r--r--   0        0        0       35 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_sync/__init__.py
--rw-r--r--   0        0        0     3217 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_sync/client.py
--rw-r--r--   0        0        0    14089 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_sync/request_builder.py
--rw-r--r--   0        0        0     1918 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/base_client.py
--rw-r--r--   0        0        0    22420 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/base_request_builder.py
--rw-r--r--   0        0        0      151 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/constants.py
--rw-r--r--   0        0        0      409 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/deprecated_client.py
--rw-r--r--   0        0        0      422 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/deprecated_get_request_builder.py
--rw-r--r--   0        0        0     1510 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/py.typed
--rw-r--r--   0        0        0      986 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/types.py
--rw-r--r--   0        0        0     1152 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/utils.py
--rw-r--r--   0        0        0     1915 2024-04-13 09:57:44.333740 postgrest-0.16.3/pyproject.toml
--rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-29 15:26:22.361417 postgrest-0.16.4/LICENSE
+-rw-r--r--   0        0        0     4078 2024-04-29 15:26:22.361417 postgrest-0.16.4/README.md
+-rw-r--r--   0        0        0      941 2024-04-29 15:26:24.345403 postgrest-0.16.4/postgrest/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_async/__init__.py
+-rw-r--r--   0        0        0     3263 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_async/client.py
+-rw-r--r--   0        0        0    14157 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_async/request_builder.py
+-rw-r--r--   0        0        0       35 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_sync/__init__.py
+-rw-r--r--   0        0        0     3217 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_sync/client.py
+-rw-r--r--   0        0        0    14089 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_sync/request_builder.py
+-rw-r--r--   0        0        0     1918 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/base_client.py
+-rw-r--r--   0        0        0    22420 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/base_request_builder.py
+-rw-r--r--   0        0        0      153 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/constants.py
+-rw-r--r--   0        0        0      409 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/deprecated_client.py
+-rw-r--r--   0        0        0      422 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/deprecated_get_request_builder.py
+-rw-r--r--   0        0        0     1510 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/py.typed
+-rw-r--r--   0        0        0      986 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/types.py
+-rw-r--r--   0        0        0     1152 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/utils.py
+-rw-r--r--   0        0        0     1915 2024-04-29 15:26:24.345403 postgrest-0.16.4/pyproject.toml
+-rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.4/PKG-INFO
```

### Comparing `postgrest-0.16.3/LICENSE` & `postgrest-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/README.md` & `postgrest-0.16.4/README.md`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/__init__.py` & `postgrest-0.16.4/postgrest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "0.16.3"
+__version__ = "0.16.4"
 
 from httpx import Timeout
 
 from ._async.client import AsyncPostgrestClient
 from ._async.request_builder import (
     AsyncFilterRequestBuilder,
     AsyncMaybeSingleRequestBuilder,
```

### Comparing `postgrest-0.16.3/postgrest/_async/client.py` & `postgrest-0.16.4/postgrest/_async/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/_async/request_builder.py` & `postgrest-0.16.4/postgrest/_async/request_builder.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/_sync/client.py` & `postgrest-0.16.4/postgrest/_sync/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/_sync/request_builder.py` & `postgrest-0.16.4/postgrest/_sync/request_builder.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/base_client.py` & `postgrest-0.16.4/postgrest/base_client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/base_request_builder.py` & `postgrest-0.16.4/postgrest/base_request_builder.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/exceptions.py` & `postgrest-0.16.4/postgrest/exceptions.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/types.py` & `postgrest-0.16.4/postgrest/types.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/postgrest/utils.py` & `postgrest-0.16.4/postgrest/utils.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.3/pyproject.toml` & `postgrest-0.16.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgrest"
-version = "0.16.3"
+version = "0.16.4"
 description = "PostgREST client for Python. This library provides an ORM interface to PostgREST."
 authors = ["Lương Quang Mạnh <luongquangmanh85@gmail.com>", "Joel Lee <joel@joellee.org>", "Anand", "Oliver Rice", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/postgrest-py"
 repository = "https://github.com/supabase-community/postgrest-py"
 documentation = "https://postgrest-py.rtfd.io"
 readme = "README.md"
 license = "MIT"
@@ -26,19 +26,19 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 flake8 = "^5.0.4"
 black = "^24.3"
 isort = "^5.12.0"
 pre-commit = "^3.5.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-depends = "^1.0.1"
 pytest-asyncio = "^0.23.6"
 unasync-cli = "^0.0.9"
-python-semantic-release = "^9.3.0"
+python-semantic-release = "^9.5.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.1.2"
 furo = ">=2023.9.10,<2025.0.0"
```

### Comparing `postgrest-0.16.3/PKG-INFO` & `postgrest-0.16.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgrest
-Version: 0.16.3
+Version: 0.16.4
 Summary: PostgREST client for Python. This library provides an ORM interface to PostgREST.
 Home-page: https://github.com/supabase-community/postgrest-py
 License: MIT
 Author: Lương Quang Mạnh
 Author-email: luongquangmanh85@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

