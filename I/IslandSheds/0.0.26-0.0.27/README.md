# Comparing `tmp/islandsheds-0.0.26.tar.gz` & `tmp/islandsheds-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.26.tar", last modified: Mon Apr 29 07:38:51 2024, max compression
+gzip compressed data, was "islandsheds-0.0.27.tar", last modified: Mon Apr 29 07:46:05 2024, max compression
```

## Comparing `islandsheds-0.0.26.tar` & `islandsheds-0.0.27.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:38:51.579317 islandsheds-0.0.26/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:38:51.553904 islandsheds-0.0.26/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.26/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     8133 2024-04-29 07:37:42.000000 islandsheds-0.0.26/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:38:51.575920 islandsheds-0.0.26/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 07:38:51.000000 islandsheds-0.0.26/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.26/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 07:38:51.578261 islandsheds-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.26/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 07:38:51.580323 islandsheds-0.0.26/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 07:37:56.000000 islandsheds-0.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:46:05.895320 islandsheds-0.0.27/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:46:05.868570 islandsheds-0.0.27/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.27/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     8373 2024-04-29 07:45:08.000000 islandsheds-0.0.27/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:46:05.892370 islandsheds-0.0.27/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:46:05.000000 islandsheds-0.0.27/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 07:46:05.000000 islandsheds-0.0.27/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:46:05.000000 islandsheds-0.0.27/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 07:46:05.000000 islandsheds-0.0.27/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 07:46:05.000000 islandsheds-0.0.27/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 07:46:05.000000 islandsheds-0.0.27/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.27/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:46:05.894367 islandsheds-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.27/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:46:05.895320 islandsheds-0.0.27/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 07:45:30.000000 islandsheds-0.0.27/setup.py
```

### Comparing `islandsheds-0.0.26/IslandSheds/__init__.py` & `islandsheds-0.0.27/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.26/IslandSheds/downloader.py` & `islandsheds-0.0.27/IslandSheds/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,22 +173,26 @@
         output_dir = output_dir if output_dir else ".//Watershed//"
         target_crs = input("Enter target CRS (optional): ")
         
         # Download the country data
         download_country(country, output_dir, target_crs)
     
     elif choice == '2':
-        # Get user input for country, watershed, and download directory
+        # Get user input for country
         country = input("Enter the country name for the watershed: ")
-        # watershed = input("Enter the watershed name (or press enter for all watersheds): ")
+        # Display available watersheds for the chosen country
+        download_watershed(geopackage_url, country)  # Temporarily call with only URL and country
+        
+        # Get user input for specific watershed and download directory
+        watershed = input("Enter the watershed name to download (or press enter for all watersheds): ")
         download_dir = input("Enter download directory (default is .//Watershed//): ")
         download_dir = download_dir if download_dir else ".//Watershed//"
         target_crs = input("Enter target CRS (optional): ")
         
-        # Download the watershed data
-        download_watershed(geopackage_url, country, download_dir, target_crs)
+        # Download the specified watershed data
+        download_watershed(geopackage_url, country, download_dir, target_crs, watershed)
     
     else:
         print("Invalid choice. Please restart the program and enter 1 or 2.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `islandsheds-0.0.26/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.27/IslandSheds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.26
+Version: 0.0.27
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.26/LICENSE.txt` & `islandsheds-0.0.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.26/PKG-INFO` & `islandsheds-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.26
+Version: 0.0.27
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.26/setup.py` & `islandsheds-0.0.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.26'
+VERSION = '0.0.27'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

