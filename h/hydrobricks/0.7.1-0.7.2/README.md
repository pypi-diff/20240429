# Comparing `tmp/hydrobricks-0.7.1.tar.gz` & `tmp/hydrobricks-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobricks-0.7.1.tar", last modified: Sat Apr 27 16:07:24 2024, max compression
+gzip compressed data, was "hydrobricks-0.7.2.tar", last modified: Mon Apr 29 07:54:20 2024, max compression
```

## Comparing `hydrobricks-0.7.1.tar` & `hydrobricks-0.7.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/hydrobricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.777595 hydrobricks-0.7.1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.781595 hydrobricks-0.7.1/python/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/python/src/hydrobricks/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py
--rw-r--r--   0 runner    (1001) docker     (127)    57573 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/catchment.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    29697 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/forcing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/hydro_units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/python/src/hydrobricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/model_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/socont.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)    31056 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/hydrobricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-29 07:54:20.000000 hydrobricks-0.7.2/hydrobricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-29 07:54:20.000000 hydrobricks-0.7.2/hydrobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:54:20.000000 hydrobricks-0.7.2/hydrobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:54:19.000000 hydrobricks-0.7.2/hydrobricks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 07:54:20.000000 hydrobricks-0.7.2/hydrobricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 07:54:20.000000 hydrobricks-0.7.2/hydrobricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.109537 hydrobricks-0.7.2/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.109537 hydrobricks-0.7.2/python/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/python/src/hydrobricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/python/src/hydrobricks/behaviours/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/behaviours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/behaviours/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57470 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/catchment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29697 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/hydro_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/python/src/hydrobricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/models/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/models/socont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31056 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/python/src/hydrobricks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:54:20.117537 hydrobricks-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-29 07:54:06.000000 hydrobricks-0.7.2/setup.py
```

### Comparing `hydrobricks-0.7.1/LICENSE` & `hydrobricks-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/PKG-INFO` & `hydrobricks-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobricks
-Version: 0.7.1
+Version: 0.7.2
 Summary: A modular hydrological modelling framework
 Author: Pascal Horton
 Author-email: pascal.horton@unibe.ch
 License: MIT
 Project-URL: Source Code, https://github.com/hydrobricks/hydrobricks
 Project-URL: Bug Tracker, https://github.com/hydrobricks/hydrobricks/issues
 Classifier: Programming Language :: C++
```

### Comparing `hydrobricks-0.7.1/README.md` & `hydrobricks-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/hydrobricks.egg-info/PKG-INFO` & `hydrobricks-0.7.2/hydrobricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobricks
-Version: 0.7.1
+Version: 0.7.2
 Summary: A modular hydrological modelling framework
 Author: Pascal Horton
 Author-email: pascal.horton@unibe.ch
 License: MIT
 Project-URL: Source Code, https://github.com/hydrobricks/hydrobricks
 Project-URL: Bug Tracker, https://github.com/hydrobricks/hydrobricks/issues
 Classifier: Programming Language :: C++
```

### Comparing `hydrobricks-0.7.1/hydrobricks.egg-info/SOURCES.txt` & `hydrobricks-0.7.2/hydrobricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/pyproject.toml` & `hydrobricks-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/__init__.py` & `hydrobricks-0.7.2/python/src/hydrobricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py` & `hydrobricks-0.7.2/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/catchment.py` & `hydrobricks-0.7.2/python/src/hydrobricks/catchment.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,16 +876,16 @@
             raise ValueError("Argument of arccos is above or below 1.")
 
         # Angle of incidence matrix
         incidence_angle[incidence_angle > 90 * TO_RAD] = 90 * TO_RAD
 
         return incidence_angle
 
-    def calculate_cast_shadows(self, dem_dataset, masked_dem,
-                               zenith, azimuth, lat):
+    @staticmethod
+    def calculate_cast_shadows(dem_dataset, masked_dem, zenith, azimuth):
         """
         Calculate the cast shadows.
 
         The approach relies on tilting the DEM to obtain a horizon matching the sun
         rays and filling the DEM. The algorithm is applied to the whole topography
         before masking the areas outside the catchment.
 
@@ -895,16 +895,14 @@
             DEM as read by rasterio, containing the DEM topography
         masked_dem : float
             DEM topography, masked with np.nan for the areas outside the study catchment
         zenith : float
             Solar zenith (IQBAL 2012), in degrees
         azimuth : float
             Azimuth relative to the south for ZSLOPE CALC, in degrees
-        lat : float
-            Mean latitude of the catchment, in degrees
 
         Returns
         -------
         A np.array with the cast shadows (1), the in sun areas (0),
         and the masked area (np.nan).
 
         Notes
@@ -1078,16 +1076,16 @@
                 potential_radiation = self._calculate_radiation_hock_equation(
                     mean_elevation, atmos_transmissivity, day_of_year[i],
                     zenith[j], incidence_angle)
 
                 # Account for cast shadows
                 if with_cast_shadows:
                     cast_shadows = self.calculate_cast_shadows(
-                        dem, masked_dem_data, zenith[j], azimuth[j], mean_lat)
-                    potential_radiation = potential_radiation * cast_shadows
+                        dem, masked_dem_data, zenith[j], azimuth[j])
+                    potential_radiation = potential_radiation * (1 - cast_shadows)
 
                 inter_pot_radiation[j, :, :] = potential_radiation.copy()
 
             with warnings.catch_warnings():
                 # This function throws a warning for the first slides of nanmean,
                 # it is normal and due to the NaN bands at the sides of the
                 # slope rasters, etc.
```

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/constants.py` & `hydrobricks-0.7.2/python/src/hydrobricks/constants.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/forcing.py` & `hydrobricks-0.7.2/python/src/hydrobricks/forcing.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/hydro_units.py` & `hydrobricks-0.7.2/python/src/hydrobricks/hydro_units.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/models/model.py` & `hydrobricks-0.7.2/python/src/hydrobricks/models/model.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/models/model_settings.py` & `hydrobricks-0.7.2/python/src/hydrobricks/models/model_settings.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/models/socont.py` & `hydrobricks-0.7.2/python/src/hydrobricks/models/socont.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/observations.py` & `hydrobricks-0.7.2/python/src/hydrobricks/observations.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/parameters.py` & `hydrobricks-0.7.2/python/src/hydrobricks/parameters.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/plotting.py` & `hydrobricks-0.7.2/python/src/hydrobricks/plotting.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/results.py` & `hydrobricks-0.7.2/python/src/hydrobricks/results.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/time_series.py` & `hydrobricks-0.7.2/python/src/hydrobricks/time_series.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/trainer.py` & `hydrobricks-0.7.2/python/src/hydrobricks/trainer.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/units.py` & `hydrobricks-0.7.2/python/src/hydrobricks/units.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/python/src/hydrobricks/utils.py` & `hydrobricks-0.7.2/python/src/hydrobricks/utils.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.1/setup.py` & `hydrobricks-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 # Read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "python" / "README.md").read_text()
 
 # Setup
 setup(
     name="hydrobricks",
-    version="0.7.1",
+    version="0.7.2",
     author="Pascal Horton",
     author_email="pascal.horton@unibe.ch",
     description="A modular hydrological modelling framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension("_hydrobricks")],
     cmdclass={"build_ext": CMakeBuild},
```

