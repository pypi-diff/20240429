# Comparing `tmp/islandsheds-0.0.24.tar.gz` & `tmp/islandsheds-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.24.tar", last modified: Mon Apr 29 07:16:20 2024, max compression
+gzip compressed data, was "islandsheds-0.0.25.tar", last modified: Mon Apr 29 07:30:23 2024, max compression
```

## Comparing `islandsheds-0.0.24.tar` & `islandsheds-0.0.25.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:16:20.797295 islandsheds-0.0.24/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:16:20.767240 islandsheds-0.0.24/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.24/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7623 2024-04-29 07:15:13.000000 islandsheds-0.0.24/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:16:20.793636 islandsheds-0.0.24/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 07:16:20.000000 islandsheds-0.0.24/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.24/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 07:16:20.795216 islandsheds-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.24/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 07:16:20.797295 islandsheds-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 07:15:30.000000 islandsheds-0.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:30:23.887003 islandsheds-0.0.25/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:30:23.860022 islandsheds-0.0.25/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.25/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     8133 2024-04-29 07:28:38.000000 islandsheds-0.0.25/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:30:23.882015 islandsheds-0.0.25/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 07:30:23.000000 islandsheds-0.0.25/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.25/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 07:30:23.883988 islandsheds-0.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.25/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:30:23.887003 islandsheds-0.0.25/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 07:29:13.000000 islandsheds-0.0.25/setup.py
```

### Comparing `islandsheds-0.0.24/IslandSheds/__init__.py` & `islandsheds-0.0.25/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.24/IslandSheds/downloader.py` & `islandsheds-0.0.25/IslandSheds/downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         output_file_path = os.path.join(output_dir, f"{country}_watersheds.gpkg")
         country_gdf.to_file(output_file_path, driver='GPKG')
         
         print(f"Data for {country} downloaded successfully.")
     else:
         print(f"Failed to download GeoPackage. Status code: {response.status_code}")
 
-def download_watershed(geopackage_url, country, download_dir="//Watershed//"):
+def download_watershed(geopackage_url, country, download_dir="//Watershed//", target_crs=None):
     """
     Downloads watershed data for a specified country and optionally a specific watershed.
 
     Parameters:
     - geopackage_url (str): The URL to the GeoPackage file.
     - country (str): The country for which watershed data is to be downloaded.
     - download_dir (str): The directory where the watershed data will be saved. Defaults to "//Watershed//".
@@ -113,28 +113,40 @@
 
     # Load the GeoPackage
     gdf = gpd.read_file(geopackage_url, layer='caribbean_watersheds')
     
     # Filter data for the specified country
     country_gdf = gdf[gdf['Country'] == country]
     
+    # Check and inform user about CRS
+    crs = gdf.crs
+    print(f"The CRS of the data is {crs}")
+    
     # Display available watersheds in the country
     print(f"Available watersheds in {country}:")
     unique_watersheds = country_gdf['Watershed'].unique()
     for watershed in unique_watersheds:
         print(watershed)
     
     # Ask user which watershed to download
     watershed = input("Enter the watershed name to download (or press enter for all watersheds): ")
     
     # Filter for the specific watershed if provided
     if watershed:
         watershed_gdf = country_gdf[country_gdf['Watershed'] == watershed]
     else:
         watershed_gdf = country_gdf
+        
+    # Ask user if they want to change the CRS
+    if target_crs:
+        # Change CRS if target_crs is specified
+        watershed_gdf = watershed_gdf.to_crs(target_crs)
+        print(f"Data CRS changed to {target_crs}")
+    else:
+        print("Data will be downloaded with the original CRS.")
     
     # Save the filtered data to a GPKG file
     output_file_path = os.path.join(download_dir, f"{country}_{watershed or 'all_watersheds'}.gpkg")
     watershed_gdf.to_file(output_file_path, layer='data', driver='GPKG')
     
     print(f"Downloaded {watershed or 'all watersheds'} for {country} successfully.")
     
@@ -166,16 +178,17 @@
     
     elif choice == '2':
         # Get user input for country, watershed, and download directory
         country = input("Enter the country name for the watershed: ")
         # watershed = input("Enter the watershed name (or press enter for all watersheds): ")
         download_dir = input("Enter download directory (default is .//Watershed//): ")
         download_dir = download_dir if download_dir else ".//Watershed//"
+        target_crs = input("Enter target CRS (optional): ")
         
         # Download the watershed data
-        download_watershed(geopackage_url, country, download_dir)
+        download_watershed(geopackage_url, country, download_dir, target_crs)
     
     else:
         print("Invalid choice. Please restart the program and enter 1 or 2.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `islandsheds-0.0.24/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.25/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.24
+Version: 0.0.25
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.24/LICENSE.txt` & `islandsheds-0.0.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.24/PKG-INFO` & `islandsheds-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.24
+Version: 0.0.25
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.24/setup.py` & `islandsheds-0.0.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.24'
+VERSION = '0.0.25'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

