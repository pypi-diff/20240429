# Comparing `tmp/caustic.parser-2.2.6.tar.gz` & `tmp/caustic.parser-2.2.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.parser-2.2.6.tar", last modified: Thu Apr 25 23:01:39 2024, max compression
+gzip compressed data, was "caustic.parser-2.2.6.post1.tar", last modified: Sun Apr 28 22:32:53 2024, max compression
```

## Comparing `caustic.parser-2.2.6.tar` & `caustic.parser-2.2.6.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 23:01:39.503916 caustic.parser-2.2.6/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.6/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 23:01:39.503916 caustic.parser-2.2.6/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.6/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-25 22:55:15.000000 caustic.parser-2.2.6/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-25 23:01:39.503916 caustic.parser-2.2.6/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 23:01:39.493916 caustic.parser-2.2.6/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 23:01:39.493916 caustic.parser-2.2.6/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 23:01:39.503916 caustic.parser-2.2.6/src/caustic/parser/
--rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.6/src/caustic/parser/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     5643 2024-04-25 22:54:55.000000 caustic.parser-2.2.6/src/caustic/parser/cli.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3688 2024-04-25 22:16:48.000000 caustic.parser-2.2.6/src/caustic/parser/error.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 23:01:39.503916 caustic.parser-2.2.6/src/caustic.parser.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 23:01:39.000000 caustic.parser-2.2.6/src/caustic.parser.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-25 23:01:39.000000 caustic.parser-2.2.6/src/caustic.parser.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-25 23:01:39.000000 caustic.parser-2.2.6/src/caustic.parser.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-25 23:01:39.000000 caustic.parser-2.2.6/src/caustic.parser.egg-info/entry_points.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-25 23:01:39.000000 caustic.parser-2.2.6/src/caustic.parser.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-25 23:01:39.000000 caustic.parser-2.2.6/src/caustic.parser.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.6.post1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     1890 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.6.post1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1013 2024-04-28 22:32:30.000000 caustic.parser-2.2.6.post1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.089672 caustic.parser-2.2.6.post1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.089672 caustic.parser-2.2.6.post1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/src/caustic/parser/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.6.post1/src/caustic/parser/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     5643 2024-04-25 22:54:55.000000 caustic.parser-2.2.6.post1/src/caustic/parser/cli.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3688 2024-04-25 22:16:48.000000 caustic.parser-2.2.6.post1/src/caustic/parser/error.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1890 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-28 22:32:53.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/entry_points.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/top_level.txt
```

### Comparing `caustic.parser-2.2.6/LICENSE` & `caustic.parser-2.2.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6/PKG-INFO` & `caustic.parser-2.2.6.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.6
+Version: 2.2.6.post1
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Topic :: File Formats
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: parglare
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 Caustic's Parser -- uses grammar specification to compile Caustic source code
 into a [CST (Caustic AST)](https://codeberg.org/Caustic/CausticAST)
 
 Uses [ParGlare](https://github.com/igordejanovic/parglare) for parsing,
```

### Comparing `caustic.parser-2.2.6/README.md` & `caustic.parser-2.2.6.post1/README.md`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6/pyproject.toml` & `caustic.parser-2.2.6.post1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "caustic.parser"
-version = "2.2.6"
-dependencies = []
+version = "2.2.6-1"
+dependencies = ['parglare']
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's parsing framework"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'syntax', 'grammar']
 classifiers = [
```

### Comparing `caustic.parser-2.2.6/src/caustic/parser/__init__.py` & `caustic.parser-2.2.6.post1/src/caustic/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6/src/caustic/parser/cli.py` & `caustic.parser-2.2.6.post1/src/caustic/parser/cli.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6/src/caustic/parser/error.py` & `caustic.parser-2.2.6.post1/src/caustic/parser/error.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6/src/caustic.parser.egg-info/PKG-INFO` & `caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.6
+Version: 2.2.6.post1
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Topic :: File Formats
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: parglare
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 Caustic's Parser -- uses grammar specification to compile Caustic source code
 into a [CST (Caustic AST)](https://codeberg.org/Caustic/CausticAST)
 
 Uses [ParGlare](https://github.com/igordejanovic/parglare) for parsing,
```

