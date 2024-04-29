# Comparing `tmp/sqlfluff_common_conventions-0.0.1.tar.gz` & `tmp/sqlfluff_common_conventions-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff_common_conventions-0.0.1.tar", last modified: Thu Apr 11 06:18:10 2024, max compression
+gzip compressed data, was "sqlfluff_common_conventions-0.1.0.tar", last modified: Mon Apr 29 03:26:46 2024, max compression
```

## Comparing `sqlfluff_common_conventions-0.0.1.tar` & `sqlfluff_common_conventions-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-11 06:18:10.749178 sqlfluff_common_conventions-0.0.1/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     1067 2024-04-08 03:18:16.000000 sqlfluff_common_conventions-0.0.1/LICENSE
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2069 2024-04-11 06:18:10.748727 sqlfluff_common_conventions-0.0.1/PKG-INFO
--rw-r--r--   0 valerie.tan   (502) staff       (20)      306 2024-04-11 06:17:11.000000 sqlfluff_common_conventions-0.0.1/README.md
--rw-r--r--   0 valerie.tan   (502) staff       (20)      830 2024-04-11 06:17:30.000000 sqlfluff_common_conventions-0.0.1/pyproject.toml
--rw-r--r--   0 valerie.tan   (502) staff       (20)       38 2024-04-11 06:18:10.749278 sqlfluff_common_conventions-0.0.1/setup.cfg
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-11 06:18:10.741954 sqlfluff_common_conventions-0.0.1/src/
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-11 06:18:10.745176 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2671 2024-04-08 07:06:47.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions/CC01.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2626 2024-04-08 08:35:45.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions/CC02.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2388 2024-04-08 09:10:27.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions/CC03.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)      464 2024-04-11 06:16:57.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions/__init__.py
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-11 06:18:10.748229 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2069 2024-04-11 06:18:10.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/PKG-INFO
--rw-r--r--   0 valerie.tan   (502) staff       (20)      528 2024-04-11 06:18:10.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/SOURCES.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)        1 2024-04-11 06:18:10.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/dependency_links.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       69 2024-04-11 06:18:10.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/entry_points.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       16 2024-04-11 06:18:10.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/requires.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       28 2024-04-11 06:18:10.000000 sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/top_level.txt
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 03:26:46.470224 sqlfluff_common_conventions-0.1.0/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1067 2024-04-08 03:18:16.000000 sqlfluff_common_conventions-0.1.0/LICENSE
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       65 2024-04-11 09:37:24.000000 sqlfluff_common_conventions-0.1.0/MANIFEST.in
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2967 2024-04-29 03:26:46.469819 sqlfluff_common_conventions-0.1.0/PKG-INFO
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      465 2024-04-25 08:30:59.000000 sqlfluff_common_conventions-0.1.0/README.md
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1506 2024-04-29 03:23:27.000000 sqlfluff_common_conventions-0.1.0/pyproject.toml
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       38 2024-04-29 03:26:46.470286 sqlfluff_common_conventions-0.1.0/setup.cfg
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 03:26:46.460801 sqlfluff_common_conventions-0.1.0/src/
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 03:26:46.465785 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     3979 2024-04-25 08:30:59.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/CC01.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2544 2024-04-25 08:30:59.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/CC02.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2306 2024-04-25 08:30:59.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/CC03.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     3059 2024-04-25 06:50:57.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/CC04.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1281 2024-04-25 08:30:59.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/__init__.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      196 2024-04-25 08:30:59.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions/plugin_default_config.cfg
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 03:26:46.469236 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2967 2024-04-29 03:26:46.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      638 2024-04-29 03:26:46.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)        1 2024-04-29 03:26:46.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/dependency_links.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       69 2024-04-29 03:26:46.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/entry_points.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       16 2024-04-29 03:26:46.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/requires.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       28 2024-04-29 03:26:46.000000 sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/top_level.txt
```

### Comparing `sqlfluff_common_conventions-0.0.1/LICENSE` & `sqlfluff_common_conventions-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.0.1/PKG-INFO` & `sqlfluff_common_conventions-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff_common_conventions
-Version: 0.0.1
+Version: 0.1.0
 Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
 Author-email: Valerie Tan <valerietanhx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Valerie Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,25 +20,43 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Keywords: sqlfluff
-Classifier: Programming Language :: Python :: 3
+Keywords: sqlfluff,sql,linter,formatter,bigquery
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: SQL
+Classifier: Topic :: Utilities
+Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlfluff>=0.4.0
 
 # sqlfluff-common-conventions
 
 A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
 
 ## Rules
 
-- CC01: Start boolean columns with `is_` or `has_`.
-- CC02: End datetime, time, and timestamp columns with `_at`.
-- CC03: End date columns with `_date`.
+As of 25 April 2024, all rules are compatible with snake, dromedary, and pascal case.
+
+- CC01: Start boolean columns with `is` or `has`.
+- CC02: End datetime, time, and timestamp columns with `at`.
+- CC03: End date columns with `date`.
+- CC04: Only allows a list of configurable words to be used in identifiers.
```

### Comparing `sqlfluff_common_conventions-0.0.1/src/sqlfluff_common_conventions.egg-info/PKG-INFO` & `sqlfluff_common_conventions-0.1.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff_common_conventions
-Version: 0.0.1
+Version: 0.1.0
 Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
 Author-email: Valerie Tan <valerietanhx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Valerie Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,25 +20,43 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Keywords: sqlfluff
-Classifier: Programming Language :: Python :: 3
+Keywords: sqlfluff,sql,linter,formatter,bigquery
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: SQL
+Classifier: Topic :: Utilities
+Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlfluff>=0.4.0
 
 # sqlfluff-common-conventions
 
 A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
 
 ## Rules
 
-- CC01: Start boolean columns with `is_` or `has_`.
-- CC02: End datetime, time, and timestamp columns with `_at`.
-- CC03: End date columns with `_date`.
+As of 25 April 2024, all rules are compatible with snake, dromedary, and pascal case.
+
+- CC01: Start boolean columns with `is` or `has`.
+- CC02: End datetime, time, and timestamp columns with `at`.
+- CC03: End date columns with `date`.
+- CC04: Only allows a list of configurable words to be used in identifiers.
```

