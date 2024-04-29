# Comparing `tmp/gempy_plugins-2023.2.0b1.tar.gz` & `tmp/gempy_plugins-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy_plugins-2023.2.0b1.tar", last modified: Wed Nov 22 15:23:40 2023, max compression
+gzip compressed data, was "gempy_plugins-2024.1.0.tar", last modified: Mon Apr 29 09:20:38 2024, max compression
```

## Comparing `gempy_plugins-2023.2.0b1.tar` & `gempy_plugins-2024.1.0.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_plugins-2023.2.0b1/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:24:22.000000 gempy_plugins-2023.2.0b1/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)      555 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/PKG-INFO
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/
--rw-r--r--   0 leguark   (1000) leguark   (1000)       45 2023-11-22 15:00:16.000000 gempy_plugins-2023.2.0b1/gempy_plugins/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:23:21.000000 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      219 2023-09-11 09:37:43.000000 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/gdal_reader.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6833 2023-09-11 09:37:43.000000 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/load_dem_gdal.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:48:35.000000 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/tests/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      267 2023-09-12 07:46:16.000000 gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/tests/test_gdal.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/kriging/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:44:38.000000 gempy_plugins-2023.2.0b1/gempy_plugins/kriging/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    41806 2023-06-18 08:55:36.000000 gempy_plugins-2023.2.0b1/gempy_plugins/kriging/coKriging.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    25504 2023-10-10 07:39:13.000000 gempy_plugins-2023.2.0b1/gempy_plugins/kriging/kriging.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:46:33.000000 gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7684 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/map2gempy.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:39:56.000000 gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/tests/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7091 2023-09-08 10:47:34.000000 gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/tests/test_map2loop.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1178 2023-08-17 07:46:59.000000 gempy_plugins-2023.2.0b1/gempy_plugins/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      100 2023-09-08 10:43:04.000000 gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1403 2023-09-27 10:46:38.000000 gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/_orientations_generator.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:40:22.000000 gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/tests/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2632 2023-09-11 09:47:39.000000 gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/tests/test_orientations_from_surface_points.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/spill_analysis/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:43:50.000000 gempy_plugins-2023.2.0b1/gempy_plugins/spill_analysis/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    19878 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/gempy_plugins/spill_analysis/spill_analysis.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/topology_analysis/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:45:46.000000 gempy_plugins-2023.2.0b1/gempy_plugins/topology_analysis/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    20392 2023-10-10 11:44:25.000000 gempy_plugins-2023.2.0b1/gempy_plugins/topology_analysis/topology.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins/utils/
--rw-r--r--   0 leguark   (1000) leguark   (1000)       71 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/gempy_plugins/utils/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6482 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/gempy_plugins/utils/analysis.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    15504 2023-07-26 14:40:40.000000 gempy_plugins-2023.2.0b1/gempy_plugins/utils/export.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2800 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/gempy_plugins/utils/gradient.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8343 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/gempy_plugins/utils/input_manipulation.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      555 2023-11-22 15:23:40.000000 gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1416 2023-11-22 15:23:40.000000 gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-11-22 15:23:40.000000 gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       20 2023-11-22 15:23:40.000000 gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/top_level.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)      891 2023-11-22 15:22:39.000000 gempy_plugins-2023.2.0b1/setup.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:54:12.000000 gempy_plugins-2023.2.0b1/tests/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/tests/test_addons/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/tests/test_addons/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:23:40.791514 gempy_plugins-2023.2.0b1/tests/test_integrations/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_plugins-2023.2.0b1/tests/test_integrations/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3237 2023-06-19 10:15:39.000000 gempy_plugins-2024.1.0/.gitignore
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_plugins-2024.1.0/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:24:22.000000 gempy_plugins-2024.1.0/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      557 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/PKG-INFO
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.275399 gempy_plugins-2024.1.0/gempy_plugins/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       45 2023-11-22 15:00:16.000000 gempy_plugins-2024.1.0/gempy_plugins/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-04-29 09:20:38.000000 gempy_plugins-2024.1.0/gempy_plugins/_version.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.275399 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:23:21.000000 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      219 2023-09-11 09:37:43.000000 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/gdal_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6833 2023-09-11 09:37:43.000000 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/load_dem_gdal.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:48:35.000000 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/tests/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/tests/data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10204 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/tests/data/_cropped_DEM_coarse.tif
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      267 2023-09-12 07:46:16.000000 gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/tests/test_gdal.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/kriging/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:44:38.000000 gempy_plugins-2024.1.0/gempy_plugins/kriging/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    41806 2023-06-18 08:55:36.000000 gempy_plugins-2024.1.0/gempy_plugins/kriging/coKriging.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    25644 2024-04-12 11:22:48.000000 gempy_plugins-2024.1.0/gempy_plugins/kriging/kriging.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/map2gempy/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:46:33.000000 gempy_plugins-2024.1.0/gempy_plugins/map2gempy/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7684 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/map2gempy/map2gempy.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/map2gempy/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:39:56.000000 gempy_plugins-2024.1.0/gempy_plugins/map2gempy/tests/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7091 2023-09-08 10:47:34.000000 gempy_plugins-2024.1.0/gempy_plugins/map2gempy/tests/test_map2loop.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1178 2023-08-17 07:46:59.000000 gempy_plugins-2024.1.0/gempy_plugins/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      100 2023-09-08 10:43:04.000000 gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1403 2023-09-27 10:46:38.000000 gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/_orientations_generator.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-11 09:40:22.000000 gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/tests/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2632 2023-09-11 09:47:39.000000 gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/tests/test_orientations_from_surface_points.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/spill_analysis/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:43:50.000000 gempy_plugins-2024.1.0/gempy_plugins/spill_analysis/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    19878 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/spill_analysis/spill_analysis.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/topology_analysis/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:45:46.000000 gempy_plugins-2024.1.0/gempy_plugins/topology_analysis/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    20409 2024-04-12 12:48:05.000000 gempy_plugins-2024.1.0/gempy_plugins/topology_analysis/topology.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins/utils/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       71 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/utils/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6482 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/utils/analysis.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    15504 2023-07-26 14:40:40.000000 gempy_plugins-2024.1.0/gempy_plugins/utils/export.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2800 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/utils/gradient.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8343 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/gempy_plugins/utils/input_manipulation.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/gempy_plugins.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      557 2024-04-29 09:20:38.000000 gempy_plugins-2024.1.0/gempy_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1590 2024-04-29 09:20:38.000000 gempy_plugins-2024.1.0/gempy_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 09:20:38.000000 gempy_plugins-2024.1.0/gempy_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       20 2024-04-29 09:20:38.000000 gempy_plugins-2024.1.0/gempy_plugins.egg-info/top_level.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      967 2024-04-15 11:42:53.000000 gempy_plugins-2024.1.0/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:54:12.000000 gempy_plugins-2024.1.0/tests/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/tests/data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      163 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/tests/data/model5_orientations.csv
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      480 2023-08-17 14:09:26.000000 gempy_plugins-2024.1.0/tests/data/model5_surface_points.csv
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/tests/test_addons/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/tests/test_addons/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:20:38.285399 gempy_plugins-2024.1.0/tests/test_integrations/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_plugins-2024.1.0/tests/test_integrations/__init__.py
```

### Comparing `gempy_plugins-2023.2.0b1/AUTHORS.rst` & `gempy_plugins-2024.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/LICENSE` & `gempy_plugins-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/PKG-INFO` & `gempy_plugins-2024.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gempy_plugins
-Version: 2023.2.0b1
+Version: 2024.1.0
 Summary: Extra plugins for the geological modeling package GemPy
 Home-page: 
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
-License: EUPL
+License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/gdal_topography/load_dem_gdal.py` & `gempy_plugins-2024.1.0/gempy_plugins/gdal_topography/load_dem_gdal.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/kriging/coKriging.py` & `gempy_plugins-2024.1.0/gempy_plugins/kriging/coKriging.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/kriging/kriging.py` & `gempy_plugins-2024.1.0/gempy_plugins/kriging/kriging.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @author: Jan von Harten
 """
 
 import warnings
 from typing import Optional, Sequence
 
 import gempy as gp
+from gempy_engine.core.data.engine_grid import EngineGrid
 
 from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
 
 from gempy_viewer.modules.plot_2d.visualization_2d import Plot2D
 from gempy_viewer.modules.plot_2d.drawer_regular_grid_2d import plot_regular_grid_area
 
 try:
@@ -35,17 +36,20 @@
         # TODO: Check if I actually need all this or if its easier to just get grid and lith of the solution
         self.sol: RawArraysSolution = model_solutions.raw_arrays
 
         # set kriging surfaces, basically in which lithologies to do all this, default is everything
         # TODO: Maybe also allow to pass a gempy regular grid object
         if domain is None:
             domain = np.unique(self.sol.lith_block)
+
+        # ! This works for now only on the dense grid.
+        centers: EngineGrid = model_solutions.octrees_output[0].grid_centers
         self.set_domain(
             domain=domain,
-            grid_values=transform.apply_inverse(model_solutions.octrees_output[-1].grid_centers.regular_grid.original_values)
+            grid_values=transform.apply_inverse(centers.dense_grid.values)
         )
 
         # set data, default is None
         # TODO: need to figure out a way to then set mean and variance for the SGS and SK
         if data is None:
             data = None  # why do you do this, data is none already if it is none?
         self.set_data(data)
```

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/map2gempy.py` & `gempy_plugins-2024.1.0/gempy_plugins/map2gempy/map2gempy.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/map2gempy/tests/test_map2loop.py` & `gempy_plugins-2024.1.0/gempy_plugins/map2gempy/tests/test_map2loop.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/optional_dependencies.py` & `gempy_plugins-2024.1.0/gempy_plugins/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/_orientations_generator.py` & `gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/_orientations_generator.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/orientations_generator/tests/test_orientations_from_surface_points.py` & `gempy_plugins-2024.1.0/gempy_plugins/orientations_generator/tests/test_orientations_from_surface_points.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/spill_analysis/spill_analysis.py` & `gempy_plugins-2024.1.0/gempy_plugins/spill_analysis/spill_analysis.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/topology_analysis/topology.py` & `gempy_plugins-2024.1.0/gempy_plugins/topology_analysis/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,40 +13,44 @@
 
     You should have received a copy of the GNU General Public License
     along with gempy.  If not, see <http://www.gnu.org/licenses/>.
 
 
 @author: Alexander Schaaf and Miguel de la Varga
 """
