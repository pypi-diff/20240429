# Comparing `tmp/rcmpy-1.5.3.tar.gz` & `tmp/rcmpy-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.5.3.tar", last modified: Sun Aug  6 07:13:33 2023, max compression
+gzip compressed data, was "rcmpy-1.5.4.tar", last modified: Mon Apr 29 04:18:15 2024, max compression
```

## Comparing `rcmpy-1.5.3.tar` & `rcmpy-1.5.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:12:12.000000 rcmpy-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-06 07:13:33.480410 rcmpy-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-08-06 07:12:12.000000 rcmpy-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-06 07:12:12.000000 rcmpy-1.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/watch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/watch/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:13:33.480410 rcmpy-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-06 07:12:12.000000 rcmpy-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-06 07:12:12.000000 rcmpy-1.5.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 07:12:12.000000 rcmpy-1.5.3/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-06 07:12:12.000000 rcmpy-1.5.3/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.318467 rcmpy-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 04:17:00.000000 rcmpy-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-29 04:18:15.318467 rcmpy-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-29 04:17:00.000000 rcmpy-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-29 04:17:00.000000 rcmpy-1.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.310467 rcmpy-1.5.4/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.310467 rcmpy-1.5.4/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/watch/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.318467 rcmpy-1.5.4/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:18:15.318467 rcmpy-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-29 04:17:00.000000 rcmpy-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.318467 rcmpy-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-29 04:17:00.000000 rcmpy-1.5.4/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 04:17:00.000000 rcmpy-1.5.4/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 04:17:00.000000 rcmpy-1.5.4/tests/test_xdg.py
```

### Comparing `rcmpy-1.5.3/LICENSE` & `rcmpy-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/PKG-INFO` & `rcmpy-1.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,16 @@
-Metadata-Version: 2.1
-Name: rcmpy
-Version: 1.5.3
-Summary: A configuration-file management system.
-Home-page: https://github.com/vkottler/rcmpy
-Author: Vaughn Kottler
-Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=1378c10a9410bc7e897df3efc11350c1
+    version=3.1.4
+    hash=4a63d867ef56ebbd2d59aaddb06364c5
     =====================================
 -->
 
