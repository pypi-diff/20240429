# Comparing `tmp/msal_streamlit_t2-1.0.9.tar.gz` & `tmp/msal_streamlit_t2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_streamlit_t2-1.0.9.tar", max compression
+gzip compressed data, was "msal_streamlit_t2-1.1.0.tar", max compression
```

## Comparing `msal_streamlit_t2-1.0.9.tar` & `msal_streamlit_t2-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.0.9/LICENSE
--rw-r--r--   0        0        0     3830 2024-04-26 21:37:22.661333 msal_streamlit_t2-1.0.9/README.md
--rw-r--r--   0        0        0     1202 2024-04-26 21:37:00.716102 msal_streamlit_t2-1.0.9/msal_streamlit_t2/__init__.py
--rw-r--r--   0        0        0      934 2024-04-29 07:26:33.841024 msal_streamlit_t2-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-26 21:37:22.650102 msal_streamlit_t2-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3830 2024-04-26 21:37:22.661333 msal_streamlit_t2-1.1.0/README.md
+-rw-r--r--   0        0        0     1192 2024-04-29 12:58:41.131067 msal_streamlit_t2-1.1.0/msal_streamlit_t2/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-29 13:04:15.876500 msal_streamlit_t2-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 msal_streamlit_t2-1.1.0/PKG-INFO
```

### Comparing `msal_streamlit_t2-1.0.9/LICENSE` & `msal_streamlit_t2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.0.9/README.md` & `msal_streamlit_t2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `msal_streamlit_t2-1.0.9/msal_streamlit_t2/__init__.py` & `msal_streamlit_t2-1.1.0/msal_streamlit_t2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 from pathlib import Path
 import streamlit.components.v1 as components
 
 
-_USE_WEB_DEV_SERVER = os.getenv("USE_WEB_DEV_SERVER", True)
+_USE_WEB_DEV_SERVER = os.getenv("USE_WEB_DEV_SERVER", False)
 _WEB_DEV_SERVER_URL = os.getenv("WEB_DEV_SERVER_URL", "http://localhost:5173")
-COMPONENT_NAME = "msal_authentication_test"
+COMPONENT_NAME = "msal_authentication"
 
 if _USE_WEB_DEV_SERVER:
     _component_func = components.declare_component(name=COMPONENT_NAME, url=_WEB_DEV_SERVER_URL)
 else:
     build_dir = str(Path(__file__).parent / "frontend" / "dist")
     _component_func = components.declare_component(name=COMPONENT_NAME, path=build_dir)
 
 
-def msal_authentication_test(
+def msal_authentication(
         auth,
         cache,
         login_request=None,
         logout_request=None,
         login_button_text="Login_",
-        logout_button_text="Logout_Y",
+        logout_button_text="Logout_",
         class_name=None,
         html_id=None,
         key=None
 ):
     authenticated_user_profile = _component_func(
         auth=auth,
         cache=cache,
```

### Comparing `msal_streamlit_t2-1.0.9/pyproject.toml` & `msal_streamlit_t2-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msal_streamlit_t2"
-version = "1.0.9"
+version = "1.1.0"
 description = "Streamlit Authentication library based on MSAL.JS"
 readme = "README.md"
 repository = "https://github.com/mstaal/msal_streamlit_t2"
 authors = ["Michael Staal-Olsen"]
 packages=[
     { include="msal_streamlit_t2" }
 ]
```

### Comparing `msal_streamlit_t2-1.0.9/PKG-INFO` & `msal_streamlit_t2-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_streamlit_t2
-Version: 1.0.9
+Version: 1.1.0
 Summary: Streamlit Authentication library based on MSAL.JS
 Home-page: https://github.com/mstaal/msal_streamlit_t2
 Author: Michael Staal-Olsen
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

