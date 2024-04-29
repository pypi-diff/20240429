# Comparing `tmp/moraine-0.5.1.tar.gz` & `tmp/moraine-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moraine-0.5.1.tar", last modified: Mon Apr 29 02:27:45 2024, max compression
+gzip compressed data, was "moraine-0.6.1.tar", last modified: Mon Apr 29 03:02:13 2024, max compression
```

## Comparing `moraine-0.5.1.tar` & `moraine-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:45.000000 moraine-0.5.1/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    33253 2023-01-13 02:56:44.000000 moraine-0.5.1/LICENSE
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      111 2023-01-13 02:56:44.000000 moraine-0.5.1/MANIFEST.in
--rw-r--r--   0 kangl    (509674) kangl    (509674)     9344 2024-04-29 02:27:45.000000 moraine-0.5.1/PKG-INFO
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     8100 2024-04-29 02:09:02.000000 moraine-0.5.1/README.md
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      191 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/__init__.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    16297 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/_modidx.py
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:45.000000 moraine-0.5.1/moraine/cli/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      402 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/__init__.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     7175 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/co.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    19775 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/load.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2537 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/logging.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2409 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/math.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    26890 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/pc.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     5740 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/pl.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    22427 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/plot.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2758 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/ps.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     7198 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/shp.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2786 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/transform.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     9136 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/co.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     4386 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/coord_.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    12046 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/pc.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     1340 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/pl.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     6731 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/plot.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2065 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/ps.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    13999 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/rtree.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     3362 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/shp.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      444 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/utils_.py
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/
--rw-r--r--   0 kangl    (509674) kangl    (509674)     9344 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/PKG-INFO
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      671 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/SOURCES.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/dependency_links.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       36 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/entry_points.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2024-04-28 00:33:02.000000 moraine-0.5.1/moraine.egg-info/not-zip-safe
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      200 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/requires.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        8 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/top_level.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     1317 2024-04-27 22:49:16.000000 moraine-0.5.1/settings.ini
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       38 2024-04-29 02:27:45.000000 moraine-0.5.1/setup.cfg
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2548 2023-01-13 02:56:44.000000 moraine-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.870034 moraine-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 03:01:16.000000 moraine-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 03:01:16.000000 moraine-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:02:13.870034 moraine-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 03:01:16.000000 moraine-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.866034 moraine-0.6.1/moraine/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.870034 moraine-0.6.1/moraine/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/cli/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/coord_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 03:01:16.000000 moraine-0.6.1/moraine/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:02:13.870034 moraine-0.6.1/moraine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:02:11.000000 moraine-0.6.1/moraine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 03:02:13.000000 moraine-0.6.1/moraine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-29 03:01:16.000000 moraine-0.6.1/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:02:13.870034 moraine-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 03:01:16.000000 moraine-0.6.1/setup.py
```

### Comparing `moraine-0.5.1/LICENSE` & `moraine-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/PKG-INFO` & `moraine-0.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,25 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.5.1
+Version: 0.6.1
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: zarr
-Requires-Dist: dask
-Requires-Dist: colorcet
-Requires-Dist: fastcore
-Requires-Dist: toml
-Requires-Dist: numba>=0.59
-Requires-Dist: numexpr
-Requires-Dist: bokeh>=3.4.1
-Requires-Dist: holoviews>=1.18.3
-Requires-Dist: datashader
-Requires-Dist: pyproj>=3.0
-Requires-Dist: numcodecs
-Requires-Dist: spatialpandas
-Requires-Dist: dask[complete]
 Provides-Extra: dev
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: quarto; extra == "dev"
+License-File: LICENSE
 
 # Moraine
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 > Modern Radar Interferometry Environment; A simple, stupid InSAR
 > postprocessing tool in big data era
@@ -119,21 +99,20 @@
 intended to fill the needs of those contributing to it, rather than
 trying to appeal to as many users as possible. It is targeted at the
 proficient InSAR user, or anyone with a do-it-yourself attitude who is
 willing to read the documentation, and solve their own problems.
 
 All users are encouraged to participate and contribute to this package.
 Reporting bugs and requesting new features by raising a Github
