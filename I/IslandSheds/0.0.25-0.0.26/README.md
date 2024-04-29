# Comparing `tmp/islandsheds-0.0.25.tar.gz` & `tmp/islandsheds-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.25.tar", last modified: Mon Apr 29 07:30:23 2024, max compression
+gzip compressed data, was "islandsheds-0.0.26.tar", last modified: Mon Apr 29 07:38:51 2024, max compression
```

## Comparing `islandsheds-0.0.25.tar` & `islandsheds-0.0.26.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:30:23.887003 islandsheds-0.0.25/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:30:23.860022 islandsheds-0.0.25/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.25/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     8133 2024-04-29 07:28:38.000000 islandsheds-0.0.25/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:30:23.882015 islandsheds-0.0.25/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.25/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 07:30:23.883988 islandsheds-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.25/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 07:30:23.887003 islandsheds-0.0.25/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 07:29:13.000000 islandsheds-0.0.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:38:51.579317 islandsheds-0.0.26/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:38:51.553904 islandsheds-0.0.26/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.26/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     8133 2024-04-29 07:37:42.000000 islandsheds-0.0.26/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:38:51.575920 islandsheds-0.0.26/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.26/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:38:51.578261 islandsheds-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.26/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:38:51.580323 islandsheds-0.0.26/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 07:37:56.000000 islandsheds-0.0.26/setup.py
```

### Comparing `islandsheds-0.0.25/IslandSheds/__init__.py` & `islandsheds-0.0.26/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.25/IslandSheds/downloader.py` & `islandsheds-0.0.26/IslandSheds/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,16 +120,16 @@
     # Check and inform user about CRS
     crs = gdf.crs
     print(f"The CRS of the data is {crs}")
     
     # Display available watersheds in the country
     print(f"Available watersheds in {country}:")
     unique_watersheds = country_gdf['Watershed'].unique()
-    for watershed in unique_watersheds:
-        print(watershed)
+    for Watershed in unique_watersheds:
+        print(Watershed)
     
     # Ask user which watershed to download
     watershed = input("Enter the watershed name to download (or press enter for all watersheds): ")
     
     # Filter for the specific watershed if provided
     if watershed:
         watershed_gdf = country_gdf[country_gdf['Watershed'] == watershed]
```

### Comparing `islandsheds-0.0.25/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.26/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.25
+Version: 0.0.26
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.25/LICENSE.txt` & `islandsheds-0.0.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.25/PKG-INFO` & `islandsheds-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.25
+Version: 0.0.26
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.25/setup.py` & `islandsheds-0.0.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.25'
+VERSION = '0.0.26'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

