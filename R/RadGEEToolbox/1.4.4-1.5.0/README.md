# Comparing `tmp/RadGEEToolbox-1.4.4.tar.gz` & `tmp/RadGEEToolbox-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RadGEEToolbox-1.4.4.tar", last modified: Mon Nov 20 22:37:30 2023, max compression
+gzip compressed data, was "RadGEEToolbox-1.5.0.tar", last modified: Mon Apr 29 18:10:39 2024, max compression
```

## Comparing `RadGEEToolbox-1.4.4.tar` & `RadGEEToolbox-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 22:37:30.402000 RadGEEToolbox-1.4.4/
--rw-rw-rw-   0        0        0     1089 2023-11-20 21:53:42.000000 RadGEEToolbox-1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0     7089 2023-11-20 22:37:30.386000 RadGEEToolbox-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     6538 2023-11-20 22:34:34.000000 RadGEEToolbox-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-20 22:37:30.219000 RadGEEToolbox-1.4.4/RadGEEToolbox/
--rw-rw-rw-   0        0        0     3591 2023-11-20 18:31:16.000000 RadGEEToolbox-1.4.4/RadGEEToolbox/CollectionStitch.py
--rw-rw-rw-   0        0        0     1649 2023-11-07 17:49:01.000000 RadGEEToolbox-1.4.4/RadGEEToolbox/GetPalette.py
--rw-rw-rw-   0        0        0    73465 2023-11-20 18:31:30.000000 RadGEEToolbox-1.4.4/RadGEEToolbox/LandsatCollection.py
--rw-rw-rw-   0        0        0    54526 2023-11-20 18:31:48.000000 RadGEEToolbox-1.4.4/RadGEEToolbox/Sentinel2Collection.py
--rw-rw-rw-   0        0        0     5173 2023-11-18 03:34:57.000000 RadGEEToolbox-1.4.4/RadGEEToolbox/VisParams.py
--rw-rw-rw-   0        0        0      250 2023-11-18 03:15:31.000000 RadGEEToolbox-1.4.4/RadGEEToolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-20 22:37:30.370000 RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/
--rw-rw-rw-   0        0        0     7089 2023-11-20 22:37:29.000000 RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-11-20 22:37:29.000000 RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 22:37:29.000000 RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-11-20 22:37:29.000000 RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-11-20 22:37:29.000000 RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-20 22:37:30.399000 RadGEEToolbox-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      915 2023-11-20 22:35:48.000000 RadGEEToolbox-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:10:39.054312 RadGEEToolbox-1.5.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-29 16:59:14.000000 RadGEEToolbox-1.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     8175 2024-04-29 18:10:39.052811 RadGEEToolbox-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7547 2024-04-26 22:24:49.000000 RadGEEToolbox-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 18:10:39.033309 RadGEEToolbox-1.5.0/RadGEEToolbox/
+-rw-rw-rw-   0        0        0     3591 2023-11-20 18:31:21.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/CollectionStitch.py
+-rw-rw-rw-   0        0        0     1649 2023-11-07 17:49:01.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/GetPalette.py
+-rw-rw-rw-   0        0        0    85457 2024-04-29 17:03:52.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/LandsatCollection.py
+-rw-rw-rw-   0        0        0    55214 2024-04-29 16:33:33.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/Sentinel1Collection.py
+-rw-rw-rw-   0        0        0    66502 2024-04-29 17:04:48.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/Sentinel2Collection.py
+-rw-rw-rw-   0        0        0     5173 2023-11-18 03:35:03.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/VisParams.py
+-rw-rw-rw-   0        0        0      304 2024-04-29 17:20:35.000000 RadGEEToolbox-1.5.0/RadGEEToolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:10:39.051809 RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/
+-rw-rw-rw-   0        0        0     8175 2024-04-29 18:10:38.000000 RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-04-29 18:10:38.000000 RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 18:10:38.000000 RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-29 18:10:38.000000 RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 18:10:38.000000 RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 18:10:39.054312 RadGEEToolbox-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      952 2024-04-26 22:11:29.000000 RadGEEToolbox-1.5.0/setup.py
```

### Comparing `RadGEEToolbox-1.4.4/LICENSE.txt` & `RadGEEToolbox-1.5.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Mark Radwin
+Copyright (c) 2024 Mark Radwin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `RadGEEToolbox-1.4.4/PKG-INFO` & `RadGEEToolbox-1.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-Metadata-Version: 2.1
-Name: RadGEEToolbox
-Version: 1.4.4
-Summary: Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel
-Home-page: https://github.com/radwinskis/RadGEEToolbox
-Author: Mark Radwin
-Author-email: markradwin@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 [![PyPI version](https://badge.fury.io/py/RadGEEToolbox.svg)](https://pypi.org/project/RadGEEToolbox/)
 # RadGEEToolbox 🛠️
 
 ### 🌎 Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel 
 
 ### [See documentation here](https://radgeetoolbox.readthedocs.io/en/latest/)
 
 Initially created by Mark Radwin to help simplify processing imagery for PhD studies and general image exploration, this package offers helpful functionality with an outlook to add furthur functionality to aid assorted Earth observation specialists. 
 
-The package is divided into four modules:
+The package is divided into six modules:
 - LandsatCollection
    - Define and process Landsat 5 TM, 8 OLI, and 9 OLI surface reflectance imagery
+- Sentinel1Collection
+   - Define and process Sentinel 1 Synthetic Aperture Radar (SAR) backscatter imagery
 - Sentinel2Collection
    - Define and process Sentinel 2 MSI surface reflectance imagery
 - CollectionStitch
    - Accessory module to perform mosaicing functions on traditional GEE collections
 - GetPalette
    - Retrieve color palettes compatible with visualiztion GEE layers
 - VisParams
    - Alternative to visualization parameters dictionaries, define vis params using a function and retrieve palettes from GetPalette - makes visualizing images a bit easier
 
 
-LandsatCollection.py and Sentinel2Collection.py are the main two modules for the majority of image processing. 
+LandsatCollection.py, Sentinel1Collection.py, and Sentinel2Collection.py are the main modules for the majority of image processing. 
+
+CollectionStitch.py, GetPalette.py, and VisParams.py are supplemental for additional processing and image display
 
 Almost all functionality is server-side friendly AND most results are cached, providing very fast processing times.
 
 You can easily go back-and-forth from RadGEEToolbox and GEE objects to maximize efficiency in workflow.
 
 ### 🤔 Why use RadGEEToolbox?
 
@@ -61,14 +51,28 @@
 - Temporally reduce image collections using: minimum, maximum, median, or mean
 - Calculate geodesically corrected surface area from pixels corresponding to values greater than a defined threshold from any singleband image
 - Calculate geodesically corrected surface area from NDWI (water) pixels using dynamic thresholding via Otsu methods
 - Easily call in a variety of useful color palettes for image visualization
 - Easily define visualization parameter dictionaries
 - AND more with a continual list of growing features
 
+### New features included in version 1.5.0
+- Support for Sentinel 1 SAR data
+   - Includes all high-level functionality from the LandsatCollection and Sentinel2Collection modules
+   - Easy to defin the type of S1 data to use (instrument mode, polarization, pixel size, orbit direction, etc)
+   - Multilooking
+   - Speckle filtering (Lee-Sigma)
+   - Converting dB to sigma naught, or sigma naught to dB
+- Support for calculating the values along a transect or collection of transects
+   - Works for each image collection module
+   - Can iterate along an image collection and store transect values for each transect and for each image
+   - Stores transect data as a DataFrame
+   - Automatically saves transect data to csv files when iterating along a collection
+
+
 ### ⌨️ Basic Usage
 RadGEEToolbox is organized so that all functions are associated with each LandsatCollection and Sentinel2Collection class modules. You will need to define a base class collection, using arguments standard to defining ee.ImageCollections, and then you can call any of the class property attributes, methods, or static methods to complete processing. Utilizing class attribute propertues allows for very short code lines and very fast processing, while utilizing the methods allows for expanded customization of processing but requires more arguments and interaction from the user. The choice is up to you!
 
 - #### See the /Example Notebooks folder for examples showing how to define and filter collections, process the rasters for multispectral or other spectral products, and easily access color palettes and visualization parameter dictionaries for image visualization. 
 
 - #### See below for basic examples using the LandsatCollection class module. 
 
@@ -102,30 +106,30 @@
 
 ## 🚀 Installation Instructions
 
 ### 🔍 Prerequisites
 
 - **Python**: Ensure you have version 3.6 or higher installed.
 - **pip**: This is Python's package installer. 
-- **conda-forge**: Conda channel installer (Coming soon...)
+- **conda-forge**: Community led Conda package installer channel
 
 ### 📦 Installing via pip
 
-To install `RadGEEToolbox` version 1.4.4 using pip (NOTE: it is recommended to create a new virtual environment):
+To install `RadGEEToolbox` version 1.5.0 using pip (NOTE: it is recommended to create a new virtual environment):
 
 ```bash
