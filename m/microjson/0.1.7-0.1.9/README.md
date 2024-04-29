# Comparing `tmp/microjson-0.1.7.tar.gz` & `tmp/microjson-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microjson-0.1.7.tar", max compression
+gzip compressed data, was "microjson-0.1.9.tar", max compression
```

## Comparing `microjson-0.1.7.tar` & `microjson-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-30 15:35:28.770599 microjson-0.1.7/LICENSE
--rw-r--r--   0        0        0     2044 2023-09-12 12:24:23.562547 microjson-0.1.7/README_short.md
--rw-r--r--   0        0        0     1331 2023-09-15 12:24:01.770581 microjson-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      100 2023-09-15 12:24:01.770581 microjson-0.1.7/src/microjson/__init__.py
--rw-r--r--   0        0        0     1868 2023-09-12 12:24:23.562547 microjson-0.1.7/src/microjson/automodel.py
--rw-r--r--   0        0        0     8123 2023-09-12 12:24:23.562547 microjson-0.1.7/src/microjson/geojson.py
--rw-r--r--   0        0        0     5187 2023-09-15 11:42:34.377610 microjson-0.1.7/src/microjson/model.py
--rw-r--r--   0        0        0     6347 2023-09-13 07:13:08.773429 microjson-0.1.7/src/microjson/roundtrip.py
--rw-r--r--   0        0        0      369 2023-09-12 12:24:23.562547 microjson-0.1.7/src/microjson/utils.py
--rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 microjson-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-09-26 23:13:13.489020 microjson-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2044 2023-09-26 23:13:13.489020 microjson-0.1.9/README_short.md
+-rw-r--r--   0        0        0     1368 2023-10-13 16:34:37.997380 microjson-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-10-13 16:34:37.997380 microjson-0.1.9/src/microjson/__init__.py
+-rw-r--r--   0        0        0     1480 2023-10-06 02:46:04.637385 microjson-0.1.9/src/microjson/automodel.py
+-rw-r--r--   0        0        0     8123 2023-09-26 23:13:13.489020 microjson-0.1.9/src/microjson/geojson.py
+-rw-r--r--   0        0        0     5050 2023-10-06 03:46:09.787748 microjson-0.1.9/src/microjson/model.py
+-rw-r--r--   0        0        0     6347 2023-09-26 23:13:13.489020 microjson-0.1.9/src/microjson/roundtrip.py
+-rw-r--r--   0        0        0      460 2023-10-06 02:46:04.621385 microjson-0.1.9/src/microjson/utils.py
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 microjson-0.1.9/PKG-INFO
```

### Comparing `microjson-0.1.7/LICENSE` & `microjson-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `microjson-0.1.7/README_short.md` & `microjson-0.1.9/README_short.md`

 * *Files identical despite different names*

### Comparing `microjson-0.1.7/pyproject.toml` & `microjson-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "microjson"
-version = "0.1.7"
+version = "0.1.9"
 description = "MicroJSON is a library for validating, parsing, and manipulating MicroJSON data."
 readme = "README_short.md"
 authors = ["Bengt Ljungquist <bengt.ljungquist@nextonicsolutions.com>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,26 +25,29 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 nox = "^2022.1.7"
-pre-commit = "^2.15.0"
-pydantic-to-typescript = "^1.0.10"
 datamodel-code-generator = "^0.21.4"
 bumpver = "^2023.1125"
-nox-poetry = "^1.0.3"
+pre-commit = "^3.3.3"
+black = "^23.3.0"
+ruff = "^0.0.274"
+mypy = "^1.4.0"
+mkdocs = "^1.5.3"
+mkdocstrings = "^0.23.0"
 
 
 [tool.pytest.ini_options]
 testpaths = ["tests/"]
 
 [tool.bumpver]
-current_version = "0.1.7"
+current_version = "0.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `microjson-0.1.7/src/microjson/geojson.py` & `microjson-0.1.9/src/microjson/geojson.py`

 * *Files identical despite different names*

### Comparing `microjson-0.1.7/src/microjson/roundtrip.py` & `microjson-0.1.9/src/microjson/roundtrip.py`

 * *Files identical despite different names*

### Comparing `microjson-0.1.7/PKG-INFO` & `microjson-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microjson
-Version: 0.1.7
+Version: 0.1.9
 Summary: MicroJSON is a library for validating, parsing, and manipulating MicroJSON data.
 License: MIT
 Keywords: json,microscopy,microjson
 Author: Bengt Ljungquist
 Author-email: bengt.ljungquist@nextonicsolutions.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

