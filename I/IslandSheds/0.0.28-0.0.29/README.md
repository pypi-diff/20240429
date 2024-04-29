# Comparing `tmp/islandsheds-0.0.28.tar.gz` & `tmp/islandsheds-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.28.tar", last modified: Mon Apr 29 07:54:08 2024, max compression
+gzip compressed data, was "islandsheds-0.0.29.tar", last modified: Mon Apr 29 08:01:50 2024, max compression
```

## Comparing `islandsheds-0.0.28.tar` & `islandsheds-0.0.29.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:54:08.762725 islandsheds-0.0.28/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:54:08.734287 islandsheds-0.0.28/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.28/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7539 2024-04-29 07:53:11.000000 islandsheds-0.0.28/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:54:08.757744 islandsheds-0.0.28/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 07:54:08.000000 islandsheds-0.0.28/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 07:54:08.000000 islandsheds-0.0.28/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:54:08.000000 islandsheds-0.0.28/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 07:54:08.000000 islandsheds-0.0.28/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 07:54:08.000000 islandsheds-0.0.28/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 07:54:08.000000 islandsheds-0.0.28/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.28/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 07:54:08.758722 islandsheds-0.0.28/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.28/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 07:54:08.762725 islandsheds-0.0.28/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 07:53:30.000000 islandsheds-0.0.28/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:01:50.290850 islandsheds-0.0.29/
+drwxrwxrwx   0        0        0        0 2024-04-29 08:01:50.265779 islandsheds-0.0.29/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.29/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7606 2024-04-29 08:00:17.000000 islandsheds-0.0.29/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:01:50.287850 islandsheds-0.0.29/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 08:01:49.000000 islandsheds-0.0.29/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 08:01:50.000000 islandsheds-0.0.29/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:01:49.000000 islandsheds-0.0.29/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 08:01:49.000000 islandsheds-0.0.29/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 08:01:49.000000 islandsheds-0.0.29/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 08:01:49.000000 islandsheds-0.0.29/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.29/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 08:01:50.289852 islandsheds-0.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.29/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:01:50.290850 islandsheds-0.0.29/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 08:00:31.000000 islandsheds-0.0.29/setup.py
```

### Comparing `islandsheds-0.0.28/IslandSheds/__init__.py` & `islandsheds-0.0.29/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.28/IslandSheds/downloader.py` & `islandsheds-0.0.29/IslandSheds/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         output_file_path = os.path.join(output_dir, f"{country}_watersheds.gpkg")
         country_gdf.to_file(output_file_path, driver='GPKG')
         
         print(f"Data for {country} downloaded successfully.")
     else:
         print(f"Failed to download GeoPackage. Status code: {response.status_code}")
 
-def download_watershed(geopackage_url, country, download_dir="//Watershed//", target_crs=None, watershed=None):
+def download_watershed(geopackage_url, country, download_dir="./Watershed/", target_crs=None, watershed=None):
     """
     Downloads watershed data for a specified country and optionally a specific watershed.
 
     Parameters:
     - geopackage_url (str): The URL to the GeoPackage file.
     - country (str): The country for which watershed data is to be downloaded.
     - download_dir (str): The directory where the watershed data will be saved. Defaults to "//Watershed//".
@@ -140,36 +140,36 @@
     # Save the filtered data to a GPKG file
     output_file_path = os.path.join(download_dir, f"{country}_{watershed or 'all_watersheds'}.gpkg")
     watershed_gdf.to_file(output_file_path, layer='data', driver='GPKG')
     
     print(f"Downloaded {watershed or 'all watersheds'} for {country} successfully.")
     
 def main():
-    """
-    Main function to run the Watershed Downloader program.
-    """
     geopackage_url = "https://github.com/kgdthomas/IslandSheds/raw/main/CARIBBEAN_WATERSHEDS.gpkg"
     print("Welcome to the Watershed Downloader!")
     
     show_available_datasets(geopackage_url)
     
     choice = input("Would you like to download data for a (1) specific country or (2) specific watershed? Enter 1 or 2: ")
     
     if choice == '1':
         country = input("Enter the country name: ")
-        output_dir = input("Enter download directory (default is .//Watershed//): ")
+        output_dir = input("Enter download directory (default is ./Watershed/): ")
+        output_dir = output_dir if output_dir else "./Watershed/"
         target_crs = input("Enter target CRS (optional): ")
+        
         download_country(country, output_dir, target_crs)
     
     elif choice == '2':
         country = input("Enter the country name for the watershed: ")
         download_watershed(geopackage_url, country)  # First call to display watersheds
         
         watershed = input("Enter the watershed name to download (or press enter for all watersheds): ")
-        download_dir = input("Enter download directory (default is .//Watershed//): ")
+        download_dir = input("Enter download directory (default is ./Watershed/): ")
+        download_dir = download_dir if download_dir else "./Watershed/"
         target_crs = input("Enter target CRS (optional): ")
         
         download_watershed(geopackage_url, country, download_dir, target_crs, watershed)  # Second call to download
         
     else:
         print("Invalid choice. Please restart the program and enter 1 or 2.")
```

### Comparing `islandsheds-0.0.28/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.29/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.28
+Version: 0.0.29
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.28/LICENSE.txt` & `islandsheds-0.0.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.28/PKG-INFO` & `islandsheds-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.28
+Version: 0.0.29
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.28/setup.py` & `islandsheds-0.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.28'
+VERSION = '0.0.29'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

