# Comparing `tmp/myelectricaldatapy-2.1.9.tar.gz` & `tmp/myelectricaldatapy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.1.9.tar", last modified: Fri Apr 26 15:57:14 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.2.0.tar", last modified: Mon Apr 29 07:26:24 2024, max compression
```

## Comparing `myelectricaldatapy-2.1.9.tar` & `myelectricaldatapy-2.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.455092 myelectricaldatapy-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.451092 myelectricaldatapy-2.1.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.451092 myelectricaldatapy-2.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.github/workflows/dependbot-auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.451092 myelectricaldatapy-2.1.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-26 15:57:14.455092 myelectricaldatapy-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.455092 myelectricaldatapy-2.1.9/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.455092 myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-26 15:57:14.000000 myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 15:57:14.000000 myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:57:14.000000 myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:57:14.000000 myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:57:14.000000 myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:57:14.455092 myelectricaldatapy-2.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:14.455092 myelectricaldatapy-2.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-26 15:57:00.000000 myelectricaldatapy-2.1.9/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.783862 myelectricaldatapy-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/dependbot-auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.9/.github/dependabot.yml` & `myelectricaldatapy-2.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/.github/workflows/dependbot-auto-approve.yml` & `myelectricaldatapy-2.2.0/.github/workflows/dependbot-auto-approve.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/.github/workflows/lint.yml` & `myelectricaldatapy-2.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.2.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/.github/workflows/release.yml` & `myelectricaldatapy-2.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/.gitignore` & `myelectricaldatapy-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/.pre-commit-config.yaml` & `myelectricaldatapy-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/LICENSE` & `myelectricaldatapy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/PKG-INFO` & `myelectricaldatapy-2.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.9
+Version: 2.2.0
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.9/README.md` & `myelectricaldatapy-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/example.py` & `myelectricaldatapy-2.2.0/example.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.2.0/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.2.0/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.2.0/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.2.0/myelectricaldatapy/mypdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,21 +181,21 @@
             if self.access.get("quota_reached", False):
                 detail = self.access.get("information", "Quota reached")
                 raise LimitReached(409, {"detail": detail})
 
             if self.is_connected is False:
                 raise EnedisException(200, {"detail": "Api access not valid"})
 
-            if not self.contract:
+            if not self.contract and self.has_collected is False:
                 try:
                     self.contract = await self._api.async_get_contract(self.pdl)
                 except EnedisException as error:
                     _LOGGER.warning(error)
 
-            if not self.address:
+            if not self.address and self.has_collected is False:
                 try:
                     self.address = await self._api.async_get_address(self.pdl)
                 except EnedisException as error:
                     _LOGGER.warning(error)
 
             if not self.ecowatt and self._ecowatt_subs:
                 self.ecowatt = await self._api.async_get_ecowatt(start, end)
```

### Comparing `myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.9
+Version: 2.2.0
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.9/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/pyproject.toml` & `myelectricaldatapy-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/tests/conftest.py` & `myelectricaldatapy-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/tests/consts.py` & `myelectricaldatapy-2.2.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/tests/test_analytics.py` & `myelectricaldatapy-2.2.0/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.9/tests/test_load_data.py` & `myelectricaldatapy-2.2.0/tests/test_load_data.py`

 * *Files identical despite different names*

