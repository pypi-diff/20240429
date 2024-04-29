# Comparing `tmp/lightning_extensions-0.0.7.tar.gz` & `tmp/lightning_extensions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_extensions-0.0.7.tar", last modified: Thu Nov 23 21:35:17 2023, max compression
+gzip compressed data, was "lightning_extensions-0.0.9.tar", last modified: Thu Nov 23 23:26:46 2023, max compression
```

## Comparing `lightning_extensions-0.0.7.tar` & `lightning_extensions-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 21:35:17.625783 lightning_extensions-0.0.7/
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)     1073 2023-10-25 20:36:56.000000 lightning_extensions-0.0.7/LICENSE
--rw-r--r--   0 edvardsz  (1000) edvardsz  (1000)      626 2023-11-23 21:35:17.625783 lightning_extensions-0.0.7/PKG-INFO
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       63 2023-10-24 19:01:26.000000 lightning_extensions-0.0.7/README.md
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      636 2023-11-23 21:33:14.000000 lightning_extensions-0.0.7/pyproject.toml
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       38 2023-11-23 21:35:17.625783 lightning_extensions-0.0.7/setup.cfg
-drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 21:35:17.621783 lightning_extensions-0.0.7/src/
-drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 21:35:17.621783 lightning_extensions-0.0.7/src/lightning_extensions/
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       31 2023-11-23 21:32:05.000000 lightning_extensions-0.0.7/src/lightning_extensions/__init__.py
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      874 2023-10-29 10:59:42.000000 lightning_extensions-0.0.7/src/lightning_extensions/base_module.py
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)     1474 2023-11-23 21:31:31.000000 lightning_extensions-0.0.7/src/lightning_extensions/extended_trainer.py
-drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 21:35:17.621783 lightning_extensions-0.0.7/src/lightning_extensions.egg-info/
--rw-r--r--   0 edvardsz  (1000) edvardsz  (1000)      626 2023-11-23 21:35:17.000000 lightning_extensions-0.0.7/src/lightning_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      346 2023-11-23 21:35:17.000000 lightning_extensions-0.0.7/src/lightning_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)        1 2023-11-23 21:35:17.000000 lightning_extensions-0.0.7/src/lightning_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       21 2023-11-23 21:35:17.000000 lightning_extensions-0.0.7/src/lightning_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 23:26:46.866284 lightning_extensions-0.0.9/
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)     1073 2023-10-25 20:36:56.000000 lightning_extensions-0.0.9/LICENSE
+-rw-r--r--   0 edvardsz  (1000) edvardsz  (1000)      626 2023-11-23 23:26:46.862284 lightning_extensions-0.0.9/PKG-INFO
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       63 2023-10-24 19:01:26.000000 lightning_extensions-0.0.9/README.md
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      636 2023-11-23 23:25:14.000000 lightning_extensions-0.0.9/pyproject.toml
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       38 2023-11-23 23:26:46.866284 lightning_extensions-0.0.9/setup.cfg
+drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 23:26:46.862284 lightning_extensions-0.0.9/src/
+drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 23:26:46.862284 lightning_extensions-0.0.9/src/lightning_extensions/
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       31 2023-11-23 21:32:05.000000 lightning_extensions-0.0.9/src/lightning_extensions/__init__.py
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      874 2023-10-29 10:59:42.000000 lightning_extensions-0.0.9/src/lightning_extensions/base_module.py
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      540 2023-11-23 22:41:34.000000 lightning_extensions-0.0.9/src/lightning_extensions/data_module.py
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)     2706 2023-11-23 22:48:33.000000 lightning_extensions-0.0.9/src/lightning_extensions/extended_trainer.py
+drwxrwxr-x   0 edvardsz  (1000) edvardsz  (1000)        0 2023-11-23 23:26:46.862284 lightning_extensions-0.0.9/src/lightning_extensions.egg-info/
+-rw-r--r--   0 edvardsz  (1000) edvardsz  (1000)      626 2023-11-23 23:26:46.000000 lightning_extensions-0.0.9/src/lightning_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)      386 2023-11-23 23:26:46.000000 lightning_extensions-0.0.9/src/lightning_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)        1 2023-11-23 23:26:46.000000 lightning_extensions-0.0.9/src/lightning_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 edvardsz  (1000) edvardsz  (1000)       21 2023-11-23 23:26:46.000000 lightning_extensions-0.0.9/src/lightning_extensions.egg-info/top_level.txt
```

### Comparing `lightning_extensions-0.0.7/LICENSE` & `lightning_extensions-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_extensions-0.0.7/PKG-INFO` & `lightning_extensions-0.0.9/src/lightning_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lightning_extensions
-Version: 0.0.7
+Name: lightning-extensions
+Version: 0.0.9
 Summary: A small lightning extension package
 Author-email: Edvards Zakovskis <edvards1999@gmail.com>
 Project-URL: Homepage, https://github.com/EdvardsZ/LightningExtensions
 Project-URL: Bug Tracker, https://github.com/EdvardsZ/LightningExtensions/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lightning_extensions-0.0.7/pyproject.toml` & `lightning_extensions-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightning_extensions"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Edvards Zakovskis", email="edvards1999@gmail.com" },
 ]
 description = "A small lightning extension package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lightning_extensions-0.0.7/src/lightning_extensions/base_module.py` & `lightning_extensions-0.0.9/src/lightning_extensions/base_module.py`

 * *Files identical despite different names*

### Comparing `lightning_extensions-0.0.7/src/lightning_extensions.egg-info/PKG-INFO` & `lightning_extensions-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lightning-extensions
-Version: 0.0.7
+Name: lightning_extensions
+Version: 0.0.9
 Summary: A small lightning extension package
 Author-email: Edvards Zakovskis <edvards1999@gmail.com>
 Project-URL: Homepage, https://github.com/EdvardsZ/LightningExtensions
 Project-URL: Bug Tracker, https://github.com/EdvardsZ/LightningExtensions/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

