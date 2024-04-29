# Comparing `tmp/subsurface-0.2.9.tar.gz` & `tmp/subsurface-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsurface-0.2.9.tar", last modified: Fri Nov 12 14:01:05 2021, max compression
+gzip compressed data, was "subsurface-2024.1.0.tar", last modified: Mon Apr 29 08:44:40 2024, max compression
```

## Comparing `subsurface-0.2.9.tar` & `subsurface-2024.1.0.tar`

### file list

```diff
@@ -1,100 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11403 2021-11-12 14:00:47.000000 subsurface-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2021-11-12 14:01:05.256258 subsurface-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2021-11-12 14:00:47.000000 subsurface-0.2.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-12 14:01:05.256258 subsurface-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2021-11-12 14:00:47.000000 subsurface-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.248257 subsurface-0.2.9/subsurface/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-11-12 14:01:04.000000 subsurface-0.2.9/subsurface/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/geological_formats/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/geological_formats/OMF/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/geological_formats/OMF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/geological_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/geological_formats/boreholes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/geological_formats/fault.py
--rw-r--r--   0 runner    (1001) docker     (121)     2394 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/geological_formats/segy_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4543 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/geological_formats/seismic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)      457 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/interfaces/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/interfaces/liquid_earth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/interfaces/liquid_earth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/interfaces/liquid_earth/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/faults/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/faults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/faults/faults.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/geo_object/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/geo_object/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/mesh/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/mesh/surface_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/mesh/surfaces_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/petrel/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/petrel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4183 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/profiles/profiles_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/read_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/readers_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/topography/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/topography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/topography/topo_core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/volume/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/volume/read_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/volume/volume_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.252257 subsurface-0.2.9/subsurface/reader/wells/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6101 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/pandas_to_welly.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/well_files_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/wells_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/wells_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4487 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/reader/wells/welly_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/structs/
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/structs/base_structures/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/base_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/base_structures/common_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/base_structures/structured_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12096 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/base_structures/unstructured_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/structured_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/structs/unstructured_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/utils/utils_core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/visualization/to_pyvista.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/writer/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/writer/to_liquid_earth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_liquid_earth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/writer/to_rex/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/data_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.256258 subsurface-0.2.9/subsurface/writer/to_rex/doc/
--rw-r--r--   0 runner    (1001) docker     (121)    25075 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/doc/rex-spec-v1.md
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/doc/right-handed.png
--rw-r--r--   0 runner    (1001) docker     (121)   137215 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/doc/sketchup_example.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    29539 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/gempy_to_rexfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/material_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/mesh_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    11168 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/rex_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/to_rex.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2021-11-12 14:00:47.000000 subsurface-0.2.9/subsurface/writer/to_rex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 14:01:05.248257 subsurface-0.2.9/subsurface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2021-11-12 14:01:04.000000 subsurface-0.2.9/subsurface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2765 2021-11-12 14:01:05.000000 subsurface-0.2.9/subsurface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-12 14:01:04.000000 subsurface-0.2.9/subsurface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-12 14:00:55.000000 subsurface-0.2.9/subsurface.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-12 14:01:04.000000 subsurface-0.2.9/subsurface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-11-12 14:01:04.000000 subsurface-0.2.9/subsurface.egg-info/top_level.txt
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      276 2024-04-29 08:12:18.000000 subsurface-2024.1.0/.env.example
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11403 2023-06-18 07:50:00.000000 subsurface-2024.1.0/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5798 2024-04-29 08:44:40.645504 subsurface-2024.1.0/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3377 2023-06-18 07:50:00.000000 subsurface-2024.1.0/README.rst
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/requirements/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       32 2024-04-29 08:12:59.000000 subsurface-2024.1.0/requirements/requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      192 2024-04-29 08:42:27.000000 subsurface-2024.1.0/requirements/requirements_all.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      195 2024-04-29 08:11:02.000000 subsurface-2024.1.0/requirements/requirements_dev.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       32 2024-04-29 08:12:59.000000 subsurface-2024.1.0/requirements/requirements_geospatial.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       97 2024-04-29 08:38:52.000000 subsurface-2024.1.0/requirements/requirements_mesh.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      142 2024-04-29 08:42:27.000000 subsurface-2024.1.0/requirements/requirements_opt.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       42 2024-04-29 08:12:59.000000 subsurface-2024.1.0/requirements/requirements_plot.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       11 2024-04-29 08:12:59.000000 subsurface-2024.1.0/requirements/requirements_traces.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       24 2024-04-29 08:12:59.000000 subsurface-2024.1.0/requirements/requirements_volume.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      109 2024-04-29 08:12:18.000000 subsurface-2024.1.0/requirements/requirements_wells.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-04-29 08:44:40.645504 subsurface-2024.1.0/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2857 2024-04-29 08:43:11.000000 subsurface-2024.1.0/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      867 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-04-29 08:44:40.000000 subsurface-2024.1.0/subsurface/_version.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/geological_formats/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/geological_formats/OMF/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/geological_formats/OMF/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/geological_formats/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      164 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/geological_formats/boreholes.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1547 2024-04-29 08:11:02.000000 subsurface-2024.1.0/subsurface/geological_formats/fault.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2109 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/geological_formats/segy_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4950 2024-04-29 08:13:09.000000 subsurface-2024.1.0/subsurface/geological_formats/seismic.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/interfaces/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      457 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/interfaces/README.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        3 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/interfaces/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2276 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/optional_requirements.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      177 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/README.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      368 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/faults/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/faults/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2242 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/faults/faults.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1341 2024-04-29 08:10:31.000000 subsurface-2024.1.0/subsurface/reader/from_binary.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/geo_object/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/geo_object/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/mesh/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      258 2024-04-29 08:10:31.000000 subsurface-2024.1.0/subsurface/reader/mesh/NOTES.md
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/mesh/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1969 2024-04-29 08:10:31.000000 subsurface-2024.1.0/subsurface/reader/mesh/csv_mesh_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2226 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/reader/mesh/dxf_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       56 2024-04-29 08:10:31.000000 subsurface-2024.1.0/subsurface/reader/mesh/obj_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1086 2024-04-29 08:11:02.000000 subsurface-2024.1.0/subsurface/reader/mesh/omf_mesh_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2273 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/reader/mesh/surface_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2608 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/mesh/surfaces_api.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/petrel/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/petrel/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/profiles/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        3 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/profiles/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4979 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/reader/profiles/profiles_core.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      981 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/read_netcdf.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3740 2024-04-29 08:10:31.000000 subsurface-2024.1.0/subsurface/reader/readers_data.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/topography/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        7 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/topography/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3190 2024-04-29 08:11:02.000000 subsurface-2024.1.0/subsurface/reader/topography/topo_core.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/volume/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/volume/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1665 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/reader/volume/read_volume.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1286 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/reader/volume/volume_utils.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/wells/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/wells/DEP/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7273 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/_well_files_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2334 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/_wells_api.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6468 2024-04-29 08:15:29.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/_welly_reader.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6925 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/pandas_to_welly.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/reader/wells/DEP/test_wells/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/test_wells/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1329 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/test_wells/test_io_wells.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    19323 2024-04-29 08:15:40.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/test_wells/test_welly_to_subsurface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2206 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/DEP/wells_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      407 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/README.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2183 2024-04-29 08:12:18.000000 subsurface-2024.1.0/subsurface/reader/wells/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/structs/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1681 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/structs/README.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      202 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/structs/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/structs/base_structures/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       92 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/structs/base_structures/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1875 2024-04-29 08:10:31.000000 subsurface-2024.1.0/subsurface/structs/base_structures/common_data_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3415 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/structs/base_structures/structured_data.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12842 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/structs/base_structures/unstructured_data.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      186 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/structs/errors.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2112 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/structs/structured_elements.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7003 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/structs/unstructured_elements.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/utils/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        3 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/utils/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      150 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/utils/utils_core.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/visualization/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       65 2024-04-29 08:11:02.000000 subsurface-2024.1.0/subsurface/visualization/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9069 2024-04-29 08:12:59.000000 subsurface-2024.1.0/subsurface/visualization/to_pyvista.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/writer/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       50 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      415 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_binary.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/writer/to_liquid_earth/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_liquid_earth/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/writer/to_rex/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2227 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/common.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1546 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/data_struct.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface/writer/to_rex/doc/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    25075 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/doc/rex-spec-v1.md
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3044 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/doc/right-handed.png
+-rw-r--r--   0 leguark   (1000) leguark   (1000)   137215 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/doc/sketchup_example.jpg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    29539 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/gempy_to_rexfile.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1637 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/material_encoder.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6291 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/mesh_encoder.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3685 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/to_rex.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      364 2023-06-18 07:50:00.000000 subsurface-2024.1.0/subsurface/writer/to_rex/utils.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 08:44:40.645504 subsurface-2024.1.0/subsurface.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5798 2024-04-29 08:44:40.000000 subsurface-2024.1.0/subsurface.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3494 2024-04-29 08:44:40.000000 subsurface-2024.1.0/subsurface.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 08:44:40.000000 subsurface-2024.1.0/subsurface.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 08:41:17.000000 subsurface-2024.1.0/subsurface.egg-info/not-zip-safe
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      558 2024-04-29 08:44:40.000000 subsurface-2024.1.0/subsurface.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       26 2024-04-29 08:44:40.000000 subsurface-2024.1.0/subsurface.egg-info/top_level.txt
```

### Comparing `subsurface-0.2.9/LICENSE` & `subsurface-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/README.rst` & `subsurface-2024.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/__init__.py` & `subsurface-2024.1.0/subsurface/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-import subsurface.reader
-import subsurface.interfaces
-import subsurface.writer
-from subsurface.structs import *
-from datetime import datetime
-
-try:
-    from subsurface import visualization
-except ImportError:
-    pass
-
-# Version.
-try:
-    # - Released versions just tags:       0.8.0
-    # - GitHub commits add .dev#+hash:     0.8.1.dev4+g2785721
-    # - Uncommitted changes add timestamp: 0.8.1.dev4+g2785721.d20191022
-    from ._version import version as __version__
-except ImportError:
-    # If it was not installed, then we don't know the version. We could throw a
-    # warning here, but this case *should* be rare. subsurface should be
-    # installed properly!
-    __version__ = 'unknown-'+datetime.today().strftime('%Y%m%d')
-
-if __name__ == '__main__':
-    pass
+import subsurface.reader
+import subsurface.interfaces
+import subsurface.writer
+import subsurface.visualization
+from subsurface.structs import *
+from datetime import datetime
+import dotenv
+
+dotenv.load_dotenv()
+
+try:
+    from subsurface import visualization
+except ImportError:
+    pass
+
+# Version.
+try:
+    # - Released versions just tags:       0.8.0
+    # - GitHub commits add .dev#+hash:     0.8.1.dev4+g2785721
+    # - Uncommitted changes add timestamp: 0.8.1.dev4+g2785721.d20191022
+    from ._version import version as __version__
+except ImportError:
+    # If it was not installed, then we don't know the version. We could throw a
+    # warning here, but this case *should* be rare. subsurface should be
+    # installed properly!
+    __version__ = 'unknown-'+datetime.today().strftime('%Y%m%d')
+
+if __name__ == '__main__':
+    pass
```

### Comparing `subsurface-0.2.9/subsurface/geological_formats/segy_reader.py` & `subsurface-2024.1.0/subsurface/geological_formats/segy_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,60 @@
-from typing import Union
-from scipy.spatial.qhull import Delaunay
-from shapely.geometry import LineString
-from subsurface.structs.base_structures import StructuredData
-import numpy as np
-
-try:
-    import segyio
-    segyio_imported = True
-except ImportError:
-    segyio_imported = False
-
-
-def read_in_segy(filepath: str, coords=None) -> StructuredData:
-    """Reader for seismic data stored in sgy/segy files
-
-    Args:
-        filepath (str): the path of the sgy/segy file
-        coords (dict): If data is a numpy array coords provides the values for
-         the xarray dimension. These dimensions are 'x', 'y' and 'z'
-
-    Returns: a StructuredData object with data, the traces with samples written into an xr.Dataset, optionally with
-     labels defined by coords
-
-    """
-
-    segyfile = segyio.open(filepath, ignore_geometry=True)
-
-    data = np.asarray([np.copy(tr) for tr in segyfile.trace[:]])
-
-    sd = StructuredData.from_numpy(data)  # data holds traces * (samples per trace) values
-    segyfile.close()
-    return sd
-
-
-def create_mesh_from_coords(coords: Union[dict, LineString],
-                           zmin: Union[float, int], zmax: Union[float, int] = 0.0):
-    """Creates a mesh for plotting StructuredData
-
-    Args:
-        coords (Union[dict, LineString]): the x and y, i.e. latitude and longitude, location of the traces of the seismic profile
-        zmax (float): the maximum elevation of the seismic profile, by default 0.0
-        zmin (float): the location in z where the lowest sample was taken
-
-    Returns: vertices and faces for creating an UnstructuredData object
-
-    """
-    if type(coords) == LineString:
-        linestring = coords
-        n = len(list(linestring.coords))
-        coords = np.array([[x[0] for x in list(linestring.coords)],
-                           [y[1] for y in list(linestring.coords)]]).T
-    else:
-        n = len(coords['x'])
-        coords = np.array([coords['x'],
-                           coords['y']]).T
-    # duplicating the line, once with z=lower and another with z=upper values
-    vertices = np.zeros((2*n, 3))
-    vertices[:n, :2] = coords
-    vertices[:n, 2] = zmin
-    vertices[n:, :2] = coords
-    vertices[n:, 2] = zmax
-    # i+n --- i+n+1
-    # |\      |
-    # | \     |
-    # |  \    |
-    # |   \   |
-    # i  --- i+1
-
-    tri = Delaunay(vertices[:, [0, 2]])
-    faces = tri.simplices
-    return vertices, faces
-
+from typing import Union
+
+from subsurface import optional_requirements
+from subsurface.structs.base_structures import StructuredData
+import numpy as np
+
+
+def read_in_segy(filepath: str, coords=None) -> StructuredData:
+    """Reader for seismic data stored in sgy/segy files
+
+    Args:
+        filepath (str): the path of the sgy/segy file
+        coords (dict): If data is a numpy array coords provides the values for
+         the xarray dimension. These dimensions are 'x', 'y' and 'z'
+
+    Returns: a StructuredData object with data, the traces with samples written into an xr.Dataset, optionally with
+     labels defined by coords
+
+    """
+
+    segyio = optional_requirements.require_segyio()
+    segyfile = segyio.open(filepath, ignore_geometry=True)
+
+    data = np.asarray([np.copy(tr) for tr in segyfile.trace[:]])
+
+    sd = StructuredData.from_numpy(data)  # data holds traces * (samples per trace) values
+    segyfile.close()
+    return sd
+
+
+def create_mesh_from_coords(coords: dict, zmin: Union[float, int], zmax: Union[float, int] = 0.0):
+    """Creates a mesh for plotting StructuredData
+
+    Args:
+        coords (Union[dict, LineString]): the x and y, i.e. latitude and longitude, location of the traces of the seismic profile
+        zmax (float): the maximum elevation of the seismic profile, by default 0.0
+        zmin (float): the location in z where the lowest sample was taken
+
+    Returns: vertices and faces for creating an UnstructuredData object
+
+    """
+    n = len(coords['x'])
+    coords = np.array([coords['x'], coords['y']]).T
+    # duplicating the line, once with z=lower and another with z=upper values
+    vertices = np.zeros((2 * n, 3))
+    vertices[:n, :2] = coords
+    vertices[:n, 2] = zmin
+    vertices[n:, :2] = coords
+    vertices[n:, 2] = zmax
+    # i+n --- i+n+1
+    # |\      |
+    # | \     |
+    # |  \    |
+    # |   \   |
+    # i  --- i+1
+
+    scipy = optional_requirements.require_scipy()
+    tri = scipy.spatial.qhull.Delaunay(vertices[:, [0, 2]])
+    faces = tri.simplices
+    return vertices, faces
```

### Comparing `subsurface-0.2.9/subsurface/reader/faults/faults.py` & `subsurface-2024.1.0/subsurface/reader/faults/faults.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/reader/mesh/surfaces_api.py` & `subsurface-2024.1.0/subsurface/reader/mesh/surfaces_api.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/reader/read_netcdf.py` & `subsurface-2024.1.0/subsurface/reader/read_netcdf.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/reader/readers_data.py` & `subsurface-2024.1.0/subsurface/reader/readers_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,116 @@
-import pathlib
-import io
-from dataclasses import dataclass, field
-from typing import Union, Literal, Dict, Optional, List, Callable, Any
-
-import numpy as np
-import pandas as pd
-import xarray as xr
-from pandas._typing import FilePathOrBuffer
-
-from subsurface.utils.utils_core import get_extension
-
-
-__all__ = ['ReaderFilesHelper', 'ReaderUnstructuredHelper',
-           'ReaderWellsHelper', 'RawDataOptions', 'RawDataUnstructured']
-
-
-@dataclass
-class ReaderFilesHelper:
-    file_or_buffer: FilePathOrBuffer
-
-    usecols: Union[List[str], List[int]] = None # Use a subset of columns
-    col_names: List[Union[str, int]] = None # Give a name
-    drop_cols: List[str] = None # Drop a subset of columns
-    format: str = None
-    index_map: Union[None, Callable, dict, pd.Series] = None
-    columns_map: Union[None, Callable, dict, pd.Series] = None
-    additional_reader_kwargs: dict = field(default_factory=dict)
-    file_or_buffer_type: Any = field(init=False)
-
-    index_col: Union[int, str] = False
-    header: Union[None, int, List[int]] = "infer"
-
-    def __post_init__(self):
-        if self.format is None: self.format = get_extension(self.file_or_buffer)
-        self.file_or_buffer_type = type(self.file_or_buffer)
-
-    @property
-    def pandas_reader_kwargs(self):
-        attr_dict = {"names": self.col_names,
-                     "header": self.header,
-                     "index_col": self.index_col,
-                     "usecols": self.usecols
-                     }
-        return {**attr_dict, **self.additional_reader_kwargs}
-
-    @property
-    def is_file_in_disk(self):
-        return self.file_or_buffer_type == str or isinstance(self.file_or_buffer, pathlib.PurePath)
-
-    @property
-    def is_bytes_string(self):
-        return self.file_or_buffer_type == io.BytesIO or self.file_or_buffer_type == io.StringIO
-
-    @property
-    def is_python_dict(self):
-        return self.file_or_buffer_type == dict
-
-@dataclass
-class ReaderUnstructuredHelper:
-    reader_vertex_args: ReaderFilesHelper
-    reader_cells_args: ReaderFilesHelper = None
-    reader_vertex_attr_args: ReaderFilesHelper = None
-    reader_cells_attr_args: ReaderFilesHelper = None
-
-
-@dataclass
-class ReaderWellsHelper:
-    reader_collars_args: ReaderFilesHelper
-    reader_survey_args: ReaderFilesHelper
-    reader_lith_args: ReaderFilesHelper = None
-    reader_attr_args: List[ReaderFilesHelper] = None
-
-
-@dataclass
-class RawDataOptions:
-    swap_yz_cells: bool = False
-
-
-@dataclass(init=False)
-class RawDataUnstructured:
-    vertex: np.ndarray
-    cells: Union[np.ndarray, Literal["lines", "points"]]
-    cells_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None
-    vertex_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None
-
-    def swap_yz_col_cells(self):
-        cells_aux = self.cells.copy()
-        self.cells[:, 1] = cells_aux[:, 2]
-        self.cells[:, 2] = cells_aux[:, 1]
+import enum
+import pathlib
+import io
+from dataclasses import dataclass, field
+from typing import Union, Literal, Dict, Optional, List, Callable, Any
+
+import numpy as np
+import pandas as pd
+import xarray as xr
+
+from subsurface.utils.utils_core import get_extension
+
+__all__ = ['ReaderFilesHelper', 'ReaderUnstructuredHelper',
+           'ReaderWellsHelper', 'RawDataOptions', 'RawDataUnstructured']
+
+if pd.__version__ < '1.4.0':
+    from pandas._typing import FilePathOrBuffer
+
+    fb = FilePathOrBuffer
+elif pd.__version__ >= '1.4.0':
+    from pandas._typing import FilePath, ReadCsvBuffer
+
+    fb = Union[FilePath, ReadCsvBuffer[bytes], ReadCsvBuffer[str]]
+
+
+class SupportedFormats(enum.Enum):
+    DXF = "dxf"
+    DXFStream = "dxfstream"
+    CSV = "csv"
+    JSON = "json"
+    XLXS = "xlsx"
+
+
+@dataclass
+class ReaderFilesHelper:
+    file_or_buffer: fb
+    usecols: Union[List[str], List[int]] = None  # Use a subset of columns
+    col_names: List[Union[str, int]] = None  # Give a name
+    drop_cols: List[str] = None  # Drop a subset of columns
+    format: SupportedFormats = None
+    index_map: Union[None, Callable, dict, pd.Series] = None
+    columns_map: Union[None, Callable, dict, pd.Series] = None
+    additional_reader_kwargs: dict = field(default_factory=dict)
+    file_or_buffer_type: Any = field(init=False)
+
+    index_col: Union[int, str] = False
+    header: Union[None, int, List[int]] = 0
+
+    def __post_init__(self):
+        if self.format is None:
+            extension: str = get_extension(self.file_or_buffer)
+            if extension == ".dxf":
+                self.format = SupportedFormats.DXF
+            elif extension == ".csv":
+                self.format = SupportedFormats.CSV
+            elif extension == ".json":
+                self.format = SupportedFormats.JSON
+            elif extension == ".xlsx":
+                self.format = SupportedFormats.XLXS
+
+        self.file_or_buffer_type = type(self.file_or_buffer)
+
+    @property
+    def pandas_reader_kwargs(self):
+        attr_dict = {"names": self.col_names,
+                     "header": self.header,
+                     "index_col": self.index_col,
+                     "usecols": self.usecols
+                     }
+        return {**attr_dict, **self.additional_reader_kwargs}
+
+    @property
+    def is_file_in_disk(self):
+        return self.file_or_buffer_type == str or isinstance(self.file_or_buffer, pathlib.PurePath)
+
+    @property
+    def is_bytes_string(self):
+        return self.file_or_buffer_type == io.BytesIO or self.file_or_buffer_type == io.StringIO
+
+    @property
+    def is_python_dict(self):
+        return self.file_or_buffer_type == dict
+
+
+@dataclass
+class ReaderUnstructuredHelper:
+    reader_vertex_args: ReaderFilesHelper
+    reader_cells_args: ReaderFilesHelper = None
+    reader_vertex_attr_args: ReaderFilesHelper = None
+    reader_cells_attr_args: ReaderFilesHelper = None
+
+
+@dataclass
+class ReaderWellsHelper:
+    reader_collars_args: ReaderFilesHelper
+    reader_survey_args: ReaderFilesHelper
+    reader_lith_args: ReaderFilesHelper = None
+    reader_attr_args: List[ReaderFilesHelper] = None
+
+
+@dataclass
+class RawDataOptions:
+    swap_yz_cells: bool = False
+
+
+@dataclass(init=False)
+class RawDataUnstructured:
+    vertex: np.ndarray
+    cells: Union[np.ndarray, Literal["lines", "points"]]
+    cells_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None
+    vertex_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None
+
+    def swap_yz_col_cells(self):
+        cells_aux = self.cells.copy()
+        self.cells[:, 1] = cells_aux[:, 2]
+        self.cells[:, 2] = cells_aux[:, 1]
```

### Comparing `subsurface-0.2.9/subsurface/reader/volume/read_volume.py` & `subsurface-2024.1.0/subsurface/reader/volume/read_volume.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,46 @@
-from subsurface.structs import UnstructuredData
-
-from subsurface.reader.readers_data import ReaderFilesHelper
-import pandas as pd
-
-
-__all__ = ['read_volumetric_mesh_to_subsurface',
-           'read_volumetric_mesh_coord_file',
-           'read_volumetric_mesh_attr_file']
-
-
-def read_volumetric_mesh_to_subsurface(reader_helper_coord: ReaderFilesHelper,
-                                       reader_helper_attr: ReaderFilesHelper) -> UnstructuredData:
-    df_coord = read_volumetric_mesh_coord_file(reader_helper_coord)
-    df_attr = read_volumetric_mesh_attr_file(reader_helper_attr)
-    combined_df = df_coord.merge(df_attr, left_index=True, right_index=True)
-    ud = UnstructuredData.from_array(
-        vertex=combined_df[['x', 'y', 'z']], cells="points",
-        attributes=combined_df[['pres', 'temp', 'sg', 'xco2']]
-    )
-    return ud
-
-
-def read_volumetric_mesh_coord_file(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
-    df = pd.read_csv(
-        filepath_or_buffer=reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
-    if reader_helper.columns_map is not None: df.rename(reader_helper.columns_map,
-                                                        axis="columns", inplace=True)
-    df.dropna(axis=0, inplace=True)
-
-    df.x = df.x.astype(float)
-    df.y = df.y.astype(float)
-    df.z = df.z.astype(float)
-    return df
-
-
-def read_volumetric_mesh_attr_file(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
-    df = pd.read_table(reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
-    df.columns = df.columns.str.strip()
-    return df
+from subsurface.structs import UnstructuredData
+
+from subsurface.reader.readers_data import ReaderFilesHelper
+import pandas as pd
+
+__all__ = ['read_volumetric_mesh_to_subsurface',
+           'read_volumetric_mesh_coord_file',
+           'read_volumetric_mesh_attr_file']
+
+
+def read_volumetric_mesh_to_subsurface(reader_helper_coord: ReaderFilesHelper,
+                                       reader_helper_attr: ReaderFilesHelper) -> UnstructuredData:
+    df_coord = read_volumetric_mesh_coord_file(reader_helper_coord)
+    df_attr = read_volumetric_mesh_attr_file(reader_helper_attr)
+    combined_df = df_coord.merge(df_attr, left_index=True, right_index=True)
+    ud = UnstructuredData.from_array(
+        vertex=combined_df[['x', 'y', 'z']], cells="points",
+        attributes=combined_df[['pres', 'temp', 'sg', 'xco2']]
+    )
+    return ud
+
+
+def read_volumetric_mesh_coord_file(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
+    df = pd.read_csv(
+        filepath_or_buffer=reader_helper.file_or_buffer,
+        **reader_helper.pandas_reader_kwargs
+    )
+    if reader_helper.columns_map is not None:
+        df.rename(
+            mapper=reader_helper.columns_map,
+            axis="columns",
+            inplace=True
+        )
+        
+    df.dropna(axis=0, inplace=True)
+
+    df.x = df.x.astype(float)
+    df.y = df.y.astype(float)
+    df.z = df.z.astype(float)
+    return df
+
+
+def read_volumetric_mesh_attr_file(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
+    df = pd.read_table(reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
+    df.columns = df.columns.str.strip()
+    return df
```

### Comparing `subsurface-0.2.9/subsurface/reader/volume/volume_utils.py` & `subsurface-2024.1.0/subsurface/reader/volume/volume_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+import enum
 from typing import List
 
 from scipy.interpolate import griddata
 import numpy as np
 
 from subsurface.structs import UnstructuredData, StructuredData
 
 
 __all__ = ['interpolate_unstructured_data_to_structured_data', ]
 
 
-def interpolate_unstructured_data_to_structured_data(ud: UnstructuredData, attr_name: str,
-                                                     resolution: List[int] = None) -> StructuredData:
+class InterpolationMethod(enum.Enum):
+    linear = "linear"
+    nearest = "nearest"
+
+
+def interpolate_unstructured_data_to_structured_data(
+        ud: UnstructuredData, attr_name: str,
+        resolution: List[int] = None,
+        interpolation_method: InterpolationMethod = InterpolationMethod.nearest) -> StructuredData:
     if resolution is None:
         resolution = [50, 50, 50]
     boundaries_max = ud.vertex.max(axis=0)
-    boundaries_min = ud.vertex.min(axis=1)
+    boundaries_min = ud.vertex.min(axis=0)
     coords = dict()
     dims = ['x', 'y', 'z']
     for e, i in enumerate(dims):
         coords[i] = np.linspace(boundaries_min[e], boundaries_max[e], resolution[e], endpoint=False)
 
     grid = np.meshgrid(*coords.values())
 
     interpolated_attributes = griddata(ud.vertex,
                                        ud.attributes.loc[:, attr_name],
-                                       tuple(grid), method='linear')
+                                       tuple(grid), method=interpolation_method.value)
 
     sd = StructuredData.from_numpy(
         array=interpolated_attributes,
         data_array_name=attr_name,
         coords=coords
     )
     return sd
```

### Comparing `subsurface-0.2.9/subsurface/reader/wells/well_files_reader.py` & `subsurface-2024.1.0/subsurface/reader/wells/DEP/_well_files_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,167 +1,187 @@
-import warnings
-from typing import Dict
-
-import pandas as pd
-
-from subsurface.reader.readers_data import ReaderFilesHelper, ReaderWellsHelper
-from subsurface.reader.wells.wells_utils import add_tops_from_base_and_altitude_in_place
-
-
-__all__ = ['read_borehole_files', 'read_collar', 'read_survey', 'read_lith',
-           'read_attributes', 'check_format_and_read_to_df',
-           'map_rows_and_cols_inplace']
-
-
-def read_borehole_files(reader_wells_helper: ReaderWellsHelper) -> Dict[str, pd.DataFrame]:
-    data_frames = dict()
-
-    data_frames['collar_df'] = read_collar(reader_wells_helper.reader_collars_args)
-
-    data_frames['survey_df'] = read_survey(reader_wells_helper.reader_survey_args)
-
-    if reader_wells_helper.reader_lith_args is not None:
-        data_frames['lith_df'] = read_lith(reader_wells_helper.reader_lith_args)
-
-    if reader_wells_helper.reader_attr_args is not None:
-        attributes_ = list()
-        for e in reader_wells_helper.reader_attr_args:
-            attributes_.append(read_attributes(e))
-        data_frames['attrib_dfs'] = attributes_
-
-    return data_frames
-
-
-def read_collar(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
-
-    if reader_helper.usecols is None: reader_helper.usecols = [0, 1, 2, 3]
-    if reader_helper.index_col is False: reader_helper.index_col = 0
-
-    # Check file_or_buffer type
-    d = check_format_and_read_to_df(reader_helper)
-    map_rows_and_cols_inplace(d, reader_helper)
-
-    return d
-
-
-def read_survey(reader_helper: ReaderFilesHelper):
-    if reader_helper.index_col is False: reader_helper.index_col = 0
-
-    d = check_format_and_read_to_df(reader_helper)
-    map_rows_and_cols_inplace(d, reader_helper)
-
-    d_no_singles = _validate_survey_data(d)
-
-    return d_no_singles
-
-
-def read_lith(reader_helper: ReaderFilesHelper):
-    """Columns MUST contain:
-        - top
-        - base
-        - component lith
-    """
-    if reader_helper.index_col is False: reader_helper.index_col = 0
-
-    d = check_format_and_read_to_df(reader_helper)
-    map_rows_and_cols_inplace(d, reader_helper)
-    lith_df = _validate_lith_data(d, reader_helper)
-
-    return lith_df
-
-
-def read_attributes(reader_helper: ReaderFilesHelper)-> pd.DataFrame:
-    if reader_helper.index_col is False: reader_helper.index_col = 0
-
-    d = check_format_and_read_to_df(reader_helper)
-
-    if reader_helper.columns_map is not None: d.rename(reader_helper.columns_map, axis=1, inplace=True)
-    if reader_helper.drop_cols is not None: d.drop(reader_helper.drop_cols, axis=1, inplace=True)
-
-    _validate_attr_data(d)
-    return d
-
-
-def check_format_and_read_to_df(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
-    if reader_helper.format == ".json":
-        d = pd.read_json(reader_helper.file_or_buffer, orient='split')
-    elif reader_helper.is_file_in_disk:
-        reader = _get_reader(reader_helper.format)
-        d = reader(reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
-    elif reader_helper.is_bytes_string:
-        reader = _get_reader('.csv')
-        d = reader(reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
-    elif reader_helper.is_python_dict:
-        reader = _get_reader('dict')
-        d = reader(reader_helper.file_or_buffer)
-    else:
-        raise AttributeError('file_or_buffer must be either a path or a dict')
-
-    if type(d.columns) is str:  d.columns = d.columns.str.strip() # Remove spaces at the beginning and end
-    if type(d.index) is str: d.index = d.index.str.strip()  # Remove spaces at the beginning and end
-    return d
-
-
-def map_rows_and_cols_inplace(d: pd.DataFrame, reader_helper: ReaderFilesHelper):
-    if reader_helper.index_map is not None:
-        d.rename(reader_helper.index_map, axis="index", inplace=True)#d.index = d.index.map(reader_helper.index_map)
-    if reader_helper.columns_map is not None:
-        d.rename(reader_helper.columns_map, axis="columns", inplace=True)
-        #d.columns = d.columns.map(reader_helper.columns_map)
-
-
-def _get_reader(file_format):
-    if file_format == '.xlsx':
-        reader = pd.read_excel
-    elif file_format == 'dict':
-        reader = _dict_reader
-    else:
-        reader = pd.read_csv
-    return reader
-
-
-def _dict_reader(dict_):
-    """
-
-    Args:
-        dict_: data, index, columns
-
-    """
-    return pd.DataFrame(data=dict_['data'],
-                        columns=dict_['columns'],
-                        index=dict_['index'])
-
-
-def _validate_survey_data(d):
-    if not d.columns.isin(['md']).any():
-        raise AttributeError('md, inc, and azi columns must be present in the file.'
-                             'Use columns_map to assign column names to these fields.')
-
-    elif not pd.np.isin(['md', 'inc', 'azi'], d.columns).all():
-        warnings.warn('inc and/or azi columns are not present in the file.'
-                      ' The boreholes will be straight.')
-        d['inc'] = 0
-        d['azi'] = 0
-
-    # Drop wells that contain only one value
-    d_no_singles = d[d.index.duplicated(keep=False)]
-    return d_no_singles
-
-
-def _validate_lith_data(d: pd.DataFrame, reader_helper: ReaderFilesHelper) -> pd.DataFrame:
-    given_top = pd.np.isin(['top', 'base', 'component lith'], d.columns).all()
-    given_altitude_and_base = pd.np.isin(['altitude', 'base', 'component lith'], d.columns).all()
-
-    if given_altitude_and_base and not given_top:
-        d = add_tops_from_base_and_altitude_in_place(d, reader_helper.index_col, 'base', 'altitude')
-    elif not given_top and not given_altitude_and_base:
-        raise ValueError('basis column must be present in the file. Use '
-                         'columns_map to assign column names to these fields.')
-    lith_df = d[['top', 'base', 'component lith']]
-    return lith_df
-
-
-def _validate_attr_data(d):
-    assert d.columns.isin(['basis']).any(), 'basis column' \
-                                            'must be present in the file.' \
-                                            'Use columns_map to assign' \
-                                            'column names to these fields.'
+import pandas as pd
+import warnings
+from typing import Dict
+
+from subsurface.reader.readers_data import ReaderFilesHelper, ReaderWellsHelper, SupportedFormats
+from subsurface.reader.wells.wells_utils import add_tops_from_base_and_altitude_in_place
+
+
+def read_borehole_files(reader_wells_helper: ReaderWellsHelper) -> Dict[str, pd.DataFrame]:
+    data_frames = dict()
+
+    data_frames['collar_df'] = read_collar(reader_wells_helper.reader_collars_args)
+
+    data_frames['survey_df'] = read_survey(reader_wells_helper.reader_survey_args)
+
+    if reader_wells_helper.reader_lith_args is not None:
+        data_frames['lith_df'] = read_lith(reader_wells_helper.reader_lith_args)
+
+    if reader_wells_helper.reader_attr_args is not None:
+        attributes_ = list()
+        for e in reader_wells_helper.reader_attr_args:
+            attributes_.append(read_attributes(e))
+        data_frames['attrib_dfs'] = attributes_
+
+    return data_frames
+
+
+def read_collar(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
+    if reader_helper.usecols is None: reader_helper.usecols = [0, 1, 2, 3]
+    if reader_helper.index_col is False: reader_helper.index_col = 0
+
+    # Check file_or_buffer type
+    d = check_format_and_read_to_df(reader_helper)
+    map_rows_and_cols_inplace(d, reader_helper)
+
+    return d
+
+
+def read_survey(reader_helper: ReaderFilesHelper):
+    if reader_helper.index_col is False: reader_helper.index_col = 0
+
+    d = check_format_and_read_to_df(reader_helper)
+    map_rows_and_cols_inplace(d, reader_helper)
+
+    d_no_singles = _validate_survey_data(d)
+
+    return d_no_singles
+
+
+def read_lith(reader_helper: ReaderFilesHelper):
+    """Columns MUST contain:
+        - top
+        - base
+        - component lith
+    """
+    if reader_helper.index_col is False: reader_helper.index_col = 0
+
+    d = check_format_and_read_to_df(reader_helper)
+    map_rows_and_cols_inplace(d, reader_helper)
+    lith_df = _validate_lith_data(d, reader_helper)
+
+    return lith_df
+
+
+def read_attributes(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
+    if reader_helper.index_col is False: reader_helper.index_col = 0
+
+    d = check_format_and_read_to_df(reader_helper)
+
+    if reader_helper.columns_map is not None: d.rename(reader_helper.columns_map, axis=1, inplace=True)
+    if reader_helper.drop_cols is not None: d.drop(reader_helper.drop_cols, axis=1, inplace=True)
+
+    _validate_attr_data(d)
+    return d
+
+
+def read_survey_df_from_las(reader_helper: ReaderFilesHelper, well_name: str) -> pd.DataFrame:
+    """
+    Reads a las file and returns a dataframe.
+    
+    """
+    from subsurface.reader.wells._welly_reader import _create_welly_well_from_las
+    welly_well = _create_welly_well_from_las(well_name, reader_helper.file_or_buffer)
+    survey_df = welly_well.df()[reader_helper.usecols]
+    map_rows_and_cols_inplace(survey_df, reader_helper)
+    survey_df["well_name"] = well_name
+    survey_df.set_index("well_name", inplace=True)
+    return survey_df
+
+
+def read_assay_df_from_las(reader_helper: ReaderFilesHelper, well_name: str) -> pd.DataFrame:
+    from subsurface.reader.wells._welly_reader import _create_welly_well_from_las
+    welly_well = _create_welly_well_from_las(well_name, reader_helper.file_or_buffer)
+    assay_df = welly_well.df()
+    assay_df["well_name"] = well_name
+    assay_df.set_index("well_name", inplace=True)
+    return assay_df
+
+
+def check_format_and_read_to_df(reader_helper: ReaderFilesHelper) -> pd.DataFrame:
+    if reader_helper.format == ".json":
+        d = pd.read_json(reader_helper.file_or_buffer, orient='split')
+    elif reader_helper.is_file_in_disk:
+        reader = _get_reader(reader_helper.format)
+        d = reader(reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
+    elif reader_helper.is_bytes_string:
+        reader = _get_reader('.csv')
+        d = reader(reader_helper.file_or_buffer, **reader_helper.pandas_reader_kwargs)
+    elif reader_helper.is_python_dict:
+        reader = _get_reader('dict')
+        d = reader(reader_helper.file_or_buffer)
+    else:
+        raise AttributeError('file_or_buffer must be either a path or a dict')
+
+    if type(d.columns) is str:  d.columns = d.columns.str.strip()  # Remove spaces at the beginning and end
+    if type(d.index) is str: d.index = d.index.str.strip()  # Remove spaces at the beginning and end
+    return d
+
+
+def map_rows_and_cols_inplace(d: pd.DataFrame, reader_helper: ReaderFilesHelper):
+    if reader_helper.index_map is not None:
+        d.rename(reader_helper.index_map, axis="index", inplace=True)  # d.index = d.index.map(reader_helper.index_map)
+    if reader_helper.columns_map is not None:
+        d.rename(reader_helper.columns_map, axis="columns", inplace=True)
+        # d.columns = d.columns.map(reader_helper.columns_map)
+
+
+def _get_reader(file_format):
+    if file_format == SupportedFormats.XLXS:
+        reader = pd.read_excel
+    elif file_format == 'dict':
+        reader = _dict_reader
+    elif file_format == SupportedFormats.CSV:
+        reader = pd.read_csv
+    elif file_format == SupportedFormats.JSON:
+        reader = _dict_reader
+    else:
+        raise ValueError(f"Subsurface is not able to read the following extension: {file_format}")
+    return reader
+
+
+def _dict_reader(dict_):
+    """
+
+    Args:
+        dict_: data, index, columns
+
+    """
+    return pd.DataFrame(data=dict_['data'],
+                        columns=dict_['columns'],
+                        index=dict_['index'])
+
+
+def _validate_survey_data(d):
+    if not d.columns.isin(['md']).any():
+        raise AttributeError('md, inc, and azi columns must be present in the file.'
+                             'Use columns_map to assign column names to these fields.')
+
+    elif not pd.np.isin(['md', 'inc', 'azi'], d.columns).all():
+        warnings.warn('inc and/or azi columns are not present in the file.'
+                      ' The boreholes will be straight.')
+        d['inc'] = 0
+        d['azi'] = 0
+
+    # Drop wells that contain only one value
+    d_no_singles = d[d.index.duplicated(keep=False)]
+    return d_no_singles
+
+
+def _validate_lith_data(d: pd.DataFrame, reader_helper: ReaderFilesHelper) -> pd.DataFrame:
+    given_top = pd.np.isin(['top', 'base', 'component lith'], d.columns).all()
+    given_altitude_and_base = pd.np.isin(['altitude', 'base', 'component lith'], d.columns).all()
+
+    if given_altitude_and_base and not given_top:
+        d = add_tops_from_base_and_altitude_in_place(d, reader_helper.index_col, 'base', 'altitude')
+    elif not given_top and not given_altitude_and_base:
+        raise ValueError('basis column must be present in the file. Use '
+                         'columns_map to assign column names to these fields.')
+    lith_df = d[['top', 'base', 'component lith']]
+    return lith_df
+
+
+def _validate_attr_data(d):
+    assert d.columns.isin(['basis']).any(), 'basis column' \
+                                            'must be present in the file.' \
+                                            'Use columns_map to assign' \
+                                            'column names to these fields.'
```

### Comparing `subsurface-0.2.9/subsurface/reader/wells/wells_api.py` & `subsurface-2024.1.0/subsurface/reader/wells/DEP/_wells_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,61 @@
-from typing import List
-
-import pandas as pd
-from striplog import Component
-
-from subsurface.reader.wells.pandas_to_welly import WellyToSubsurfaceHelper
-from subsurface.reader.wells.well_files_reader import read_borehole_files
-from subsurface.reader.wells.welly_reader import welly_to_subsurface
-from subsurface.reader.readers_data import ReaderWellsHelper, ReaderFilesHelper
-
-from subsurface.structs import UnstructuredData
-
-from subsurface.reader.wells import read_collar
-
-
-__all__ = ['read_wells_to_unstruct', 'borehole_location_to_unstruct']
-
-
-def read_wells_to_unstruct(reader_wells_helper: ReaderWellsHelper,
-                            backend='welly', n_vertex_per_well=80,
-                           table: List[Component] = None) -> UnstructuredData:
-    """Read from csv files (or excel) to `subsurface.Unstructured` object.
-
-    Args:
-        backend (string): Which library use for reading and processing of data.
-         So far: welly
-        table (List[Striplog.Component]): List of components to map lithologies
-         to value.
-        n_vertex_per_well (int): Number of vertex used to describe the geometry of the
-         well.
-
-    Returns:
-        `subsurface.UnstructuredData`:  if `return_welly` also the
-         welly object
-
-    """
-    pandas_dict = read_borehole_files(reader_wells_helper)
-
-    if backend == 'welly':
-        wts = WellyToSubsurfaceHelper(**pandas_dict)
-        unstruct = welly_to_subsurface(wts, n_vertex_per_well=n_vertex_per_well, table=table)
-    else:
-        raise AttributeError('Only welly is available at the moment')
-
-    return unstruct
-
-
-def borehole_location_to_unstruct(reader_helper: ReaderFilesHelper,
-                                  add_number_segments: bool = True) -> UnstructuredData:
-
-    collars = read_collar(reader_helper)
-    collars_attributes = pd.DataFrame()
-
-    # Remove duplicates
-    collars_single_well = collars[~collars.index.duplicated()]
-    wells_names = collars_single_well.index
-
-    if add_number_segments is True:
-        number_of_segments = collars.index.value_counts(sort=False).values
-        collars_attributes['number_segments'] = number_of_segments
-
-    ud = UnstructuredData.from_array(
-        vertex=collars_single_well[['x', 'y', 'altitude']].values.astype('float32'),
-        cells="points",
-        cells_attr=collars_attributes.astype('float32'),
-        xarray_attributes={"wells_names": wells_names.values.tolist()})  # TODO: This should be int16!
-
-    return ud
+from typing import List
+
+import pandas as pd
+
+from .pandas_to_welly import WellyToSubsurfaceHelper
+from ._well_files_reader import read_borehole_files, read_collar
+from ._welly_reader import welly_to_subsurface
+
+from subsurface.reader.readers_data import ReaderWellsHelper, ReaderFilesHelper
+from subsurface.structs import UnstructuredData
+
+
+def read_wells_to_unstruct(reader_wells_helper: ReaderWellsHelper,
+                           backend='welly', n_vertex_per_well=80,
+                           table: List['welly.Component'] = None) -> UnstructuredData:
+    """Read from csv files (or excel) to `subsurface.Unstructured` object.
+
+    Args:
+        backend (string): Which library use for reading and processing of data.
+         So far: welly
+        table (List[Striplog.Component]): List of components to map lithologies
+         to value.
+        n_vertex_per_well (int): Number of vertex used to describe the geometry of the
+         well.
+
+    Returns:
+        `subsurface.UnstructuredData`:  if `return_welly` also the
+         welly object
+
+    """
+    pandas_dict = read_borehole_files(reader_wells_helper)
+
+    if backend == 'welly':
+        wts = WellyToSubsurfaceHelper(**pandas_dict)
+        unstruct = welly_to_subsurface(wts, n_vertex_per_well=n_vertex_per_well, table=table)
+    else:
+        raise AttributeError('Only welly is available at the moment')
+
+    return unstruct
+
+
+def borehole_location_to_unstruct(reader_helper: ReaderFilesHelper,
+                                  add_number_segments: bool = True) -> UnstructuredData:
+    collars = read_collar(reader_helper)
+    collars_attributes = pd.DataFrame()
+
+    # Remove duplicates
+    collars_single_well = collars[~collars.index.duplicated()]
+    wells_names = collars_single_well.index
+
+    if add_number_segments is True:
+        number_of_segments = collars.index.value_counts(sort=False).values
+        collars_attributes['number_segments'] = number_of_segments
+
+    ud = UnstructuredData.from_array(
+        vertex=collars_single_well[['x', 'y', 'altitude']].values.astype('float32'),
+        cells="points",
+        cells_attr=collars_attributes.astype('float32'),
+        xarray_attributes={"wells_names": wells_names.values.tolist()})  # TODO: This should be int16!
+
+    return ud
```

### Comparing `subsurface-0.2.9/subsurface/reader/wells/wells_utils.py` & `subsurface-2024.1.0/subsurface/reader/wells/DEP/wells_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from typing import List
-
-import pandas as pd
-
-
-__all__ = ['add_tops_from_base_and_altitude_in_place',
-           'fix_wells_higher_base_than_top_inplace', 'map_attr_to_segments',
-           'pivot_wells_df_into_segment_per_row']
-
-
-def add_tops_from_base_and_altitude_in_place(data: pd.DataFrame, col_well_name: str, col_base: str,
-                                             col_altitude: str) -> pd.DataFrame:
-    d = data
-    d = _remove_repeated_rows(d)
-    _create_base_col(col_altitude, col_base, d)
-    _create_top_col(col_altitude, col_well_name, d)
-    _add_md_col_if_missing(d)
-    return d
-
-
-def fix_wells_higher_base_than_top_inplace(df_fixed) -> pd.DataFrame:
-    top_base_error = df_fixed["top"] > df_fixed["base"]
-    df_fixed["base"][top_base_error] = df_fixed["top"] + 0.01
-    return df_fixed
-
-
-def map_attr_to_segments(df, attr_per_segment: List, n_wells: int) -> pd.DataFrame:
-    tiled_formations = pd.np.tile(attr_per_segment, (n_wells))
-    df['formation'] = tiled_formations
-    return df
-
-
-def pivot_wells_df_into_segment_per_row(df: pd.DataFrame, start_segment_cols: int, n_segments_per_well: int) -> pd.DataFrame:
-    # Repeat fixed rows (collar name and so)
-    df_fixed = df.iloc[:, :start_segment_cols]
-    df_fixed = df_fixed.loc[df_fixed.index.repeat(n_segments_per_well)]
-
-    df_bottoms = df.iloc[:, start_segment_cols:start_segment_cols + n_segments_per_well]
-    df_fixed['base'] = df_bottoms.values.reshape(-1, 1, order='C')
-
-    return df_fixed
-
-
-def _add_md_col_if_missing(d):
-    if "md" not in d.columns:
-        d.loc[:, 'md'] = d['top']
-
-
-def _create_top_col(col_altitude, col_well_name, d):
-    Z_shift = d.groupby(col_well_name)['base'].shift(1)
-    Z_0 = Z_shift.fillna(0)
-    v = Z_0 + d[col_altitude]
-    d.loc[:, 'top'] = Z_0
-    d.loc[:, '_top_abs'] = v
-
-
-def _create_base_col(col_altitude, col_base, d):
-    d.loc[:, 'base'] = d[col_altitude] - d[col_base]
-
-
-def _remove_repeated_rows(d):
-    repeated_rows = _mark_repeated_rows(d['base'])
-    d = d[~repeated_rows]  # removed repeated rows
-    return d
-
-
-def _mark_repeated_rows(series: pd.Series):
-    return series.shift(1) == series
+from typing import List
+
+import pandas as pd
+
+
+__all__ = ['add_tops_from_base_and_altitude_in_place',
+           'fix_wells_higher_base_than_top_inplace', 'map_attr_to_segments',
+           'pivot_wells_df_into_segment_per_row']
+
+
+def add_tops_from_base_and_altitude_in_place(data: pd.DataFrame, col_well_name: str, col_base: str,
+                                             col_altitude: str) -> pd.DataFrame:
+    d = data
+    d = _remove_repeated_rows(d)
+    _create_base_col(col_altitude, col_base, d)
+    _create_top_col(col_altitude, col_well_name, d)
+    _add_md_col_if_missing(d)
+    return d
+
+
+def fix_wells_higher_base_than_top_inplace(df_fixed) -> pd.DataFrame:
+    top_base_error = df_fixed["top"] > df_fixed["base"]
+    df_fixed["base"][top_base_error] = df_fixed["top"] + 0.01
+    return df_fixed
+
+
+def map_attr_to_segments(df, attr_per_segment: List, n_wells: int) -> pd.DataFrame:
+    tiled_formations = pd.np.tile(attr_per_segment, (n_wells))
+    df['formation'] = tiled_formations
+    return df
+
+
+def pivot_wells_df_into_segment_per_row(df: pd.DataFrame, start_segment_cols: int, n_segments_per_well: int) -> pd.DataFrame:
+    # Repeat fixed rows (collar name and so)
+    df_fixed = df.iloc[:, :start_segment_cols]
+    df_fixed = df_fixed.loc[df_fixed.index.repeat(n_segments_per_well)]
+
+    df_bottoms = df.iloc[:, start_segment_cols:start_segment_cols + n_segments_per_well]
+    df_fixed['base'] = df_bottoms.values.reshape(-1, 1, order='C')
+
+    return df_fixed
+
+
+def _add_md_col_if_missing(d):
+    if "md" not in d.columns:
+        d.loc[:, 'md'] = d['top']
+
+
+def _create_top_col(col_altitude, col_well_name, d):
+    Z_shift = d.groupby(col_well_name)['base'].shift(1)
+    Z_0 = Z_shift.fillna(0)
+    v = Z_0 + d[col_altitude]
+    d.loc[:, 'top'] = Z_0
+    d.loc[:, '_top_abs'] = v
+
+
+def _create_base_col(col_altitude, col_base, d):
+    d.loc[:, 'base'] = d[col_altitude] - d[col_base]
+
+
+def _remove_repeated_rows(d):
+    repeated_rows = _mark_repeated_rows(d['base'])
+    d = d[~repeated_rows]  # removed repeated rows
+    return d
+
+
+def _mark_repeated_rows(series: pd.Series):
+    return series.shift(1) == series
```

### Comparing `subsurface-0.2.9/subsurface/structs/README.rst` & `subsurface-2024.1.0/subsurface/structs/README.rst`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/structs/base_structures/common_data_utils.py` & `subsurface-2024.1.0/subsurface/structs/base_structures/common_data_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-import os
-from typing import Union
-
-from subsurface.structs.base_structures.structured_data import StructuredData
-from subsurface.structs.base_structures.unstructured_data import UnstructuredData
-
-
-__all__ = ['replace_outliers', 'to_netcdf', 'default_path_and_name']
-
-
-def replace_outliers(base_data: Union[StructuredData, UnstructuredData], dim=0, perc=0.99, replace_for=None):
-    """@Edoardo Guerreiro https://stackoverflow.com/questions/60816533/
-     is-there-a-built-in-function-in-xarray-to-remove-outliers-from-a-dataset"""
-
-    data = base_data.data
-    # calculate percentile
-    threshold = data[dim].quantile(perc)
-
-    # find outliers and replace them with max among remaining values
-    mask = data[dim].where(abs(data[dim]) <= threshold)
-    if replace_for == 'max':
-        max_value = mask.max().values
-        # .where replace outliers with nan
-        mask = mask.fillna(max_value)
-    elif replace_for == 'min':
-        min_value = mask.min().values
-        # .where replace outliers with nan
-        mask = mask.fillna(min_value)
-
-    print(mask)
-    data[dim] = mask
-
-    return data
-
-
-def to_netcdf(base_data: Union[StructuredData, UnstructuredData], path=None, file: str = None, **kwargs):
-    if path is None and file is not None:
-        name, path = default_path_and_name(path, file)
-    return base_data.data.to_netcdf(path, **kwargs)
-
-
-def default_path_and_name(path, name='subsurface_data.nc', ):
-
-    if not path:
-        path = './'
-    if os.path.isdir(path):
-        print("Directory already exists, files will be overwritten")
-    else:
-        os.makedirs(f'{path}')
-    path = f'{path}/{name}'
-    return name, path
+import os
+import warnings
+from typing import Union
+
+from subsurface.structs.base_structures.structured_data import StructuredData
+from subsurface.structs.base_structures.unstructured_data import UnstructuredData
+
+__all__ = ['replace_outliers', 'to_netcdf', 'default_path_and_name']
+
+
+def replace_outliers(base_data: Union[StructuredData, UnstructuredData], dim=0, perc=0.99, replace_for=None):
+    """@Edoardo Guerreiro https://stackoverflow.com/questions/60816533/
+     is-there-a-built-in-function-in-xarray-to-remove-outliers-from-a-dataset"""
+
+    data = base_data.data
+    # calculate percentile
+    threshold = data[dim].quantile(perc)
+
+    # find outliers and replace them with max among remaining values
+    mask = data[dim].where(abs(data[dim]) <= threshold)
+    if replace_for == 'max':
+        max_value = mask.max().values
+        # .where replace outliers with nan
+        mask = mask.fillna(max_value)
+    elif replace_for == 'min':
+        min_value = mask.min().values
+        # .where replace outliers with nan
+        mask = mask.fillna(min_value)
+
+    print(mask)
+    data[dim] = mask
+
+    return data
+
+
+def to_netcdf(base_data: Union[StructuredData, UnstructuredData], path=None, file: str = None, **kwargs):
+    if path is None and file is not None:
+        # TODO: Mark file as deprecated
+        warnings.warn("file argument is deprecated, please use path instead", DeprecationWarning)
+        name, path = default_path_and_name(path, file)
+    return base_data.data.to_netcdf(path, format="NETCDF4", **kwargs)
+
+
+def default_path_and_name(path, name='subsurface_data.nc', ):
+    if not path:
+        path = './'
+    if os.path.isdir(path):
+        print("Directory already exists, files will be overwritten")
+    else:
+        os.makedirs(f'{path}')
+    path = f'{path}/{name}'
+    return name, path
```

### Comparing `subsurface-0.2.9/subsurface/structs/base_structures/structured_data.py` & `subsurface-2024.1.0/subsurface/structs/base_structures/structured_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from dataclasses import dataclass
-from typing import Dict, List
+from typing import Dict, List, Tuple
 
 import numpy as np
 import xarray as xr
 
-
 __all__ = ['StructuredData', ]
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=False)
 class StructuredData:
     data: xr.Dataset
-    data_array_name: str = "data_array"
+    _data_array_name: str = "data_array"
 
     """Primary structure definition for structured data
 
        Check out other constructors: `StructuredData.from_numpy`,
         `StructuredData.from_data_array` and `StructuredData.from_dict`
 
     Args:
@@ -27,14 +26,25 @@
         data_array_name (str): If data is a numpy array or xarray DataArray, data_name
          provides the name for the xarray data variable
      
     Attributes:
         data (xarray.Dataset)
     """
 
+    @property
+    def data_array_name(self):
+        data_var_list = list(self.data.data_vars.keys())
+        if self._data_array_name not in data_var_list:
+            raise ValueError("data_array_name not found in data_vars: {}".format(data_var_list))
+        return self._data_array_name
+
+    @data_array_name.setter
+    def data_array_name(self, data_array_name: str):
+        self._data_array_name = data_array_name
+
     @classmethod
     def from_numpy(cls, array: np.ndarray, coords: dict = None, data_array_name: str = "data_array",
                    dim_names: List[str] = None):
         if dim_names is None:
             if array.ndim == 2:
                 dim_names = ['x', 'y']
             elif array.ndim == 3:
@@ -54,24 +64,31 @@
         return cls(xr.Dataset(data_vars=data_dict, coords=coords))
 
     @property
     def values(self):
         return self.data[self.data_array_name].values
 
     @property
-    def default_dataset(self):
+    def default_data_array(self):
         return self.data[self.data_array_name]
 
-    def to_binary(self, order='F'):
-        bytearray_le = self._to_bytearray(order)
-        header = self._set_binary_header()
+    def default_data_array_to_binary(self, order='F'):
+        bytearray_le = self._to_bytearray(self.default_data_array, order)
+        header = self._set_binary_header(self.default_data_array)
 
         return bytearray_le, header
-
-    def _set_binary_header(self):
-        header = {"data_shape": self.values.shape}
+    
+    def to_binary(self, data_array: xr.DataArray, order: str = 'F') -> Tuple[bytes, Dict]:
+        bytearray_le = self._to_bytearray(data_array, order)
+        header = self._set_binary_header(data_array)
+        return bytearray_le, header
+        
+    @staticmethod
+    def _set_binary_header(data_array: xr.DataArray) -> Dict:
+        header = {"data_shape": data_array.shape}
         return header
 
-    def _to_bytearray(self, order):
-        data = self.values.astype('float32').tobytes(order)
+    @staticmethod
+    def _to_bytearray(data_array: xr.DataArray, order: str) -> bytes:
+        data = data_array.values.astype('float32').tobytes(order)
         bytearray_le = data
         return bytearray_le
```

### Comparing `subsurface-0.2.9/subsurface/structs/base_structures/unstructured_data.py` & `subsurface-2024.1.0/subsurface/structs/base_structures/unstructured_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,296 +1,308 @@
-from dataclasses import dataclass
-from typing import Union, Dict, Mapping, Hashable, Any, Literal, List
-
-import numpy as np
-import pandas as pd
-import xarray as xr
-
-from subsurface.reader.readers_data import RawDataUnstructured
-
-
-__all__ = ['UnstructuredData', ]
-
-
-@dataclass(frozen=True)
-class UnstructuredData:
-    data: xr.Dataset
-    cells_attr_name: str = "cell_attrs"
-    vertex_attr_name: str = "vertex_attrs"
-
-    """Primary structure definition for unstructured data
-
-    Attributes:
-        data (`xarray.Dataset`): Data structure where we store
-
-    Args:
-
-        ds (xarray.Dataset): Directly a dataset with the expected structured. This
-         arg is specially thought for loading data from disk
-
-    Notes:
-        Depending on the shape of `edge` the following unstructured elements can
-        be created:
-
-        - cells NDArray[(Any, 0), IntX] or NDArray[(Any, 1), IntX] -> *Point cloud*.
-          E.g. Outcrop scan with lidar
-        - cells NDArray[(Any, 2), IntX] -> *Lines*. E.g. Borehole
-        - cells NDArray[(Any, 3), IntX] -> *Mesh*. E.g surface-DEM Topography
-        - cells NDArray[(Any, 4), IntX]
-           - -> *tetrahedron*
-           - -> *quadrilateral (or tetragon)* UNSUPPORTED?
-        - cells NDArray[(Any, 8), IntX] -> *Hexahedron: Unstructured grid/Prisms*
-    """
-
-    def __post_init__(self):
-        self._validate()
-
-    def __repr__(self):
-        return self.data.__repr__()
-
-    @classmethod
-    def from_raw_data(cls, raw_data: RawDataUnstructured,
-                      coords: Mapping[Hashable, Any] = None,
-                      xarray_attributes: Mapping[Hashable, Any] = None,
-                      default_cells_attributes_name: str = "cell_attrs",
-                      default_points_attributes_name: str = "vertex_attrs"
-                      ):
-        return cls.from_array(raw_data.vertex, raw_data.cells, raw_data.cells_attr, raw_data.vertex_attr, coords,
-                              xarray_attributes, default_cells_attributes_name, default_points_attributes_name)
-
-    @classmethod
-    def from_array(
-            cls,
-            vertex: np.ndarray,
-            cells: Union[np.ndarray, Literal["lines", "points"]],
-            cells_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None,
-            vertex_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None,
-            coords: Mapping[Hashable, Any] = None,
-            xarray_attributes: Mapping[Hashable, Any] = None,
-            default_cells_attr_name: str = "cell_attrs",
-            default_points_attr_name: str = "vertex_attrs",
-            attributes: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None  # TODO Obsolete
-    ):
-        """ Constructor of UnstructuredData from arrays or pandas DataFrames.
-
-        Args:
-            vertex (np.ndarray): NDArray[(Any, 3), FloatX]: XYZ point data
-            cells (Union[np.ndarray, Literal["lines", "points"]]): NDArray[(Any, ...), IntX]:
-             Combination of vertex that create different geometric elements. If
-             str use default values for either points or lines
-            cells_attr (Union[None, pd.DataFrame, Dict[str, xr.DataArray]]]: Number associated to an element
-            vertex_attr (Union[None, pd.DataFrame, Dict[str, xr.DataArray]]]: Number
-             associated to points
-            coords:
-            xarray_attributes:
-            attributes:
-            default_cells_attr_name:
-            default_points_attr_name:
-
-        Returns:
-
-        """
-        if attributes is not None:
-            cells_attr = attributes
-
-        cells_data_array, n_cells, n_vertex, vertex_data_array = cls.vertex_and_cells_arrays_to_data_array(cells,
-                                                                                                           vertex)
-        points_attributes_xarray_dict = cls.raw_attributes_to_dict_data_arrays(
-            default_points_attr_name, n_vertex, ["points", "vertex_attr"], vertex_attr)
-        cells_attributes_xarray_dict = cls.raw_attributes_to_dict_data_arrays(
-            default_cells_attr_name, n_cells, ["cell", "cell_attr"], cells_attr)
-
-        xarray_dict = {
-            "vertex": vertex_data_array, "cells": cells_data_array,
-            **cells_attributes_xarray_dict,
-            **points_attributes_xarray_dict
-        }
-
-        default_cells_attr_name = cells_attributes_xarray_dict.get(None, next(iter(cells_attributes_xarray_dict)))
-        default_points_attr_name = points_attributes_xarray_dict.get(None,
-                                                                     next(iter(points_attributes_xarray_dict)))
-
-        return cls.from_data_arrays_dict(xarray_dict, coords, xarray_attributes,
-                                         default_cells_attr_name, default_points_attr_name)
-
-    @classmethod
-    def from_data_arrays_dict(cls, xarray_dict: Dict[str, xr.DataArray],
-                              coords: Mapping[Hashable, Any] = None,
-                              xarray_attributes: Mapping[Hashable, Any] = None,
-                              default_cells_attributes_name="cell_attrs",
-                              default_points_attributes_name="vertex_attrs"):
-
-        ds = xr.Dataset(xarray_dict, coords=coords, attrs=xarray_attributes)
-
-        # Try to unstack pandas dataframe if exist
-        # TODO: This is an issue in wells. If it is only there maybe we should move it there
-        try:
-            ds = ds.reset_index('cell')
-        except KeyError:
-            pass
-
-        return cls(ds, default_cells_attributes_name, default_points_attributes_name)
-
-    @classmethod
-    def raw_attributes_to_dict_data_arrays(
-            cls, default_attributes_name: str, n_items: int, dims: List[str],
-            raw_attributes: Union[None, pd.DataFrame, Dict[str, xr.DataArray]]) \
-            -> Dict[str, xr.DataArray]:
-
-        if raw_attributes is None or type(raw_attributes) == pd.DataFrame:
-            points_attributes_xarray_dict = {
-                default_attributes_name: cls.data_array_attributes_from_raw_data(raw_attributes, dims, n_items)
-            }
-        else:
-            points_attributes_xarray_dict = raw_attributes
-        return points_attributes_xarray_dict
-
-    @classmethod
-    def vertex_and_cells_arrays_to_data_array(cls, cells: Union[np.ndarray, Literal["lines", "points"]],
-                                              vertex: np.ndarray):
-        n_vertex = vertex.shape[0]
-        if type(cells) != np.ndarray:
-            cells = cls.create_default_cells_arg(cells, n_vertex)
-        n_cells = cells.shape[0]
-        vertex_data_array = xr.DataArray(vertex, dims=['points', 'XYZ'],
-                                         coords={'XYZ': ['X', 'Y', 'Z']})
-        cells_data_array = xr.DataArray(cells, dims=['cell', 'nodes'])
-        return cells_data_array, n_cells, n_vertex, vertex_data_array
-
-    @classmethod
-    def data_array_attributes_from_raw_data(cls, raw_data: Union[None, pd.DataFrame],
-                                            dims: List[str], n_rows: int) -> xr.DataArray:
-        if raw_data is None:
-            raw_data = pd.DataFrame(np.zeros((n_rows, 0)))
-
-        if type(raw_data) is pd.DataFrame:
-            data_array = xr.DataArray(raw_data, dims=dims)
-        else:
-            raise ValueError("cells_attributes must be either pd.DataFrame or "
-                             "None/default.")
-        return data_array
-
-    @classmethod
-    def create_default_cells_arg(cls, cells: Literal["points", "lines"], n_vertex: int) -> np.ndarray:
-
-        if cells is None or cells == 'points':
-            cells = np.arange(0, n_vertex).reshape(-1, 1)
-        elif cells == 'lines':
-            a = np.arange(0, n_vertex - 1, dtype=np.int_)
-            b = np.arange(1, n_vertex, dtype=np.int_)
-            cells = np.vstack([a, b]).T
-        elif type(cells) != np.ndarray:
-            raise ValueError("cells must be either None (will default to 'points'),"
-                             "'points', 'lines' or a 2D ndarray.")
-        return cells
-
-    def _validate(self):
-        try:
-            _ = self.data[self.cells_attr_name]['cell']
-            _ = self.data[self.cells_attr_name]['cell_attr']
-
-        except KeyError:
-            raise KeyError('Cell attribute DataArrays must contain dimension cell and '
-                           'cell_attr')
-
-        try:
-            _ = self.data[self.vertex_attr_name]['vertex_attr']
-            _ = self.data[self.vertex_attr_name]['points']
-        except KeyError:
-            raise KeyError('Point attribute DataArrays must contain dimensions'
-                           ' points and vertex_attr.')
-
-        # Make sure the number of vertices matches the associated data.
-        if self.data['cells']['cell'].size != self.data[self.cells_attr_name]['cell'].size:
-            raise AttributeError('Attributes and cells must have the same length.')
-
-        if self.n_points != self.data[self.vertex_attr_name]['points'].size:
-            raise AttributeError('points_attributes and vertex must have the same length.')
-
-    @property
-    def vertex(self) -> np.ndarray:
-        return self.data['vertex'].values
-
-    @property
-    def cells(self):
-        return self.data['cells'].values
-
-    @property
-    def attributes(self):
-        xarray = self.data[self.cells_attr_name]
-        return xarray.to_dataframe()[self.cells_attr_name].unstack(level=1)
-
-    @attributes.setter
-    def attributes(self, dataframe):
-        self.data[self.cells_attr_name] = xr.DataArray(dataframe, dims=['element', 'cell_attr'])
-
-    @property
-    def points_attributes(self):
-        return self.data[self.vertex_attr_name].to_dataframe()[
-            self.vertex_attr_name].unstack(level=1)
-
-    @points_attributes.setter
-    def points_attributes(self, dataframe):
-        self.data[self.vertex_attr_name] = xr.DataArray(dataframe, dims=['points', 'vertex_attr'])
-
-    @property
-    def n_elements(self):
-        return self.cells.shape[0]
-
-    @property
-    def n_vertex_per_element(self):
-        return self.cells.shape[1]
-
-    @property
-    def n_points(self):
-        return self.vertex.shape[0]
-
-    @property
-    def attributes_to_dict(self, orient='list'):
-        return self.attributes.to_dict(orient)
-
-    @property
-    def points_attributes_to_dict(self, orient='list'):
-        return self.points_attributes.to_dict(orient)
-
-    @property
-    def extent(self):
-        max = self.vertex.max(axis=0)
-        min = self.vertex.min(axis=0)
-        extent = np.stack((min, max), axis = 1).ravel()
-        return extent
-
-    def to_xarray(self):
-        a = xr.DataArray(self.vertex, dims=['points', 'XYZ'])
-        b = xr.DataArray(self.cells, dims=['cells', 'node'])
-        e = xr.DataArray(self.attributes, dims=['element', 'cell_attr'])
-        c = xr.Dataset({'v': a, 'e': b, 'a': e})
-        return c
-
-    def to_binary(self, order='F'):
-        bytearray_le = self._to_bytearray(order)
-        header = self._set_binary_header()
-
-        return bytearray_le, header
-
-    def _set_binary_header(self):
-
-        header = {
-            "vertex_shape": self.vertex.shape,
-            "cell_shape": self.cells.shape,
-            "cell_attr_shape": self.attributes.shape,
-            "vertex_attr_shape": self.points_attributes.shape,
-            "cell_attr_names": self.attributes.columns.to_list(),
-            "cell_attr_types": self.attributes.dtypes.astype(str).to_list(),
-            "vertex_attr_names": self.points_attributes.columns.to_list(),
-            "vertex_attr_types": self.attributes.dtypes.astype(str).to_list(),
-            "xarray_attrs": self.data.attrs
-        }
-        return header
-
-    def _to_bytearray(self, order):
-        vertex = self.vertex.astype('float32').tobytes(order)
-        cells = self.cells.astype('int32').tobytes(order)
-        cell_attribute = self.attributes.values.astype('float32').tobytes(order)
-        vertex_attribute = self.points_attributes.values.astype('float32').tobytes(order)
-        bytearray_le = vertex + cells + cell_attribute + vertex_attribute
-        return bytearray_le
+from dataclasses import dataclass
+from typing import Union, Dict, Mapping, Hashable, Any, Literal, List
+
+import numpy as np
+import pandas as pd
+import xarray as xr
+
+from subsurface.reader.readers_data import RawDataUnstructured
+
+__all__ = ['UnstructuredData', ]
+
+
+@dataclass(frozen=False)
+class UnstructuredData:
+    data: xr.Dataset
+    cells_attr_name: str = "cell_attrs"
+    vertex_attr_name: str = "vertex_attrs"
+
+    """Primary structure definition for unstructured data
+
+    Attributes:
+        data (`xarray.Dataset`): Data structure where we store
+
+    Args:
+
+        ds (xarray.Dataset): Directly a dataset with the expected structured. This
+         arg is specially thought for loading data from disk
+
+    Notes:
+        Depending on the shape of `edge` the following unstructured elements can
+        be created:
+
+        - cells NDArray[(Any, 0), IntX] or NDArray[(Any, 1), IntX] -> *Point cloud*.
+          E.g. Outcrop scan with lidar
+        - cells NDArray[(Any, 2), IntX] -> *Lines*. E.g. Borehole
+        - cells NDArray[(Any, 3), IntX] -> *Mesh*. E.g surface-DEM Topography
+        - cells NDArray[(Any, 4), IntX]
+           - -> *tetrahedron*
+           - -> *quadrilateral (or tetragon)* UNSUPPORTED?
+        - cells NDArray[(Any, 8), IntX] -> *Hexahedron: Unstructured grid/Prisms*
+    """
+
+    def __post_init__(self):
+        self._validate()
+
+    def __repr__(self):
+        return self.data.__repr__()
+
+    @classmethod
+    def from_raw_data(cls, raw_data: RawDataUnstructured,
+                      coords: Mapping[Hashable, Any] = None,
+                      xarray_attributes: Mapping[Hashable, Any] = None,
+                      default_cells_attributes_name: str = "cell_attrs",
+                      default_points_attributes_name: str = "vertex_attrs"
+                      ):
+        return cls.from_array(raw_data.vertex, raw_data.cells, raw_data.cells_attr, raw_data.vertex_attr, coords,
+                              xarray_attributes, default_cells_attributes_name, default_points_attributes_name)
+
+    @classmethod
+    def from_array(
+            cls,
+            vertex: np.ndarray,
+            cells: Union[np.ndarray, Literal["lines", "points"]],
+            cells_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None,
+            vertex_attr: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None,
+            coords: Mapping[Hashable, Any] = None,
+            xarray_attributes: Mapping[Hashable, Any] = None,
+            default_cells_attr_name: str = "cell_attrs",
+            default_points_attr_name: str = "vertex_attrs",
+            attributes: Union[None, pd.DataFrame, Dict[str, xr.DataArray]] = None  # TODO Obsolete
+    ):
+        """ Constructor of UnstructuredData from arrays or pandas DataFrames.
+
+        Args:
+            vertex (np.ndarray): NDArray[(Any, 3), FloatX]: XYZ point data
+            cells (Union[np.ndarray, Literal["lines", "points"]]): NDArray[(Any, ...), IntX]:
+             Combination of vertex that create different geometric elements. If
+             str use default values for either points or lines
+            cells_attr (Union[None, pd.DataFrame, Dict[str, xr.DataArray]]]: Number associated to an element
+            vertex_attr (Union[None, pd.DataFrame, Dict[str, xr.DataArray]]]: Number
+             associated to points
+            coords:
+            xarray_attributes:
+            attributes:
+            default_cells_attr_name:
+            default_points_attr_name:
+
+        Returns:
+
+        """
+        if attributes is not None:
+            cells_attr = attributes
+
+        cells_data_array, n_cells, n_vertex, vertex_data_array = cls.vertex_and_cells_arrays_to_data_array(cells,
+                                                                                                           vertex)
+        points_attributes_xarray_dict = cls.raw_attributes_to_dict_data_arrays(
+            default_attributes_name=default_points_attr_name,
+            n_items=n_vertex,
+            dims=["points", "vertex_attr"],
+            raw_attributes=vertex_attr
+        )
+
+        cells_attributes_xarray_dict = cls.raw_attributes_to_dict_data_arrays(
+            default_attributes_name=default_cells_attr_name,
+            n_items=n_cells,
+            dims=["cell", "cell_attr"],
+            raw_attributes=cells_attr
+        )
+
+        xarray_dict = {
+            "vertex": vertex_data_array,
+            "cells" : cells_data_array,
+            **cells_attributes_xarray_dict,
+            **points_attributes_xarray_dict
+        }
+
+        default_cells_attr_name = cells_attributes_xarray_dict.get(None, next(iter(cells_attributes_xarray_dict)))
+        default_points_attr_name = points_attributes_xarray_dict.get(None, next(iter(points_attributes_xarray_dict)))
+
+        return cls.from_data_arrays_dict(
+            xarray_dict=xarray_dict,
+            coords=coords,
+            xarray_attributes=xarray_attributes,
+            default_cells_attributes_name=default_cells_attr_name,
+            default_points_attributes_name=default_points_attr_name
+        )
+
+    @classmethod
+    def from_data_arrays_dict(cls, xarray_dict: Dict[str, xr.DataArray],
+                              coords: Mapping[Hashable, Any] = None,
+                              xarray_attributes: Mapping[Hashable, Any] = None,
+                              default_cells_attributes_name="cell_attrs",
+                              default_points_attributes_name="vertex_attrs"):
+
+        # TODO: xr.Dataset seems to have been changed with 2022.06. needs to be adapted for indexing
+        ds = xr.Dataset(xarray_dict, coords=coords, attrs=xarray_attributes)
+
+        # Try to unstack pandas dataframe if exist
+        # TODO: This is an issue in wells. If it is only there maybe we should move it there
+        try:
+            ds = ds.reset_index('cell')
+        except (KeyError, ValueError) as e:
+            print(f"{e} xarray dataset must include 'cell' key (KeyError) or xarray 'cell' has no index (ValueError).")
+
+        return cls(ds, default_cells_attributes_name, default_points_attributes_name)
+
+    @classmethod
+    def raw_attributes_to_dict_data_arrays(
+            cls, default_attributes_name: str, n_items: int, dims: List[str],
+            raw_attributes: Union[None, pd.DataFrame, Dict[str, xr.DataArray]]) \
+            -> Dict[str, xr.DataArray]:
+
+        if raw_attributes is None or type(raw_attributes) == pd.DataFrame:
+            points_attributes_xarray_dict = {
+                default_attributes_name: cls.data_array_attributes_from_raw_data(raw_attributes, dims, n_items)
+            }
+        else:
+            points_attributes_xarray_dict = raw_attributes
+        return points_attributes_xarray_dict
+
+    @classmethod
+    def vertex_and_cells_arrays_to_data_array(cls, cells: Union[np.ndarray, Literal["lines", "points"]], vertex: np.ndarray):
+        n_vertex = vertex.shape[0]
+        if type(cells) != np.ndarray:
+            cells = cls.create_default_cells_arg(cells, n_vertex)
+        n_cells = cells.shape[0]
+        
+        vertex_data_array = xr.DataArray(
+            data=vertex,
+            dims=['points', 'XYZ'],
+            coords={'XYZ': ['X', 'Y', 'Z']}
+        )
+        cells_data_array = xr.DataArray(cells, dims=['cell', 'nodes'])
+        return cells_data_array, n_cells, n_vertex, vertex_data_array
+
+    @classmethod
+    def data_array_attributes_from_raw_data(cls, raw_data: Union[None, pd.DataFrame],
+                                            dims: List[str], n_rows: int) -> xr.DataArray:
+        if raw_data is None:
+            raw_data = pd.DataFrame(np.zeros((n_rows, 0)))
+
+        if type(raw_data) is pd.DataFrame:
+            data_array = xr.DataArray(raw_data, dims=dims)
+        else:
+            raise ValueError("cells_attributes must be either pd.DataFrame or " "None/default.")
+        return data_array
+
+    @classmethod
+    def create_default_cells_arg(cls, cells: Literal["points", "lines"], n_vertex: int) -> np.ndarray:
+        if cells is None or cells == 'points':
+            cells = np.arange(0, n_vertex).reshape(-1, 1)
+        elif cells == 'lines':
+            a = np.arange(0, n_vertex - 1, dtype=np.int_)
+            b = np.arange(1, n_vertex, dtype=np.int_)
+            cells = np.vstack([a, b]).T
+        elif type(cells) != np.ndarray:
+            raise ValueError("cells must be either None (will default to 'points'),"
+                             "'points', 'lines' or a 2D ndarray.")
+        return cells
+
+    def _validate(self):
+        try:
+            _ = self.data[self.cells_attr_name]['cell']
+            _ = self.data[self.cells_attr_name]['cell_attr']
+        except KeyError:
+            raise KeyError('Cell attribute DataArrays must contain dimension cell and cell_attr')
+        try:
+            _ = self.data[self.vertex_attr_name]['vertex_attr']
+            _ = self.data[self.vertex_attr_name]['points']
+        except KeyError:
+            raise KeyError('Point attribute DataArrays must contain dimensions points and vertex_attr.')
+
+        # Make sure the number of vertices matches the associated data.
+        if self.data['cells']['cell'].size != self.data[self.cells_attr_name]['cell'].size:
+            raise AttributeError('Attributes and cells must have the same length.')
+
+        if self.n_points != self.data[self.vertex_attr_name]['points'].size:
+            raise AttributeError('points_attributes and vertex must have the same length.')
+
+    @property
+    def vertex(self) -> np.ndarray:
+        return self.data['vertex'].values
+
+    @property
+    def cells(self):
+        return self.data['cells'].values
+
+    @property
+    def attributes(self) -> pd.DataFrame:
+        xarray = self.data[self.cells_attr_name]
+        return xarray.to_dataframe()[self.cells_attr_name].unstack(level=1)
+
+    @attributes.setter
+    def attributes(self, dataframe):
+        self.data[self.cells_attr_name] = xr.DataArray(dataframe, dims=['element', 'cell_attr'])
+
+    @property
+    def points_attributes(self):
+        return self.data[self.vertex_attr_name].to_dataframe()[
+            self.vertex_attr_name].unstack(level=1)
+
+    @points_attributes.setter
+    def points_attributes(self, dataframe: pd.DataFrame):
+        vertex_attr: xr.DataArray = self.data[self.vertex_attr_name] 
+        vertex_attr.values = dataframe.values
+
+    @property
+    def n_elements(self):
+        return self.cells.shape[0]
+
+    @property
+    def n_vertex_per_element(self):
+        return self.cells.shape[1]
+
+    @property
+    def n_points(self):
+        return self.vertex.shape[0]
+
+    @property
+    def attributes_to_dict(self, orient='list'):
+        return self.attributes.to_dict(orient)
+
+    @property
+    def points_attributes_to_dict(self, orient='list'):
+        return self.points_attributes.to_dict(orient)
+
+    @property
+    def extent(self):
+        max = self.vertex.max(axis=0)
+        min = self.vertex.min(axis=0)
+        extent = np.stack((min, max), axis=1).ravel()
+        return extent
+
+    def to_xarray(self):
+        a = xr.DataArray(self.vertex, dims=['points', 'XYZ'])
+        b = xr.DataArray(self.cells, dims=['cells', 'node'])
+        e = xr.DataArray(self.attributes, dims=['element', 'cell_attr'])
+        c = xr.Dataset({'v': a, 'e': b, 'a': e})
+        return c
+
+    def to_binary(self, order='F'):
+        bytearray_le = self._to_bytearray(order)
+        header = self._set_binary_header()
+
+        return bytearray_le, header
+
+    def _set_binary_header(self):
+
+        header = {
+            "vertex_shape"     : self.vertex.shape,
+            "cell_shape"       : self.cells.shape,
+            "cell_attr_shape"  : self.attributes.shape,
+            "vertex_attr_shape": self.points_attributes.shape,
+            "cell_attr_names"  : self.attributes.columns.to_list(),
+            "cell_attr_types"  : self.attributes.dtypes.astype(str).to_list(),
+            "vertex_attr_names": self.points_attributes.columns.to_list(),
+            "vertex_attr_types": self.attributes.dtypes.astype(str).to_list(),
+            "xarray_attrs"     : self.data.attrs
+        }
+        return header
+
+    def _to_bytearray(self, order):
+        vertex = self.vertex.astype('float32').tobytes(order)
+        cells = self.cells.astype('int32').tobytes(order)
+        cell_attribute = self.attributes.values.astype('float32').tobytes(order)
+        vertex_attribute = self.points_attributes.values.astype('float32').tobytes(order)
+        bytearray_le = vertex + cells + cell_attribute + vertex_attribute
+        return bytearray_le
```

### Comparing `subsurface-0.2.9/subsurface/structs/structured_elements.py` & `subsurface-2024.1.0/subsurface/structs/structured_elements.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/common.py` & `subsurface-2024.1.0/subsurface/writer/to_rex/common.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/data_struct.py` & `subsurface-2024.1.0/subsurface/writer/to_rex/data_struct.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/doc/rex-spec-v1.md` & `subsurface-2024.1.0/subsurface/writer/to_rex/doc/rex-spec-v1.md`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/doc/right-handed.png` & `subsurface-2024.1.0/subsurface/writer/to_rex/doc/right-handed.png`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/doc/sketchup_example.jpg` & `subsurface-2024.1.0/subsurface/writer/to_rex/doc/sketchup_example.jpg`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/gempy_to_rexfile.py` & `subsurface-2024.1.0/subsurface/writer/to_rex/gempy_to_rexfile.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/material_encoder.py` & `subsurface-2024.1.0/subsurface/writer/to_rex/material_encoder.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/mesh_encoder.py` & `subsurface-2024.1.0/subsurface/writer/to_rex/mesh_encoder.py`

 * *Files identical despite different names*

### Comparing `subsurface-0.2.9/subsurface/writer/to_rex/to_rex.py` & `subsurface-2024.1.0/subsurface/writer/to_rex/to_rex.py`

 * *Files identical despite different names*