-import gempy as gp
+import matplotlib.pyplot as plt
 import numpy as np
 from typing import List, Set, Tuple, Dict, Union, Optional
-import matplotlib.pyplot as plt
+
+import gempy as gp
+from gempy_engine.core.data import Solutions
 
 
 def _get_nunconf(geo_model) -> int:
     return np.count_nonzero(geo_model._stack.df.BottomRelation == "Erosion") - 2  # TODO -2 n other lith series
 
 
 def _get_nfaults(geo_model) -> int:
     return np.count_nonzero(geo_model._faults.df.isFault)
 
 
 def _get_fault_blocks(geo_model: gp.data.GeoModel) -> np.ndarray:
-    fault_blocks = geo_model.solutions.raw_arrays.block_matrix[geo_model.structural_frame.group_is_fault]
-    resolution = geo_model.solutions.octrees_output[-1].grid_centers.regular_grid.resolution
-
+    solutions: Solutions = geo_model.solutions
+    fault_blocks = solutions.raw_arrays.block_matrix[geo_model.structural_frame.group_is_fault]
+    resolution = solutions.block_solution_resolution
+   
     int__sum_axis__reshape = np.round(fault_blocks).astype(int).sum(axis=0).reshape(*resolution)
     return int__sum_axis__reshape
 
 
 def _get_lith_blocks(geo_model: gp.data.GeoModel) -> np.ndarray:
