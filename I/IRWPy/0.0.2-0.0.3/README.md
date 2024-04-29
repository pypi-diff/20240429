# Comparing `tmp/IRWPy-0.0.2.tar.gz` & `tmp/irwpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IRWPy-0.0.2.tar", last modified: Fri Apr 26 21:07:02 2024, max compression
+gzip compressed data, was "irwpy-0.0.3.tar", last modified: Mon Apr 29 18:43:37 2024, max compression
```

## Comparing `IRWPy-0.0.2.tar` & `irwpy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-26 21:07:02.718024 IRWPy-0.0.2/
--rw-r--r--   0 aeleish    (503) staff       (20)      137 2024-04-26 21:06:25.000000 IRWPy-0.0.2/CHANGELOG.txt
-drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-26 21:07:02.717459 IRWPy-0.0.2/IRWPy.egg-info/
--rw-r--r--   0 aeleish    (503) staff       (20)      211 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/PKG-INFO
--rw-r--r--   0 aeleish    (503) staff       (20)      213 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/SOURCES.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/dependency_links.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        6 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/requires.txt
--rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-26 21:07:02.000000 IRWPy-0.0.2/IRWPy.egg-info/top_level.txt
--rw-r--r--   0 aeleish    (503) staff       (20)     1061 2024-04-26 19:43:47.000000 IRWPy-0.0.2/LICENSE.txt
--rw-r--r--   0 aeleish    (503) staff       (20)       25 2024-04-26 19:42:49.000000 IRWPy-0.0.2/MANIFEST.in
--rw-r--r--   0 aeleish    (503) staff       (20)      211 2024-04-26 21:07:02.717830 IRWPy-0.0.2/PKG-INFO
--rw-r--r--   0 aeleish    (503) staff       (20)      383 2024-04-26 19:40:22.000000 IRWPy-0.0.2/README.txt
--rw-r--r--   0 aeleish    (503) staff       (20)     1695 2024-04-26 21:06:36.000000 IRWPy-0.0.2/__init__.py
--rw-r--r--   0 aeleish    (503) staff       (20)       38 2024-04-26 21:07:02.718071 IRWPy-0.0.2/setup.cfg
--rw-r--r--   0 aeleish    (503) staff       (20)      520 2024-04-26 21:06:01.000000 IRWPy-0.0.2/setup.py
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.678605 irwpy-0.0.3/
+-rw-r--r--   0 aeleish    (503) staff       (20)      243 2024-04-29 18:41:11.000000 irwpy-0.0.3/CHANGELOG.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)     1061 2024-04-26 19:43:47.000000 irwpy-0.0.3/LICENSE.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)       25 2024-04-29 17:14:20.000000 irwpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 aeleish    (503) staff       (20)      863 2024-04-29 18:43:37.678078 irwpy-0.0.3/PKG-INFO
+-rw-r--r--   0 aeleish    (503) staff       (20)      383 2024-04-26 19:40:22.000000 irwpy-0.0.3/README.md
+-rw-r--r--   0 aeleish    (503) staff       (20)      474 2024-04-29 18:39:15.000000 irwpy-0.0.3/pyproject.toml
+-rw-r--r--   0 aeleish    (503) staff       (20)       38 2024-04-29 18:43:37.678675 irwpy-0.0.3/setup.cfg
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.671103 irwpy-0.0.3/src/
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.677485 irwpy-0.0.3/src/IRWPy.egg-info/
+-rw-r--r--   0 aeleish    (503) staff       (20)      863 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/PKG-INFO
+-rw-r--r--   0 aeleish    (503) staff       (20)      220 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/SOURCES.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)        1 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/dependency_links.txt
+-rw-r--r--   0 aeleish    (503) staff       (20)       10 2024-04-29 18:43:37.000000 irwpy-0.0.3/src/IRWPy.egg-info/top_level.txt
+drwxr-xr-x   0 aeleish    (503) staff       (20)        0 2024-04-29 18:43:37.676517 irwpy-0.0.3/src/IRWPytest/
+-rw-r--r--   0 aeleish    (503) staff       (20)     1694 2024-04-29 18:09:38.000000 irwpy-0.0.3/src/IRWPytest/__init__.py
```

### Comparing `IRWPy-0.0.2/LICENSE.txt` & `irwpy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `IRWPy-0.0.2/__init__.py` & `irwpy-0.0.3/src/IRWPytest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 def inverse_radius_weighting(x, y, E, values, xi, yi, power=2, neighbors=12):
     """
     Inverse Radius Weighting (IRW) interpolation.
     
     Parameters:
     - x, y: Arrays of measured point coordinates.
     - E: Array of elevations corresponding to the points.
```

