# Comparing `tmp/edgegap_api-0.1.1.tar.gz` & `tmp/edgegap_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_api-0.1.1.tar", max compression
+gzip compressed data, was "edgegap_api-1.0.0.tar", max compression
```

## Comparing `edgegap_api-0.1.1.tar` & `edgegap_api-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.385564 edgegap_api-0.1.1/LICENSE
--rw-r--r--   0        0        0     2171 2024-04-29 14:41:21.934331 edgegap_api-0.1.1/README.md
--rw-r--r--   0        0        0      132 2024-04-25 13:10:38.952298 edgegap_api-0.1.1/edgegap_api/__init__.py
--rw-r--r--   0        0        0      626 2024-04-26 20:24:37.666063 edgegap_api-0.1.1/edgegap_api/_configuration.py
--rw-r--r--   0        0        0     4163 2024-04-26 20:23:02.963540 edgegap_api-0.1.1/edgegap_api/_helper.py
--rw-r--r--   0        0        0      536 2024-04-29 14:52:37.399950 edgegap_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 edgegap_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:13:42.710660 edgegap_api-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2171 2024-04-29 18:13:42.710660 edgegap_api-1.0.0/README.md
+-rw-r--r--   0        0        0      132 2024-04-29 18:13:42.710660 edgegap_api-1.0.0/edgegap_api/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-29 18:13:42.710660 edgegap_api-1.0.0/edgegap_api/_configuration.py
+-rw-r--r--   0        0        0     4163 2024-04-29 18:13:42.710660 edgegap_api-1.0.0/edgegap_api/_helper.py
+-rw-r--r--   0        0        0      536 2024-04-29 18:13:51.594708 edgegap_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 edgegap_api-1.0.0/PKG-INFO
```

### Comparing `edgegap_api-0.1.1/LICENSE` & `edgegap_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_api-0.1.1/README.md` & `edgegap_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_api-0.1.1/edgegap_api/_configuration.py` & `edgegap_api-1.0.0/edgegap_api/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_api-0.1.1/edgegap_api/_helper.py` & `edgegap_api-1.0.0/edgegap_api/_helper.py`

 * *Files identical despite different names*

### Comparing `edgegap_api-0.1.1/pyproject.toml` & `edgegap_api-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-api"
-version = "0.1.1"
+version = "1.0.0"
 description = "The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_api-0.1.1/PKG-INFO` & `edgegap_api-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-api
-Version: 0.1.1
+Version: 1.0.0
 Summary: The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp[speedups] (>=3.9.5,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap API Library
```
