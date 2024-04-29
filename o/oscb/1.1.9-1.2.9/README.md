# Comparing `tmp/oscb-1.1.9.tar.gz` & `tmp/oscb-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.1.9.tar", last modified: Sun Apr 28 06:25:12 2024, max compression
+gzip compressed data, was "oscb-1.2.9.tar", last modified: Sun Apr 28 06:51:51 2024, max compression
```

## Comparing `oscb-1.1.9.tar` & `oscb-1.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:25:12.588127 oscb-1.1.9/
--rw-rw-rw-   0        0        0       48 2024-04-28 06:24:03.000000 oscb-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      658 2024-04-28 06:25:12.587128 oscb-1.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 06:25:12.548467 oscb-1.1.9/oscb/
--rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.1.9/oscb/__init__.py
--rw-rw-rw-   0        0        0      650 2024-04-28 06:24:57.000000 oscb-1.1.9/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:25:12.585129 oscb-1.1.9/oscb.egg-info/
--rw-rw-rw-   0        0        0      658 2024-04-28 06:25:12.000000 oscb-1.1.9/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-28 06:25:12.000000 oscb-1.1.9/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:25:12.000000 oscb-1.1.9/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-28 06:25:12.000000 oscb-1.1.9/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 06:25:12.000000 oscb-1.1.9/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:25:12.589127 oscb-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1925 2024-04-28 06:24:39.000000 oscb-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:51:51.507456 oscb-1.2.9/
+-rw-rw-rw-   0        0        0       48 2024-04-28 06:24:03.000000 oscb-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      658 2024-04-28 06:51:51.506456 oscb-1.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 06:51:51.471676 oscb-1.2.9/oscb/
+-rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.2.9/oscb/__init__.py
+-rw-rw-rw-   0        0        0      650 2024-04-28 06:51:43.000000 oscb-1.2.9/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:51:51.505457 oscb-1.2.9/oscb.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:51:51.507456 oscb-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2024-04-28 06:51:36.000000 oscb-1.2.9/setup.py
```

### Comparing `oscb-1.1.9/PKG-INFO` & `oscb-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.1.9
+Version: 1.2.9
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oscb-1.1.9/oscb/version.py` & `oscb-1.2.9/oscb/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.1.9'
+__version__ = '1.2.9'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.1.9/oscb.egg-info/PKG-INFO` & `oscb-1.2.9/oscb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.1.9
+Version: 1.2.9
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oscb-1.1.9/setup.py` & `oscb-1.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,18 @@
             oscb_contents.append(os.path.relpath(os.path.join(root, file), here))
         for dir in dirs:
             oscb_contents.append(os.path.relpath(os.path.join(root, dir), here))
     return oscb_contents
 
 # Include the oscb/download_dataset directory as well
 oscb_contents = find_oscb_contents()
-oscb_contents.extend(['oscb/download_dataset/*'])  # Include the download_dataset folder and its contents
 
 setup(
     name='oscb',
-    version='1.1.9',
+    version='1.2.9',
     description='Description of your package',
     long_description='Long description of your package',
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/oscb',
     author='Your Name',
     author_email='your.email@example.com',
     classifiers=[
```

