# Comparing `tmp/islandsheds-0.0.19.tar.gz` & `tmp/islandsheds-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.19.tar", last modified: Mon Apr 29 05:27:27 2024, max compression
+gzip compressed data, was "islandsheds-0.0.20.tar", last modified: Mon Apr 29 05:46:42 2024, max compression
```

## Comparing `islandsheds-0.0.19.tar` & `islandsheds-0.0.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:27:27.117596 islandsheds-0.0.19/
-drwxrwxrwx   0        0        0        0 2024-04-29 05:27:27.088596 islandsheds-0.0.19/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.19/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7346 2024-04-29 05:26:35.000000 islandsheds-0.0.19/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:27:27.114637 islandsheds-0.0.19/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 05:27:26.000000 islandsheds-0.0.19/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.19/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 05:27:27.116558 islandsheds-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.19/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 05:27:27.117596 islandsheds-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 05:18:30.000000 islandsheds-0.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:46:42.957898 islandsheds-0.0.20/
+drwxrwxrwx   0        0        0        0 2024-04-29 05:46:42.923132 islandsheds-0.0.20/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.20/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7361 2024-04-29 05:41:58.000000 islandsheds-0.0.20/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:46:42.954808 islandsheds-0.0.20/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.20/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 05:46:42.956892 islandsheds-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.20/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 05:46:42.959082 islandsheds-0.0.20/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 05:43:10.000000 islandsheds-0.0.20/setup.py
```

### Comparing `islandsheds-0.0.19/IslandSheds/__init__.py` & `islandsheds-0.0.20/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.19/IslandSheds/downloader.py` & `islandsheds-0.0.20/IslandSheds/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,26 @@
     # URL of the GeoPackage hosted on GitHub
     geopackage_url = "https://github.com/kgdthomas/IslandSheds/raw/main/CARIBBEAN_WATERSHEDS.gpkg"
     
     # Download the GeoPackage
     response = requests.get(geopackage_url)
     
     if response.status_code == 200:
-         # Save the GeoPackage locally
+        # Ensure the output directory exists
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+        
+        # Save the GeoPackage locally
         local_path = os.path.join(output_dir, 'temp.gpkg')
         with open(local_path, 'wb') as f:
             f.write(response.content)
         
         # Load the GeoPackage from the local file
         gdf = gpd.read_file(local_path, layer='caribbean_watersheds')
+        
         # Filter data for the specified country
         country_gdf = gdf[gdf['Country'] == country]
         
         # Check and inform user about CRS
         crs = gdf.crs
         print(f"The CRS of the data is {crs}")
         
@@ -43,18 +48,14 @@
         if target_crs:
             # Change CRS if target_crs is specified
             country_gdf = country_gdf.to_crs(target_crs)
             print(f"Data CRS changed to {target_crs}")
         else:
             print("Data will be downloaded with the original CRS.")
         
-        # Create output directory if it doesn't exist
-        if output_dir:
-            create_directory(output_dir)
-        
         # Save the filtered data to a new GeoPackage file
         output_file_path = os.path.join(output_dir, f"{country}_watersheds.gpkg")
         country_gdf.to_file(output_file_path, driver='GPKG')
         
         print(f"Data for {country} downloaded successfully.")
     else:
         print(f"Failed to download GeoPackage. Status code: {response.status_code}")
```

### Comparing `islandsheds-0.0.19/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.20/IslandSheds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.19
+Version: 0.0.20
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.19/LICENSE.txt` & `islandsheds-0.0.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.19/PKG-INFO` & `islandsheds-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.19
+Version: 0.0.20
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.19/setup.py` & `islandsheds-0.0.20/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.19'
+VERSION = '0.0.20'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

