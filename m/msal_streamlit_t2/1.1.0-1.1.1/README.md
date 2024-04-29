# Comparing `tmp/msal_streamlit_t2-1.1.0.tar.gz` & `tmp/msal_streamlit_t2-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_streamlit_t2-1.1.0.tar", max compression
+gzip compressed data, was "msal_streamlit_t2-1.1.1.tar", max compression
```

## Comparing `msal_streamlit_t2-1.1.0.tar` & `msal_streamlit_t2-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.0/LICENSE
--rw-r--r--   0        0        0     3830 2024-04-26 21:37:22.661333 msal_streamlit_t2-1.1.0/README.md
--rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.0/msal_streamlit_t2/__init__.py
--rw-r--r--   0        0        0      934 2024-04-29 13:04:15.876500 msal_streamlit_t2-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3830 2024-04-26 21:37:22.661333 msal_streamlit_t2-1.1.1/README.md
+-rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.1/msal_streamlit_t2/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-29 13:15:24.077422 msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/assets/index-297265e4.css
+-rw-r--r--   0        0        0   622361 2024-04-29 13:15:24.077650 msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/assets/index-d9a76572.js
+-rw-r--r--   0        0        0      399 2024-04-29 13:15:24.077391 msal_streamlit_t2-1.1.1/msal_streamlit_t2/frontend/dist/index.html
+-rw-r--r--   0        0        0      934 2024-04-29 13:15:58.643086 msal_streamlit_t2-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.1/PKG-INFO
```

### Comparing `msal_streamlit_t2-1.1.0/LICENSE` & `msal_streamlit_t2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.0/README.md` & `msal_streamlit_t2-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.0/msal_streamlit_t2/__init__.py` & `msal_streamlit_t2-1.1.1/msal_streamlit_t2/__init__.py`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.1.0/pyproject.toml` & `msal_streamlit_t2-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msal_streamlit_t2"
-version = "1.1.0"
+version = "1.1.1"
 description = "Streamlit Authentication library based on MSAL.JS"
 readme = "README.md"
 repository = "https://github.com/mstaal/msal_streamlit_t2"
 authors = ["Michael Staal-Olsen"]
 packages=[
     { include="msal_streamlit_t2" }
 ]
```

### Comparing `msal_streamlit_t2-1.1.0/PKG-INFO` & `msal_streamlit_t2-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_streamlit_t2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Streamlit Authentication library based on MSAL.JS
 Home-page: https://github.com/mstaal/msal_streamlit_t2
 Author: Michael Staal-Olsen
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

