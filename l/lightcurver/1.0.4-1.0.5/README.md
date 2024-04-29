# Comparing `tmp/lightcurver-1.0.4.tar.gz` & `tmp/lightcurver-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurver-1.0.4.tar", last modified: Mon Apr  1 18:13:20 2024, max compression
+gzip compressed data, was "lightcurver-1.0.5.tar", last modified: Mon Apr 29 15:28:04 2024, max compression
```

## Comparing `lightcurver-1.0.4.tar` & `lightcurver-1.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.158257 lightcurver-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 18:13:11.000000 lightcurver-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-01 18:13:20.158257 lightcurver-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-01 18:13:11.000000 lightcurver-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.150257 lightcurver-1.0.4/lightcurver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.150257 lightcurver-1.0.4/lightcurver/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/pipeline_dependency_graph.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/state_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/task_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/workflow_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.154257 lightcurver-1.0.4/lightcurver/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/footprint_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/image_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/normalization_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/psf_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/sources_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/star_photometry_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.154257 lightcurver-1.0.4/lightcurver/processes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/alternate_plate_solving_with_gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/background_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/cutout_making.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/frame_characterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/frame_importation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/frame_star_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/normalization_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/plate_solving.py
--rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/psf_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/roi_deconv_file_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/roi_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/star_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/star_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/star_querying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.154257 lightcurver-1.0.4/lightcurver/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/user_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/user_header_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.158257 lightcurver-1.0.4/lightcurver/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/chi2_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/lightcurves_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/star_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/starred_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/zeropoint_from_gaia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.158257 lightcurver-1.0.4/lightcurver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 18:13:11.000000 lightcurver-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:13:20.158257 lightcurver-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.972880 lightcurver-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 15:27:55.000000 lightcurver-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-29 15:28:04.972880 lightcurver-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-29 15:27:55.000000 lightcurver-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.964880 lightcurver-1.0.5/lightcurver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.964880 lightcurver-1.0.5/lightcurver/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/pipeline_dependency_graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/state_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/task_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/workflow_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.964880 lightcurver-1.0.5/lightcurver/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/footprint_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/image_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/normalization_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/psf_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/sources_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/star_photometry_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.968880 lightcurver-1.0.5/lightcurver/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/alternate_plate_solving_with_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/background_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/cutout_making.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/frame_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/frame_importation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/frame_star_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/normalization_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/plate_solving.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/psf_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/roi_deconv_file_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/roi_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/star_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/star_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/star_querying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.968880 lightcurver-1.0.5/lightcurver/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/user_header_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.972880 lightcurver-1.0.5/lightcurver/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/chi2_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/lightcurves_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/star_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/starred_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/zeropoint_from_gaia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.972880 lightcurver-1.0.5/lightcurver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-29 15:27:55.000000 lightcurver-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:28:04.972880 lightcurver-1.0.5/setup.cfg
```

### Comparing `lightcurver-1.0.4/LICENSE` & `lightcurver-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/PKG-INFO` & `lightcurver-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.4
+Version: 1.0.5
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 Requires-Dist: scipy
 Requires-Dist: ephem
 Requires-Dist: pandas
 Requires-Dist: shapely
 Requires-Dist: astroquery
 Requires-Dist: h5py
 Requires-Dist: astroscrappy
