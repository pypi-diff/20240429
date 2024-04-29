# Comparing `tmp/c4t-1.2.4.tar.gz` & `tmp/c4t-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4t-1.2.4.tar", last modified: Sat Apr 27 08:07:02 2024, max compression
+gzip compressed data, was "c4t-1.3.0.tar", last modified: Mon Apr 29 09:45:29 2024, max compression
```

## Comparing `c4t-1.2.4.tar` & `c4t-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.347408 c4t-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-27 08:06:55.000000 c4t-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-27 08:07:02.347408 c4t-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-27 08:06:55.000000 c4t-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-27 08:06:55.000000 c4t-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:07:02.347408 c4t-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-27 08:06:55.000000 c4t-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.339408 c4t-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.343408 c4t-1.2.4/src/c4t/
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-27 08:06:55.000000 c4t-1.2.4/src/c4t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-27 08:06:55.000000 c4t-1.2.4/src/c4t/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.343408 c4t-1.2.4/src/c4t.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 08:07:02.000000 c4t-1.2.4/src/c4t.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:07:02.343408 c4t-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-27 08:06:55.000000 c4t-1.2.4/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.426590 c4t-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 09:45:23.000000 c4t-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 09:45:29.426590 c4t-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-29 09:45:23.000000 c4t-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-29 09:45:23.000000 c4t-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:45:29.426590 c4t-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 09:45:23.000000 c4t-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/src/c4t/
+-rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-04-29 09:45:23.000000 c4t-1.3.0/src/c4t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-29 09:45:23.000000 c4t-1.3.0/src/c4t/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/src/c4t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 09:45:29.000000 c4t-1.3.0/src/c4t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:45:29.422590 c4t-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-29 09:45:23.000000 c4t-1.3.0/tests/tests.py
```

### Comparing `c4t-1.2.4/LICENSE` & `c4t-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `c4t-1.2.4/PKG-INFO` & `c4t-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.2.4
+Version: 1.3.0
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,20 +35,21 @@
 Provides-Extra: dev
 Requires-Dist: bumpver>=2023.1126; extra == "dev"
 Requires-Dist: c4t[lint]; extra == "dev"
 Requires-Dist: c4t[test]; extra == "dev"
 Requires-Dist: c4t[package]; extra == "dev"
 
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
+[![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.2.4
+# c4t: Chrome for Testing - v1.3.0
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.4/README.md` & `c4t-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
+[![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.2.4
+# c4t: Chrome for Testing - v1.3.0
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.4/pyproject.toml` & `c4t-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c4t"
-version = "1.2.4"
+version = "1.3.0"
 authors = [
   { name="p4irin", email="139928764+p4irin@users.noreply.github.com" },
 ]
 description = "Install Chrome for Testing assets."
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -65,15 +65,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "1.2.4"
+current_version = "1.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `c4t-1.2.4/setup.py` & `c4t-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `c4t-1.2.4/src/c4t/__init__.py` & `c4t-1.3.0/src/c4t/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,29 @@
     browser.close()
     browser.quit()
 """
 
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.2.4'
+__version__ = '1.3.0'
 
 
 import requests
 import os
 import json
 import wget
 import zipfile
 from typing import Literal, List, Union
 
 
-_path_to_assets = './assets'
+_default_path_to_assets = './assets'
+_path_to_assets = os.getenv(
+    'C4T_PATH_TO_ASSETS', _default_path_to_assets
+)
 
 
 class _Location:
     """Specify the location/path to the assets' binaries.
     
     Attributes:
         chrome: The path to the 'Chrome for Testing' binary
@@ -112,19 +115,18 @@
 
     def _create_assets_dir(self) -> None:
         """Create the installation directory for multiple versions of assets.
 
         Raises:
             SystemExit on unhandled exceptions.
         """
-        print('Create "assets" directory.')
         try:
             os.mkdir(_path_to_assets)
-        except FileExistsError:            
-            print('Skipping: The assets directory already exists.')
+        except FileExistsError:
+            pass
         except Exception as e:
             raise SystemExit(e)
         
     def _installation_path_of(
             self, binary: Literal['chrome', 'chromedriver']
         ) -> str:
         """Returns the installation path of the binary.
```

### Comparing `c4t-1.2.4/src/c4t/cli.py` & `c4t-1.3.0/src/c4t/cli.py`

 * *Files identical despite different names*

### Comparing `c4t-1.2.4/src/c4t.egg-info/PKG-INFO` & `c4t-1.3.0/src/c4t.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.2.4
+Version: 1.3.0
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,20 +35,21 @@
 Provides-Extra: dev
 Requires-Dist: bumpver>=2023.1126; extra == "dev"
 Requires-Dist: c4t[lint]; extra == "dev"
 Requires-Dist: c4t[test]; extra == "dev"
 Requires-Dist: c4t[package]; extra == "dev"
 
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
+[![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.2.4
+# c4t: Chrome for Testing - v1.3.0
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.4/tests/tests.py` & `c4t-1.3.0/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import os
 import time
 from selenium.webdriver import ChromeOptions, ChromeService, Chrome
 import c4t
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.2.4'
+__version__ = '1.3.0'
 
 
 class C4tTests(unittest.TestCase):
 
     class _TestData:
         specific_version_of_assets = '116.0.5794.0'
 
     @classmethod
     def setUpClass(cls) -> None:
-        cls.assets_dir = './assets'
+        cls.assets_dir = c4t._path_to_assets
         cls.chrome_options = ChromeOptions()
         cls.chrome_options.binary_location = c4t.location.chrome
         cls.chrome_options.add_argument('--no-sandbox')
         cls.chrome_options.add_argument('--headless')        
         cls.chrome_service = ChromeService(
             executable_path=c4t.location.chromedriver
         )
@@ -69,15 +69,15 @@
 
         self.verify_chrome_for_testing_version_with_selenium(
             expected_version=assets.active_version
         )
 
     def test_002_installation_of_a_specific_version_of_assets(self):     
         assets = c4t.Assets()
-        self.assertTrue(os.path.isdir('./assets'))
+        self.assertTrue(os.path.isdir(self.assets_dir))
         assets.install(self._TestData.specific_version_of_assets)
         self.assertTrue(
             assets.active_version == self._TestData.specific_version_of_assets)
         self.assertTrue(
             os.path.exists(
                 f'{self.assets_dir}/{assets.active_version}/chrome-linux64/chrome'
             )
```

