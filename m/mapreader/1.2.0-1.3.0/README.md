# Comparing `tmp/mapreader-1.2.0.tar.gz` & `tmp/mapreader-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.2.0.tar", last modified: Wed Apr 10 09:44:51 2024, max compression
+gzip compressed data, was "mapreader-1.3.0.tar", last modified: Mon Apr 29 15:18:33 2024, max compression
```

## Comparing `mapreader-1.2.0.tar` & `mapreader-1.3.0.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.129624 mapreader-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 09:44:44.000000 mapreader-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-10 09:44:51.129624 mapreader-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-10 09:44:44.000000 mapreader-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.129624 mapreader-1.2.0/mapreader/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 09:44:51.129624 mapreader-1.2.0/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.121624 mapreader-1.2.0/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/annotate/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75056 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    98833 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/process/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:44:50.000000 mapreader-1.2.0/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 09:44:51.129624 mapreader-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-10 09:44:44.000000 mapreader-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_geo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-04-10 09:44:44.000000 mapreader-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.779410 mapreader-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-29 15:18:26.000000 mapreader-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-29 15:18:33.779410 mapreader-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-29 15:18:26.000000 mapreader-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.779410 mapreader-1.3.0/mapreader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 15:18:33.779410 mapreader-1.3.0/mapreader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.771410 mapreader-1.3.0/mapreader/annotate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/annotate/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/annotate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.771410 mapreader-1.3.0/mapreader/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75056 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.771410 mapreader-1.3.0/mapreader/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/tile_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/download/tile_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98834 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/process/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/process/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/spot_text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/spot_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/spot_text/deepsolo_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/spot_text/dptext_detr_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-29 15:18:26.000000 mapreader-1.3.0/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/mapreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 15:18:33.000000 mapreader-1.3.0/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 15:18:33.779410 mapreader-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-29 15:18:26.000000 mapreader-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:18:33.775410 mapreader-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_geo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-04-29 15:18:26.000000 mapreader-1.3.0/tests/test_sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-04-29 15:18:26.000000 mapreader-1.3.0/versioneer.py
```

### Comparing `mapreader-1.2.0/LICENSE` & `mapreader-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/PKG-INFO` & `mapreader-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.2.0
+Version: 1.3.0
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.2.0 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.3.0 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `mapreader-1.2.0/README.md` & `mapreader-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/__init__.py` & `mapreader-1.3.0/mapreader/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 
 from mapreader.classify.load_annotations import AnnotationsLoader
 from mapreader.classify.datasets import PatchDataset
 from mapreader.classify.datasets import PatchContextDataset
 from mapreader.classify.classifier import ClassifierContainer
 from mapreader.classify import custom_models
 
+try:
+    from mapreader.spot_text.deepsolo_runner import DeepSoloRunner
+except ImportError:
+    pass
+
+try:
+    from mapreader.spot_text.dptext_detr_runner import DPTextDETRRunner
+except ImportError:
+    pass
+
 from mapreader.process import process
 
 from mapreader.annotate.annotator import Annotator
 
 from . import _version
 
 __version__ = _version.get_versions()["version"]
```

### Comparing `mapreader-1.2.0/mapreader/annotate/annotator.py` & `mapreader-1.3.0/mapreader/annotate/annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/annotate/utils.py` & `mapreader-1.3.0/mapreader/annotate/utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/classify/classifier.py` & `mapreader-1.3.0/mapreader/classify/classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/classify/custom_models.py` & `mapreader-1.3.0/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/classify/datasets.py` & `mapreader-1.3.0/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/classify/load_annotations.py` & `mapreader-1.3.0/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/download/data_structures.py` & `mapreader-1.3.0/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/download/downloader.py` & `mapreader-1.3.0/mapreader/download/downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/download/downloader_utils.py` & `mapreader-1.3.0/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/download/sheet_downloader.py` & `mapreader-1.3.0/mapreader/download/sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/download/tile_loading.py` & `mapreader-1.3.0/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/download/tile_merging.py` & `mapreader-1.3.0/mapreader/download/tile_merging.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/load/geo_utils.py` & `mapreader-1.3.0/mapreader/load/geo_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/load/images.py` & `mapreader-1.3.0/mapreader/load/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -1749,15 +1749,15 @@
                     self._create_kml(
                         kml_out_path=kml_out_path,
                         column_to_plot=column_to_plot,
                         coords=self.parents[image_id]["coordinates"],
                         counter=-1,
                     )
 
-                ax.set_title(image_id)
+                ax.set_title(parent_id)
                 figures.append(fig)
 
                 if column_to_plot and plot_histogram:
                     self._hist_values_array(column_to_plot, values_array)
 
             return figures
```

### Comparing `mapreader-1.2.0/mapreader/load/loader.py` & `mapreader-1.3.0/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/process/post_process.py` & `mapreader-1.3.0/mapreader/process/post_process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/process/process.py` & `mapreader-1.3.0/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.3.0/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader/utils/slice_parallel.py` & `mapreader-1.3.0/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/mapreader.egg-info/PKG-INFO` & `mapreader-1.3.0/mapreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.2.0
+Version: 1.3.0
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.2.0 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.3.0 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `mapreader-1.2.0/mapreader.egg-info/SOURCES.txt` & `mapreader-1.3.0/mapreader.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 mapreader/load/__init__.py
 mapreader/load/geo_utils.py
 mapreader/load/images.py
 mapreader/load/loader.py
 mapreader/process/__init__.py
 mapreader/process/post_process.py
 mapreader/process/process.py
+mapreader/spot_text/__init__.py
+mapreader/spot_text/deepsolo_runner.py
+mapreader/spot_text/dptext_detr_runner.py
 mapreader/utils/__init__.py
 mapreader/utils/compute_and_save_stats.py
 mapreader/utils/slice_parallel.py
 tests/test_annotator.py
 tests/test_geo_pipeline.py
 tests/test_import.py
 tests/test_post_processing.py
```

### Comparing `mapreader-1.2.0/mapreader.egg-info/requires.txt` & `mapreader-1.3.0/mapreader.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/setup.py` & `mapreader-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/tests/test_annotator.py` & `mapreader-1.3.0/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/tests/test_geo_pipeline.py` & `mapreader-1.3.0/tests/test_geo_pipeline.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/tests/test_post_processing.py` & `mapreader-1.3.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/tests/test_sheet_downloader.py` & `mapreader-1.3.0/tests/test_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.2.0/versioneer.py` & `mapreader-1.3.0/versioneer.py`

 * *Files identical despite different names*

