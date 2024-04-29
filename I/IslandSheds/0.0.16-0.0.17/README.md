# Comparing `tmp/islandsheds-0.0.16.tar.gz` & `tmp/islandsheds-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.16.tar", last modified: Sun Apr 28 22:50:55 2024, max compression
+gzip compressed data, was "islandsheds-0.0.17.tar", last modified: Sun Apr 28 23:56:56 2024, max compression
```

## Comparing `islandsheds-0.0.16.tar` & `islandsheds-0.0.17.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 22:50:55.169384 islandsheds-0.0.16/
-drwxrwxrwx   0        0        0        0 2024-04-28 22:50:55.120380 islandsheds-0.0.16/IslandSheds/
--rw-rw-rw-   0        0        0      893 2024-04-28 22:26:39.000000 islandsheds-0.0.16/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     6227 2024-04-28 22:21:36.000000 islandsheds-0.0.16/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-28 22:50:55.165646 islandsheds-0.0.16/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      844 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      844 2024-04-28 22:50:55.167079 islandsheds-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-28 22:50:55.169384 islandsheds-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-28 22:50:06.000000 islandsheds-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:56:56.278882 islandsheds-0.0.17/
+drwxrwxrwx   0        0        0        0 2024-04-28 23:56:56.228024 islandsheds-0.0.17/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.17/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     6227 2024-04-28 22:21:36.000000 islandsheds-0.0.17/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:56:56.275889 islandsheds-0.0.17/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.17/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-28 23:56:56.276880 islandsheds-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.17/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 23:56:56.278882 islandsheds-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-28 23:55:22.000000 islandsheds-0.0.17/setup.py
```

### Comparing `islandsheds-0.0.16/IslandSheds/__init__.py` & `islandsheds-0.0.17/IslandSheds/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from importlib.metadata import version, PackageNotFoundError
 import inspect
 from .downloader import *
 
 _display_details = True
 
 def configure(display_details=True):
```

### Comparing `islandsheds-0.0.16/IslandSheds/downloader.py` & `islandsheds-0.0.17/IslandSheds/downloader.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.16/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.17/IslandSheds.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.16
+Version: 0.0.17
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
 Project-URL: Tracker, https://github.com/kgdthomas/IslandSheds/issues
 Keywords: watershed geospatial data download Caribbean
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: geopandas
 Requires-Dist: requests
 
 Python package for downloading country-specific Caribbean watershed data.
```

### Comparing `islandsheds-0.0.16/PKG-INFO` & `islandsheds-0.0.17/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.16
+Version: 0.0.17
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
 Project-URL: Tracker, https://github.com/kgdthomas/IslandSheds/issues
 Keywords: watershed geospatial data download Caribbean
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: geopandas
 Requires-Dist: requests
 
 Python package for downloading country-specific Caribbean watershed data.
```

### Comparing `islandsheds-0.0.16/setup.py` & `islandsheds-0.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.16'
+VERSION = '0.0.17'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

