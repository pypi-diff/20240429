# Comparing `tmp/irwpy-0.0.3.tar.gz` & `tmp/irwpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irwpy-0.0.3.tar", last modified: Mon Apr 29 18:43:37 2024, max compression
+gzip compressed data, was "irwpy-0.0.4.tar", last modified: Mon Apr 29 18:51:09 2024, max compression
```

## Comparing `irwpy-0.0.3.tar` & `irwpy-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.678605 irwpy-0.0.3/
--rw-r--r--   0 aeleish    (503) staff       (20)      243 2024-04-29 18:41:11.000000 irwpy-0.0.3/CHANGELOG.txt
--rw-r--r--   0 aeleish    (503) staff       (20)     1061 2024-04-26 19:43:47.000000 irwpy-0.0.3/LICENSE.txt
--rw-r--r--   0 aeleish    (503) staff       (20)       25 2024-04-29 17:14:20.000000 irwpy-0.0.3/MANIFEST.in
--rw-r--r--   0 aeleish    (503) staff       (20)      863 2024-04-29 18:43:37.678078 irwpy-0.0.3/PKG-INFO
--rw-r--r--   0 aeleish    (503) staff       (20)      383 2024-04-26 19:40:22.000000 irwpy-0.0.3/README.md
--rw-r--r--   0 aeleish    (503) staff       (20)      474 2024-04-29 18:39:15.000000 irwpy-0.0.3/pyproject.toml
--rw-r--r--   0 aeleish    (503) staff       (20)       38 2024-04-29 18:43:37.678675 irwpy-0.0.3/setup.cfg
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.671103 irwpy-0.0.3/src/
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.677485 irwpy-0.0.3/src/IRWPy.egg-info/
--rw-r--r--   0 aeleish    (503) staff       (20)      863 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/PKG-INFO
--rw-r--r--   0 aeleish    (503) staff       (20)      220 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/SOURCES.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/dependency_links.txt
--rw-r--r--   0 aeleish    (503) staff       (20)       10 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/top_level.txt
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.676517 irwpy-0.0.3/src/IRWPytest/
--rw-r--r--   0 aeleish    (503) staff       (20)     1694 2024-04-29 18:09:38.000000 irwpy-0.0.3/src/IRWPytest/__init__.py
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:51:09.222415 irwpy-0.0.4/
+-rw-r--r--   0 aeleish    (503) staff       (20)      302 2024-04-29 18:48:04.000000 irwpy-0.0.4/CHANGELOG.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)     1061 2024-04-26 19:43:47.000000 irwpy-0.0.4/LICENSE.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)       25 2024-04-29 17:14:20.000000 irwpy-0.0.4/MANIFEST.in
+-rw-r--r--   0 aeleish    (503) staff       (20)      863 2024-04-29 18:51:09.221783 irwpy-0.0.4/PKG-INFO
+-rw-r--r--   0 aeleish    (503) staff       (20)      383 2024-04-26 19:40:22.000000 irwpy-0.0.4/README.md
+-rw-r--r--   0 aeleish    (503) staff       (20)      474 2024-04-29 18:51:01.000000 irwpy-0.0.4/pyproject.toml
+-rw-r--r--   0 aeleish    (503) staff       (20)       38 2024-04-29 18:51:09.222490 irwpy-0.0.4/setup.cfg
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:51:09.213945 irwpy-0.0.4/src/
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:51:09.217634 irwpy-0.0.4/src/IRWPy/
+-rw-r--r--   0 aeleish    (503) staff       (20)     1694 2024-04-29 18:09:38.000000 irwpy-0.0.4/src/IRWPy/__init__.py
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:51:09.221091 irwpy-0.0.4/src/IRWPy.egg-info/
+-rw-r--r--   0 aeleish    (503) staff       (20)      863 2024-04-29 18:51:09.000000 irwpy-0.0.4/src/IRWPy.egg-info/PKG-INFO
+-rw-r--r--   0 aeleish    (503) staff       (20)      216 2024-04-29 18:51:09.000000 irwpy-0.0.4/src/IRWPy.egg-info/SOURCES.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-29 18:51:09.000000 irwpy-0.0.4/src/IRWPy.egg-info/dependency_links.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)        6 2024-04-29 18:51:09.000000 irwpy-0.0.4/src/IRWPy.egg-info/top_level.txt
```

### Comparing `irwpy-0.0.3/LICENSE.txt` & `irwpy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irwpy-0.0.3/PKG-INFO` & `irwpy-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IRWPy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Inverse Radius Weighting Interpolation
 Author-email: Bahnam Sadeghi <z5218858@zmail.unsw.edu.au>, Ahmed Eleish <ahmedmorad@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.11
```

### Comparing `irwpy-0.0.3/src/IRWPy.egg-info/PKG-INFO` & `irwpy-0.0.4/src/IRWPy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IRWPy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Inverse Radius Weighting Interpolation
 Author-email: Bahnam Sadeghi <z5218858@zmail.unsw.edu.au>, Ahmed Eleish <ahmedmorad@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.11
```

### Comparing `irwpy-0.0.3/src/IRWPytest/__init__.py` & `irwpy-0.0.4/src/IRWPy/__init__.py`

 * *Files identical despite different names*

