# Comparing `tmp/kellyapi-0.0.2.tar.gz` & `tmp/kellyapi-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.2.tar", last modified: Wed Apr 24 17:06:44 2024, max compression
+gzip compressed data, was "kellyapi-0.0.2.1.tar", last modified: Mon Apr 29 15:58:15 2024, max compression
```

## Comparing `kellyapi-0.0.2.tar` & `kellyapi-0.0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:06:44.080221 kellyapi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 17:06:40.000000 kellyapi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-24 17:06:44.080221 kellyapi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-24 17:06:40.000000 kellyapi-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:06:44.076221 kellyapi-0.0.2/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 17:06:40.000000 kellyapi-0.0.2/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-24 17:06:40.000000 kellyapi-0.0.2/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 17:06:40.000000 kellyapi-0.0.2/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:06:44.080221 kellyapi-0.0.2/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-24 17:06:44.000000 kellyapi-0.0.2/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 17:06:44.000000 kellyapi-0.0.2/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:06:44.000000 kellyapi-0.0.2/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 17:06:44.000000 kellyapi-0.0.2/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 17:06:44.000000 kellyapi-0.0.2/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:06:44.080221 kellyapi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 17:06:40.000000 kellyapi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 15:58:15.000000 kellyapi-0.0.2.1/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:58:15.035273 kellyapi-0.0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-29 15:58:11.000000 kellyapi-0.0.2.1/setup.py
```

### Comparing `kellyapi-0.0.2/LICENSE` & `kellyapi-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2/PKG-INFO` & `kellyapi-0.0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.2/README.md` & `kellyapi-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2/kellyapi/errors.py` & `kellyapi-0.0.2.1/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.2.1/kellyapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.2/setup.py` & `kellyapi-0.0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.2",
+    version="0.0.2.1",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

