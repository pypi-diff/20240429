# Comparing `tmp/oscb-1.2.9.tar.gz` & `tmp/oscb-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscb-1.2.9.tar", last modified: Sun Apr 28 06:51:51 2024, max compression
+gzip compressed data, was "oscb-1.3.9.tar", last modified: Mon Apr 29 01:48:48 2024, max compression
```

## Comparing `oscb-1.2.9.tar` & `oscb-1.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:51:51.507456 oscb-1.2.9/
--rw-rw-rw-   0        0        0       48 2024-04-28 06:24:03.000000 oscb-1.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0      658 2024-04-28 06:51:51.506456 oscb-1.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-28 06:51:51.471676 oscb-1.2.9/oscb/
--rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.2.9/oscb/__init__.py
--rw-rw-rw-   0        0        0      650 2024-04-28 06:51:43.000000 oscb-1.2.9/oscb/version.py
-drwxrwxrwx   0        0        0        0 2024-04-28 06:51:51.505457 oscb-1.2.9/oscb.egg-info/
--rw-rw-rw-   0        0        0      658 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 06:51:51.000000 oscb-1.2.9/oscb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:51:51.507456 oscb-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1818 2024-04-28 06:51:36.000000 oscb-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 01:48:48.668681 oscb-1.3.9/
+-rw-rw-rw-   0        0        0       48 2024-04-28 06:24:03.000000 oscb-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      658 2024-04-29 01:48:48.668681 oscb-1.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 01:48:48.625198 oscb-1.3.9/oscb/
+-rw-rw-rw-   0        0        0       32 2024-03-11 22:44:16.000000 oscb-1.3.9/oscb/__init__.py
+-rw-rw-rw-   0        0        0      650 2024-04-29 01:45:56.000000 oscb-1.3.9/oscb/version.py
+drwxrwxrwx   0        0        0        0 2024-04-29 01:48:48.666696 oscb-1.3.9/oscb.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-04-29 01:48:48.000000 oscb-1.3.9/oscb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-29 01:48:48.000000 oscb-1.3.9/oscb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 01:48:48.000000 oscb-1.3.9/oscb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-29 01:48:48.000000 oscb-1.3.9/oscb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-29 01:48:48.000000 oscb-1.3.9/oscb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 01:48:48.668681 oscb-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1670 2024-04-29 01:48:40.000000 oscb-1.3.9/setup.py
```

### Comparing `oscb-1.2.9/PKG-INFO` & `oscb-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.2.9
+Version: 1.3.9
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oscb-1.2.9/oscb/version.py` & `oscb-1.3.9/oscb/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '1.2.9'
+__version__ = '1.3.9'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `oscb-1.2.9/oscb.egg-info/PKG-INFO` & `oscb-1.3.9/oscb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oscb
-Version: 1.2.9
+Version: 1.3.9
 Summary: Description of your package
 Home-page: https://github.com/your_username/oscb
 Author: Your Name
 Author-email: your.email@example.com
 Keywords: sample setuptools development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oscb-1.2.9/setup.py` & `oscb-1.3.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from setuptools import setup, find_packages
 import os
 
 # Get the current directory
 here = os.path.abspath(os.path.dirname(__file__))
 
-# Function to collect all files and directories under oscb folder
-def find_oscb_contents():
-    oscb_contents = []
-    for root, dirs, files in os.walk(os.path.join(here, 'oscb')):
+# Function to collect all files under oscb folder
+def find_oscb_files():
+    oscb_files = []
+    for root, _, files in os.walk(os.path.join(here, 'oscb')):
         for file in files:
-            oscb_contents.append(os.path.relpath(os.path.join(root, file), here))
-        for dir in dirs:
-            oscb_contents.append(os.path.relpath(os.path.join(root, dir), here))
-    return oscb_contents
+            oscb_files.append(os.path.relpath(os.path.join(root, file), here))
+    return oscb_files
 
 # Include the oscb/download_dataset directory as well
-oscb_contents = find_oscb_contents()
+oscb_files = find_oscb_files()
 
 setup(
     name='oscb',
-    version='1.2.9',
+    version='1.3.9',
     description='Description of your package',
     long_description='Long description of your package',
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/oscb',
     author='Your Name',
     author_email='your.email@example.com',
     classifiers=[
@@ -33,15 +31,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     keywords='sample setuptools development',
     packages=find_packages(),
-    package_data={'oscb': oscb_contents},  # Specify package data directly
+    package_data={'oscb': oscb_files},  # Specify package data directly
     include_package_data=True,
     install_requires=[
         'torch>=1.6.0',
         'numpy>=1.16.0',
         'tqdm>=4.29.0',
         'scikit-learn>=0.20.0',
         'pandas>=0.24.0',
```

