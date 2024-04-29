# Comparing `tmp/duckduckgo_search_api-0.1.3.tar.gz` & `tmp/duckduckgo_search_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search_api-0.1.3.tar", last modified: Sun Feb 25 23:35:36 2024, max compression
+gzip compressed data, was "duckduckgo_search_api-0.1.5.tar", last modified: Mon Apr 29 10:28:33 2024, max compression
```

## Comparing `duckduckgo_search_api-0.1.3.tar` & `duckduckgo_search_api-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:35:36.863911 duckduckgo_search_api-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-25 23:35:28.000000 duckduckgo_search_api-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-25 23:35:36.863911 duckduckgo_search_api-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-25 23:35:28.000000 duckduckgo_search_api-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 23:35:36.863911 duckduckgo_search_api-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-25 23:35:28.000000 duckduckgo_search_api-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:35:36.859910 duckduckgo_search_api-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:35:36.863911 duckduckgo_search_api-0.1.3/src/ddg/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 23:35:28.000000 duckduckgo_search_api-0.1.3/src/ddg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-25 23:35:28.000000 duckduckgo_search_api-0.1.3/src/ddg/apiDDG.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 23:35:36.863911 duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-25 23:35:36.000000 duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-25 23:35:36.000000 duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 23:35:36.000000 duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 23:35:36.000000 duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-25 23:35:36.000000 duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:33.501020 duckduckgo_search_api-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 10:28:29.000000 duckduckgo_search_api-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-29 10:28:33.501020 duckduckgo_search_api-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-29 10:28:29.000000 duckduckgo_search_api-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:28:33.501020 duckduckgo_search_api-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 10:28:29.000000 duckduckgo_search_api-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:33.497020 duckduckgo_search_api-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:33.501020 duckduckgo_search_api-0.1.5/src/ddg/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 10:28:29.000000 duckduckgo_search_api-0.1.5/src/ddg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-29 10:28:29.000000 duckduckgo_search_api-0.1.5/src/ddg/apiDDG.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:33.501020 duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-29 10:28:33.000000 duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 10:28:33.000000 duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:28:33.000000 duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 10:28:33.000000 duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 10:28:33.000000 duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/top_level.txt
```

### Comparing `duckduckgo_search_api-0.1.3/LICENSE` & `duckduckgo_search_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `duckduckgo_search_api-0.1.3/PKG-INFO` & `duckduckgo_search_api-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search_api
-Version: 0.1.3
+Version: 0.1.5
 Summary: A simple and lightweight Python wrapper for DuckDuckGo search.
 Home-page: https://github.com/giaco8020/duckduckgo-search-api
 Author: giaco8020
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -27,15 +27,15 @@
 pip install duckduckgo_search_api
 ```
 
 ## Available Methods
 
 The `Duckduckgo` class offers the following main methods:
 
-- `search(query)`: Accepts a query string and returns search results.
+- `search(query)`: Accepts a query string and returns search results ( ~ 20 results per input ~ )
 
 ## Usage
 
 Here's an example of how to use the DuckDuckGoSearchApi:
 
 ```python
 from ddg import Duckduckgo
@@ -45,14 +45,15 @@
 results = ddg_api.search("Google")
 ```
 
 ## Success request
 
 Search results are returned as a Python dictionary. Each result contains the page title, URL, and a description
 
+
 ```json
 {
   "success": true,
   "data": [
     {
       "title": "Page Title",
       "url": "https://www.example.com",
```

### Comparing `duckduckgo_search_api-0.1.3/README.md` & `duckduckgo_search_api-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip install duckduckgo_search_api
 ```
 
 ## Available Methods
 
 The `Duckduckgo` class offers the following main methods:
 
-- `search(query)`: Accepts a query string and returns search results.
+- `search(query)`: Accepts a query string and returns search results ( ~ 20 results per input ~ )
 
 ## Usage
 
 Here's an example of how to use the DuckDuckGoSearchApi:
 
 ```python
 from ddg import Duckduckgo
@@ -28,14 +28,15 @@
 results = ddg_api.search("Google")
 ```
 
 ## Success request
 
 Search results are returned as a Python dictionary. Each result contains the page title, URL, and a description
 
+
 ```json
 {
   "success": true,
   "data": [
     {
       "title": "Page Title",
       "url": "https://www.example.com",
```

### Comparing `duckduckgo_search_api-0.1.3/setup.py` & `duckduckgo_search_api-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="duckduckgo_search_api",
-    version="0.1.3",
+    version="0.1.5",
     author="giaco8020",
     description="A simple and lightweight Python wrapper for DuckDuckGo search.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/giaco8020/duckduckgo-search-api",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `duckduckgo_search_api-0.1.3/src/duckduckgo_search_api.egg-info/PKG-INFO` & `duckduckgo_search_api-0.1.5/src/duckduckgo_search_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search_api
-Version: 0.1.3
+Version: 0.1.5
 Summary: A simple and lightweight Python wrapper for DuckDuckGo search.
 Home-page: https://github.com/giaco8020/duckduckgo-search-api
 Author: giaco8020
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -27,15 +27,15 @@
 pip install duckduckgo_search_api
 ```
 
 ## Available Methods
 
 The `Duckduckgo` class offers the following main methods:
 
-- `search(query)`: Accepts a query string and returns search results.
+- `search(query)`: Accepts a query string and returns search results ( ~ 20 results per input ~ )
 
 ## Usage
 
 Here's an example of how to use the DuckDuckGoSearchApi:
 
 ```python
 from ddg import Duckduckgo
@@ -45,14 +45,15 @@
 results = ddg_api.search("Google")
 ```
 
 ## Success request
 
 Search results are returned as a Python dictionary. Each result contains the page title, URL, and a description
 
+
 ```json
 {
   "success": true,
   "data": [
     {
       "title": "Page Title",
       "url": "https://www.example.com",
```

