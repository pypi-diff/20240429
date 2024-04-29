# Comparing `tmp/islandsheds-0.0.18.tar.gz` & `tmp/islandsheds-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.18.tar", last modified: Mon Apr 29 02:00:21 2024, max compression
+gzip compressed data, was "islandsheds-0.0.19.tar", last modified: Mon Apr 29 05:27:27 2024, max compression
```

## Comparing `islandsheds-0.0.18.tar` & `islandsheds-0.0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 02:00:21.810905 islandsheds-0.0.18/
-drwxrwxrwx   0        0        0        0 2024-04-29 02:00:21.793956 islandsheds-0.0.18/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.18/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     6247 2024-04-29 01:55:44.000000 islandsheds-0.0.18/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 02:00:21.807859 islandsheds-0.0.18/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 02:00:21.000000 islandsheds-0.0.18/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.18/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 02:00:21.809900 islandsheds-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.18/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 02:00:21.810905 islandsheds-0.0.18/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 01:58:09.000000 islandsheds-0.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:27:27.117596 islandsheds-0.0.19/
+drwxrwxrwx   0        0        0        0 2024-04-29 05:27:27.088596 islandsheds-0.0.19/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.19/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7346 2024-04-29 05:26:35.000000 islandsheds-0.0.19/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:27:27.114637 islandsheds-0.0.19/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.19/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 05:27:27.116558 islandsheds-0.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.19/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 05:27:27.117596 islandsheds-0.0.19/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 05:18:30.000000 islandsheds-0.0.19/setup.py
```

### Comparing `islandsheds-0.0.18/IslandSheds/__init__.py` & `islandsheds-0.0.19/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.18/IslandSheds/downloader.py` & `islandsheds-0.0.19/IslandSheds/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,21 @@
     # URL of the GeoPackage hosted on GitHub
     geopackage_url = "https://github.com/kgdthomas/IslandSheds/raw/main/CARIBBEAN_WATERSHEDS.gpkg"
     
     # Download the GeoPackage
     response = requests.get(geopackage_url)
     
     if response.status_code == 200:
-        # Load the GeoPackage from the response content
-        gdf = gpd.read_file(response.content, layer='caribbean_watersheds')
+         # Save the GeoPackage locally
+        local_path = os.path.join(output_dir, 'temp.gpkg')
+        with open(local_path, 'wb') as f:
+            f.write(response.content)
         
+        # Load the GeoPackage from the local file
+        gdf = gpd.read_file(local_path, layer='caribbean_watersheds')
         # Filter data for the specified country
         country_gdf = gdf[gdf['Country'] == country]
         
         # Check and inform user about CRS
         crs = gdf.crs
         print(f"The CRS of the data is {crs}")
         
@@ -126,19 +130,39 @@
     Main function to run the Watershed Downloader program.
 
     Interactively prompts the user to enter a country name, an optional watershed name, and a download directory. It then downloads the specified watershed data using the provided details.
     """
     # URL to the GeoPackage
     geopackage_url = "https://github.com/kgdthomas/IslandSheds/raw/main/CARIBBEAN_WATERSHEDS.gpkg"
     print("Welcome to the Watershed Downloader!")
+    
     # Display available datasets
     show_available_datasets(geopackage_url)
-    # Get user input for country, watershed, and download directory
-    country = input("Enter the country name: ")
-    output_dir = input("Enter download directory (default is .//Watershed//): ")
-    output_dir = output_dir if output_dir else ".//Watershed//"
-    target_crs = input("Enter target CRS (optional): ")
-    # Download the country data
-    download_country(country, output_dir, target_crs)
+    
+    # Ask user if they want to download data for a country or a specific watershed
+    choice = input("Would you like to download data for a (1) specific country or (2) specific watershed? Enter 1 or 2: ")
+    
+    if choice == '1':
+        # Get user input for country and download directory
+        country = input("Enter the country name: ")
+        output_dir = input("Enter download directory (default is .//Watershed//): ")
+        output_dir = output_dir if output_dir else ".//Watershed//"
+        target_crs = input("Enter target CRS (optional): ")
+        
+        # Download the country data
+        download_country(country, output_dir, target_crs)
+    
+    elif choice == '2':
+        # Get user input for country, watershed, and download directory
+        country = input("Enter the country name for the watershed: ")
+        watershed = input("Enter the watershed name (or press enter for all watersheds): ")
+        download_dir = input("Enter download directory (default is .//Watershed//): ")
+        download_dir = download_dir if download_dir else ".//Watershed//"
+        
+        # Download the watershed data
+        download_watershed(geopackage_url, country, watershed, download_dir)
+    
+    else:
+        print("Invalid choice. Please restart the program and enter 1 or 2.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `islandsheds-0.0.18/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.19/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.18
+Version: 0.0.19
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.18/LICENSE.txt` & `islandsheds-0.0.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.18/PKG-INFO` & `islandsheds-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.18
+Version: 0.0.19
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.18/setup.py` & `islandsheds-0.0.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.18'
+VERSION = '0.0.19'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