-Requires-Dist: starred-astro
+Requires-Dist: starred-astro>=1.4.1
 Requires-Dist: pytest
 Requires-Dist: dill
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxopt
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `lightcurver-1.0.4/README.md` & `lightcurver-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/pipeline/pipeline_dependency_graph.yaml` & `lightcurver-1.0.5/lightcurver/pipeline/pipeline_dependency_graph.yaml`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/pipeline/state_checkers.py` & `lightcurver-1.0.5/lightcurver/pipeline/state_checkers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/pipeline/task_wrappers.py` & `lightcurver-1.0.5/lightcurver/pipeline/task_wrappers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/pipeline/workflow_manager.py` & `lightcurver-1.0.5/lightcurver/pipeline/workflow_manager.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/plotting/footprint_plotting.py` & `lightcurver-1.0.5/lightcurver/plotting/footprint_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/plotting/image_plotting.py` & `lightcurver-1.0.5/lightcurver/plotting/image_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/plotting/normalization_plotting.py` & `lightcurver-1.0.5/lightcurver/plotting/normalization_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/plotting/psf_plotting.py` & `lightcurver-1.0.5/lightcurver/plotting/psf_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/plotting/sources_plotting.py` & `lightcurver-1.0.5/lightcurver/plotting/sources_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/plotting/star_photometry_plotting.py` & `lightcurver-1.0.5/lightcurver/plotting/star_photometry_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/alternate_plate_solving_with_gaia.py` & `lightcurver-1.0.5/lightcurver/processes/alternate_plate_solving_with_gaia.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,16 @@
     Returns:
         Nothing, but loops over the frames and updates database and fits headers.
 
     """
     user_config = get_user_config()
     ra, dec = user_config['ROI_ra_deg'], user_config['ROI_dec_deg']
     center_radius = {'center': (ra, dec), 'radius':  user_config['alternate_plate_solve_gaia_radius']/3600.}
-    gaia_stars = find_gaia_stars('circle', center_radius=center_radius)
+    gaia_stars = find_gaia_stars('circle', center_radius=center_radius,
+                                 gaia_provider=user_config['gaia_provider'])
     gaia_stars['pmra'][np.isnan(gaia_stars['pmra'])] = 0
     gaia_stars['pmdec'][np.isnan(gaia_stars['pmdec'])] = 0
     gaia_coords = SkyCoord(ra=gaia_stars['ra'],
                            dec=gaia_stars['dec'],
                            pm_ra_cosdec=gaia_stars['pmra'],
                            pm_dec=gaia_stars['pmdec'],
                            frame='icrs',
```

### Comparing `lightcurver-1.0.4/lightcurver/processes/background_estimation.py` & `lightcurver-1.0.5/lightcurver/processes/background_estimation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/cutout_making.py` & `lightcurver-1.0.5/lightcurver/processes/cutout_making.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/frame_characterization.py` & `lightcurver-1.0.5/lightcurver/processes/frame_characterization.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/frame_importation.py` & `lightcurver-1.0.5/lightcurver/processes/frame_importation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/frame_star_assignment.py` & `lightcurver-1.0.5/lightcurver/processes/frame_star_assignment.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/normalization_calculation.py` & `lightcurver-1.0.5/lightcurver/processes/normalization_calculation.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,19 @@
                             conditions=['plate_solved = 1', 'eliminated = 0', 'roi_in_footprint = 1'])
     combined_footprint_hash = get_combined_footprint_hash(user_config, frames_ini['id'].to_list())
 
     fluxes_fit_chi2_min, fluxes_fit_chi2_max = get_chi2_bounds(psf_or_fluxes='fluxes')
     df = get_fluxes(combined_footprint_hash=combined_footprint_hash,
                     photometry_chi2_min=fluxes_fit_chi2_min,
                     photometry_chi2_max=fluxes_fit_chi2_max)
+    stars_to_use = user_config['stars_to_use_norm']
+
+    if type(stars_to_use) is list:
+        df = df[df['name'].isin(stars_to_use)]
+
     logger.info(f"Calculating a normalization coefficient using {len(df)} flux measurements.")
     # 1. normalize by median in each star -- get a 'norm' of each frame for each individual star.
     median_flux_per_star = df.groupby('star_gaia_id')['flux'].median().rename('median_flux')
     df2 = df.merge(median_flux_per_star, on='star_gaia_id')
     df2['normalized_flux'] = df2['flux'] / df2['median_flux']
     df2['normalized_d_flux'] = df2['d_flux'] / df2['median_flux']
```

### Comparing `lightcurver-1.0.4/lightcurver/processes/plate_solving.py` & `lightcurver-1.0.5/lightcurver/processes/plate_solving.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/psf_modelling.py` & `lightcurver-1.0.5/lightcurver/processes/psf_modelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,16 @@
 
         # we set the initial guess for the position of the star to the center (guess_method thing)
         # because we are confident that is where the star will be (plate solving + gaia proper motions)
         result = build_psf(datas, noisemaps, subsampling_factor=user_config['subsampling_factor'],
                            n_iter_analytic=user_config['psf_n_iter_analytic'],
                            n_iter_adabelief=user_config['psf_n_iter_pixels'],
                            masks=masks,
-                           guess_method_star_position='center')
+                           guess_method_star_position='center', 
+                           guess_fwhm_pixels=frame['seeing_pixels'])
         psf_plots_dir = user_config['plots_dir'] / 'PSFs' / str(combined_footprint_hash)
         psf_plots_dir.mkdir(exist_ok=True, parents=True)
         frame_name = Path(frame['image_relpath']).stem
         seeing = frame['seeing_pixels'] * frame['pixel_scale']
         loss_history = result['adabelief_extra_fields']['loss_history']
         plot_psf_diagnostic(datas=datas, noisemaps=noisemaps, residuals=result['residuals'],
                             full_psf=result['full_psf'],
```

### Comparing `lightcurver-1.0.4/lightcurver/processes/roi_deconv_file_preparation.py` & `lightcurver-1.0.5/lightcurver/processes/roi_deconv_file_preparation.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 
 from ..structure.database import get_pandas, execute_sqlite_query
 from ..utilities.footprint import get_combined_footprint_hash
 from ..utilities.chi2_selector import get_chi2_bounds
 from ..structure.user_config import get_user_config
 
 
-def get_frames_for_roi(combined_footprint_hash, psf_fit_chi2_min, psf_fit_chi2_max, **constraints_on_frame_columns_dict):
+def get_frames_for_roi(combined_footprint_hash, psf_fit_chi2_min, psf_fit_chi2_max,
+                       constraints_on_frame_columns_dict, constraints_on_normalization_coeff_dict):
     """
     Retrieves frames and associated PSFs (built with stars of the given footprint)
     provided that those frames have a PSF with a chi2 between psf_fit_chi2_min and psf_fit_chi2_max.
     Optionally, can filter to include only frames without a flux measurement.
 
     :param combined_footprint_hash: int, the hash of the combined footprint we are processing.
     :param psf_fit_chi2_min: The minimum acceptable chi2 value for the PSF fit.
     :param psf_fit_chi2_max: The maximum acceptable chi2 value for the PSF fit.
     :param constraints_on_frame_columns_dict: a dictionary, with keys identical to that of the frames table and values
                                               intervals of allowed values. E.g., {'seeing_arcseconds': (0, 1.1), ...}
