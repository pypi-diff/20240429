# Comparing `tmp/islandsheds-0.0.21.tar.gz` & `tmp/islandsheds-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.21.tar", last modified: Mon Apr 29 06:47:43 2024, max compression
+gzip compressed data, was "islandsheds-0.0.22.tar", last modified: Mon Apr 29 06:55:58 2024, max compression
```

## Comparing `islandsheds-0.0.21.tar` & `islandsheds-0.0.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:47:43.585521 islandsheds-0.0.21/
-drwxrwxrwx   0        0        0        0 2024-04-29 06:47:43.564238 islandsheds-0.0.21/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.21/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7615 2024-04-29 06:42:09.000000 islandsheds-0.0.21/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:47:43.582514 islandsheds-0.0.21/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.21/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 06:47:43.584530 islandsheds-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.21/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 06:47:43.586527 islandsheds-0.0.21/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 06:45:19.000000 islandsheds-0.0.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:55:58.581755 islandsheds-0.0.22/
+drwxrwxrwx   0        0        0        0 2024-04-29 06:55:58.553197 islandsheds-0.0.22/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.22/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7619 2024-04-29 06:54:35.000000 islandsheds-0.0.22/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:55:58.577227 islandsheds-0.0.22/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.22/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 06:55:58.579757 islandsheds-0.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.22/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 06:55:58.581755 islandsheds-0.0.22/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 06:54:56.000000 islandsheds-0.0.22/setup.py
```

### Comparing `islandsheds-0.0.21/IslandSheds/__init__.py` & `islandsheds-0.0.22/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.21/IslandSheds/downloader.py` & `islandsheds-0.0.22/IslandSheds/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         watershed_gdf = country_gdf
     
     # Save the filtered data to a GeoJSON file
     output_file_path = os.path.join(download_dir, f"{country}_{watershed or 'all_watersheds'}.geojson")
     watershed_gdf.to_file(output_file_path, driver='GeoJSON')
     
     print(f"Downloaded {watershed or 'all watersheds'} for {country} successfully.")
-
+    
 def main():
     """
     Main function to run the Watershed Downloader program.
 
     Interactively prompts the user to enter a country name, an optional watershed name, and a download directory. It then downloads the specified watershed data using the provided details.
     """
     # URL to the GeoPackage
```

### Comparing `islandsheds-0.0.21/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.22/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.21
+Version: 0.0.22
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.21/LICENSE.txt` & `islandsheds-0.0.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.21/PKG-INFO` & `islandsheds-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.21
+Version: 0.0.22
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.21/setup.py` & `islandsheds-0.0.22/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.21'
+VERSION = '0.0.22'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

