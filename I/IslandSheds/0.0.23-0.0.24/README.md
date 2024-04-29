# Comparing `tmp/islandsheds-0.0.23.tar.gz` & `tmp/islandsheds-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.23.tar", last modified: Mon Apr 29 07:09:30 2024, max compression
+gzip compressed data, was "islandsheds-0.0.24.tar", last modified: Mon Apr 29 07:16:20 2024, max compression
```

## Comparing `islandsheds-0.0.23.tar` & `islandsheds-0.0.24.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:09:30.145007 islandsheds-0.0.23/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:09:30.121191 islandsheds-0.0.23/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.23/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7621 2024-04-29 07:08:16.000000 islandsheds-0.0.23/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:09:30.141917 islandsheds-0.0.23/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.23/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 07:09:30.142931 islandsheds-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.23/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 07:09:30.145007 islandsheds-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 07:08:31.000000 islandsheds-0.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:16:20.797295 islandsheds-0.0.24/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:16:20.767240 islandsheds-0.0.24/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.24/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7623 2024-04-29 07:15:13.000000 islandsheds-0.0.24/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:16:20.793636 islandsheds-0.0.24/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.24/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:16:20.795216 islandsheds-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.24/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:16:20.797295 islandsheds-0.0.24/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 07:15:30.000000 islandsheds-0.0.24/setup.py
```

### Comparing `islandsheds-0.0.23/IslandSheds/__init__.py` & `islandsheds-0.0.24/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.23/IslandSheds/downloader.py` & `islandsheds-0.0.24/IslandSheds/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         
         # Download the country data
         download_country(country, output_dir, target_crs)
     
     elif choice == '2':
         # Get user input for country, watershed, and download directory
         country = input("Enter the country name for the watershed: ")
-        watershed = input("Enter the watershed name (or press enter for all watersheds): ")
+        # watershed = input("Enter the watershed name (or press enter for all watersheds): ")
         download_dir = input("Enter download directory (default is .//Watershed//): ")
         download_dir = download_dir if download_dir else ".//Watershed//"
         
         # Download the watershed data
         download_watershed(geopackage_url, country, download_dir)
     
     else:
```

### Comparing `islandsheds-0.0.23/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.24/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.23
+Version: 0.0.24
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.23/LICENSE.txt` & `islandsheds-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.23/PKG-INFO` & `islandsheds-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.23
+Version: 0.0.24
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.23/setup.py` & `islandsheds-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.23'
+VERSION = '0.0.24'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