-[issue](https://github.com/kanglcn/decorrelation/issues) is highly
-valued and bugs fixing, documentation improving and features
-implementation by make a Github [pull
-request](https://github.com/kanglcn/decorrelation/pulls) are very
-appreciated. Users can also freely ask questions, provide technical
+[issue](https://github.com/kanglcn/moraine/issues) is highly valued and
+bugs fixing, documentation improving and features implementation by make
+a Github [pull request](https://github.com/kanglcn/moraine/pulls) are
+very appreciated. Users can also freely ask questions, provide technical
 assistance to others or just exchange opinions in the
-[discussions](https://github.com/kanglcn/decorrelation/discussions).
+[discussions](https://github.com/kanglcn/moraine/discussions).
 
 ## Install
 
 Because of GPU driver and CUDA Version Compatibility, there is no simple
 solution for CUDA related packages installation. Users need to
 successfully install
 [cupy](https://docs.cupy.dev/en/stable/install.html#installation) and
```

### Comparing `moraine-0.5.1/README.md` & `moraine-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,21 +80,20 @@
 intended to fill the needs of those contributing to it, rather than
 trying to appeal to as many users as possible. It is targeted at the
 proficient InSAR user, or anyone with a do-it-yourself attitude who is
 willing to read the documentation, and solve their own problems.
 
 All users are encouraged to participate and contribute to this package.
 Reporting bugs and requesting new features by raising a Github
-[issue](https://github.com/kanglcn/decorrelation/issues) is highly
-valued and bugs fixing, documentation improving and features
-implementation by make a Github [pull
-request](https://github.com/kanglcn/decorrelation/pulls) are very
-appreciated. Users can also freely ask questions, provide technical
+[issue](https://github.com/kanglcn/moraine/issues) is highly valued and
+bugs fixing, documentation improving and features implementation by make
+a Github [pull request](https://github.com/kanglcn/moraine/pulls) are
+very appreciated. Users can also freely ask questions, provide technical
 assistance to others or just exchange opinions in the
-[discussions](https://github.com/kanglcn/decorrelation/discussions).
+[discussions](https://github.com/kanglcn/moraine/discussions).
 
 ## Install
 
 Because of GPU driver and CUDA Version Compatibility, there is no simple
 solution for CUDA related packages installation. Users need to
 successfully install
 [cupy](https://docs.cupy.dev/en/stable/install.html#installation) and
```

### Comparing `moraine-0.5.1/moraine/_modidx.py` & `moraine-0.6.1/moraine/_modidx.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/co.py` & `moraine-0.6.1/moraine/cli/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/load.py` & `moraine-0.6.1/moraine/cli/load.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/logging.py` & `moraine-0.6.1/moraine/cli/logging.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/math.py` & `moraine-0.6.1/moraine/cli/math.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/pc.py` & `moraine-0.6.1/moraine/cli/pc.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/pl.py` & `moraine-0.6.1/moraine/cli/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/plot.py` & `moraine-0.6.1/moraine/cli/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/ps.py` & `moraine-0.6.1/moraine/cli/ps.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/shp.py` & `moraine-0.6.1/moraine/cli/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/cli/transform.py` & `moraine-0.6.1/moraine/cli/transform.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/co.py` & `moraine-0.6.1/moraine/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/coord_.py` & `moraine-0.6.1/moraine/coord_.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/pc.py` & `moraine-0.6.1/moraine/pc.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/pl.py` & `moraine-0.6.1/moraine/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/plot.py` & `moraine-0.6.1/moraine/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/ps.py` & `moraine-0.6.1/moraine/ps.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/rtree.py` & `moraine-0.6.1/moraine/rtree.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine/shp.py` & `moraine-0.6.1/moraine/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/moraine.egg-info/PKG-INFO` & `moraine-0.6.1/moraine.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,25 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.5.1
+Version: 0.6.1
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: zarr
-Requires-Dist: dask
-Requires-Dist: colorcet
-Requires-Dist: fastcore
-Requires-Dist: toml
-Requires-Dist: numba>=0.59
-Requires-Dist: numexpr
-Requires-Dist: bokeh>=3.4.1
-Requires-Dist: holoviews>=1.18.3
-Requires-Dist: datashader
-Requires-Dist: pyproj>=3.0
-Requires-Dist: numcodecs
-Requires-Dist: spatialpandas
-Requires-Dist: dask[complete]
 Provides-Extra: dev
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: quarto; extra == "dev"
+License-File: LICENSE
 
 # Moraine
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 > Modern Radar Interferometry Environment; A simple, stupid InSAR
 > postprocessing tool in big data era
@@ -119,21 +99,20 @@
 intended to fill the needs of those contributing to it, rather than
 trying to appeal to as many users as possible. It is targeted at the
 proficient InSAR user, or anyone with a do-it-yourself attitude who is
 willing to read the documentation, and solve their own problems.
 
 All users are encouraged to participate and contribute to this package.
 Reporting bugs and requesting new features by raising a Github
-[issue](https://github.com/kanglcn/decorrelation/issues) is highly
-valued and bugs fixing, documentation improving and features
-implementation by make a Github [pull
-request](https://github.com/kanglcn/decorrelation/pulls) are very
-appreciated. Users can also freely ask questions, provide technical
+[issue](https://github.com/kanglcn/moraine/issues) is highly valued and
+bugs fixing, documentation improving and features implementation by make
+a Github [pull request](https://github.com/kanglcn/moraine/pulls) are
+very appreciated. Users can also freely ask questions, provide technical
 assistance to others or just exchange opinions in the
-[discussions](https://github.com/kanglcn/decorrelation/discussions).
+[discussions](https://github.com/kanglcn/moraine/discussions).
 
 ## Install
 
 Because of GPU driver and CUDA Version Compatibility, there is no simple
 solution for CUDA related packages installation. Users need to
 successfully install
 [cupy](https://docs.cupy.dev/en/stable/install.html#installation) and
```

### Comparing `moraine-0.5.1/moraine.egg-info/SOURCES.txt` & `moraine-0.6.1/moraine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moraine-0.5.1/settings.ini` & `moraine-0.6.1/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = moraine
 lib_name = moraine
-version = 0.5.1
+version = 0.6.1
 min_python = 3.10
 license = gpl3
 doc_path = _docs
 lib_path = moraine
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,17 +21,18 @@
 author_email = kanglcn@gmail.com
 copyright = 2022-2024, Kang Liang
 description = Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 keywords = InSAR PS DS CUDA Deep-learning
 language = English
 status = 3
 user = kanglcn
-requirements = numpy scipy matplotlib zarr dask colorcet fastcore toml numba>=0.59 numexpr bokeh>=3.4.1 holoviews>=1.18.3 datashader pyproj>=3.0 numcodecs spatialpandas dask[complete]
+requirements = numpy scipy matplotlib zarr dask colorcet fastcore toml numba>=0.59 numexpr bokeh>=3.4.1 holoviews>=1.18.3 datashader pyproj>=3.0 numcodecs spatialpandas cupy-cuda11x>=13.0 dask[complete]
 dev_requirements = nbdev pre-commit quarto
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
-label_groups = {"feature":"New Features", "enhancement":"Features improved", "breaking": "Breaking Changes", "bug":"Bugs Squashed", "documentation":"Improvements to documentation", "deprecation":"Features deprecation", "packaging":"(For Developer) Packaging"}
+label_groups = {"feature":"New Features", "enhancement":"Features improved", "breaking": "Breaking Changes", "bug":"Bugs Squashed", "documentation":"Improvements to documentation", "deprecation":"Features deprecation", "packaging":"(For Developer) Packaging"}
+
```

### Comparing `moraine-0.5.1/setup.py` & `moraine-0.6.1/setup.py`

 * *Files identical despite different names*

