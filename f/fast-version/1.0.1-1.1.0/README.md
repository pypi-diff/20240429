# Comparing `tmp/fast_version-1.0.1.tar.gz` & `tmp/fast_version-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_version-1.0.1.tar", max compression
+gzip compressed data, was "fast_version-1.1.0.tar", max compression
```

## Comparing `fast_version-1.0.1.tar` & `fast_version-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 fast_version-1.0.1/LICENSE
--rw-r--r--   0        0        0     1107 2024-03-30 10:36:32.830511 fast_version-1.0.1/README.md
--rw-r--r--   0        0        0      177 2023-09-10 19:49:22.104243 fast_version-1.0.1/fast_version/__init__.py
--rw-r--r--   0        0        0     4530 2024-03-30 10:36:37.772582 fast_version-1.0.1/fast_version/app.py
--rw-r--r--   0        0        0      800 2023-09-04 07:12:34.000000 fast_version-1.0.1/fast_version/helpers.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 fast_version-1.0.1/fast_version/py.typed
--rw-r--r--   0        0        0     2351 2024-03-30 10:36:37.772924 fast_version-1.0.1/fast_version/router.py
--rw-r--r--   0        0        0     1159 2024-03-30 10:36:37.774609 fast_version-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 fast_version-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 fast_version-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1107 2024-03-30 10:36:32.830511 fast_version-1.1.0/README.md
+-rw-r--r--   0        0        0      177 2023-09-10 19:49:22.104243 fast_version-1.1.0/fast_version/__init__.py
+-rw-r--r--   0        0        0     4511 2024-03-31 09:14:00.747145 fast_version-1.1.0/fast_version/app.py
+-rw-r--r--   0        0        0      800 2023-09-04 07:12:34.000000 fast_version-1.1.0/fast_version/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 fast_version-1.1.0/fast_version/py.typed
+-rw-r--r--   0        0        0     2351 2024-03-30 10:36:37.772924 fast_version-1.1.0/fast_version/router.py
+-rw-r--r--   0        0        0     1392 2024-04-29 08:00:34.410728 fast_version-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 fast_version-1.1.0/PKG-INFO
```

### Comparing `fast_version-1.0.1/LICENSE` & `fast_version-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_version-1.0.1/README.md` & `fast_version-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fast_version-1.0.1/fast_version/app.py` & `fast_version-1.1.0/fast_version/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     routes = []
     for route_item in self.routes:
         if not isinstance(route_item, VersionedAPIRoute):
             routes.append(route_item)
             continue
 
         # trick to avoid merging routes
-        route_copy: VersionedAPIRoute = copy.copy(route_item)
+        route_copy = copy.copy(route_item)
         route_copy.path_format = f"{route_copy.path_format}:{route_copy.version_str}"
         routes.append(route_copy)
 
     self.openapi_schema = get_openapi(
         title=self.title,
         version=self.version,
         openapi_version=self.openapi_version,
```

### Comparing `fast_version-1.0.1/fast_version/helpers.py` & `fast_version-1.1.0/fast_version/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_version-1.0.1/fast_version/router.py` & `fast_version-1.1.0/fast_version/router.py`

 * *Files identical despite different names*

### Comparing `fast_version-1.0.1/pyproject.toml` & `fast_version-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-version"
-version = "1.0.1"
+version = "1.1.0"
 description = "Fastapi versioning package with accept header"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 classifiers = ["Programming Language :: Python :: 3.11", "Framework :: Pytest"]
 homepage = "https://github.com/modern-python/fast-version"
 packages = [
     { include = "fast_version" },
@@ -34,14 +34,18 @@
 select = ["ALL"]
 ignore = [
     "D1", # allow missing docstrings
     "S101", # allow asserts
     "TCH", # ignore flake8-type-checking
     "FBT", # allow boolean args
     "ANN101", # missing-type-self
+    "D203", # "one-blank-line-before-class" conflicting with D211
+    "D213", # "multi-line-summary-second-line" conflicting with D212
+    "COM812", # flake8-commas "Trailing comma missing"
+    "ISC001", # flake8-implicit-str-concat
 ]
 isort.lines-after-imports = 2
 isort.no-lines-before = ["standard-library", "local-folder"]
 
 [tool.pytest.ini_options]
 addopts = "--cov=. --cov-report term-missing"
 asyncio_mode = "auto"
```

### Comparing `fast_version-1.0.1/PKG-INFO` & `fast_version-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-version
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fastapi versioning package with accept header
 Home-page: https://github.com/modern-python/fast-version
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.8,<4
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

