# Comparing `tmp/islandsheds-0.0.20.tar.gz` & `tmp/islandsheds-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islandsheds-0.0.20.tar", last modified: Mon Apr 29 05:46:42 2024, max compression
+gzip compressed data, was "islandsheds-0.0.21.tar", last modified: Mon Apr 29 06:47:43 2024, max compression
```

## Comparing `islandsheds-0.0.20.tar` & `islandsheds-0.0.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:46:42.957898 islandsheds-0.0.20/
-drwxrwxrwx   0        0        0        0 2024-04-29 05:46:42.923132 islandsheds-0.0.20/IslandSheds/
--rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.20/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     7361 2024-04-29 05:41:58.000000 islandsheds-0.0.20/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:46:42.954808 islandsheds-0.0.20/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 05:46:42.000000 islandsheds-0.0.20/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.20/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2024-04-29 05:46:42.956892 islandsheds-0.0.20/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.20/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 05:46:42.959082 islandsheds-0.0.20/setup.cfg
--rw-rw-rw-   0        0        0     1326 2024-04-29 05:43:10.000000 islandsheds-0.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:47:43.585521 islandsheds-0.0.21/
+drwxrwxrwx   0        0        0        0 2024-04-29 06:47:43.564238 islandsheds-0.0.21/IslandSheds/
+-rw-rw-rw-   0        0        0      905 2024-04-28 23:55:00.000000 islandsheds-0.0.21/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     7615 2024-04-29 06:42:09.000000 islandsheds-0.0.21/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:47:43.582514 islandsheds-0.0.21/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 06:47:43.000000 islandsheds-0.0.21/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2024-04-28 23:06:12.000000 islandsheds-0.0.21/LICENSE.txt
+-rw-rw-rw-   0        0        0      871 2024-04-29 06:47:43.584530 islandsheds-0.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-28 23:06:19.000000 islandsheds-0.0.21/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 06:47:43.586527 islandsheds-0.0.21/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-29 06:45:19.000000 islandsheds-0.0.21/setup.py
```

### Comparing `islandsheds-0.0.20/IslandSheds/__init__.py` & `islandsheds-0.0.21/IslandSheds/__init__.py`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.20/IslandSheds/downloader.py` & `islandsheds-0.0.21/IslandSheds/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,48 +87,60 @@
     # Load the GeoPackage directly
     gdf = gpd.read_file(geopackage_url, layer='caribbean_watersheds')
     unique_countries = gdf['Country'].unique()
     print("Available countries in the dataset:")
     for Country in unique_countries:
         print(Country)
 
-def download_watershed(base_url, country, watershed=None, download_dir="//Watershed//"):
+def download_watershed(geopackage_url, country, download_dir="//Watershed//"):
     """
     Downloads watershed data for a specified country and optionally a specific watershed.
 
     Parameters:
-    - base_url (str): The base URL where watershed data files are hosted.
+    - geopackage_url (str): The URL to the GeoPackage file.
     - country (str): The country for which watershed data is to be downloaded.
-    - watershed (str, optional): The specific watershed to download. If None, all watersheds for the country are downloaded.
     - download_dir (str): The directory where the watershed data will be saved. Defaults to "//Watershed//".
 
     Outputs:
     - Downloads and saves the specified watershed data as a GeoJSON file in the specified directory.
     - Console messages about the status of the download.
 
     Raises:
     - Prints an error message if the data cannot be downloaded (e.g., due to network issues or an incorrect URL).
     """
-    # Check if the directory exists and create it if it doesn't
+    # Ensure the output directory exists
     if not os.path.exists(download_dir):
         os.makedirs(download_dir)
-    # Construct the URL for the specific watershed or all watersheds
+
+    # Load the GeoPackage
+    gdf = gpd.read_file(geopackage_url, layer='caribbean_watersheds')
+    
+    # Filter data for the specified country
+    country_gdf = gdf[gdf['Country'] == country]
+    
+    # Display available watersheds in the country
+    print(f"Available watersheds in {country}:")
+    unique_watersheds = country_gdf['Watershed'].unique()
+    for watershed in unique_watersheds:
+        print(watershed)
+    
+    # Ask user which watershed to download
+    watershed = input("Enter the watershed name to download (or press enter for all watersheds): ")
+    
+    # Filter for the specific watershed if provided
     if watershed:
-        url = f"{base_url}/{country}/{watershed}.geojson"
-    else:
-        url = f"{base_url}/{country}/all_watersheds.geojson"
-    # Download the watershed data
-    response = requests.get(url)
-    if response.status_code == 200:
-        # Save the downloaded data to a file
-        with open(os.path.join(download_dir, f"{watershed or 'all_watersheds'}.geojson"), 'wb') as f:
-            f.write(response.content)
-        print(f"Downloaded {watershed or 'all watersheds'} for {country} successfully.")
+        watershed_gdf = country_gdf[country_gdf['Watershed'] == watershed]
     else:
-        print("Failed to download the data.")
+        watershed_gdf = country_gdf
+    
+    # Save the filtered data to a GeoJSON file
+    output_file_path = os.path.join(download_dir, f"{country}_{watershed or 'all_watersheds'}.geojson")
+    watershed_gdf.to_file(output_file_path, driver='GeoJSON')
+    
+    print(f"Downloaded {watershed or 'all watersheds'} for {country} successfully.")
 
 def main():
     """
     Main function to run the Watershed Downloader program.
 
     Interactively prompts the user to enter a country name, an optional watershed name, and a download directory. It then downloads the specified watershed data using the provided details.
     """
@@ -156,14 +168,14 @@
         # Get user input for country, watershed, and download directory
         country = input("Enter the country name for the watershed: ")
         watershed = input("Enter the watershed name (or press enter for all watersheds): ")
         download_dir = input("Enter download directory (default is .//Watershed//): ")
         download_dir = download_dir if download_dir else ".//Watershed//"
         
         # Download the watershed data
-        download_watershed(geopackage_url, country, watershed, download_dir)
+        download_watershed(geopackage_url, country, download_dir)
     
     else:
         print("Invalid choice. Please restart the program and enter 1 or 2.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `islandsheds-0.0.20/IslandSheds.egg-info/PKG-INFO` & `islandsheds-0.0.21/IslandSheds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.20
+Version: 0.0.21
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.20/LICENSE.txt` & `islandsheds-0.0.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `islandsheds-0.0.20/PKG-INFO` & `islandsheds-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IslandSheds
-Version: 0.0.20
+Version: 0.0.21
 Summary: A Caribbean watershed shapefile downloader package.
 Home-page: https://github.com/kgdthomas/IslandSheds
 Author: Kent Thomas
 Author-email: kthomas.wsrn@gmail.com
 License: MIT
 Project-URL: Documentation, https://islandsheds.readthedocs.io/
 Project-URL: Source, https://github.com/kgdthomas/IslandSheds
```

### Comparing `islandsheds-0.0.20/setup.py` & `islandsheds-0.0.21/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.20'
+VERSION = '0.0.21'
 DESCRIPTION = 'A Caribbean watershed shapefile downloader package.'
 LONG_DESCRIPTION = 'Python package for downloading country-specific Caribbean watershed data.'
 
 setup(
     name='IslandSheds',
     version=VERSION,
     packages=find_packages(),
```

