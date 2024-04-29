# Comparing `tmp/mfprocess-0.0.2.tar.gz` & `tmp/mfprocess-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-0.0.2.tar", last modified: Mon Apr 29 19:29:55 2024, max compression
+gzip compressed data, was "mfprocess-0.0.3.tar", last modified: Mon Apr 29 20:07:27 2024, max compression
```

## Comparing `mfprocess-0.0.2.tar` & `mfprocess-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-29 19:29:55.528270 mfprocess-0.0.2/
--rw-rw-r--   0 agus      (1000) agus      (1000)     1077 2024-04-29 19:10:47.000000 mfprocess-0.0.2/LICENCE
--rw-r--r--   0 agus      (1000) agus      (1000)      647 2024-04-29 19:29:55.528270 mfprocess-0.0.2/PKG-INFO
--rw-rw-r--   0 agus      (1000) agus      (1000)       25 2024-04-29 19:10:47.000000 mfprocess-0.0.2/README.md
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-29 19:29:55.528270 mfprocess-0.0.2/mfprocess/
--rw-rw-r--   0 agus      (1000) agus      (1000)       24 2024-04-29 19:10:47.000000 mfprocess-0.0.2/mfprocess/__init__.py
--rw-rw-r--   0 agus      (1000) agus      (1000)       33 2024-04-29 19:29:24.000000 mfprocess-0.0.2/mfprocess/functions.py
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-29 19:29:55.528270 mfprocess-0.0.2/mfprocess.egg-info/
--rw-r--r--   0 agus      (1000) agus      (1000)      647 2024-04-29 19:29:55.000000 mfprocess-0.0.2/mfprocess.egg-info/PKG-INFO
--rw-rw-r--   0 agus      (1000) agus      (1000)      235 2024-04-29 19:29:55.000000 mfprocess-0.0.2/mfprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)        1 2024-04-29 19:29:55.000000 mfprocess-0.0.2/mfprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       13 2024-04-29 19:29:55.000000 mfprocess-0.0.2/mfprocess.egg-info/requires.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       10 2024-04-29 19:29:55.000000 mfprocess-0.0.2/mfprocess.egg-info/top_level.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       38 2024-04-29 19:29:55.528270 mfprocess-0.0.2/setup.cfg
--rw-rw-r--   0 agus      (1000) agus      (1000)      997 2024-04-29 19:29:24.000000 mfprocess-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:27.075333 mfprocess-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 20:07:22.000000 mfprocess-0.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 20:07:27.075333 mfprocess-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 20:07:22.000000 mfprocess-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:27.075333 mfprocess-0.0.3/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 20:07:22.000000 mfprocess-0.0.3/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 20:07:22.000000 mfprocess-0.0.3/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:27.075333 mfprocess-0.0.3/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 20:07:27.000000 mfprocess-0.0.3/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 20:07:27.000000 mfprocess-0.0.3/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:07:27.000000 mfprocess-0.0.3/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 20:07:27.000000 mfprocess-0.0.3/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 20:07:27.000000 mfprocess-0.0.3/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:07:27.075333 mfprocess-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 20:07:22.000000 mfprocess-0.0.3/setup.py
```

### Comparing `mfprocess-0.0.2/LICENCE` & `mfprocess-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-0.0.2/PKG-INFO` & `mfprocess-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-0.0.2/mfprocess.egg-info/PKG-INFO` & `mfprocess-0.0.3/mfprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-0.0.2/setup.py` & `mfprocess-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '0.0.2',   #'{{VERSION_PLACEHOLDER}}',
+    version= '0.0.3',   #'{{VERSION_PLACEHOLDER}}',
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

