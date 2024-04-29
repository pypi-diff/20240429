# Comparing `tmp/backupfolders-0.3.tar.gz` & `tmp/backupfolders-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backupfolders-0.3.tar", last modified: Mon Apr 22 18:33:49 2024, max compression
+gzip compressed data, was "backupfolders-0.4.tar", last modified: Mon Apr 29 16:17:19 2024, max compression
```

## Comparing `backupfolders-0.3.tar` & `backupfolders-0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:17:19.238134 backupfolders-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 16:17:16.000000 backupfolders-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-29 16:17:19.238134 backupfolders-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-29 16:17:16.000000 backupfolders-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:17:19.234135 backupfolders-0.4/backupfolders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:17:16.000000 backupfolders-0.4/backupfolders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-29 16:17:16.000000 backupfolders-0.4/backupfolders/backupfolders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:17:19.234135 backupfolders-0.4/backupfolders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-29 16:17:19.000000 backupfolders-0.4/backupfolders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-29 16:17:19.000000 backupfolders-0.4/backupfolders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:17:19.000000 backupfolders-0.4/backupfolders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 16:17:19.000000 backupfolders-0.4/backupfolders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 16:17:19.000000 backupfolders-0.4/backupfolders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:17:19.238134 backupfolders-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-29 16:17:16.000000 backupfolders-0.4/setup.py
```

### Comparing `backupfolders-0.3/LICENSE` & `backupfolders-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `backupfolders-0.3/PKG-INFO` & `backupfolders-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: backupfolders
-Version: 0.3
+Version: 0.4
 Summary: Backup your folders from one location to another with ease.
 Home-page: https://github.com/Fahad-codecraft
 Author: Fahad Devnikar
 Author-email: devnikarfahad@gmail.com
 License: MIT
 Keywords: backup,folders,files
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: shutil
+Requires-Dist: datetime
+Requires-Dist: filecmp
 
 # Python Backup Script
 
 This Python script performs backups of a specified directory to another location. It can be useful for creating regular backups of important data.
 
 ## Features
```

### Comparing `backupfolders-0.3/README.md` & `backupfolders-0.4/README.md`

 * *Files identical despite different names*

### Comparing `backupfolders-0.3/backupfolders.egg-info/PKG-INFO` & `backupfolders-0.4/backupfolders.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: backupfolders
-Version: 0.3
+Version: 0.4
 Summary: Backup your folders from one location to another with ease.
 Home-page: https://github.com/Fahad-codecraft
 Author: Fahad Devnikar
 Author-email: devnikarfahad@gmail.com
 License: MIT
 Keywords: backup,folders,files
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: shutil
+Requires-Dist: datetime
+Requires-Dist: filecmp
 
 # Python Backup Script
 
 This Python script performs backups of a specified directory to another location. It can be useful for creating regular backups of important data.
 
 ## Features
```

### Comparing `backupfolders-0.3/setup.py` & `backupfolders-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import setuptools
 
 with open("README.md","r") as f:
     long_description = f.read()
 
 setuptools.setup(
   name = 'backupfolders',
-  version = '0.3',
+  version = '0.4',
   license='MIT',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   description = 'Backup your folders from one location to another with ease.',
   author = 'Fahad Devnikar',
   author_email = 'devnikarfahad@gmail.com',
   url = 'https://github.com/Fahad-codecraft',
   keywords = ['backup', 'folders', 'files'],
   install_requires=[
+          'shutil',
+          'datetime',
+          'filecmp'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
```

