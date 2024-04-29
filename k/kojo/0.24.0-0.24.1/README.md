# Comparing `tmp/kojo-0.24.0.tar.gz` & `tmp/kojo-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojo-0.24.0.tar", last modified: Thu Apr 25 09:52:08 2024, max compression
+gzip compressed data, was "kojo-0.24.1.tar", last modified: Mon Apr 29 08:25:51 2024, max compression
```

## Comparing `kojo-0.24.0.tar` & `kojo-0.24.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 09:52:08.738711 kojo-0.24.0/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    35148 2023-04-27 08:31:58.000000 kojo-0.24.0/LICENSE.txt
--rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-25 09:52:08.738711 kojo-0.24.0/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     3752 2023-04-27 09:07:15.000000 kojo-0.24.0/README.md
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 09:52:08.738711 kojo-0.24.0/kojo/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      346 2024-04-25 09:47:16.000000 kojo-0.24.0/kojo/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1115 2024-04-24 05:46:05.000000 kojo-0.24.0/kojo/extra.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     4696 2024-04-25 08:56:19.000000 kojo-0.24.0/kojo/item.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2368 2024-04-25 09:46:56.000000 kojo-0.24.0/kojo/process.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:40:38.000000 kojo-0.24.0/kojo/py.typed
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-25 09:52:08.738711 kojo-0.24.0/kojo.egg-info/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-25 09:52:08.000000 kojo-0.24.0/kojo.egg-info/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      222 2024-04-25 09:52:08.000000 kojo-0.24.0/kojo.egg-info/SOURCES.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-25 09:52:08.000000 kojo-0.24.0/kojo.egg-info/dependency_links.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        5 2024-04-25 09:52:08.000000 kojo-0.24.0/kojo.egg-info/top_level.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      801 2024-04-25 09:51:34.000000 kojo-0.24.0/pyproject.toml
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-25 09:52:08.738711 kojo-0.24.0/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 08:25:51.933063 kojo-0.24.1/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    35148 2023-04-27 08:31:58.000000 kojo-0.24.1/LICENSE.txt
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-29 08:25:51.933063 kojo-0.24.1/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3752 2023-04-27 09:07:15.000000 kojo-0.24.1/README.md
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 08:25:51.933063 kojo-0.24.1/kojo/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      346 2024-04-25 09:47:16.000000 kojo-0.24.1/kojo/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1115 2024-04-24 05:46:05.000000 kojo-0.24.1/kojo/extra.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     4727 2024-04-29 08:23:02.000000 kojo-0.24.1/kojo/item.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     2368 2024-04-25 09:46:56.000000 kojo-0.24.1/kojo/process.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-25 07:40:38.000000 kojo-0.24.1/kojo/py.typed
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-29 08:25:51.933063 kojo-0.24.1/kojo.egg-info/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-29 08:25:51.000000 kojo-0.24.1/kojo.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      222 2024-04-29 08:25:51.000000 kojo-0.24.1/kojo.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-29 08:25:51.000000 kojo-0.24.1/kojo.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        5 2024-04-29 08:25:51.000000 kojo-0.24.1/kojo.egg-info/top_level.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      801 2024-04-29 08:23:14.000000 kojo-0.24.1/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-29 08:25:51.933063 kojo-0.24.1/setup.cfg
```

### Comparing `kojo-0.24.0/LICENSE.txt` & `kojo-0.24.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kojo-0.24.0/PKG-INFO` & `kojo-0.24.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojo
-Version: 0.24.0
+Version: 0.24.1
 Summary: A library to transform data through a pipeline
 Author-email: Olaf Schneider <mail@olafschneider.com>
 License: GNU GPLv3
 Project-URL: Repository, https://gitlab.com/filchos/kojo
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kojo-0.24.0/README.md` & `kojo-0.24.1/README.md`

 * *Files identical despite different names*

### Comparing `kojo-0.24.0/kojo/extra.py` & `kojo-0.24.1/kojo/extra.py`

 * *Files identical despite different names*

### Comparing `kojo-0.24.0/kojo/item.py` & `kojo-0.24.1/kojo/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def _flatten(item: DictType, prefix: str = "") -> DictType:
     flat_dict = {}
     for k, v in item.items():
         kk = k
         if prefix:
             kk = prefix + "." + k
 
-        if type(v) is dict:
+        if isinstance(v, dict) or isinstance(v, UserDict):
             for ksub, vsub in _flatten(v, kk).items():
                 flat_dict[ksub] = vsub
         else:
             flat_dict[kk] = v
     return flat_dict
```

### Comparing `kojo-0.24.0/kojo/process.py` & `kojo-0.24.1/kojo/process.py`

 * *Files identical despite different names*

### Comparing `kojo-0.24.0/kojo.egg-info/PKG-INFO` & `kojo-0.24.1/kojo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojo
-Version: 0.24.0
+Version: 0.24.1
 Summary: A library to transform data through a pipeline
 Author-email: Olaf Schneider <mail@olafschneider.com>
 License: GNU GPLv3
 Project-URL: Repository, https://gitlab.com/filchos/kojo
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kojo-0.24.0/pyproject.toml` & `kojo-0.24.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kojo"
-version = "0.24.0"
+version = "0.24.1"
 requires-python = ">= 3.10"
 authors = [{ name = "Olaf Schneider", email = "mail@olafschneider.com" }]
 description = "A library to transform data through a pipeline"
 readme = "README.md"
 license = { text = "GNU GPLv3" }
 classifiers = [
     "Development Status :: 4 - Beta",
```

