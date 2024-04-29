# Comparing `tmp/bpx_py-0.1.2.tar.gz` & `tmp/bpx_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpx_py-0.1.2.tar", max compression
+gzip compressed data, was "bpx_py-0.2.0.tar", max compression
```

## Comparing `bpx_py-0.1.2.tar` & `bpx_py-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-04-27 17:11:08.473700 bpx_py-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.876584 bpx_py-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.876817 bpx_py-0.1.2/bpx/__async/__init__.py
--rw-r--r--   0        0        0     4958 2024-04-28 22:07:10.877209 bpx_py-0.1.2/bpx/__async/account.py
--rw-r--r--   0        0        0     1351 2024-04-28 22:07:10.877504 bpx_py-0.1.2/bpx/__async/public.py
--rw-r--r--   0        0        0        1 2024-04-28 22:07:10.877678 bpx_py-0.1.2/bpx/__init__.py
--rw-r--r--   0        0        0     4813 2024-04-28 22:07:10.877924 bpx_py-0.1.2/bpx/account.py
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.877959 bpx_py-0.1.2/bpx/base/__init__.py
--rw-r--r--   0        0        0     8448 2024-04-28 22:07:10.879684 bpx_py-0.1.2/bpx/base/base_account.py
--rw-r--r--   0        0        0     1777 2024-04-28 22:07:10.879940 bpx_py-0.1.2/bpx/base/base_public.py
--rw-r--r--   0        0        0     1131 2024-04-28 22:07:10.880527 bpx_py-0.1.2/bpx/enums/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-28 22:07:10.881007 bpx_py-0.1.2/bpx/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.881056 bpx_py-0.1.2/bpx/http_client/__init__.py
--rw-r--r--   0        0        0     2100 2024-04-28 22:07:10.881976 bpx_py-0.1.2/bpx/http_client/async_http_client.py
--rw-r--r--   0        0        0      410 2024-04-28 22:07:10.882459 bpx_py-0.1.2/bpx/http_client/http_client.py
--rw-r--r--   0        0        0     1003 2024-04-28 22:07:10.883099 bpx_py-0.1.2/bpx/http_client/sync_http_client.py
--rw-r--r--   0        0        0     1230 2024-04-28 22:07:10.885263 bpx_py-0.1.2/bpx/public.py
--rw-r--r--   0        0        0     1254 2024-04-28 22:07:10.889446 bpx_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 bpx_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-27 17:11:08.473700 bpx_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 06:31:43.778424 bpx_py-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-28 22:07:10.876817 bpx_py-0.2.0/bpx/__async/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-28 22:07:10.877209 bpx_py-0.2.0/bpx/__async/account.py
+-rw-r--r--   0        0        0     1351 2024-04-28 22:07:10.877504 bpx_py-0.2.0/bpx/__async/public.py
+-rw-r--r--   0        0        0        1 2024-04-28 22:07:10.877678 bpx_py-0.2.0/bpx/__init__.py
+-rw-r--r--   0        0        0     4813 2024-04-28 22:07:10.877924 bpx_py-0.2.0/bpx/account.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:07:10.877959 bpx_py-0.2.0/bpx/base/__init__.py
+-rw-r--r--   0        0        0     8448 2024-04-28 22:07:10.879684 bpx_py-0.2.0/bpx/base/base_account.py
+-rw-r--r--   0        0        0     1777 2024-04-28 22:07:10.879940 bpx_py-0.2.0/bpx/base/base_public.py
+-rw-r--r--   0        0        0     1131 2024-04-28 22:07:10.880527 bpx_py-0.2.0/bpx/enums/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-28 22:07:10.881007 bpx_py-0.2.0/bpx/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:07:10.881056 bpx_py-0.2.0/bpx/http_client/__init__.py
+-rw-r--r--   0        0        0     1692 2024-04-29 06:32:06.126224 bpx_py-0.2.0/bpx/http_client/async_http_client.py
+-rw-r--r--   0        0        0      410 2024-04-28 22:07:10.882459 bpx_py-0.2.0/bpx/http_client/http_client.py
+-rw-r--r--   0        0        0     1003 2024-04-28 22:07:10.883099 bpx_py-0.2.0/bpx/http_client/sync_http_client.py
+-rw-r--r--   0        0        0     1230 2024-04-28 22:07:10.885263 bpx_py-0.2.0/bpx/public.py
+-rw-r--r--   0        0        0     1254 2024-04-29 06:34:12.672965 bpx_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3421 1970-01-01 00:00:00.000000 bpx_py-0.2.0/PKG-INFO
```

### Comparing `bpx_py-0.1.2/LICENSE` & `bpx_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/__async/account.py` & `bpx_py-0.2.0/bpx/__async/account.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/__async/public.py` & `bpx_py-0.2.0/bpx/__async/public.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/account.py` & `bpx_py-0.2.0/bpx/account.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/base/base_account.py` & `bpx_py-0.2.0/bpx/base/base_account.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/base/base_public.py` & `bpx_py-0.2.0/bpx/base/base_public.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/enums/__init__.py` & `bpx_py-0.2.0/bpx/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/exceptions/__init__.py` & `bpx_py-0.2.0/bpx/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/http_client/sync_http_client.py` & `bpx_py-0.2.0/bpx/http_client/sync_http_client.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/bpx/public.py` & `bpx_py-0.2.0/bpx/public.py`

 * *Files identical despite different names*

### Comparing `bpx_py-0.1.2/pyproject.toml` & `bpx_py-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpx-py"
-version = "0.1.2"
+version = "0.2.0"
 description = "Backpack API SDK tool"
 authors = ["sndmndss <yanfedorov120505@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage="https://backpack.exchange"
 repository="https://github.com/sndmndss/bpx-py/"
 keywords = ["api", "sdk", "backpack", "client", "wrapper"]
```

