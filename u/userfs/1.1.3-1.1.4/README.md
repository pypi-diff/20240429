# Comparing `tmp/userfs-1.1.3.tar.gz` & `tmp/userfs-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-1.1.3.tar", last modified: Wed Sep 13 02:25:04 2023, max compression
+gzip compressed data, was "userfs-1.1.4.tar", last modified: Mon Apr 29 04:45:01 2024, max compression
```

## Comparing `userfs-1.1.3.tar` & `userfs-1.1.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.186501 userfs-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-09-13 02:23:39.000000 userfs-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2023-09-13 02:25:04.186501 userfs-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-09-13 02:23:39.000000 userfs-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-09-13 02:23:39.000000 userfs-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 02:25:04.186501 userfs-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-09-13 02:23:39.000000 userfs-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-09-13 02:23:39.000000 userfs-1.1.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-09-13 02:23:39.000000 userfs-1.1.3/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/build/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/commands/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/config/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/data/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/data/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/data/schemas/ProjectSpecification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/data/schemas/SourceSpecification.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/project/
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs/update/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-09-13 02:23:39.000000 userfs-1.1.3/userfs/update/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 02:25:04.182501 userfs-1.1.3/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2023-09-13 02:25:04.000000 userfs-1.1.3/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-13 02:25:04.000000 userfs-1.1.3/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 02:25:04.000000 userfs-1.1.3/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-13 02:25:04.000000 userfs-1.1.3/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-09-13 02:25:04.000000 userfs-1.1.3/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-13 02:25:04.000000 userfs-1.1.3/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 04:44:02.000000 userfs-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-29 04:45:01.827280 userfs-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-29 04:44:02.000000 userfs-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-29 04:44:02.000000 userfs-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:45:01.827280 userfs-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-29 04:44:02.000000 userfs-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.823280 userfs-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 04:44:02.000000 userfs-1.1.4/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 04:44:02.000000 userfs-1.1.4/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.823280 userfs-1.1.4/userfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.823280 userfs-1.1.4/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.823280 userfs-1.1.4/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 04:44:02.000000 userfs-1.1.4/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:45:01.827280 userfs-1.1.4/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-29 04:45:01.000000 userfs-1.1.4/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 04:45:01.000000 userfs-1.1.4/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:45:01.000000 userfs-1.1.4/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 04:45:01.000000 userfs-1.1.4/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 04:45:01.000000 userfs-1.1.4/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 04:45:01.000000 userfs-1.1.4/userfs.egg-info/top_level.txt
```

### Comparing `userfs-1.1.3/LICENSE` & `userfs-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/PKG-INFO` & `userfs-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.1.3
+Version: 1.1.4
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gitPython
 Requires-Dist: rcmpy
+Requires-Dist: gitPython
 Requires-Dist: vcorelib>=1.6.2
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
@@ -34,20 +35,20 @@
 Requires-Dist: sphinx-book-theme; extra == "test"
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=dc1cf0b80c7df04bc799c2981b83e78f
+    version=3.1.4
+    hash=9f7925d85eb960826e86546d7e5531ed
     =====================================
 -->
 
