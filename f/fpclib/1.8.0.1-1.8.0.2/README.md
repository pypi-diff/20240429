# Comparing `tmp/fpclib-1.8.0.1.tar.gz` & `tmp/fpclib-1.8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpclib-1.8.0.1.tar", max compression
+gzip compressed data, was "fpclib-1.8.0.2.tar", max compression
```

## Comparing `fpclib-1.8.0.1.tar` & `fpclib-1.8.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0      393 2022-08-31 03:16:00.000000 fpclib-1.8.0.1/LICENSE.md
--rw-r--r--   0        0        0     4128 2024-04-29 20:54:45.719562 fpclib-1.8.0.1/README.md
--rw-r--r--   0        0        0    96248 2024-04-29 20:21:14.594122 fpclib-1.8.0.1/fpclib/__init__.py
--rw-r--r--   0        0        0      950 2024-04-29 21:00:37.029321 fpclib-1.8.0.1/pyproject.toml
--rw-r--r--   0        0        0     4977 1970-01-01 00:00:00.000000 fpclib-1.8.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0    20849 2024-04-29 21:20:39.702437 fpclib-1.8.0.2/LICENSE
+-rw-r--r--   0        0        0     4128 2024-04-29 20:54:45.719562 fpclib-1.8.0.2/README.md
+-rw-r--r--   0        0        0    96248 2024-04-29 20:21:14.594122 fpclib-1.8.0.2/fpclib/__init__.py
+-rw-r--r--   0        0        0     1010 2024-04-29 21:23:45.515175 fpclib-1.8.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5048 1970-01-01 00:00:00.000000 fpclib-1.8.0.2/PKG-INFO
```

### Comparing `fpclib-1.8.0.1/README.md` & `fpclib-1.8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fpclib-1.8.0.1/fpclib/__init__.py` & `fpclib-1.8.0.2/fpclib/__init__.py`

 * *Files identical despite different names*

### Comparing `fpclib-1.8.0.1/pyproject.toml` & `fpclib-1.8.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "fpclib"
-version = "1.8.0.1"
+version = "1.8.0.2"
 description = "A powerful library for curating games for Flashpoint."
 authors = ["mathgeniuszach <huntingmanzach@gmail.com>"]
 license = "CC BY-NC-SA 4.0"
 readme = "README.md"
-
 repository = "https://github.com/xMGZx/fpclib"
 homepage = "https://www.mathgeniuszach.com/"
+documentation = "https://www.mathgeniuszach.com/bin/fpclib/"
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beautifulsoup4 = "^4.12.3"
```

### Comparing `fpclib-1.8.0.1/PKG-INFO` & `fpclib-1.8.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpclib
-Version: 1.8.0.1
+Version: 1.8.0.2
 Summary: A powerful library for curating games for Flashpoint.
 Home-page: https://www.mathgeniuszach.com/
 License: CC BY-NC-SA 4.0
 Author: mathgeniuszach
 Author-email: huntingmanzach@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
+Project-URL: Documentation, https://www.mathgeniuszach.com/bin/fpclib/
 Project-URL: Repository, https://github.com/xMGZx/fpclib
 Description-Content-Type: text/markdown
 
 ## General Overview
 "fpclib" stands for "Flashpoint Curation Library" and is a powerful collection of functions and classes you can use and extend to hopefully curate any game/animation in existence through python3. If you're not familiar with curating for Flashpoint and would like to know how to curate, first follow the [Curation Tutorial](https://bluemaxima.org/flashpoint/datahub/Curation_Tutorial) page on the Flashpoint wiki. If you're not familiar with using python or coding, you should read the [official python tutorial](https://docs.python.org/3/tutorial/index.html) before using this library.
 
 Although there are already several useful tools you can use for manually curating games/animations for Flashpoint and downloading assets easily, such as Flashpoint Core, cURLsDownloader, and MAD4FP, none of these tools offer the ability to curate through code or automate the process; fpclib was created to fix that. [fpcurator](https://github.com/FlashpointProject/fpcurator) uses fpclib to automatically generate curations. Of course, you should still always manually check any curation you make with fpclib in Flashpoint Core to make sure it works properly.
```

