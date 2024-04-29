# Comparing `tmp/moraine-0.6.1.tar.gz` & `tmp/moraine-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moraine-0.6.1.tar", last modified: Mon Apr 29 03:02:13 2024, max compression
+gzip compressed data, was "moraine-0.6.2.tar", last modified: Mon Apr 29 03:57:28 2024, max compression
```

## Comparing `moraine-0.6.1.tar` & `moraine-0.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.870034 moraine-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 03:01:16.000000 moraine-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 03:01:16.000000 moraine-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:02:13.870034 moraine-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 03:01:16.000000 moraine-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.866034 moraine-0.6.1/moraine/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.870034 moraine-0.6.1/moraine/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/co.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/shp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/co.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/coord_.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/rtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/shp.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/utils_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.870034 moraine-0.6.1/moraine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:02:11.000000 moraine-0.6.1/moraine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-29 03:01:16.000000 moraine-0.6.1/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:02:13.870034 moraine-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 03:01:16.000000 moraine-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.504676 moraine-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 03:56:33.000000 moraine-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 03:56:33.000000 moraine-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:57:28.500676 moraine-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 03:56:33.000000 moraine-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.500676 moraine-0.6.2/moraine/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.500676 moraine-0.6.2/moraine/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/coord_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.500676 moraine-0.6.2/moraine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:57:26.000000 moraine-0.6.2/moraine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 03:56:33.000000 moraine-0.6.2/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:57:28.504676 moraine-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 03:56:33.000000 moraine-0.6.2/setup.py
```

### Comparing `moraine-0.6.1/LICENSE` & `moraine-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/PKG-INFO` & `moraine-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.6.1
+Version: 0.6.2
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moraine-0.6.1/README.md` & `moraine-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/_modidx.py` & `moraine-0.6.2/moraine/_modidx.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/co.py` & `moraine-0.6.2/moraine/cli/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/load.py` & `moraine-0.6.2/moraine/cli/load.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/logging.py` & `moraine-0.6.2/moraine/cli/logging.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/math.py` & `moraine-0.6.2/moraine/cli/math.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/pc.py` & `moraine-0.6.2/moraine/cli/pc.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/pl.py` & `moraine-0.6.2/moraine/cli/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/plot.py` & `moraine-0.6.2/moraine/cli/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/ps.py` & `moraine-0.6.2/moraine/cli/ps.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/shp.py` & `moraine-0.6.2/moraine/cli/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/cli/transform.py` & `moraine-0.6.2/moraine/cli/transform.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/co.py` & `moraine-0.6.2/moraine/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/coord_.py` & `moraine-0.6.2/moraine/coord_.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/pc.py` & `moraine-0.6.2/moraine/pc.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/pl.py` & `moraine-0.6.2/moraine/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/plot.py` & `moraine-0.6.2/moraine/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/ps.py` & `moraine-0.6.2/moraine/ps.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/rtree.py` & `moraine-0.6.2/moraine/rtree.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine/shp.py` & `moraine-0.6.2/moraine/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/moraine.egg-info/PKG-INFO` & `moraine-0.6.2/moraine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.6.1
+Version: 0.6.2
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moraine-0.6.1/moraine.egg-info/SOURCES.txt` & `moraine-0.6.2/moraine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moraine-0.6.1/settings.ini` & `moraine-0.6.2/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = moraine
 lib_name = moraine
-version = 0.6.1
+version = 0.6.2
 min_python = 3.10
 license = gpl3
 doc_path = _docs
 lib_path = moraine
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,15 +21,15 @@
 author_email = kanglcn@gmail.com
 copyright = 2022-2024, Kang Liang
 description = Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 keywords = InSAR PS DS CUDA Deep-learning
 language = English
 status = 3
 user = kanglcn
-requirements = numpy scipy matplotlib zarr dask colorcet fastcore toml numba>=0.59 numexpr bokeh>=3.4.1 holoviews>=1.18.3 datashader pyproj>=3.0 numcodecs spatialpandas cupy-cuda11x>=13.0 dask[complete]
+requirements = numpy scipy matplotlib zarr dask colorcet fastcore toml numba>=0.59 numexpr bokeh>=3.4.1 holoviews>=1.18.3 datashader pyproj>=3.0 numcodecs spatialpandas dask[complete]
 dev_requirements = nbdev pre-commit quarto
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
```

### Comparing `moraine-0.6.1/setup.py` & `moraine-0.6.2/setup.py`

 * *Files identical despite different names*