-# userfs ([1.1.3](https://pypi.org/project/userfs/))
+# userfs ([1.1.4](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
@@ -64,29 +65,30 @@
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
 * `windows-latest`
 
 # Introduction
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/ufs -h
+$ ./venv3.12/bin/ufs -h
 
 usage: ufs [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
            {build,custom,fetch,noop} ...
 
 A system-bootstrapping automation and introspection tool.
 
 options:
@@ -110,15 +112,15 @@
 ```
 
 ## Sub-command Options
 
 ### `build`
 
 ```
-$ ./venv3.11/bin/ufs build -h
+$ ./venv3.12/bin/ufs build -h
 
 usage: ufs build [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [-d] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
 
@@ -135,15 +137,15 @@
                         the built project assets
 
 ```
 
 ### `custom`
 
 ```
-$ ./venv3.11/bin/ufs custom -h
+$ ./venv3.12/bin/ufs custom -h
 
 usage: ufs custom [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
 
@@ -158,15 +160,15 @@
                         filtered by name
 
 ```
 
 ### `fetch`
 
 ```
-$ ./venv3.11/bin/ufs fetch -h
+$ ./venv3.12/bin/ufs fetch -h
 
 usage: ufs fetch [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [-u] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
```

### Comparing `userfs-1.1.3/README.md` & `userfs-1.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=dc1cf0b80c7df04bc799c2981b83e78f
+    version=3.1.4
+    hash=9f7925d85eb960826e86546d7e5531ed
     =====================================
 -->
 
-# userfs ([1.1.3](https://pypi.org/project/userfs/))
+# userfs ([1.1.4](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
@@ -27,29 +27,30 @@
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
 * `windows-latest`
 
 # Introduction
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/ufs -h
+$ ./venv3.12/bin/ufs -h
 
 usage: ufs [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
            {build,custom,fetch,noop} ...
 
 A system-bootstrapping automation and introspection tool.
 
 options:
@@ -73,15 +74,15 @@
 ```
 
 ## Sub-command Options
 
 ### `build`
 
 ```
-$ ./venv3.11/bin/ufs build -h
+$ ./venv3.12/bin/ufs build -h
 
 usage: ufs build [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [-d] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
 
@@ -98,15 +99,15 @@
                         the built project assets
 
 ```
 
 ### `custom`
 
 ```
-$ ./venv3.11/bin/ufs custom -h
+$ ./venv3.12/bin/ufs custom -h
 
 usage: ufs custom [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
 
@@ -121,15 +122,15 @@
                         filtered by name
 
 ```
 
 ### `fetch`
 
 ```
-$ ./venv3.11/bin/ufs fetch -h
+$ ./venv3.12/bin/ufs fetch -h
 
 usage: ufs fetch [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [-u] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
```

### Comparing `userfs-1.1.3/pyproject.toml` & `userfs-1.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "1.1.3"
+version = "1.1.4"
 description = "A system-bootstrapping automation and introspection tool."
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
```

### Comparing `userfs-1.1.3/setup.py` & `userfs-1.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
-# hash=29a6e613b5aeeb73df1bf733a9e28a56
+# version=3.1.4
+# hash=f993f366d875477ffb6517fa8dcc1e1d
 # =====================================
 
 """
 userfs - Package definition for distribution.
 """
 
 # third-party
@@ -26,13 +26,14 @@
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
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

### Comparing `userfs-1.1.3/tests/test_entry.py` & `userfs-1.1.4/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/app.py` & `userfs-1.1.4/userfs/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.4
 # hash=6b8d7773adb61a955438889b00b5cf7c
 # =====================================
 
 """
 This package's command-line entry-point application.
 """
```

### Comparing `userfs-1.1.3/userfs/build/__init__.py` & `userfs-1.1.4/userfs/build/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/commands/all.py` & `userfs-1.1.4/userfs/commands/all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.4
 # hash=c3b94c7c029203ccd0bc061a0024237d
 # =====================================
 
 """
 A module aggregating package commands.
 """
```

### Comparing `userfs-1.1.3/userfs/commands/build.py` & `userfs-1.1.4/userfs/commands/build.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/commands/common.py` & `userfs-1.1.4/userfs/commands/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Common argument-parsing utilities for package commands.
 """
+
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
 from pathlib import Path as _Path
 from re import search
 from typing import Any, Dict, Iterable, Set, Tuple
 
@@ -69,17 +70,19 @@
 
     # Apply filter.
     return (
         set(
             filter(
                 lambda x: search(args.pattern, x) and x in config.projects,
                 # Gather the set of projects.
-                set(x for x in args.projects if "=" not in x)
-                if not args.all
-                else set(config.projects.keys()),
+                (
+                    set(x for x in args.projects if "=" not in x)
+                    if not args.all
+                    else set(config.projects.keys())
+                ),
             )
         ),
         opts,
     )
 
 
 def run_command(
```

### Comparing `userfs-1.1.3/userfs/commands/custom.py` & `userfs-1.1.4/userfs/commands/custom.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/commands/fetch.py` & `userfs-1.1.4/userfs/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/config/__init__.py` & `userfs-1.1.4/userfs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/config/project.py` & `userfs-1.1.4/userfs/config/project.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/config/source.py` & `userfs-1.1.4/userfs/config/source.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/data/schemas/Config.yaml` & `userfs-1.1.4/userfs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/data/schemas/ProjectSpecification.yaml` & `userfs-1.1.4/userfs/data/schemas/ProjectSpecification.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/entry.py` & `userfs-1.1.4/userfs/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.4
 # hash=145a14a5b38e8a9f107bdedef7c2e7af
 # =====================================
 
 """
 This package's command-line entry-point (boilerplate).
 """
```

### Comparing `userfs-1.1.3/userfs/fetch/__init__.py` & `userfs-1.1.4/userfs/fetch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # built-in
 from pathlib import Path
 from typing import Any, Dict
 
 # third-party
-from git import Repo  # type: ignore
+from git import Repo
 from vcorelib.paths import rel
 
 # internal
 from userfs.config import ProjectSpecification, SourceKind
 
 
 def fetch(
```

### Comparing `userfs-1.1.3/userfs/hooks/__init__.py` & `userfs-1.1.4/userfs/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/paths.py` & `userfs-1.1.4/userfs/paths.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/project/__init__.py` & `userfs-1.1.4/userfs/project/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/schemas.py` & `userfs-1.1.4/userfs/schemas.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.3/userfs/update/__init__.py` & `userfs-1.1.4/userfs/update/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # built-in
 from contextlib import suppress
 from pathlib import Path
 from typing import Any, Dict
 
 # third-party
-from git import Repo  # type: ignore
+from git import Repo
 from git.exc import GitCommandError
 
 # internal
 from userfs.config import ProjectSpecification
 
 
 def update(
```

### Comparing `userfs-1.1.3/userfs.egg-info/PKG-INFO` & `userfs-1.1.4/userfs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.1.3
+Version: 1.1.4
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gitPython
 Requires-Dist: rcmpy
+Requires-Dist: gitPython
 Requires-Dist: vcorelib>=1.6.2
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
@@ -34,20 +35,20 @@
 Requires-Dist: sphinx-book-theme; extra == "test"
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=dc1cf0b80c7df04bc799c2981b83e78f
+    version=3.1.4
+    hash=9f7925d85eb960826e86546d7e5531ed
     =====================================
 -->
 
-# userfs ([1.1.3](https://pypi.org/project/userfs/))
+# userfs ([1.1.4](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
@@ -64,29 +65,30 @@
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
+* [`python3.12`](https://docs.python.org/3.12/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
 * `windows-latest`
 
 # Introduction
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/ufs -h
+$ ./venv3.12/bin/ufs -h
 
 usage: ufs [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
            {build,custom,fetch,noop} ...
 
 A system-bootstrapping automation and introspection tool.
 
 options:
@@ -110,15 +112,15 @@
 ```
 
 ## Sub-command Options
 
 ### `build`
 
 ```
-$ ./venv3.11/bin/ufs build -h
+$ ./venv3.12/bin/ufs build -h
 
 usage: ufs build [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [-d] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
 
@@ -135,15 +137,15 @@
                         the built project assets
 
 ```
 
 ### `custom`
 
 ```
-$ ./venv3.11/bin/ufs custom -h
+$ ./venv3.12/bin/ufs custom -h
 
 usage: ufs custom [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
 
@@ -158,15 +160,15 @@
                         filtered by name
 
 ```
 
 ### `fetch`
 
 ```
-$ ./venv3.11/bin/ufs fetch -h
+$ ./venv3.12/bin/ufs fetch -h
 
 usage: ufs fetch [-h] [-c CONFIG] [-a] [-n] [-p PATTERN] [-u] [projects ...]
 
 positional arguments:
   projects              specific projects to build, arguments in the form
                         'key=value' will be provided as interaction options
```

### Comparing `userfs-1.1.3/userfs.egg-info/SOURCES.txt` & `userfs-1.1.4/userfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

