# Comparing `tmp/gempy_viewer-2024.1.1.tar.gz` & `tmp/gempy_viewer-2024.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy_viewer-2024.1.1.tar", last modified: Mon Apr 15 11:30:45 2024, max compression
+gzip compressed data, was "gempy_viewer-2024.1.2.tar", last modified: Mon Apr 29 09:07:50 2024, max compression
```

## Comparing `gempy_viewer-2024.1.1.tar` & `gempy_viewer-2024.1.2.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3101 2023-06-19 10:17:18.000000 gempy_viewer-2024.1.1/.gitignore
--rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.1/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.1/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)      854 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1484 2023-07-26 10:50:13.000000 gempy_viewer-2024.1.1/README.md
--rw-r--r--   0 leguark   (1000) leguark   (1000)        6 2023-09-14 06:30:21.000000 gempy_viewer-2024.1.1/dev-requirements.txt
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.043536 gempy_viewer-2024.1.1/gempy_viewer/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer/API/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      296 2023-11-21 15:15:11.000000 gempy_viewer-2024.1.1/gempy_viewer/API/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10875 2023-10-10 11:45:51.000000 gempy_viewer-2024.1.1/gempy_viewer/API/_plot_2d_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7959 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/API/_plot_2d_sections_api.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6119 2023-11-21 15:10:45.000000 gempy_viewer-2024.1.1/gempy_viewer/API/_plot_3d_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3638 2023-11-21 16:20:52.000000 gempy_viewer-2024.1.1/gempy_viewer/API/_plot_others.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer/DEP/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:59:27.000000 gempy_viewer-2024.1.1/gempy_viewer/DEP/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    14538 2023-06-22 11:01:14.000000 gempy_viewer-2024.1.1/gempy_viewer/DEP/_plot.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    54327 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.1/gempy_viewer/DEP/_visualization_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4308 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.1/gempy_viewer/DEP/decorators.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    60969 2024-04-05 08:55:37.000000 gempy_viewer-2024.1.1/gempy_viewer/DEP/visualization_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      397 2024-04-12 12:54:09.000000 gempy_viewer-2024.1.1/gempy_viewer/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-04-15 11:30:45.000000 gempy_viewer-2024.1.1/gempy_viewer/_version.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer/core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:53:54.000000 gempy_viewer-2024.1.1/gempy_viewer/core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1976 2023-09-27 08:52:01.000000 gempy_viewer-2024.1.1/gempy_viewer/core/data_to_show.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      479 2023-07-10 13:33:23.000000 gempy_viewer-2024.1.1/gempy_viewer/core/plotting_2d_options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      301 2023-07-26 12:29:31.000000 gempy_viewer-2024.1.1/gempy_viewer/core/scalar_data_type.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      496 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.1/gempy_viewer/core/section_data_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      380 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.1/gempy_viewer/core/slicer_data.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer/modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:05.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:45.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3921 2023-08-02 09:19:49.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_contours_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8783 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_input_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2807 2023-12-05 14:47:00.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2983 2023-08-22 13:43:39.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4905 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_topography_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      764 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_traces_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      847 2023-11-08 11:53:57.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/helpers.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7313 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/multi_axis_manager.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5067 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/plot_2d_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12753 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/plot_utils_DEP.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4242 2023-10-09 13:35:04.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/visualization_2d.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:58.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    42120 2023-07-28 08:27:07.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/_vista.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4352 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_input_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5800 2024-04-12 12:58:30.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1321 2023-11-21 15:13:49.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3055 2023-11-21 15:14:27.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_topography_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1715 2023-09-08 13:45:29.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/plot_3d_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4569 2023-11-21 15:08:41.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/vista.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2523 2023-06-22 11:38:56.000000 gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/vista_qt.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      932 2023-11-21 16:16:36.000000 gempy_viewer-2024.1.1/gempy_viewer/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/gempy_viewer.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      854 2024-04-15 11:30:45.000000 gempy_viewer-2024.1.1/gempy_viewer.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2132 2024-04-15 11:30:45.000000 gempy_viewer-2024.1.1/gempy_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-15 11:30:45.000000 gempy_viewer-2024.1.1/gempy_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-09 07:38:51.000000 gempy_viewer-2024.1.1/gempy_viewer.egg-info/not-zip-safe
--rw-r--r--   0 leguark   (1000) leguark   (1000)       83 2024-04-15 11:30:45.000000 gempy_viewer-2024.1.1/gempy_viewer.egg-info/requires.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2024-04-15 11:30:45.000000 gempy_viewer-2024.1.1/gempy_viewer.egg-info/top_level.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       48 2023-11-21 12:41:34.000000 gempy_viewer-2024.1.1/optional_requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       36 2023-11-21 12:41:34.000000 gempy_viewer-2024.1.1/requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1337 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.1/setup.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:53:13.000000 gempy_viewer-2024.1.1/tests/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2313 2023-10-11 08:49:21.000000 gempy_viewer-2024.1.1/tests/conftest.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-15 11:30:45.053536 gempy_viewer-2024.1.1/tests/test_plotting/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.1/tests/test_plotting/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7826 2024-04-12 12:56:44.000000 gempy_viewer-2024.1.1/tests/test_plotting/test_plot_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2715 2023-08-04 09:08:59.000000 gempy_viewer-2024.1.1/tests/test_plotting/test_plot_3d.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3101 2023-06-19 10:17:18.000000 gempy_viewer-2024.1.2/.gitignore
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.2/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.2/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      852 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1484 2023-07-26 10:50:13.000000 gempy_viewer-2024.1.2/README.md
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/API/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      348 2024-04-24 08:21:05.000000 gempy_viewer-2024.1.2/gempy_viewer/API/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10875 2023-10-10 11:45:51.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7959 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_sections_api.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6119 2023-11-21 15:10:45.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_3d_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1295 2024-04-25 08:23:03.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_LiquidEarth.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3638 2023-11-21 16:20:52.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_others.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/DEP/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:59:27.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    14538 2023-06-22 11:01:14.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/_plot.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    54327 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/_visualization_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4308 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/decorators.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    60928 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/visualization_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      397 2024-04-12 12:54:09.000000 gempy_viewer-2024.1.2/gempy_viewer/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer/_version.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:53:54.000000 gempy_viewer-2024.1.2/gempy_viewer/core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1976 2023-09-27 08:52:01.000000 gempy_viewer-2024.1.2/gempy_viewer/core/data_to_show.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      479 2023-07-10 13:33:23.000000 gempy_viewer-2024.1.2/gempy_viewer/core/plotting_2d_options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      301 2023-07-26 12:29:31.000000 gempy_viewer-2024.1.2/gempy_viewer/core/scalar_data_type.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      496 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.2/gempy_viewer/core/section_data_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      380 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.2/gempy_viewer/core/slicer_data.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:05.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:45.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3921 2023-08-02 09:19:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_contours_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8783 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_input_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2807 2023-12-05 14:47:00.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2983 2023-08-22 13:43:39.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4905 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_topography_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      764 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_traces_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      847 2023-11-08 11:53:57.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/helpers.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7313 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/multi_axis_manager.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5067 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_2d_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12753 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_utils_DEP.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4242 2023-10-09 13:35:04.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/visualization_2d.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:58.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    42075 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/_vista.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4352 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_input_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5800 2024-04-12 12:58:30.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1321 2023-11-21 15:13:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3000 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_topography_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1715 2023-09-08 13:45:29.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/plot_3d_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4520 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2523 2023-06-22 11:38:56.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista_qt.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1150 2024-04-24 08:21:06.000000 gempy_viewer-2024.1.2/gempy_viewer/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/gempy_viewer.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      852 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2209 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       81 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/requirements/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        6 2023-09-14 06:30:21.000000 gempy_viewer-2024.1.2/requirements/dev-requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       50 2024-04-29 09:05:44.000000 gempy_viewer-2024.1.2/requirements/optional_requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       34 2024-04-29 09:06:54.000000 gempy_viewer-2024.1.2/requirements/requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2115 2024-04-29 09:05:44.000000 gempy_viewer-2024.1.2/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:53:13.000000 gempy_viewer-2024.1.2/tests/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2313 2023-10-11 08:49:21.000000 gempy_viewer-2024.1.2/tests/conftest.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/tests/test_plotting/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.2/tests/test_plotting/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7826 2024-04-12 12:56:44.000000 gempy_viewer-2024.1.2/tests/test_plotting/test_plot_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2715 2023-08-04 09:08:59.000000 gempy_viewer-2024.1.2/tests/test_plotting/test_plot_3d.py
```

### Comparing `gempy_viewer-2024.1.1/.gitignore` & `gempy_viewer-2024.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/AUTHORS.rst` & `gempy_viewer-2024.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/LICENSE` & `gempy_viewer-2024.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/PKG-INFO` & `gempy_viewer-2024.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gempy_viewer
-Version: 2024.1.1
+Version: 2024.1.2
 Summary: Viewer for the geological modeling package GemPy
 Home-page: 
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
 License: EUPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: gempy>=2023.1.0b0
