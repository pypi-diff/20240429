# Comparing `tmp/greyhorse_renders-0.1.0.tar.gz` & `tmp/greyhorse_renders-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_renders-0.1.0.tar", max compression
+gzip compressed data, was "greyhorse_renders-0.1.1.tar", max compression
```

## Comparing `greyhorse_renders-0.1.0.tar` & `greyhorse_renders-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       91 2024-04-28 14:19:01.675346 greyhorse_renders-0.1.0/greyhorse_renders/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-27 18:23:26.009156 greyhorse_renders-0.1.0/greyhorse_renders/abc.py
--rw-r--r--   0        0        0        0 2024-04-27 18:41:29.472483 greyhorse_renders-0.1.0/greyhorse_renders/conf/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-28 14:10:27.475399 greyhorse_renders-0.1.0/greyhorse_renders/conf/loader.py
--rw-r--r--   0        0        0     1294 2024-04-28 14:10:27.463397 greyhorse_renders-0.1.0/greyhorse_renders/conf/parser.py
--rw-r--r--   0        0        0     2890 2024-04-28 14:10:27.455396 greyhorse_renders-0.1.0/greyhorse_renders/controller.py
--rw-r--r--   0        0        0      458 2024-04-28 14:15:44.660838 greyhorse_renders-0.1.0/greyhorse_renders/errors.py
--rw-r--r--   0        0        0        0 2024-04-27 17:29:46.448417 greyhorse_renders-0.1.0/greyhorse_renders/private/__init__.py
--rw-r--r--   0        0        0     5297 2024-04-28 14:10:27.479399 greyhorse_renders-0.1.0/greyhorse_renders/private/jinja.py
--rw-r--r--   0        0        0     1762 2024-04-27 18:23:25.989157 greyhorse_renders-0.1.0/greyhorse_renders/private/simple.py
--rw-r--r--   0        0        0      313 2024-04-27 18:23:25.997156 greyhorse_renders-0.1.0/greyhorse_renders/providers.py
--rw-r--r--   0        0        0      312 2024-04-28 14:19:01.667346 greyhorse_renders-0.1.0/greyhorse_renders/translations.toml
--rw-r--r--   0        0        0     1208 2024-04-27 17:32:43.998593 greyhorse_renders-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 greyhorse_renders-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-28 14:19:01.675346 greyhorse_renders-0.1.1/greyhorse_renders/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-27 18:23:26.009156 greyhorse_renders-0.1.1/greyhorse_renders/abc.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:41:29.472483 greyhorse_renders-0.1.1/greyhorse_renders/conf/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-28 14:10:27.475399 greyhorse_renders-0.1.1/greyhorse_renders/conf/loader.py
+-rw-r--r--   0        0        0     1294 2024-04-28 14:10:27.463397 greyhorse_renders-0.1.1/greyhorse_renders/conf/parser.py
+-rw-r--r--   0        0        0     2890 2024-04-28 14:10:27.455396 greyhorse_renders-0.1.1/greyhorse_renders/controller.py
+-rw-r--r--   0        0        0      458 2024-04-28 14:15:44.660838 greyhorse_renders-0.1.1/greyhorse_renders/errors.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:29:46.448417 greyhorse_renders-0.1.1/greyhorse_renders/private/__init__.py
+-rw-r--r--   0        0        0     5297 2024-04-28 14:10:27.479399 greyhorse_renders-0.1.1/greyhorse_renders/private/jinja.py
+-rw-r--r--   0        0        0     1762 2024-04-27 18:23:25.989157 greyhorse_renders-0.1.1/greyhorse_renders/private/simple.py
+-rw-r--r--   0        0        0      313 2024-04-27 18:23:25.997156 greyhorse_renders-0.1.1/greyhorse_renders/providers.py
+-rw-r--r--   0        0        0      312 2024-04-28 14:19:01.667346 greyhorse_renders-0.1.1/greyhorse_renders/translations.toml
+-rw-r--r--   0        0        0     1208 2024-04-28 22:24:04.508453 greyhorse_renders-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 greyhorse_renders-0.1.1/PKG-INFO
```

### Comparing `greyhorse_renders-0.1.0/greyhorse_renders/abc.py` & `greyhorse_renders-0.1.1/greyhorse_renders/abc.py`

 * *Files identical despite different names*

### Comparing `greyhorse_renders-0.1.0/greyhorse_renders/conf/loader.py` & `greyhorse_renders-0.1.1/greyhorse_renders/conf/loader.py`

 * *Files identical despite different names*

### Comparing `greyhorse_renders-0.1.0/greyhorse_renders/conf/parser.py` & `greyhorse_renders-0.1.1/greyhorse_renders/conf/parser.py`

 * *Files identical despite different names*

### Comparing `greyhorse_renders-0.1.0/greyhorse_renders/controller.py` & `greyhorse_renders-0.1.1/greyhorse_renders/controller.py`

 * *Files identical despite different names*

### Comparing `greyhorse_renders-0.1.0/greyhorse_renders/private/jinja.py` & `greyhorse_renders-0.1.1/greyhorse_renders/private/jinja.py`

 * *Files identical despite different names*

### Comparing `greyhorse_renders-0.1.0/greyhorse_renders/private/simple.py` & `greyhorse_renders-0.1.1/greyhorse_renders/private/simple.py`

 * *Files identical despite different names*

### Comparing `greyhorse_renders-0.1.0/pyproject.toml` & `greyhorse_renders-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse-renders"
-version = "0.1.0"
+version = "0.1.1"
 description = "Greyhorse Renders library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -17,15 +17,15 @@
     { include = "greyhorse_renders" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 greyhorse = [
     { path = "../../core/", develop = true },
-    { version = "^0.4.2" }
+    { version = "^0.4.3" }
 ]
 pydantic = {version = "^2.0", extras = ["dotenv"]}
 pydantic-settings = "^2.2.1"
 
 jinja2 = {version = "^3.1.3", optional = true}
 
 [tool.poetry.extras]
```

### Comparing `greyhorse_renders-0.1.0/PKG-INFO` & `greyhorse_renders-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: greyhorse-renders
-Version: 0.1.0
+Version: 0.1.1
 Summary: Greyhorse Renders library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: jinja
-Requires-Dist: greyhorse (==0.4.2)
+Requires-Dist: greyhorse (>=0.4.3,<0.5.0)
+Requires-Dist: greyhorse @ file:///home/plutonium/projects/greyhorse/core
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0) ; extra == "jinja"
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```

