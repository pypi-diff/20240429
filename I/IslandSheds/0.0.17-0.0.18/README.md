# Comparing `tmp/islandsheds-0.0.17.tar.gz` & `tmp/islandsheds-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.17.tar", last modified: Sun Apr 28 23:56:56 2024, max compression
+gzip compressed data, was "islandsheds-0.0.18.tar", last modified: Mon Apr 29 02:00:21 2024, max compression
```

## Comparing `islandsheds-0.0.17.tar` & `islandsheds-0.0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 23:56:56.278882 islandsheds-0.0.17/
-drwxrwxrwx   0        0        0        0 2024-04-28 23:56:56.228024 islandsheds-0.0.17/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.17/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     6227 2024-04-28 22:21:36.000000 islandsheds-0.0.17/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:56:56.275889 islandsheds-0.0.17/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-28 23:56:55.000000 islandsheds-0.0.17/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.17/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-28 23:56:56.276880 islandsheds-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.17/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 23:56:56.278882 islandsheds-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-28 23:55:22.000000 islandsheds-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 02:00:21.810905 islandsheds-0.0.18/
+drwxrwxrwx   0        0        0        0 2024-04-29 02:00:21.793956 islandsheds-0.0.18/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.18/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     6247 2024-04-29 01:55:44.000000 islandsheds-0.0.18/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 02:00:21.807859 islandsheds-0.0.18/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.18/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 02:00:21.809900 islandsheds-0.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.18/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 02:00:21.810905 islandsheds-0.0.18/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 01:58:09.000000 islandsheds-0.0.18/setup.py
```

### Comparing `islandsheds-0.0.17/IslandSheds/__init__.py` & `islandsheds-0.0.18/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.17/IslandSheds/downloader.py` & `islandsheds-0.0.18/IslandSheds/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     geopackage_url = "https://github.com/kgdthomas/IslandSheds/raw/main/CARIBBEAN_WATERSHEDS.gpkg"
     
     # Download the GeoPackage
     response = requests.get(geopackage_url)
     
     if response.status_code == 200:
         # Load the GeoPackage from the response content
-        gdf = gpd.read_file(response.content, layer='watersheds')
+        gdf = gpd.read_file(response.content, layer='caribbean_watersheds')
         
         # Filter data for the specified country
-        country_gdf = gdf[gdf['country'] == country]
+        country_gdf = gdf[gdf['Country'] == country]
         
         # Check and inform user about CRS
         crs = gdf.crs
         print(f"The CRS of the data is {crs}")
         
         # Ask user if they want to change the CRS
         if target_crs:
@@ -76,19 +76,19 @@
     Parameters:
     - geopackage_url (str): The URL to the GeoPackage file.
 
     Outputs:
     - Prints a list of unique countries found in the GeoPackage's 'country' column.
     """
     # Load the GeoPackage directly
-    gdf = gpd.read_file(geopackage_url, layer='watersheds')
-    unique_countries = gdf['country'].unique()
+    gdf = gpd.read_file(geopackage_url, layer='caribbean_watersheds')
+    unique_countries = gdf['Country'].unique()
     print("Available countries in the dataset:")
-    for country in unique_countries:
-        print(country)
+    for Country in unique_countries:
+        print(Country)
 
 def download_watershed(base_url, country, watershed=None, download_dir="//Watershed//"):
     """
     Downloads watershed data for a specified country and optionally a specific watershed.
 
     Parameters:
     - base_url (str): The base URL where watershed data files are hosted.
```

### Comparing `islandsheds-0.0.17/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.18/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.17
+Version: 0.0.18
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.17/LICENSE.txt` & `islandsheds-0.0.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.17/PKG-INFO` & `islandsheds-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.17
+Version: 0.0.18
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.17/setup.py` & `islandsheds-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.17'
+VERSION = '0.0.18'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