+Requires-Dist: gempy==2024.1.2
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Provides-Extra: opt
 Requires-Dist: pyvista; extra == "opt"
 Requires-Dist: scipy; extra == "opt"
 Requires-Dist: pooch; extra == "opt"
 Requires-Dist: pandas; extra == "opt"
```

### Comparing `gempy_viewer-2024.1.1/README.md` & `gempy_viewer-2024.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/API/_plot_2d_API.py` & `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_API.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/API/_plot_2d_sections_api.py` & `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_sections_api.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/API/_plot_3d_API.py` & `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_3d_API.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/API/_plot_others.py` & `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_others.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/DEP/_plot.py` & `gempy_viewer-2024.1.2/gempy_viewer/DEP/_plot.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/DEP/_visualization_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/DEP/_visualization_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/DEP/decorators.py` & `gempy_viewer-2024.1.2/gempy_viewer/DEP/decorators.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/DEP/visualization_3d.py` & `gempy_viewer-2024.1.2/gempy_viewer/DEP/visualization_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 
 warnings.filterwarnings("ignore",
                         message='.*Conversion of the second argument of issubdtype *.',
                         append=True)
 try:
     import vtk
-    from vtk.util.numpy_support import numpy_to_vtk
     VTK_IMPORT = True
 except ImportError:
     VTK_IMPORT = False
 
 try:
     import steno3d
     STENO_IMPORT = True