-pip install RadGEEToolbox==1.4.4
+pip install RadGEEToolbox==1.5.0
 ```
 
-### 📦 Installing via Conda (Coming soon...)
+### 📦 Installing via Conda
 
-To install `RadGEEToolbox` version 1.4.4 using conda-forge (NOTE: it is recommended to create a new virtual environment):
+To install `RadGEEToolbox` version 1.5.0 using conda-forge (NOTE: it is recommended to create a new virtual environment):
 
 ```bash
-conda install -c conda-forge RadGEEToolbox
+conda install conda-forge::radgeetoolbox
 ```
 
 ### 🔧 Manual Installation from Source
 
 1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/radwinskis/RadGEEToolbox.git
@@ -145,8 +149,8 @@
 
 To verify that `RadGEEToolbox` was installed correctly:
 
 ```python
 python -c "import RadGEEToolbox; print(RadGEEToolbox.__version__)"
 ```
 
-You should see `1.4.4` printed as the version number.
+You should see `1.5.0` printed as the version number.
```

### Comparing `RadGEEToolbox-1.4.4/README.md` & `RadGEEToolbox-1.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,51 @@
+Metadata-Version: 2.1
+Name: RadGEEToolbox
+Version: 1.5.0
+Summary: Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel
+Home-page: https://github.com/radwinskis/RadGEEToolbox
+Author: Mark Radwin
+Author-email: markradwin@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: earthengine-api
+Requires-Dist: numpy
+Requires-Dist: pandas
+
 [![PyPI version](https://badge.fury.io/py/RadGEEToolbox.svg)](https://pypi.org/project/RadGEEToolbox/)
 # RadGEEToolbox 🛠️
 
 ### 🌎 Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel 
 
 ### [See documentation here](https://radgeetoolbox.readthedocs.io/en/latest/)
 
 Initially created by Mark Radwin to help simplify processing imagery for PhD studies and general image exploration, this package offers helpful functionality with an outlook to add furthur functionality to aid assorted Earth observation specialists. 
 
-The package is divided into four modules:
+The package is divided into six modules:
 - LandsatCollection
    - Define and process Landsat 5 TM, 8 OLI, and 9 OLI surface reflectance imagery
+- Sentinel1Collection
+   - Define and process Sentinel 1 Synthetic Aperture Radar (SAR) backscatter imagery
 - Sentinel2Collection
    - Define and process Sentinel 2 MSI surface reflectance imagery
 - CollectionStitch
    - Accessory module to perform mosaicing functions on traditional GEE collections
 - GetPalette
    - Retrieve color palettes compatible with visualiztion GEE layers
 - VisParams
    - Alternative to visualization parameters dictionaries, define vis params using a function and retrieve palettes from GetPalette - makes visualizing images a bit easier
 
 
-LandsatCollection.py and Sentinel2Collection.py are the main two modules for the majority of image processing. 
+LandsatCollection.py, Sentinel1Collection.py, and Sentinel2Collection.py are the main modules for the majority of image processing. 
+
+CollectionStitch.py, GetPalette.py, and VisParams.py are supplemental for additional processing and image display
 
 Almost all functionality is server-side friendly AND most results are cached, providing very fast processing times.
 
 You can easily go back-and-forth from RadGEEToolbox and GEE objects to maximize efficiency in workflow.
 
 ### 🤔 Why use RadGEEToolbox?
 
@@ -47,14 +68,28 @@
 - Temporally reduce image collections using: minimum, maximum, median, or mean
 - Calculate geodesically corrected surface area from pixels corresponding to values greater than a defined threshold from any singleband image
 - Calculate geodesically corrected surface area from NDWI (water) pixels using dynamic thresholding via Otsu methods
 - Easily call in a variety of useful color palettes for image visualization
 - Easily define visualization parameter dictionaries
 - AND more with a continual list of growing features
 
+### New features included in version 1.5.0
+- Support for Sentinel 1 SAR data
+   - Includes all high-level functionality from the LandsatCollection and Sentinel2Collection modules
+   - Easy to defin the type of S1 data to use (instrument mode, polarization, pixel size, orbit direction, etc)
+   - Multilooking
+   - Speckle filtering (Lee-Sigma)
+   - Converting dB to sigma naught, or sigma naught to dB
+- Support for calculating the values along a transect or collection of transects
+   - Works for each image collection module
+   - Can iterate along an image collection and store transect values for each transect and for each image
+   - Stores transect data as a DataFrame
+   - Automatically saves transect data to csv files when iterating along a collection
+
+
 ### ⌨️ Basic Usage
 RadGEEToolbox is organized so that all functions are associated with each LandsatCollection and Sentinel2Collection class modules. You will need to define a base class collection, using arguments standard to defining ee.ImageCollections, and then you can call any of the class property attributes, methods, or static methods to complete processing. Utilizing class attribute propertues allows for very short code lines and very fast processing, while utilizing the methods allows for expanded customization of processing but requires more arguments and interaction from the user. The choice is up to you!
 
 - #### See the /Example Notebooks folder for examples showing how to define and filter collections, process the rasters for multispectral or other spectral products, and easily access color palettes and visualization parameter dictionaries for image visualization. 
 
 - #### See below for basic examples using the LandsatCollection class module. 
 
@@ -88,30 +123,30 @@
 
 ## 🚀 Installation Instructions
 
 ### 🔍 Prerequisites
 
 - **Python**: Ensure you have version 3.6 or higher installed.
 - **pip**: This is Python's package installer. 
-- **conda-forge**: Conda channel installer (Coming soon...)
+- **conda-forge**: Community led Conda package installer channel
 
 ### 📦 Installing via pip
 
-To install `RadGEEToolbox` version 1.4.4 using pip (NOTE: it is recommended to create a new virtual environment):
+To install `RadGEEToolbox` version 1.5.0 using pip (NOTE: it is recommended to create a new virtual environment):
 
 ```bash
-pip install RadGEEToolbox==1.4.4
+pip install RadGEEToolbox==1.5.0
 ```
 
-### 📦 Installing via Conda (Coming soon...)
+### 📦 Installing via Conda
 
-To install `RadGEEToolbox` version 1.4.4 using conda-forge (NOTE: it is recommended to create a new virtual environment):
+To install `RadGEEToolbox` version 1.5.0 using conda-forge (NOTE: it is recommended to create a new virtual environment):
 
 ```bash
-conda install -c conda-forge RadGEEToolbox
+conda install conda-forge::radgeetoolbox
 ```
 
 ### 🔧 Manual Installation from Source
 
 1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/radwinskis/RadGEEToolbox.git
@@ -131,8 +166,8 @@
 
 To verify that `RadGEEToolbox` was installed correctly:
 
 ```python
 python -c "import RadGEEToolbox; print(RadGEEToolbox.__version__)"
 ```
 
-You should see `1.4.4` printed as the version number.
+You should see `1.5.0` printed as the version number.
```

### Comparing `RadGEEToolbox-1.4.4/RadGEEToolbox/CollectionStitch.py` & `RadGEEToolbox-1.5.0/RadGEEToolbox/CollectionStitch.py`

 * *Files identical despite different names*

### Comparing `RadGEEToolbox-1.4.4/RadGEEToolbox/GetPalette.py` & `RadGEEToolbox-1.5.0/RadGEEToolbox/GetPalette.py`

 * *Files identical despite different names*

### Comparing `RadGEEToolbox-1.4.4/RadGEEToolbox/LandsatCollection.py` & `RadGEEToolbox-1.5.0/RadGEEToolbox/LandsatCollection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import ee
+import pandas as pd
+import numpy as np
 class LandsatCollection:
     """
     Class object representing a combined collection of NASA/USGS Landsat 5, 8, and 9 TM & OLI surface reflectance satellite images at 30 m/px
 
     This class provides methods to filter, process, and analyze Landsat satellite imagery for a given period and region
 
     Arguments:
@@ -1492,7 +1494,216 @@
             new_col = ee.ImageCollection.fromImages(mosaic_list)
             col = LandsatCollection(collection=new_col)
             self._MosaicByDate = col
 
         # Convert the list of mosaics to an ImageCollection
         return self._MosaicByDate
     
+    @staticmethod
+    def ee_to_df(ee_object, columns=None, remove_geom=True, sort_columns=False, **kwargs):
+        """Converts an ee.FeatureCollection to pandas dataframe. Adapted from the geemap package (https://geemap.org/common/#geemap.common.ee_to_df)
+
+        Args:
+            ee_object (ee.FeatureCollection): ee.FeatureCollection.
+            columns (list): List of column names. Defaults to None.
+            remove_geom (bool): Whether to remove the geometry column. Defaults to True.
+            sort_columns (bool): Whether to sort the column names. Defaults to False.
+            kwargs: Additional arguments passed to ee.data.computeFeature.
+
+        Raises:
+            TypeError: ee_object must be an ee.FeatureCollection
+
+        Returns:
+            pd.DataFrame: pandas DataFrame
+        """
+        if isinstance(ee_object, ee.Feature):
+            ee_object = ee.FeatureCollection([ee_object])
+
+        if not isinstance(ee_object, ee.FeatureCollection):
+            raise TypeError("ee_object must be an ee.FeatureCollection")
+
+        try:
+            property_names = ee_object.first().propertyNames().sort().getInfo()
+            if remove_geom:
+                data = ee_object.map(
+                    lambda f: ee.Feature(None, f.toDictionary(property_names))
+                )
+            else:
+                data = ee_object
+
+            kwargs["expression"] = data
+            kwargs["fileFormat"] = "PANDAS_DATAFRAME"
+
+            df = ee.data.computeFeatures(kwargs)
+
+            if isinstance(columns, list):
+                df = df[columns]
+
+            if remove_geom and ("geo" in df.columns):
+                df = df.drop(columns=["geo"], axis=1)
+
+            if sort_columns:
+                df = df.reindex(sorted(df.columns), axis=1)
+
+            return df
+        except Exception as e:
+            raise Exception(e)
+
+    @staticmethod
+    def extract_transect(image, line, reducer="mean", n_segments=100, dist_interval=None, scale=None, crs=None, crsTransform=None, tileScale=1.0, to_pandas=False, **kwargs):
+
+        """Extracts transect from an image. Adapted from the geemap package (https://geemap.org/common/#geemap.common.extract_transect)
+
+        Args:
+            image (ee.Image): The image to extract transect from.
+            line (ee.Geometry.LineString): The LineString used to extract transect from an image.
+            reducer (str, optional): The ee.Reducer to use, e.g., 'mean', 'median', 'min', 'max', 'stdDev'. Defaults to "mean".
+            n_segments (int, optional): The number of segments that the LineString will be split into. Defaults to 100.
+            dist_interval (float, optional): The distance interval used for splitting the LineString. If specified, the n_segments parameter will be ignored. Defaults to None.
+            scale (float, optional): A nominal scale in meters of the projection to work in. Defaults to None.
+            crs (ee.Projection, optional): The projection to work in. If unspecified, the projection of the image's first band is used. If specified in addition to scale, rescaled to the specified scale. Defaults to None.
+            crsTransform (list, optional): The list of CRS transform values. This is a row-major ordering of the 3x2 transform matrix. This option is mutually exclusive with 'scale', and will replace any transform already set on the projection. Defaults to None.
+            tileScale (float, optional): A scaling factor used to reduce aggregation tile size; using a larger tileScale (e.g. 2 or 4) may enable computations that run out of memory with the default. Defaults to 1.
+            to_pandas (bool, optional): Whether to convert the result to a pandas dataframe. Default to False.
+
+        Raises:
+            TypeError: If the geometry type is not LineString.
+            Exception: If the program fails to compute.
+
+        Returns:
+            ee.FeatureCollection: The FeatureCollection containing the transect with distance and reducer values.
+        """
+        try:
+            geom_type = line.type().getInfo()
+            if geom_type != "LineString":
+                raise TypeError("The geometry type must be LineString.")
+
+            reducer = eval("ee.Reducer." + reducer + "()")
+            maxError = image.projection().nominalScale().divide(5)
+
+            length = line.length(maxError)
+            if dist_interval is None:
+                dist_interval = length.divide(n_segments)
+
+            distances = ee.List.sequence(0, length, dist_interval)
+            lines = line.cutLines(distances, maxError).geometries()
+
+            def set_dist_attr(l):
+                l = ee.List(l)
+                geom = ee.Geometry(l.get(0))
+                distance = ee.Number(l.get(1))
+                geom = ee.Geometry.LineString(geom.coordinates())
+                return ee.Feature(geom, {"distance": distance})
+
+            lines = lines.zip(distances).map(set_dist_attr)
+            lines = ee.FeatureCollection(lines)
+
+            transect = image.reduceRegions(
+                **{
+                    "collection": ee.FeatureCollection(lines),
+                    "reducer": reducer,
+                    "scale": scale,
+                    "crs": crs,
+                    "crsTransform": crsTransform,
+                    "tileScale": tileScale,
+                }
+            )
+
+            if to_pandas:
+                return LandsatCollection.ee_to_df(transect)
+            return transect
+
+        except Exception as e:
+            raise Exception(e)
+    
+    @staticmethod
+    def transect(image, lines, line_names, reducer='mean', n_segments=None, dist_interval=30, to_pandas=True):
+        """Computes and stores the values along a transect for each line in a list of lines. Builds off of the extract_transect function from the geemap package
+            where checks are ran to ensure that the reducer column is present in the transect data. If the reducer column is not present, a column of NaNs is created.
+            An ee reducer is used to aggregate the values along the transect, depending on the number of segments or distance interval specified. Defaults to 'mean' reducer.
+
+        Args:
+            image (ee.Image): ee.Image object to use for calculating transect values.
+            lines (list): List of ee.Geometry.LineString objects.
+            line_names (list of strings): List of line string names.
+            reducer (str): The ee reducer to use. Defaults to 'mean'.
+            n_segments (int): The number of segments that the LineString will be split into. Defaults to None.
+            dist_interval (float): The distance interval in meters used for splitting the LineString. If specified, the n_segments parameter will be ignored. Defaults to 30.
+            to_pandas (bool): Whether to convert the result to a pandas dataframe. Defaults to True.
+
+        Returns:
+            pd.DataFrame or ee.FeatureCollection: organized list of values along the transect(s)
+        """
+        #Create empty dataframe
+        transects_df = pd.DataFrame()
+
+        #Check if line is a list of lines or a single line - if single line, convert to list
+        if isinstance(lines, list):
+            pass
+        else:
+            lines = [lines]
+        
+        for i, line in enumerate(lines):
+            if n_segments is None:
+                transect_data = LandsatCollection.extract_transect(image=image, line=line, reducer=reducer, dist_interval=dist_interval, to_pandas=to_pandas)
+                if reducer in transect_data.columns:
+                    # Extract the 'mean' column and rename it
+                    mean_column = transect_data[['mean']]
+                else:
+                    # Handle the case where 'mean' column is not present
+                    print(f"{reducer} column not found in transect data for line {line_names[i]}")
+                    # Create a column of NaNs with the same length as the longest column in transects_df
+                    max_length = max(transects_df.shape[0], transect_data.shape[0])
+                    mean_column = pd.Series([np.nan] * max_length)
+            else:
+                transect_data = LandsatCollection.extract_transect(image=image, line=line, reducer=reducer, n_segments=n_segments, to_pandas=to_pandas)
+                if reducer in transect_data.columns:
+                    # Extract the 'mean' column and rename it
+                    mean_column = transect_data[['mean']]
+                else:
+                    # Handle the case where 'mean' column is not present
+                    print(f"{reducer} column not found in transect data for line {line_names[i]}")
+                    # Create a column of NaNs with the same length as the longest column in transects_df
+                    max_length = max(transects_df.shape[0], transect_data.shape[0])
+                    mean_column = pd.Series([np.nan] * max_length)
+            
+            transects_df = pd.concat([transects_df, mean_column], axis=1)
+
+        transects_df.columns = line_names
+                
+        return transects_df
+    
+    def transect_iterator(self, lines, line_names, save_folder_path, reducer='mean', n_segments=None, dist_interval=30, to_pandas=True):
+        """Computes and stores the values along a transect for each line in a list of lines for each image in a LandsatCollection image collection, then saves the data for each image to a csv file. Builds off of the extract_transect function from the geemap package
+            where checks are ran to ensure that the reducer column is present in the transect data. If the reducer column is not present, a column of NaNs is created.
+            An ee reducer is used to aggregate the values along the transect, depending on the number of segments or distance interval specified. Defaults to 'mean' reducer.
+            Naming conventions for the csv files follows as: "image-date_transects.csv"
+
+        Args:
+            self (LandsatCollection image collection): Image collection object to iterate for calculating transect values for each image.
+            lines (list): List of ee.Geometry.LineString objects.
+            line_names (list of strings): List of line string names.
+            save_folder_path (str): The path to the folder where the csv files will be saved.
+            reducer (str): The ee reducer to use. Defaults to 'mean'.
+            n_segments (int): The number of segments that the LineString will be split into. Defaults to None.
+            dist_interval (float): The distance interval used for splitting the LineString. If specified, the n_segments parameter will be ignored. Defaults to 10.
+            to_pandas (bool): Whether to convert the result to a pandas dataframe. Defaults to True.
+
+        Raises:
+            Exception: If the program fails to compute.
+
+        Returns:
+            csv file: file for each image with an organized list of values along the transect(s)
+        """
+        image_collection = self #.collection
+        # image_collection_dates = self._dates
+        image_collection_dates = self.dates
+        for i, date in enumerate(image_collection_dates):
+            try:
+                print(f"Processing image {i+1}/{len(image_collection_dates)}: {date}")
+                image = image_collection.image_grab(i)
+                transects_df = LandsatCollection.transect(image, lines, line_names, reducer=reducer, n_segments=n_segments, dist_interval=dist_interval, to_pandas=to_pandas)
+                image_id = date
+                transects_df.to_csv(f'{save_folder_path}{image_id}_transects.csv')
+                print(f'{image_id}_transects saved to csv')
+            except Exception as e:
+                print(f"An error occurred while processing image {i+1}: {e}")
```

### Comparing `RadGEEToolbox-1.4.4/RadGEEToolbox/Sentinel2Collection.py` & `RadGEEToolbox-1.5.0/RadGEEToolbox/Sentinel2Collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import ee
+import pandas as pd
+import numpy as np
 class Sentinel2Collection:
     """
     Class object representing a collection of ESA Sentinel-2 MSIsurface reflectance satellite images at 10 m/px resolution
 
     This class provides methods to filter, process, and analyze Sentinel-2 satellite imagery for a given period and region
 
     Arguments:
@@ -1243,7 +1245,215 @@
 
             new_col = ee.ImageCollection.fromImages(mosaic_list)
             col = Sentinel2Collection(collection=new_col)
             self._MosaicByDate = col
 
         return self._MosaicByDate
 
+    @staticmethod
+    def ee_to_df(ee_object, columns=None, remove_geom=True, sort_columns=False, **kwargs):
+        """Converts an ee.FeatureCollection to pandas dataframe. Adapted from the geemap package (https://geemap.org/common/#geemap.common.ee_to_df)
+
+        Args:
+            ee_object (ee.FeatureCollection): ee.FeatureCollection.
+            columns (list): List of column names. Defaults to None.
+            remove_geom (bool): Whether to remove the geometry column. Defaults to True.
+            sort_columns (bool): Whether to sort the column names. Defaults to False.
+            kwargs: Additional arguments passed to ee.data.computeFeature.
+
+        Raises:
+            TypeError: ee_object must be an ee.FeatureCollection
+
+        Returns:
+            pd.DataFrame: pandas DataFrame
+        """
+        if isinstance(ee_object, ee.Feature):
+            ee_object = ee.FeatureCollection([ee_object])
+
+        if not isinstance(ee_object, ee.FeatureCollection):
+            raise TypeError("ee_object must be an ee.FeatureCollection")
+
+        try:
+            property_names = ee_object.first().propertyNames().sort().getInfo()
+            if remove_geom:
+                data = ee_object.map(
+                    lambda f: ee.Feature(None, f.toDictionary(property_names))
+                )
+            else:
+                data = ee_object
+
+            kwargs["expression"] = data
+            kwargs["fileFormat"] = "PANDAS_DATAFRAME"
+
+            df = ee.data.computeFeatures(kwargs)
+
+            if isinstance(columns, list):
+                df = df[columns]
+
+            if remove_geom and ("geo" in df.columns):
+                df = df.drop(columns=["geo"], axis=1)
+
+            if sort_columns:
+                df = df.reindex(sorted(df.columns), axis=1)
+
+            return df
+        except Exception as e:
+            raise Exception(e)
+
+    @staticmethod
+    def extract_transect(image, line, reducer="mean", n_segments=100, dist_interval=None, scale=None, crs=None, crsTransform=None, tileScale=1.0, to_pandas=False, **kwargs):
+
+        """Extracts transect from an image. Adapted from the geemap package (https://geemap.org/common/#geemap.common.extract_transect)
+
+        Args:
+            image (ee.Image): The image to extract transect from.
+            line (ee.Geometry.LineString): The LineString used to extract transect from an image.
+            reducer (str, optional): The ee.Reducer to use, e.g., 'mean', 'median', 'min', 'max', 'stdDev'. Defaults to "mean".
+            n_segments (int, optional): The number of segments that the LineString will be split into. Defaults to 100.
+            dist_interval (float, optional): The distance interval in meters used for splitting the LineString. If specified, the n_segments parameter will be ignored. Defaults to None.
+            scale (float, optional): A nominal scale in meters of the projection to work in. Defaults to None.
+            crs (ee.Projection, optional): The projection to work in. If unspecified, the projection of the image's first band is used. If specified in addition to scale, rescaled to the specified scale. Defaults to None.
+            crsTransform (list, optional): The list of CRS transform values. This is a row-major ordering of the 3x2 transform matrix. This option is mutually exclusive with 'scale', and will replace any transform already set on the projection. Defaults to None.
+            tileScale (float, optional): A scaling factor used to reduce aggregation tile size; using a larger tileScale (e.g. 2 or 4) may enable computations that run out of memory with the default. Defaults to 1.
+            to_pandas (bool, optional): Whether to convert the result to a pandas dataframe. Default to False.
+
+        Raises:
+            TypeError: If the geometry type is not LineString.
+            Exception: If the program fails to compute.
+
+        Returns:
+            ee.FeatureCollection: The FeatureCollection containing the transect with distance and reducer values.
+        """
+        try:
+            geom_type = line.type().getInfo()
+            if geom_type != "LineString":
+                raise TypeError("The geometry type must be LineString.")
+
+            reducer = eval("ee.Reducer." + reducer + "()")
+            maxError = image.projection().nominalScale().divide(5)
+
+            length = line.length(maxError)
+            if dist_interval is None:
+                dist_interval = length.divide(n_segments)
+
+            distances = ee.List.sequence(0, length, dist_interval)
+            lines = line.cutLines(distances, maxError).geometries()
+
+            def set_dist_attr(l):
+                l = ee.List(l)
+                geom = ee.Geometry(l.get(0))
+                distance = ee.Number(l.get(1))
+                geom = ee.Geometry.LineString(geom.coordinates())
+                return ee.Feature(geom, {"distance": distance})
+
+            lines = lines.zip(distances).map(set_dist_attr)
+            lines = ee.FeatureCollection(lines)
+
+            transect = image.reduceRegions(
+                **{
+                    "collection": ee.FeatureCollection(lines),
+                    "reducer": reducer,
+                    "scale": scale,
+                    "crs": crs,
+                    "crsTransform": crsTransform,
+                    "tileScale": tileScale,
+                }
+            )
+
+            if to_pandas:
+                return Sentinel2Collection.ee_to_df(transect)
+            return transect
+
+        except Exception as e:
+            raise Exception(e)
+    
+    @staticmethod
+    def transect(image, lines, line_names, reducer='mean', n_segments=None, dist_interval=10, to_pandas=True):
+        """Computes and stores the values along a transect for each line in a list of lines. Builds off of the extract_transect function from the geemap package
+            where checks are ran to ensure that the reducer column is present in the transect data. If the reducer column is not present, a column of NaNs is created.
+            An ee reducer is used to aggregate the values along the transect, depending on the number of segments or distance interval specified. Defaults to 'mean' reducer.
+
+        Args:
+            image (ee.Image): ee.Image object to use for calculating transect values.
+            lines (list): List of ee.Geometry.LineString objects.
+            line_names (list of strings): List of line string names.
+            reducer (str): The ee reducer to use. Defaults to 'mean'.
+            n_segments (int): The number of segments that the LineString will be split into. Defaults to None.
+            dist_interval (float): The distance interval in meters used for splitting the LineString. If specified, the n_segments parameter will be ignored. Defaults to 10.
+            to_pandas (bool): Whether to convert the result to a pandas dataframe. Defaults to True.
+
+        Returns:
+            pd.DataFrame or ee.FeatureCollection: organized list of values along the transect(s)
+        """
+        #Create empty dataframe
+        transects_df = pd.DataFrame()
+
+        #Check if line is a list of lines or a single line - if single line, convert to list
+        if isinstance(lines, list):
+            pass
+        else:
+            lines = [lines]
+        
+        for i, line in enumerate(lines):
+            if n_segments is None:
+                transect_data = Sentinel2Collection.extract_transect(image=image, line=line, reducer=reducer, dist_interval=dist_interval, to_pandas=to_pandas)
+                if reducer in transect_data.columns:
+                    # Extract the 'mean' column and rename it
+                    mean_column = transect_data[['mean']]
+                else:
+                    # Handle the case where 'mean' column is not present
+                    print(f"{reducer} column not found in transect data for line {line_names[i]}")
+                    # Create a column of NaNs with the same length as the longest column in transects_df
+                    max_length = max(transects_df.shape[0], transect_data.shape[0])
+                    mean_column = pd.Series([np.nan] * max_length)
+            else:
+                transect_data = Sentinel2Collection.extract_transect(image=image, line=line, reducer=reducer, n_segments=n_segments, to_pandas=to_pandas)
+                if reducer in transect_data.columns:
+                    # Extract the 'mean' column and rename it
+                    mean_column = transect_data[['mean']]
+                else:
+                    # Handle the case where 'mean' column is not present
+                    print(f"{reducer} column not found in transect data for line {line_names[i]}")
+                    # Create a column of NaNs with the same length as the longest column in transects_df
+                    max_length = max(transects_df.shape[0], transect_data.shape[0])
+                    mean_column = pd.Series([np.nan] * max_length)
+            
+            transects_df = pd.concat([transects_df, mean_column], axis=1)
+
+        transects_df.columns = line_names
+                
+        return transects_df
+    
+    def transect_iterator(self, lines, line_names, save_folder_path, reducer='mean', n_segments=None, dist_interval=10, to_pandas=True):
+        """Computes and stores the values along a transect for each line in a list of lines for each image in a Sentinel2Collection image collection, then saves the data for each image to a csv file. Builds off of the extract_transect function from the geemap package
+            where checks are ran to ensure that the reducer column is present in the transect data. If the reducer column is not present, a column of NaNs is created.
+            An ee reducer is used to aggregate the values along the transect, depending on the number of segments or distance interval specified. Defaults to 'mean' reducer.
+            Naming conventions for the csv files follows as: "image-date_transects.csv"
+
+        Args:
+            self (Sentinel2Collection image collection): Image collection object to iterate for calculating transect values for each image.
+            lines (list): List of ee.Geometry.LineString objects.
+            line_names (list of strings): List of line string names.
+            save_folder_path (str): The path to the folder where the csv files will be saved.
+            reducer (str): The ee reducer to use. Defaults to 'mean'.
+            n_segments (int): The number of segments that the LineString will be split into. Defaults to None.
+            dist_interval (float): The distance interval in meters used for splitting the LineString. If specified, the n_segments parameter will be ignored. Defaults to 10.
+            to_pandas (bool): Whether to convert the result to a pandas dataframe. Defaults to True.
+
+        Raises:
+            Exception: If the program fails to compute.
+
+        Returns:
+            csv file: file for each image with an organized list of values along the transect(s)
+        """
+        image_collection = self #.collection
+        image_collection_dates = self.dates
+        for i, date in enumerate(image_collection_dates):
+            try:
+                print(f"Processing image {i+1}/{len(image_collection_dates)}: {date}")
+                image = image_collection.image_grab(i)
+                transects_df = Sentinel2Collection.transect(image, lines, line_names, reducer=reducer, n_segments=n_segments, dist_interval=dist_interval, to_pandas=to_pandas)
+                image_id = date
+                transects_df.to_csv(f'{save_folder_path}{image_id}_transects.csv')
+                print(f'{image_id}_transects saved to csv')
+            except Exception as e:
+                print(f"An error occurred while processing image {i+1}: {e}")
```

### Comparing `RadGEEToolbox-1.4.4/RadGEEToolbox/VisParams.py` & `RadGEEToolbox-1.5.0/RadGEEToolbox/VisParams.py`

 * *Files identical despite different names*

### Comparing `RadGEEToolbox-1.4.4/RadGEEToolbox.egg-info/PKG-INFO` & `RadGEEToolbox-1.5.0/RadGEEToolbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 Metadata-Version: 2.1
 Name: RadGEEToolbox
-Version: 1.4.4
+Version: 1.5.0
 Summary: Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel
 Home-page: https://github.com/radwinskis/RadGEEToolbox
 Author: Mark Radwin
 Author-email: markradwin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: earthengine-api
+Requires-Dist: numpy
+Requires-Dist: pandas
 
 [![PyPI version](https://badge.fury.io/py/RadGEEToolbox.svg)](https://pypi.org/project/RadGEEToolbox/)
 # RadGEEToolbox 🛠️
 
 ### 🌎 Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel 
 
 ### [See documentation here](https://radgeetoolbox.readthedocs.io/en/latest/)
 
 Initially created by Mark Radwin to help simplify processing imagery for PhD studies and general image exploration, this package offers helpful functionality with an outlook to add furthur functionality to aid assorted Earth observation specialists. 
 
-The package is divided into four modules:
+The package is divided into six modules:
 - LandsatCollection
    - Define and process Landsat 5 TM, 8 OLI, and 9 OLI surface reflectance imagery
+- Sentinel1Collection
+   - Define and process Sentinel 1 Synthetic Aperture Radar (SAR) backscatter imagery
 - Sentinel2Collection
    - Define and process Sentinel 2 MSI surface reflectance imagery
 - CollectionStitch
    - Accessory module to perform mosaicing functions on traditional GEE collections
 - GetPalette
    - Retrieve color palettes compatible with visualiztion GEE layers
 - VisParams
    - Alternative to visualization parameters dictionaries, define vis params using a function and retrieve palettes from GetPalette - makes visualizing images a bit easier
 
 
-LandsatCollection.py and Sentinel2Collection.py are the main two modules for the majority of image processing. 
+LandsatCollection.py, Sentinel1Collection.py, and Sentinel2Collection.py are the main modules for the majority of image processing. 
+
+CollectionStitch.py, GetPalette.py, and VisParams.py are supplemental for additional processing and image display
 
 Almost all functionality is server-side friendly AND most results are cached, providing very fast processing times.
 
 You can easily go back-and-forth from RadGEEToolbox and GEE objects to maximize efficiency in workflow.
 
 ### 🤔 Why use RadGEEToolbox?
 
@@ -61,14 +68,28 @@
 - Temporally reduce image collections using: minimum, maximum, median, or mean
 - Calculate geodesically corrected surface area from pixels corresponding to values greater than a defined threshold from any singleband image
 - Calculate geodesically corrected surface area from NDWI (water) pixels using dynamic thresholding via Otsu methods
 - Easily call in a variety of useful color palettes for image visualization
 - Easily define visualization parameter dictionaries
 - AND more with a continual list of growing features
 
+### New features included in version 1.5.0
+- Support for Sentinel 1 SAR data
+   - Includes all high-level functionality from the LandsatCollection and Sentinel2Collection modules
+   - Easy to defin the type of S1 data to use (instrument mode, polarization, pixel size, orbit direction, etc)
+   - Multilooking
+   - Speckle filtering (Lee-Sigma)
+   - Converting dB to sigma naught, or sigma naught to dB
+- Support for calculating the values along a transect or collection of transects
+   - Works for each image collection module
+   - Can iterate along an image collection and store transect values for each transect and for each image
+   - Stores transect data as a DataFrame
+   - Automatically saves transect data to csv files when iterating along a collection
+
+
 ### ⌨️ Basic Usage
 RadGEEToolbox is organized so that all functions are associated with each LandsatCollection and Sentinel2Collection class modules. You will need to define a base class collection, using arguments standard to defining ee.ImageCollections, and then you can call any of the class property attributes, methods, or static methods to complete processing. Utilizing class attribute propertues allows for very short code lines and very fast processing, while utilizing the methods allows for expanded customization of processing but requires more arguments and interaction from the user. The choice is up to you!
 
 - #### See the /Example Notebooks folder for examples showing how to define and filter collections, process the rasters for multispectral or other spectral products, and easily access color palettes and visualization parameter dictionaries for image visualization. 
 
 - #### See below for basic examples using the LandsatCollection class module. 
 
@@ -102,30 +123,30 @@
 
 ## 🚀 Installation Instructions
 
 ### 🔍 Prerequisites
 
 - **Python**: Ensure you have version 3.6 or higher installed.
 - **pip**: This is Python's package installer. 
-- **conda-forge**: Conda channel installer (Coming soon...)
+- **conda-forge**: Community led Conda package installer channel
 
 ### 📦 Installing via pip
 
-To install `RadGEEToolbox` version 1.4.4 using pip (NOTE: it is recommended to create a new virtual environment):
+To install `RadGEEToolbox` version 1.5.0 using pip (NOTE: it is recommended to create a new virtual environment):
 
 ```bash
-pip install RadGEEToolbox==1.4.4
+pip install RadGEEToolbox==1.5.0
 ```
 
-### 📦 Installing via Conda (Coming soon...)
+### 📦 Installing via Conda
 
-To install `RadGEEToolbox` version 1.4.4 using conda-forge (NOTE: it is recommended to create a new virtual environment):
+To install `RadGEEToolbox` version 1.5.0 using conda-forge (NOTE: it is recommended to create a new virtual environment):
 
 ```bash
-conda install -c conda-forge RadGEEToolbox
+conda install conda-forge::radgeetoolbox
 ```
 
 ### 🔧 Manual Installation from Source
 
 1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/radwinskis/RadGEEToolbox.git
@@ -145,8 +166,8 @@
 
 To verify that `RadGEEToolbox` was installed correctly:
 
 ```python
 python -c "import RadGEEToolbox; print(RadGEEToolbox.__version__)"
 ```
 
-You should see `1.4.4` printed as the version number.
+You should see `1.5.0` printed as the version number.
```

### Comparing `RadGEEToolbox-1.4.4/setup.py` & `RadGEEToolbox-1.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RadGEEToolbox",
-    version="1.4.4",
+    version="1.5.0",
     author="Mark Radwin",
     author_email="markradwin@gmail.com",
     description="Python package simplifying large-scale operations using Google Earth Engine (GEE) for users who utilize Landsat and Sentinel",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/radwinskis/RadGEEToolbox",
     packages=find_packages(),
@@ -15,11 +15,13 @@
         '': ['notebooks/*.ipynb'],},  
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "earthengine-api"
+        "earthengine-api",
+        "numpy",
+        "pandas"
     ],
     python_requires=">=3.6",
 )
```

