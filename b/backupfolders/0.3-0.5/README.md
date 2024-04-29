# Comparing `tmp/backupfolders-0.3.tar.gz` & `tmp/backupfolders-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backupfolders-0.3.tar", last modified: Mon Apr 22 18:33:49 2024, max compression
+gzip compressed data, was "backupfolders-0.5.tar", last modified: Mon Apr 29 16:29:14 2024, max compression
```

## Comparing `backupfolders-0.3.tar` & `backupfolders-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:33:49.241954 backupfolders-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 18:33:46.000000 backupfolders-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-22 18:33:49.241954 backupfolders-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-22 18:33:46.000000 backupfolders-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:33:49.241954 backupfolders-0.3/backupfolders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:33:46.000000 backupfolders-0.3/backupfolders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-22 18:33:46.000000 backupfolders-0.3/backupfolders/backupfolders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:33:49.241954 backupfolders-0.3/backupfolders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-22 18:33:49.000000 backupfolders-0.3/backupfolders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 18:33:49.000000 backupfolders-0.3/backupfolders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:33:49.000000 backupfolders-0.3/backupfolders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 18:33:49.000000 backupfolders-0.3/backupfolders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:33:49.241954 backupfolders-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-22 18:33:46.000000 backupfolders-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:29:14.406022 backupfolders-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 16:29:11.000000 backupfolders-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-29 16:29:14.406022 backupfolders-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-29 16:29:11.000000 backupfolders-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:29:14.406022 backupfolders-0.5/backupfolders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:29:11.000000 backupfolders-0.5/backupfolders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-29 16:29:11.000000 backupfolders-0.5/backupfolders/backupfolders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:29:14.406022 backupfolders-0.5/backupfolders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-29 16:29:14.000000 backupfolders-0.5/backupfolders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-29 16:29:14.000000 backupfolders-0.5/backupfolders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:29:14.000000 backupfolders-0.5/backupfolders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 16:29:14.000000 backupfolders-0.5/backupfolders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:29:14.406022 backupfolders-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 16:29:11.000000 backupfolders-0.5/setup.py
```

### Comparing `backupfolders-0.3/LICENSE` & `backupfolders-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `backupfolders-0.3/PKG-INFO` & `backupfolders-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backupfolders
-Version: 0.3
+Version: 0.5
 Summary: Backup your folders from one location to another with ease.
 Home-page: https://github.com/Fahad-codecraft
 Author: Fahad Devnikar
 Author-email: devnikarfahad@gmail.com
 License: MIT
 Keywords: backup,folders,files
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `backupfolders-0.3/README.md` & `backupfolders-0.5/README.md`

 * *Files identical despite different names*

### Comparing `backupfolders-0.3/backupfolders.egg-info/PKG-INFO` & `backupfolders-0.5/backupfolders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backupfolders
-Version: 0.3
+Version: 0.5
 Summary: Backup your folders from one location to another with ease.
 Home-page: https://github.com/Fahad-codecraft
 Author: Fahad Devnikar
 Author-email: devnikarfahad@gmail.com
 License: MIT
 Keywords: backup,folders,files
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `backupfolders-0.3/setup.py` & `backupfolders-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r") as f:
     long_description = f.read()
 
 setuptools.setup(
   name = 'backupfolders',
-  version = '0.3',
+  version = '0.5',
   license='MIT',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   description = 'Backup your folders from one location to another with ease.',
   author = 'Fahad Devnikar',
   author_email = 'devnikarfahad@gmail.com',
   url = 'https://github.com/Fahad-codecraft',
```

