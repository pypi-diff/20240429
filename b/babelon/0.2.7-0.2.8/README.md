# Comparing `tmp/babelon-0.2.7.tar.gz` & `tmp/babelon-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelon-0.2.7.tar", max compression
+gzip compressed data, was "babelon-0.2.8.tar", max compression
```

## Comparing `babelon-0.2.7.tar` & `babelon-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1085 2024-03-01 19:40:42.024997 babelon-0.2.7/LICENSE
--rw-r--r--   0        0        0     3128 2024-03-01 19:40:42.024997 babelon-0.2.7/README.md
--rw-r--r--   0        0        0     1741 2024-03-01 19:41:12.556998 babelon-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      236 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/__init__.py
--rw-r--r--   0        0        0    10022 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/babelon_io.py
--rw-r--r--   0        0        0    10471 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/cli.py
--rw-r--r--   0        0        0      149 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/constants.py
--rw-r--r--   0        0        0    17374 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/dataclasses.py
--rw-r--r--   0        0        0     5864 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/parsers/xliff.py
--rw-r--r--   0        0        0     7667 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/schema/babelon.yaml
--rw-r--r--   0        0        0    11737 2024-03-01 19:40:42.028997 babelon-0.2.7/src/babelon/translate.py
--rw-r--r--   0        0        0     2291 2024-03-01 19:40:42.032997 babelon-0.2.7/src/babelon/translation_profile.py
--rw-r--r--   0        0        0     3512 2024-03-01 19:40:42.032997 babelon-0.2.7/src/babelon/utils.py
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 babelon-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-29 16:37:00.430119 babelon-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3128 2024-04-29 16:37:00.430119 babelon-0.2.8/README.md
+-rw-r--r--   0        0        0     1741 2024-04-29 16:37:30.990563 babelon-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      236 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/__init__.py
+-rw-r--r--   0        0        0    10022 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/babelon_io.py
+-rw-r--r--   0        0        0    10471 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/cli.py
+-rw-r--r--   0        0        0      149 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/constants.py
+-rw-r--r--   0        0        0    17374 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/dataclasses.py
+-rw-r--r--   0        0        0     5864 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/parsers/xliff.py
+-rw-r--r--   0        0        0     7667 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/schema/babelon.yaml
+-rw-r--r--   0        0        0    11737 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/translate.py
+-rw-r--r--   0        0        0     2291 2024-04-29 16:37:00.434119 babelon-0.2.8/src/babelon/translation_profile.py
+-rw-r--r--   0        0        0     3512 2024-04-29 16:37:00.438119 babelon-0.2.8/src/babelon/utils.py
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 babelon-0.2.8/PKG-INFO
```

### Comparing `babelon-0.2.7/LICENSE` & `babelon-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/README.md` & `babelon-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/pyproject.toml` & `babelon-0.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "babelon"
-version = "v0.2.7"
+version = "v0.2.8"
 description = "babelon"
 authors = ["Vinicius de Souza <souzadevinicius@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `babelon-0.2.7/src/babelon/babelon_io.py` & `babelon-0.2.8/src/babelon/babelon_io.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/cli.py` & `babelon-0.2.8/src/babelon/cli.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/dataclasses.py` & `babelon-0.2.8/src/babelon/dataclasses.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/parsers/xliff.py` & `babelon-0.2.8/src/babelon/parsers/xliff.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/schema/babelon.yaml` & `babelon-0.2.8/src/babelon/schema/babelon.yaml`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/translate.py` & `babelon-0.2.8/src/babelon/translate.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/translation_profile.py` & `babelon-0.2.8/src/babelon/translation_profile.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/src/babelon/utils.py` & `babelon-0.2.8/src/babelon/utils.py`

 * *Files identical despite different names*

### Comparing `babelon-0.2.7/PKG-INFO` & `babelon-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelon
-Version: 0.2.7
+Version: 0.2.8
 Summary: babelon
 License: MIT
 Author: Vinicius de Souza
 Author-email: souzadevinicius@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

