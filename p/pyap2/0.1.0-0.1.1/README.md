# Comparing `tmp/pyap2-0.1.0.tar.gz` & `tmp/pyap2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyap2-0.1.0.tar", max compression
+gzip compressed data, was "pyap2-0.1.1.tar", max compression
```

## Comparing `pyap2-0.1.0.tar` & `pyap2-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1085 2024-04-26 11:07:29.455882 pyap2-0.1.0/LICENSE
--rw-r--r--   0        0        0     2189 2024-04-26 11:07:29.455882 pyap2-0.1.0/README.rst
--rw-r--r--   0        0        0      225 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/address.py
--rw-r--r--   0        0        0      741 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/api.py
--rw-r--r--   0        0        0      534 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/exceptions.py
--rw-r--r--   0        0        0     4289 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/parser.py
--rw-r--r--   0        0        0        0 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/py.typed
--rw-r--r--   0        0        0        0 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/source_CA/__init__.py
--rw-r--r--   0        0        0    21374 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_CA/data.py
--rw-r--r--   0        0        0        0 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_GB/__init__.py
--rw-r--r--   0        0        0    15020 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_GB/data.py
--rw-r--r--   0        0        0        0 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_US/__init__.py
--rw-r--r--   0        0        0    26198 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_US/data.py
--rw-r--r--   0        0        0     1060 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/utils.py
--rw-r--r--   0        0        0     2418 2024-04-26 11:07:47.016028 pyap2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 pyap2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-29 13:25:47.437915 pyap2-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2189 2024-04-29 13:25:47.437915 pyap2-0.1.1/README.rst
+-rw-r--r--   0        0        0      225 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/address.py
+-rw-r--r--   0        0        0      741 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/api.py
+-rw-r--r--   0        0        0      534 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/exceptions.py
+-rw-r--r--   0        0        0     4289 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/parser.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/py.typed
+-rw-r--r--   0        0        0        0 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/source_CA/__init__.py
+-rw-r--r--   0        0        0    21374 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/source_CA/data.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/source_GB/__init__.py
+-rw-r--r--   0        0        0    15020 2024-04-29 13:25:47.437915 pyap2-0.1.1/pyap/source_GB/data.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:25:47.441915 pyap2-0.1.1/pyap/source_US/__init__.py
+-rw-r--r--   0        0        0    26209 2024-04-29 13:25:47.441915 pyap2-0.1.1/pyap/source_US/data.py
+-rw-r--r--   0        0        0     1060 2024-04-29 13:25:47.441915 pyap2-0.1.1/pyap/utils.py
+-rw-r--r--   0        0        0     2418 2024-04-29 13:26:00.333824 pyap2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 pyap2-0.1.1/PKG-INFO
```

### Comparing `pyap2-0.1.0/LICENSE` & `pyap2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/README.rst` & `pyap2-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/address.py` & `pyap2-0.1.1/pyap/address.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/api.py` & `pyap2-0.1.1/pyap/api.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/exceptions.py` & `pyap2-0.1.1/pyap/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/parser.py` & `pyap2-0.1.1/pyap/parser.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/source_CA/data.py` & `pyap2-0.1.1/pyap/source_CA/data.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/source_GB/data.py` & `pyap2-0.1.1/pyap/source_GB/data.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyap/source_US/data.py` & `pyap2-0.1.1/pyap/source_US/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,15 @@
     "Brnch",
     "Broadway",
     "Brook",
     "Brooks",
     "Btm",
     "Burg",
     "Burgs",
+    "Bvd",
     "Byp",
     "Bypa",
     "Bypas",
     "Bypass",
     "Byps",
     "Byu",
     "Camp",
```

### Comparing `pyap2-0.1.0/pyap/utils.py` & `pyap2-0.1.1/pyap/utils.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.1.0/pyproject.toml` & `pyap2-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyap2"
-version = "0.1.0"
+version = "0.1.1"
 packages = [{ include = "pyap" }]
 description = "Pyap2 is a maintained fork of pyap, a regex-based library for parsing US, CA, and UK addresses. The fork adds typing support, handles more address formats and edge cases."
 authors = ["Argyle Developers <developers@argyle.io>"]
 documentation = "https://github.com/argyle-engineering/pyap"
 homepage = "https://github.com/argyle-engineering/pyap"
 repository = "https://github.com/argyle-engineering/pyap"
 license = "MIT"
```

### Comparing `pyap2-0.1.0/PKG-INFO` & `pyap2-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyap2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pyap2 is a maintained fork of pyap, a regex-based library for parsing US, CA, and UK addresses. The fork adds typing support, handles more address formats and edge cases.
 Home-page: https://github.com/argyle-engineering/pyap
 License: MIT
 Keywords: address,parser,regex
 Author: Argyle Developers
 Author-email: developers@argyle.io
 Requires-Python: >=3.9,<4.0
```