+    :param constraints_on_normalization_coeff_dict: a dictionary, with keys identical to the columns of the
+                                                    normalization_coefficients table columns, and values same as
+                                                    argument constraints_on_frame_columns_dict.
     :return: A pandas dataframe of frames and associated PSFs that meet the criteria.
     """
     query = """
     SELECT f.*, ps.*, nc.*
     FROM frames f
     JOIN PSFs ps ON f.id = ps.frame_id 
     JOIN normalization_coefficients nc ON f.id = nc.frame_id AND nc.combined_footprint_hash = ps.combined_footprint_hash
@@ -34,14 +38,22 @@
     params = [combined_footprint_hash, psf_fit_chi2_min, psf_fit_chi2_max]
 
     # append constraints based on the provided constraints
     for column, (min_val, max_val) in constraints_on_frame_columns_dict.items():
         query += f" AND f.{column} BETWEEN ? AND ?"
         params.extend([min_val, max_val])
 
+    # also append constraints on the normalization coefficient
+    for column, (min_val, max_val) in constraints_on_normalization_coeff_dict.items():
+        query += f" AND nc.{column} BETWEEN ? AND ?"
+        params.extend([min_val, max_val])
+
+    # and order by mjd ...
+    query += " ORDER BY f.mjd"
+
     return execute_sqlite_query(query, tuple(params), is_select=True, use_pandas=True)
 
 
 def fetch_and_adjust_zeropoints(combined_footprint_hash):
     """
     Just a helper function.
     We query our normalization coefficients and zeropoints.
@@ -107,18 +119,20 @@
     frames_ini = get_pandas(columns=['id'],
                             conditions=['plate_solved = 1', 'eliminated = 0', 'roi_in_footprint = 1'])
     combined_footprint_hash = get_combined_footprint_hash(user_config, frames_ini['id'].to_list())
 
     psf_fit_chi2_min, psf_fit_chi2_max = get_chi2_bounds(psf_or_fluxes='psf')
 
     roi_constraints = user_config['constraints_on_frame_columns_for_roi']
+    norm_constraints = user_config['constraints_on_normalization_coeff']
     frames = get_frames_for_roi(combined_footprint_hash=combined_footprint_hash,
                                 psf_fit_chi2_min=psf_fit_chi2_min,
                                 psf_fit_chi2_max=psf_fit_chi2_max,
-                                **roi_constraints)
+                                constraints_on_frame_columns_dict=roi_constraints,
+                                constraints_on_normalization_coeff_dict=norm_constraints)
     # ok, this frames database has everything: the PSF to use, the norm coeff, etc.
     logger.info(f'Preparing calibrated cutouts of the ROI from {len(frames)} frames.')
     # so, just like when we did photometry of stars, build the data for deconvolution
     with h5py.File(user_config['regions_path'], 'r') as h5f:
         data = []
         noisemap = []
         mask = []
```

### Comparing `lightcurver-1.0.4/lightcurver/processes/roi_modelling.py` & `lightcurver-1.0.5/lightcurver/processes/roi_modelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     # prepare for the random rotations of the pointing ...
     kwargs_init['kwargs_analytic']['alpha'] = angles_to_north
     kwargs_fixed['kwargs_analytic']['alpha'] = angles_to_north
     # if we provide a background:
     if user_config['starting_background'] is not None:
         bck_path = Path(user_config['starting_background'])
         if not bck_path.is_absolute():
-            bck_path = user_config['work_dir'] / bck_path
+            bck_path = user_config['workdir'] / bck_path
         if bck_path.name.endswith('fits'):
             bck = fits.getdata(bck_path)
         else:
             bck = np.load(bck_path)
         h = bck.flatten() / scale
         kwargs_init['kwargs_background']['h'] = h
         kwargs_fixed['kwargs_background']['h'] = h
@@ -196,14 +196,15 @@
                                   kwargs_down=kwargs_down)
 
     loss = Loss(data, model, parameters, noisemap**2,
                 regularization_terms='l1_starlet',
                 regularization_strength_scales=1,
                 regularization_strength_hf=1.,
                 regularization_strength_positivity=100.,
+                regularization_strength_pts_source=0.01,
                 W=W)
 
     optim = Optimizer(loss, parameters, method='adabelief')
     optimiser_optax_option = {
         'max_iterations': user_config['roi_deconv_all_iters'],
         'init_learning_rate': 1e-4, 'schedule_learning_rate': False,
         'restart_from_init': False, 'stop_at_loss_increase': False,
```

### Comparing `lightcurver-1.0.4/lightcurver/processes/star_extraction.py` & `lightcurver-1.0.5/lightcurver/processes/star_extraction.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/star_photometry.py` & `lightcurver-1.0.5/lightcurver/processes/star_photometry.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/processes/star_querying.py` & `lightcurver-1.0.5/lightcurver/processes/star_querying.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,18 @@
         radius = user_config['ROI_disk_radius_arcseconds'] / 3600.0
         region_type = 'circle'
         query_footprint = {'center': center, 'radius': radius}
     else:
         raise RuntimeError("Not an agreed upon strategy for star selection:", user_config['star_selection_strategy'])
 
     kwargs_query = {
-        'release': 'dr3',
         'astrometric_excess_noise_max': user_config['star_max_astrometric_excess_noise'],
         'gmag_range': (user_config['star_min_gmag'], user_config['star_max_gmag']),
-        'max_phot_g_mean_flux_error': user_config['star_max_phot_g_mean_flux_error']
+        'min_phot_g_mean_flux_over_error': user_config['min_phot_g_mean_flux_over_error'],
+        'gaia_provider': user_config['gaia_provider']
     }
     logging.info(f'Querying stars with the following parameters: {kwargs_query}')
 
     stars_table = find_gaia_stars(region_type, query_footprint, **kwargs_query)
 
     message = f"Too few stars compared to the config criterion! Only {len(stars_table)} stars available."
     enough_stars = len(stars_table) >= user_config['min_number_stars']
```

### Comparing `lightcurver-1.0.4/lightcurver/structure/database.py` & `lightcurver-1.0.5/lightcurver/structure/database.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/structure/user_config.py` & `lightcurver-1.0.5/lightcurver/structure/user_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,8 +50,14 @@
     # star names: make it a list if user defined a string.
     # e.g. stars_to_use = 'abcd' --> ['a', 'b', 'c', 'd']
     if type(config['stars_to_use_psf']) is str:
         config['stars_to_use_psf'] = [c for c in config['stars_to_use_psf']]
     if type(config['stars_to_use_norm']) is str:
         config['stars_to_use_norm'] = [c for c in config['stars_to_use_norm']]
 
+    # constraints on ROI cutout prep:
+    if 'constraints_on_frame_columns_for_roi' not in config:
+        config['constraints_on_frame_columns_for_roi'] = {}
+    if 'constraints_on_normalization_coeff' not in config:
+        config['constraints_on_normalization_coeff'] = {}
+
     return config
```

### Comparing `lightcurver-1.0.4/lightcurver/structure/user_header_parser.py` & `lightcurver-1.0.5/lightcurver/structure/user_header_parser.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/utilities/chi2_selector.py` & `lightcurver-1.0.5/lightcurver/utilities/chi2_selector.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/utilities/footprint.py` & `lightcurver-1.0.5/lightcurver/utilities/footprint.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/utilities/lightcurves_postprocessing.py` & `lightcurver-1.0.5/lightcurver/utilities/lightcurves_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/utilities/star_naming.py` & `lightcurver-1.0.5/lightcurver/utilities/star_naming.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/utilities/starred_utilities.py` & `lightcurver-1.0.5/lightcurver/utilities/starred_utilities.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver/utilities/zeropoint_from_gaia.py` & `lightcurver-1.0.5/lightcurver/utilities/zeropoint_from_gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/lightcurver.egg-info/PKG-INFO` & `lightcurver-1.0.5/lightcurver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.4
+Version: 1.0.5
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 Requires-Dist: scipy
 Requires-Dist: ephem
 Requires-Dist: pandas
 Requires-Dist: shapely
 Requires-Dist: astroquery
 Requires-Dist: h5py
 Requires-Dist: astroscrappy
-Requires-Dist: starred-astro
+Requires-Dist: starred-astro>=1.4.1
 Requires-Dist: pytest
 Requires-Dist: dill
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxopt
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `lightcurver-1.0.4/lightcurver.egg-info/SOURCES.txt` & `lightcurver-1.0.5/lightcurver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.4/pyproject.toml` & `lightcurver-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.6.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightcurver"
-version = "1.0.4"
+version = "1.0.5"
 authors = [{ name = "Frédéric Dux", email = "duxfrederic@gmail.com" }]
 description = "A thorough structure for precise photometry and deconvolution of time series of wide field images."
 readme = "README.md"
 keywords = ["photometry", "astronomy", "deconvolution", "PSF", "pipeline"]  
 classifiers = [] 
 dependencies = [
     "pyyaml",
@@ -19,15 +19,15 @@
     "scipy",
     "ephem",
     "pandas",
     "shapely",
     "astroquery",
     "h5py",
     "astroscrappy",
-    "starred-astro", 
+    "starred-astro >= 1.4.1", 
     "pytest",
     "dill",
     "jax",
     "jaxlib",
     "jaxopt",
     "matplotlib",
     "numpy",
```