@@ -280,15 +279,15 @@
         Points = vtk.vtkPoints()
         if self.ve != 1:
             vertices[:, 2] = vertices[:, 2] * self.ve
         #     raise NotImplementedError('Vertical exageration for surfaces not implemented yet.')
         # for v in vertices:
         #     v[-1] = self.ve * v[-1]
         #     Points.InsertNextPoint(v)
-        Points.SetData(numpy_to_vtk(vertices))
+        Points.SetData(pv.convert_array(vertices))
 
         return Points
 
     @staticmethod
     def create_surface_triangles(simplices):
         """
         Method to create the Triangles that form the surfaces
@@ -490,15 +489,15 @@
 
         points = vtk.vtkPoints()
         # for v in vertices:
         #     v[-1] = v[-1]
         #     points.InsertNextPoint(v)
         if self.ve !=1:
             vertices[:, 2]= vertices[:, 2]*self.ve
-        points.SetData(numpy_to_vtk(vertices))
+        points.SetData(pv.convert_array(vertices))
 
         # Add the grid points to a polydata object
         polydata = vtk.vtkPolyData()
         polydata.SetPoints(points)
         #
         # glyphFilter = vtk.vtkVertexGlyphFilter()
         # glyphFilter.SetInputData(polydata)
@@ -546,15 +545,15 @@
 
         # Convert hex colors to rgb
         for idx, val in self.geo_model._surfaces.df['color'].iteritems():
             rgb = (255 * np.array(mcolors.hex2color(val)))
             arr_ = np.vstack((arr_, rgb))
 
         sel = np.round(self.geo_model.solutions.geological_map[0]).astype(int)[0]
-        nv = numpy_to_vtk(arr_[sel - 1], array_type=3)
+        nv = pv.convert_array(arr_[sel - 1], array_type=3)
         self._topography_delauny.GetOutput().GetPointData().SetScalars(nv)
 
     def set_surface_points(self, indices=None):
         """
         Create all the surface_points points and set them to the corresponding renders for their posterior visualization
          with render_model
