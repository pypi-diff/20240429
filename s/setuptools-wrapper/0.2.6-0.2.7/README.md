# Comparing `tmp/setuptools-wrapper-0.2.6.tar.gz` & `tmp/setuptools_wrapper-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-wrapper-0.2.6.tar", last modified: Sun Oct 15 03:12:46 2023, max compression
+gzip compressed data, was "setuptools_wrapper-0.2.7.tar", last modified: Mon Apr 29 04:29:27 2024, max compression
```

## Comparing `setuptools-wrapper-0.2.6.tar` & `setuptools_wrapper-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 03:12:46.985341 setuptools-wrapper-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-10-15 03:12:46.985341 setuptools-wrapper-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 03:12:46.985341 setuptools-wrapper-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 03:12:46.981341 setuptools-wrapper-0.2.6/setuptools_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setuptools_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 03:12:46.981341 setuptools-wrapper-0.2.6/setuptools_wrapper/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setuptools_wrapper/data/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setuptools_wrapper/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setuptools_wrapper/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setuptools_wrapper/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/setuptools_wrapper/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 03:12:46.981341 setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-10-15 03:12:46.000000 setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-15 03:12:46.000000 setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 03:12:46.000000 setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-15 03:12:46.000000 setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-15 03:12:46.000000 setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 03:12:46.981341 setuptools-wrapper-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-10-15 03:11:12.000000 setuptools-wrapper-0.2.6/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:29:27.460423 setuptools_wrapper-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-29 04:29:27.460423 setuptools_wrapper-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:29:27.460423 setuptools_wrapper-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:29:27.456423 setuptools_wrapper-0.2.7/setuptools_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setuptools_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:29:27.456423 setuptools_wrapper-0.2.7/setuptools_wrapper/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setuptools_wrapper/data/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setuptools_wrapper/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setuptools_wrapper/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setuptools_wrapper/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/setuptools_wrapper/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:29:27.456423 setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-29 04:29:27.000000 setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-29 04:29:27.000000 setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:29:27.000000 setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 04:29:27.000000 setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 04:29:27.000000 setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:29:27.456423 setuptools_wrapper-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-29 04:28:35.000000 setuptools_wrapper-0.2.7/tests/test_setup.py
```

### Comparing `setuptools-wrapper-0.2.6/LICENSE` & `setuptools_wrapper-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-wrapper-0.2.6/PKG-INFO` & `setuptools_wrapper-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-wrapper
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple interface to setuptools's setup function.
 Home-page: https://github.com/vkottler/setuptools-wrapper
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.10
@@ -34,20 +34,20 @@
 Requires-Dist: sphinx-book-theme; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: vcorelib; extra == "test"
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=eeb76283ad94070e843c92961d79c69d
+    version=3.1.4
+    hash=49b054de642b258099743a2c9ee102ec
     =====================================
 -->
 
-# setuptools-wrapper ([0.2.6](https://pypi.org/project/setuptools-wrapper/))
+# setuptools-wrapper ([0.2.7](https://pypi.org/project/setuptools-wrapper/))
 
 [![python](https://img.shields.io/pypi/pyversions/setuptools-wrapper.svg)](https://pypi.org/project/setuptools-wrapper/)
 ![Build Status](https://github.com/vkottler/setuptools-wrapper/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/setuptools-wrapper/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/setuptools-wrapper)
 ![PyPI - Status](https://img.shields.io/pypi/status/setuptools-wrapper)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/setuptools-wrapper)
```

### Comparing `setuptools-wrapper-0.2.6/README.md` & `setuptools_wrapper-0.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=eeb76283ad94070e843c92961d79c69d
+    version=3.1.4
+    hash=49b054de642b258099743a2c9ee102ec
     =====================================
 -->
 
-# setuptools-wrapper ([0.2.6](https://pypi.org/project/setuptools-wrapper/))
+# setuptools-wrapper ([0.2.7](https://pypi.org/project/setuptools-wrapper/))
 
 [![python](https://img.shields.io/pypi/pyversions/setuptools-wrapper.svg)](https://pypi.org/project/setuptools-wrapper/)
 ![Build Status](https://github.com/vkottler/setuptools-wrapper/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/setuptools-wrapper/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/setuptools-wrapper)
 ![PyPI - Status](https://img.shields.io/pypi/status/setuptools-wrapper)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/setuptools-wrapper)
```

### Comparing `setuptools-wrapper-0.2.6/pyproject.toml` & `setuptools_wrapper-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "trove-classifiers"]
 
 [project]
 name = "setuptools-wrapper"
-version = "0.2.6"
+version = "0.2.7"
 description = "A simple interface to setuptools's setup function."
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `setuptools-wrapper-0.2.6/setup.py` & `setuptools_wrapper-0.2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.2
+# version=3.1.4
 # hash=1668f8d26ad800f736638e7eb757119a
 # =====================================
 
 """
 setuptools-wrapper - Package definition for distribution.
 """
```

### Comparing `setuptools-wrapper-0.2.6/setuptools_wrapper/setup.py` & `setuptools_wrapper-0.2.7/setuptools_wrapper/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,19 @@
 
     # Resolve defaults if necessary.
     url_override = cast(
         str, defaults["url_override"] if url_override is None else url_override
     )
     classifiers_override = cast(
         List[str],
-        defaults["classifiers_override"]
-        if classifiers_override is None
-        else classifiers_override,
+        (
+            defaults["classifiers_override"]
+            if classifiers_override is None
+            else classifiers_override
+        ),
     )
     requirements = cast(
         Set[str],
         defaults["requirements"] if requirements is None else requirements,
     )
 
     for version in pkg_info.get("versions", []):
```

### Comparing `setuptools-wrapper-0.2.6/setuptools_wrapper.egg-info/PKG-INFO` & `setuptools_wrapper-0.2.7/setuptools_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-wrapper
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple interface to setuptools's setup function.
 Home-page: https://github.com/vkottler/setuptools-wrapper
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.10
@@ -34,20 +34,20 @@
 Requires-Dist: sphinx-book-theme; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: vcorelib; extra == "test"
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.2
-    hash=eeb76283ad94070e843c92961d79c69d
+    version=3.1.4
+    hash=49b054de642b258099743a2c9ee102ec
     =====================================
 -->
 
-# setuptools-wrapper ([0.2.6](https://pypi.org/project/setuptools-wrapper/))
+# setuptools-wrapper ([0.2.7](https://pypi.org/project/setuptools-wrapper/))
 
 [![python](https://img.shields.io/pypi/pyversions/setuptools-wrapper.svg)](https://pypi.org/project/setuptools-wrapper/)
 ![Build Status](https://github.com/vkottler/setuptools-wrapper/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/setuptools-wrapper/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/setuptools-wrapper)
 ![PyPI - Status](https://img.shields.io/pypi/status/setuptools-wrapper)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/setuptools-wrapper)
```

### Comparing `setuptools-wrapper-0.2.6/tests/test_setup.py` & `setuptools_wrapper-0.2.7/tests/test_setup.py`

 * *Files identical despite different names*