-    lith_blocks = geo_model.solutions.raw_arrays.block_matrix[[not x for x in geo_model.structural_frame.group_is_fault]]
-    resolution = geo_model.solutions.octrees_output[-1].grid_centers.regular_grid.resolution
-
+    solutions: Solutions = geo_model.solutions
+    lith_blocks = solutions.raw_arrays.block_matrix[[not x for x in geo_model.structural_frame.group_is_fault]]
+    resolution = solutions.block_solution_resolution
+    
     int__sum_axis__reshape = np.round(lith_blocks).astype(int).sum(axis=0).reshape(*resolution)
     return int__sum_axis__reshape
 
 
 def compute_topology(
         geo_model,
         cell_number: int = None,
@@ -201,15 +205,15 @@
     Args:
         geo_model: GemPy geomodel instance with solutions.
         centroids (Dict[int, Array[float, 3]]): Topology node centroids.
     
     Returns:
         Dict[int, int]: Look-up table translating node id -> lith id.
     """
-    resolution = geo_model.solutions.octrees_output[-1].grid_centers.regular_grid.resolution
+    resolution = geo_model.solutions.block_solution_resolution
     lb = geo_model.solutions.raw_arrays.lith_block.reshape(resolution).astype(int)
 
     lot = {}
     for node, pos in centroids.items():
         p = np.round(pos).astype(int)
         lith_id = lb[p[0], p[1], p[2]]
         lot[node] = lith_id
```

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/utils/analysis.py` & `gempy_plugins-2024.1.0/gempy_plugins/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/utils/export.py` & `gempy_plugins-2024.1.0/gempy_plugins/utils/export.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/utils/gradient.py` & `gempy_plugins-2024.1.0/gempy_plugins/utils/gradient.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins/utils/input_manipulation.py` & `gempy_plugins-2024.1.0/gempy_plugins/utils/input_manipulation.py`

 * *Files identical despite different names*

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/PKG-INFO` & `gempy_plugins-2024.1.0/gempy_plugins.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: gempy-plugins
-Version: 2023.2.0b1
+Name: gempy_plugins
+Version: 2024.1.0
 Summary: Extra plugins for the geological modeling package GemPy
 Home-page: 
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
-License: EUPL
+License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gempy_plugins-2023.2.0b1/gempy_plugins.egg-info/SOURCES.txt` & `gempy_plugins-2024.1.0/gempy_plugins.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+.gitignore
 AUTHORS.rst
 LICENSE
 setup.py
 gempy_plugins/__init__.py
+gempy_plugins/_version.py
 gempy_plugins/optional_dependencies.py
 gempy_plugins.egg-info/PKG-INFO
 gempy_plugins.egg-info/SOURCES.txt
 gempy_plugins.egg-info/dependency_links.txt
 gempy_plugins.egg-info/top_level.txt
 gempy_plugins/gdal_topography/__init__.py
 gempy_plugins/gdal_topography/gdal_reader.py
 gempy_plugins/gdal_topography/load_dem_gdal.py
 gempy_plugins/gdal_topography/tests/__init__.py
 gempy_plugins/gdal_topography/tests/test_gdal.py
+gempy_plugins/gdal_topography/tests/data/_cropped_DEM_coarse.tif
 gempy_plugins/kriging/__init__.py
 gempy_plugins/kriging/coKriging.py
 gempy_plugins/kriging/kriging.py
 gempy_plugins/map2gempy/__init__.py
 gempy_plugins/map2gempy/map2gempy.py
 gempy_plugins/map2gempy/tests/__init__.py
 gempy_plugins/map2gempy/tests/test_map2loop.py
@@ -29,9 +32,11 @@
 gempy_plugins/topology_analysis/topology.py
 gempy_plugins/utils/__init__.py
 gempy_plugins/utils/analysis.py
 gempy_plugins/utils/export.py
 gempy_plugins/utils/gradient.py
 gempy_plugins/utils/input_manipulation.py
 tests/__init__.py
+tests/data/model5_orientations.csv
+tests/data/model5_surface_points.csv
 tests/test_addons/__init__.py
 tests/test_integrations/__init__.py
```

### Comparing `gempy_plugins-2023.2.0b1/setup.py` & `gempy_plugins-2024.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 ﻿# setup.py for gempy_viewer. Requierements are numpy and matplotlib
+from os import path
 
 from setuptools import setup, find_packages
 
-import gempy
-
-version = gempy.__version__
-
-
-def read_requirements(file_name):
-    with open(file_name, "r", encoding="utf-8") as f:
-        return [line.strip() for line in f.readlines()]
-
-
 setup(
     name='gempy_plugins',
-    version=version,
     packages=find_packages(),
     url='',
-    license='EUPL',
+    license='EUPL-1.2',
     author='Miguel de la Varga', 
     author_email="miguel@terranigma-solutions.com",
     description='Extra plugins for the geological modeling package GemPy',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Visualization',
         'Topic :: Scientific/Engineering :: GIS',
         'Programming Language :: Python :: 3.10'
     ],
-    python_requires='>=3.10'
+    python_requires='>=3.10',
+    setup_requires=['setuptools_scm'],
+    use_scm_version={
+            "root"            : ".",
+            "relative_to"     : __file__,
+            "write_to"        : path.join("gempy_plugins", "_version.py"),
+            "fallback_version": "3.0.0"
+    },
 )
```