-# rcmpy ([1.5.3](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.4](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -48,18 +25,17 @@
 * By [pydoc](https://vkottler.github.io/python/pydoc/rcmpy.html)
 (What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -141,15 +117,15 @@
    an existing one at any arbitrary location.
 5. Run `rcmpy apply` to perform tasks specified in the
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/rcmpy -h
+$ ./venv3.12/bin/rcmpy -h
 
 usage: rcmpy [-h] [--version] [-v] [-C DIR]
              {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
@@ -173,41 +149,41 @@
 ```
 
 ## Sub-command Options
 
 ### `apply`
 
 ```
-$ ./venv3.11/bin/rcmpy apply -h
+$ ./venv3.12/bin/rcmpy apply -h
 
 usage: rcmpy apply [-h] [-f] [-d]
 
 options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `dump`
 
 ```
-$ ./venv3.11/bin/rcmpy dump -h
+$ ./venv3.12/bin/rcmpy dump -h
 
 usage: rcmpy dump [-h]
 
 options:
   -h, --help  show this help message and exit
 
 ```
 
 ### `use`
 
 ```
-$ ./venv3.11/bin/rcmpy use -h
+$ ./venv3.12/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
 
 positional arguments:
   directory      the directory to use
 
 options:
@@ -215,15 +191,15 @@
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `variant`
 
 ```
-$ ./venv3.11/bin/rcmpy variant -h
+$ ./venv3.12/bin/rcmpy variant -h
 
 usage: rcmpy variant [-h] [-d] [variant]
 
 positional arguments:
   variant        new variant to use
 
 options:
@@ -231,15 +207,15 @@
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `watch`
 
 ```
-$ ./venv3.11/bin/rcmpy watch -h
+$ ./venv3.12/bin/rcmpy watch -h
 
 usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] [-n] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
```

### Comparing `rcmpy-1.5.3/README.md` & `rcmpy-1.5.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,53 @@
+Metadata-Version: 2.1
+Name: rcmpy
+Version: 1.5.4
+Summary: A configuration-file management system.
+Home-page: https://github.com/vkottler/rcmpy
+Author: Vaughn Kottler
+Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
+Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: vcorelib>=1.6.6
+Requires-Dist: datazen
+Provides-Extra: test
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: yamllint; extra == "test"
+Requires-Dist: yambs; extra == "test"
+Requires-Dist: vmklib; extra == "test"
+Requires-Dist: sphinx; extra == "test"
+Requires-Dist: sphinx-book-theme; extra == "test"
+Requires-Dist: setuptools-wrapper; extra == "test"
+Requires-Dist: types-setuptools; extra == "test"
+
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=1378c10a9410bc7e897df3efc11350c1
+    version=3.1.4
+    hash=4a63d867ef56ebbd2d59aaddb06364c5
     =====================================
 -->
 
-# rcmpy ([1.5.3](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.4](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -25,18 +62,17 @@
 * By [pydoc](https://vkottler.github.io/python/pydoc/rcmpy.html)
 (What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -118,15 +154,15 @@
    an existing one at any arbitrary location.
 5. Run `rcmpy apply` to perform tasks specified in the
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/rcmpy -h
+$ ./venv3.12/bin/rcmpy -h
 
 usage: rcmpy [-h] [--version] [-v] [-C DIR]
              {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
@@ -150,41 +186,41 @@
 ```
 
 ## Sub-command Options
 
 ### `apply`
 
 ```
-$ ./venv3.11/bin/rcmpy apply -h
+$ ./venv3.12/bin/rcmpy apply -h
 
 usage: rcmpy apply [-h] [-f] [-d]
 
 options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `dump`
 
 ```
-$ ./venv3.11/bin/rcmpy dump -h
+$ ./venv3.12/bin/rcmpy dump -h
 
 usage: rcmpy dump [-h]
 
 options:
   -h, --help  show this help message and exit
 
 ```
 
 ### `use`
 
 ```
-$ ./venv3.11/bin/rcmpy use -h
+$ ./venv3.12/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
 
 positional arguments:
   directory      the directory to use
 
 options:
@@ -192,15 +228,15 @@
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `variant`
 
 ```
-$ ./venv3.11/bin/rcmpy variant -h
+$ ./venv3.12/bin/rcmpy variant -h
 
 usage: rcmpy variant [-h] [-d] [variant]
 
 positional arguments:
   variant        new variant to use
 
 options:
@@ -208,15 +244,15 @@
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `watch`
 
 ```
-$ ./venv3.11/bin/rcmpy watch -h
+$ ./venv3.12/bin/rcmpy watch -h
 
 usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] [-n] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
```

### Comparing `rcmpy-1.5.3/rcmpy/app.py` & `rcmpy-1.5.4/rcmpy/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.4
 # hash=0cb0fd902b7216726825ed86f95176e5
 # =====================================
 
 """
 This package's command-line entry-point application.
 """
```

### Comparing `rcmpy-1.5.3/rcmpy/commands/all.py` & `rcmpy-1.5.4/rcmpy/commands/all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.4
 # hash=2b9927a9d538a17ed80c0411b8d02364
 # =====================================
 
 """
 A module aggregating package commands.
 """
```

### Comparing `rcmpy-1.5.3/rcmpy/commands/apply.py` & `rcmpy-1.5.4/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/commands/common.py` & `rcmpy-1.5.4/rcmpy/commands/common.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/commands/dump.py` & `rcmpy-1.5.4/rcmpy/commands/dump.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/commands/use.py` & `rcmpy-1.5.4/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/commands/variant.py` & `rcmpy-1.5.4/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/commands/watch.py` & `rcmpy-1.5.4/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/config/__init__.py` & `rcmpy-1.5.4/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/config/file.py` & `rcmpy-1.5.4/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.5.4/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/entry.py` & `rcmpy-1.5.4/rcmpy/entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
-# hash=c6ac61aef12193bf7272d503bc1b2df1
+# version=3.1.4
+# hash=7ab0baae7a3ee4f18724d2e1ad059bdf
 # =====================================
 
 """
 This package's command-line entry-point (boilerplate).
 """
 
 # built-in
 import argparse
-import logging
 import os
 from pathlib import Path
 import sys
 from typing import List
 
+# third-party
+from vcorelib.logging import init_logging, logging_args
+
 # internal
 from rcmpy import DESCRIPTION, VERSION
 from rcmpy.app import add_app_args, entry
 
 
 def main(argv: List[str] = None) -> int:
     """Program entry-point."""
@@ -34,20 +36,15 @@
     # initialize argument parsing
     parser = argparse.ArgumentParser(description=DESCRIPTION)
     parser.add_argument(
         "--version",
         action="version",
         version=f"%(prog)s {VERSION}",
     )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="set to increase logging verbosity",
-    )
+    logging_args(parser)
     parser.add_argument(
         "-C",
         "--dir",
         default=Path.cwd(),
         dest="dir",
         type=Path,
         help="execute from a specific directory",
@@ -59,18 +56,16 @@
     # parse arguments and execute the requested command
     try:
         args = parser.parse_args(command_args[1:])
         args.version = VERSION
         args.dir = args.dir.resolve()
 
         # initialize logging
-        log_level = logging.DEBUG if args.verbose else logging.INFO
-        logging.basicConfig(
-            level=log_level,
-            format="%(name)-36s - %(levelname)-6s - %(message)s",
+        init_logging(
+            args, default_format="%(name)-36s - %(levelname)-6s - %(message)s"
         )
 
         # change to the specified directory
         os.chdir(args.dir)
 
         # run the application
         result = entry(args)
```

### Comparing `rcmpy-1.5.3/rcmpy/environment/__init__.py` & `rcmpy-1.5.4/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/environment/base.py` & `rcmpy-1.5.4/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/environment/data.py` & `rcmpy-1.5.4/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/environment/template.py` & `rcmpy-1.5.4/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/paths/__init__.py` & `rcmpy-1.5.4/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/schemas.py` & `rcmpy-1.5.4/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/state/__init__.py` & `rcmpy-1.5.4/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/watch/__init__.py` & `rcmpy-1.5.4/rcmpy/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/watch/params.py` & `rcmpy-1.5.4/rcmpy/watch/params.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy/xdg/__init__.py` & `rcmpy-1.5.4/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.5.4/rcmpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.3
+Version: 1.5.4
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: vcorelib>=1.6.6
+Requires-Dist: datazen
+Provides-Extra: test
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: yamllint; extra == "test"
+Requires-Dist: yambs; extra == "test"
+Requires-Dist: vmklib; extra == "test"
+Requires-Dist: sphinx; extra == "test"
+Requires-Dist: sphinx-book-theme; extra == "test"
+Requires-Dist: setuptools-wrapper; extra == "test"
+Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=1378c10a9410bc7e897df3efc11350c1
+    version=3.1.4
+    hash=4a63d867ef56ebbd2d59aaddb06364c5
     =====================================
 -->
 
-# rcmpy ([1.5.3](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.4](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -48,18 +62,17 @@
 * By [pydoc](https://vkottler.github.io/python/pydoc/rcmpy.html)
 (What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -141,15 +154,15 @@
    an existing one at any arbitrary location.
 5. Run `rcmpy apply` to perform tasks specified in the
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/rcmpy -h
+$ ./venv3.12/bin/rcmpy -h
 
 usage: rcmpy [-h] [--version] [-v] [-C DIR]
              {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
@@ -173,41 +186,41 @@
 ```
 
 ## Sub-command Options
 
 ### `apply`
 
 ```
-$ ./venv3.11/bin/rcmpy apply -h
+$ ./venv3.12/bin/rcmpy apply -h
 
 usage: rcmpy apply [-h] [-f] [-d]
 
 options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `dump`
 
 ```
-$ ./venv3.11/bin/rcmpy dump -h
+$ ./venv3.12/bin/rcmpy dump -h
 
 usage: rcmpy dump [-h]
 
 options:
   -h, --help  show this help message and exit
 
 ```
 
 ### `use`
 
 ```
-$ ./venv3.11/bin/rcmpy use -h
+$ ./venv3.12/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
 
 positional arguments:
   directory      the directory to use
 
 options:
@@ -215,15 +228,15 @@
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `variant`
 
 ```
-$ ./venv3.11/bin/rcmpy variant -h
+$ ./venv3.12/bin/rcmpy variant -h
 
 usage: rcmpy variant [-h] [-d] [variant]
 
 positional arguments:
   variant        new variant to use
 
 options:
@@ -231,15 +244,15 @@
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `watch`
 
 ```
-$ ./venv3.11/bin/rcmpy watch -h
+$ ./venv3.12/bin/rcmpy watch -h
 
 usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] [-n] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
```

### Comparing `rcmpy-1.5.3/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.5.4/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.3/setup.py` & `rcmpy-1.5.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
-# hash=41029b1d344eff0720907ad9b29da09b
+# version=3.1.4
+# hash=7afa325a6c78283f5a73152c93d9eab5
 # =====================================
 
 """
 rcmpy - Package definition for distribution.
 """
 
 # third-party
@@ -24,17 +24,16 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.8",
-        "3.9",
         "3.10",
         "3.11",
+        "3.12",
     ],
 }
 setup(
     pkg_info,
     author_info,
 )
```

### Comparing `rcmpy-1.5.3/tests/test_entry.py` & `rcmpy-1.5.4/tests/test_entry.py`

 * *Files identical despite different names*

