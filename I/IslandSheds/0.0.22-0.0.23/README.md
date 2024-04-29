# Comparing `tmp/islandsheds-0.0.22.tar.gz` & `tmp/islandsheds-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.22.tar", last modified: Mon Apr 29 06:55:58 2024, max compression
+gzip compressed data, was "islandsheds-0.0.23.tar", last modified: Mon Apr 29 07:09:30 2024, max compression
```

## Comparing `islandsheds-0.0.22.tar` & `islandsheds-0.0.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:55:58.581755 islandsheds-0.0.22/
-drwxrwxrwx   0        0        0        0 2024-04-29 06:55:58.553197 islandsheds-0.0.22/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.22/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7619 2024-04-29 06:54:35.000000 islandsheds-0.0.22/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:55:58.577227 islandsheds-0.0.22/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 06:55:58.000000 islandsheds-0.0.22/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.22/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 06:55:58.579757 islandsheds-0.0.22/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.22/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 06:55:58.581755 islandsheds-0.0.22/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 06:54:56.000000 islandsheds-0.0.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:09:30.145007 islandsheds-0.0.23/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:09:30.121191 islandsheds-0.0.23/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.23/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7621 2024-04-29 07:08:16.000000 islandsheds-0.0.23/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:09:30.141917 islandsheds-0.0.23/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 07:09:29.000000 islandsheds-0.0.23/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.23/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:09:30.142931 islandsheds-0.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.23/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:09:30.145007 islandsheds-0.0.23/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 07:08:31.000000 islandsheds-0.0.23/setup.py
```

### Comparing `islandsheds-0.0.22/IslandSheds/__init__.py` & `islandsheds-0.0.23/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.22/IslandSheds/downloader.py` & `islandsheds-0.0.23/IslandSheds/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,42 @@
 import geopandas as gpd
 import os
 import requests
 
+def create_directory(directory):
+    """
+    Creates a directory if it does not already exist.
+
+    Parameters:
+    - directory (str): The path of the directory to be created.
+
+    Effects:
+    - A new directory is created at the specified path if it does not exist. If the directory already exists, no action is taken.
+    """
+    # Check if the directory exists and create it if it doesn't
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+def show_available_datasets(geopackage_url):
+    """
+    Loads a GeoPackage and displays all unique countries available in the 'country' column of the dataset.
+
+    Parameters:
+    - geopackage_url (str): The URL to the GeoPackage file.
+
+    Outputs:
+    - Prints a list of unique countries found in the GeoPackage's 'country' column.
+    """
+    # Load the GeoPackage directly
+    gdf = gpd.read_file(geopackage_url, layer='caribbean_watersheds')
+    unique_countries = gdf['Country'].unique()
+    print("Available countries in the dataset:")
+    for Country in unique_countries:
+        print(Country)
+
 def download_country(country, output_dir=".//Watershed//", target_crs=None):
     """
     Downloads and saves watershed data for a specified country from a GeoPackage.
 
     Parameters:
     - country (str): The name of the country for which watershed data is to be downloaded.
     - output_dir (str): The directory where the GeoPackage will be saved. Defaults to ".//Watershed//".
@@ -56,56 +87,25 @@
         output_file_path = os.path.join(output_dir, f"{country}_watersheds.gpkg")
         country_gdf.to_file(output_file_path, driver='GPKG')
         
         print(f"Data for {country} downloaded successfully.")
     else:
         print(f"Failed to download GeoPackage. Status code: {response.status_code}")
 
-def create_directory(directory):
-    """
-    Creates a directory if it does not already exist.
-
-    Parameters:
-    - directory (str): The path of the directory to be created.
-
-    Effects:
-    - A new directory is created at the specified path if it does not exist. If the directory already exists, no action is taken.
-    """
-    # Check if the directory exists and create it if it doesn't
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-
-def show_available_datasets(geopackage_url):
-    """
-    Loads a GeoPackage and displays all unique countries available in the 'country' column of the dataset.
-
-    Parameters:
-    - geopackage_url (str): The URL to the GeoPackage file.
-
-    Outputs:
-    - Prints a list of unique countries found in the GeoPackage's 'country' column.
-    """
-    # Load the GeoPackage directly
-    gdf = gpd.read_file(geopackage_url, layer='caribbean_watersheds')
-    unique_countries = gdf['Country'].unique()
-    print("Available countries in the dataset:")
-    for Country in unique_countries:
-        print(Country)
-
 def download_watershed(geopackage_url, country, download_dir="//Watershed//"):
     """
     Downloads watershed data for a specified country and optionally a specific watershed.
 
     Parameters:
     - geopackage_url (str): The URL to the GeoPackage file.
     - country (str): The country for which watershed data is to be downloaded.
     - download_dir (str): The directory where the watershed data will be saved. Defaults to "//Watershed//".
 
     Outputs:
-    - Downloads and saves the specified watershed data as a GeoJSON file in the specified directory.
+    - Downloads and saves the specified watershed data as a GPKG file in the specified directory.
     - Console messages about the status of the download.
 
     Raises:
     - Prints an error message if the data cannot be downloaded (e.g., due to network issues or an incorrect URL).
     """
     # Ensure the output directory exists
     if not os.path.exists(download_dir):
@@ -128,17 +128,17 @@
     
     # Filter for the specific watershed if provided
     if watershed:
         watershed_gdf = country_gdf[country_gdf['Watershed'] == watershed]
     else:
         watershed_gdf = country_gdf
     
-    # Save the filtered data to a GeoJSON file
-    output_file_path = os.path.join(download_dir, f"{country}_{watershed or 'all_watersheds'}.geojson")
-    watershed_gdf.to_file(output_file_path, driver='GeoJSON')
+    # Save the filtered data to a GPKG file
+    output_file_path = os.path.join(download_dir, f"{country}_{watershed or 'all_watersheds'}.gpkg")
+    watershed_gdf.to_file(output_file_path, layer='data', driver='GPKG')
     
     print(f"Downloaded {watershed or 'all watersheds'} for {country} successfully.")
     
 def main():
     """
     Main function to run the Watershed Downloader program.
```

### Comparing `islandsheds-0.0.22/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.23/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.22
+Version: 0.0.23
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.22/LICENSE.txt` & `islandsheds-0.0.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.22/PKG-INFO` & `islandsheds-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.22
+Version: 0.0.23
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.22/setup.py` & `islandsheds-0.0.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.22'
+VERSION = '0.0.23'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