```

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/core/data_to_show.py` & `gempy_viewer-2024.1.2/gempy_viewer/core/data_to_show.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_contours_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_contours_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_input_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_input_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_topography_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_topography_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/drawer_traces_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_traces_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/helpers.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/helpers.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/multi_axis_manager.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/multi_axis_manager.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/plot_2d_utils.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_2d_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/plot_utils_DEP.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_utils_DEP.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_2d/visualization_2d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/visualization_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/_vista.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/_vista.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     action="ignore",
     message='.*Conversion of the second argument of issubdtype *.',
     append=True
 )
 
 try:
     import vtk
-    from vtk.util.numpy_support import numpy_to_vtk
 
     VTK_IMPORT = True
 except ImportError:
     VTK_IMPORT = False
 
 from logging import debug
 
@@ -422,15 +421,15 @@
             # Convert hex colors to rgb
             for val in list(self._color_lot):
                 rgb = (255 * np.array(mcolors.hex2color(val)))
                 arr_ = np.vstack((arr_, rgb))
 
             sel = np.round(self.model.solutions.geological_map[0]).astype(int)[0]
 
-            scalars_val = numpy_to_vtk(arr_[sel - 1], array_type=3)
+            scalars_val = pv.convert_array(arr_[sel - 1], array_type=3)
             cm = None
             rgb = True
 
         elif scalars == 'topography':
             scalars_val = topography[:, 2]
             cm = 'terrain'
 
@@ -1125,15 +1124,15 @@
             # convert hex colors to rgb
             for val in list(self._get_color_lot(faults=False)):
                 rgb = (255 * np.array(mcolors.hex2color(val)))
                 arr_ = np.vstack((arr_, rgb))
 
             sel = np.round(self.model.solutions.geological_map[0]).astype(int)[0]
 
-            scalars_val = numpy_to_vtk(arr_[sel - 1], array_type=3)
+            scalars_val = pv.convert_array(arr_[sel - 1], array_type=3)
             cm = None
             rgb = True
         elif scalars == "topography":
             scalars_val = topography[:, 2]
             cm = 'terrain'
         elif type(scalars) is np.ndarray:
             scalars_val = scalars
```

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_input_3d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_input_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/drawer_topography_3d.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_topography_3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         solution: Optional[RawArraysSolution],
         topography_scalar_type: TopographyDataType,
         elements_colors: list[str],
         contours=True,
         **kwargs
 ):
     pv = require_pyvista()
-    from vtkmodules.util.numpy_support import numpy_to_vtk
     
     rgb = False
 
     xx, yy = np.meshgrid(topography.y, topography.x)
 
     grid = pv.StructuredGrid(yy, xx, topography.values_2d[:, :, 2])
     polydata = grid.extract_surface()
@@ -39,15 +38,15 @@
         case TopographyDataType.GEOMAP, True:
             colors_hex = elements_colors
             colors_rgb_ = [list(mcolors.hex2color(val)) for val in colors_hex]  # Convert hex to RGB using list comprehension
 
             colors_rgb = np.array(colors_rgb_) * 255  # Multiply by 255 to get RGB values in [0, 255]
             sel = np.round(geological_map).astype(int) - 1
             selected_colors = colors_rgb[sel]  # Use numpy advanced indexing to get the corresponding RGB values
-            scalars_val = numpy_to_vtk(selected_colors, array_type=3)  # Convert to vtk array
+            scalars_val = pv.convert_array(selected_colors, array_type=3)  # Convert to vtk array
 
             cm = mcolors.ListedColormap(elements_colors)
             rgb = True
 
             show_scalar_bar = False
             scalars = 'id'
             clim = (0, len(elements_colors) - 1),
```

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/plot_3d_utils.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/plot_3d_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/vista.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 import matplotlib
 
 warnings.filterwarnings("ignore",
                         message='.*Conversion of the second argument of issubdtype *.',
                         append=True)
 try:
     import vtk
-    from vtk.util.numpy_support import numpy_to_vtk
 
     VTK_IMPORT = True
 except ImportError:
     VTK_IMPORT = False
 
 from gempy_viewer.optional_dependencies import require_pyvista
 
@@ -109,15 +108,15 @@
         self.orientations_actor = None
         self.orientations_mesh = None
         self.orientations_widgets = {}
 
         # Private attributes
         self._grid_values = None
         col = matplotlib.colormaps['viridis'](np.linspace(0, 1, 255)) * 255
-        nv = numpy_to_vtk(col, array_type=3)
+        nv = pv.convert_array(col, array_type=3)
         self._cmaps = {'viridis': nv}
 
         # Topology properties
         self.topo_edges = None
         self.topo_ctrs = None
 
     def set_bounds(self, extent: List[float], **kwargs):
```

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/modules/plot_3d/vista_qt.py` & `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista_qt.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/gempy_viewer/optional_dependencies.py` & `gempy_viewer-2024.1.2/gempy_viewer/optional_dependencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-﻿def require_gempy_plugins():
+﻿def require_liquid_earth_api():
+    try:
+        import liquid_earth_api
+    except ImportError:
+        raise ImportError("The liquid_earth_api package is required to run this function.")
+    return liquid_earth_api
+
+def require_gempy_plugins():
     try:
         import gempy.plugins
     except ImportError:
         raise ImportError("The gempy.plugins package is required to run this function.")
     return gempy.plugins
```

### Comparing `gempy_viewer-2024.1.1/gempy_viewer.egg-info/PKG-INFO` & `gempy_viewer-2024.1.2/gempy_viewer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gempy_viewer
-Version: 2024.1.1
+Version: 2024.1.2
 Summary: Viewer for the geological modeling package GemPy
 Home-page: 
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
 License: EUPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: gempy>=2023.1.0b0
+Requires-Dist: gempy==2024.1.2
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Provides-Extra: opt
 Requires-Dist: pyvista; extra == "opt"
 Requires-Dist: scipy; extra == "opt"
 Requires-Dist: pooch; extra == "opt"
 Requires-Dist: pandas; extra == "opt"
```

### Comparing `gempy_viewer-2024.1.1/gempy_viewer.egg-info/SOURCES.txt` & `gempy_viewer-2024.1.2/gempy_viewer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 .gitignore
 AUTHORS.rst
 LICENSE
 README.md
-dev-requirements.txt
-optional_requirements.txt
-requirements.txt
 setup.py
 gempy_viewer/__init__.py
 gempy_viewer/_version.py
 gempy_viewer/optional_dependencies.py
 gempy_viewer.egg-info/PKG-INFO
 gempy_viewer.egg-info/SOURCES.txt
 gempy_viewer.egg-info/dependency_links.txt
 gempy_viewer.egg-info/not-zip-safe
 gempy_viewer.egg-info/requires.txt
 gempy_viewer.egg-info/top_level.txt
 gempy_viewer/API/__init__.py
 gempy_viewer/API/_plot_2d_API.py
 gempy_viewer/API/_plot_2d_sections_api.py
 gempy_viewer/API/_plot_3d_API.py
+gempy_viewer/API/_plot_LiquidEarth.py
 gempy_viewer/API/_plot_others.py
 gempy_viewer/DEP/__init__.py
 gempy_viewer/DEP/_plot.py
 gempy_viewer/DEP/_visualization_2d.py
 gempy_viewer/DEP/decorators.py
 gempy_viewer/DEP/visualization_3d.py
 gempy_viewer/core/__init__.py
@@ -49,12 +47,15 @@
 gempy_viewer/modules/plot_3d/drawer_input_3d.py
 gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
 gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
 gempy_viewer/modules/plot_3d/drawer_topography_3d.py
 gempy_viewer/modules/plot_3d/plot_3d_utils.py
 gempy_viewer/modules/plot_3d/vista.py
 gempy_viewer/modules/plot_3d/vista_qt.py
+requirements/dev-requirements.txt
+requirements/optional_requirements.txt
+requirements/requirements.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_plotting/__init__.py
 tests/test_plotting/test_plot_2d.py
 tests/test_plotting/test_plot_3d.py
```

### Comparing `gempy_viewer-2024.1.1/tests/conftest.py` & `gempy_viewer-2024.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/tests/test_plotting/test_plot_2d.py` & `gempy_viewer-2024.1.2/tests/test_plotting/test_plot_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.1/tests/test_plotting/test_plot_3d.py` & `gempy_viewer-2024.1.2/tests/test_plotting/test_plot_3d.py`

 * *Files identical despite different names*

