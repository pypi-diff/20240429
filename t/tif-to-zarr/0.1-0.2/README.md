# Comparing `tmp/tif_to_zarr-0.1.tar.gz` & `tmp/tif_to_zarr-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tif_to_zarr-0.1.tar", last modified: Mon Apr 29 21:05:46 2024, max compression
+gzip compressed data, was "tif_to_zarr-0.2.tar", last modified: Mon Apr 29 21:35:17 2024, max compression
```

## Comparing `tif_to_zarr-0.1.tar` & `tif_to_zarr-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:05:46.925972 tif_to_zarr-0.1/
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1518 2024-04-29 20:35:53.000000 tif_to_zarr-0.1/LICENSE
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1319 2024-04-29 21:05:46.921972 tif_to_zarr-0.1/PKG-INFO
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      924 2024-04-29 20:13:11.000000 tif_to_zarr-0.1/README.md
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      516 2024-04-29 20:13:11.000000 tif_to_zarr-0.1/pyproject.toml
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)       38 2024-04-29 21:05:46.925972 tif_to_zarr-0.1/setup.cfg
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      717 2024-04-29 21:05:43.000000 tif_to_zarr-0.1/setup.py
-drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:05:46.921972 tif_to_zarr-0.1/tif_to_zarr.egg-info/
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1319 2024-04-29 21:05:46.000000 tif_to_zarr-0.1/tif_to_zarr.egg-info/PKG-INFO
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)      215 2024-04-29 21:05:46.000000 tif_to_zarr-0.1/tif_to_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:05:46.000000 tif_to_zarr-0.1/tif_to_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)       45 2024-04-29 21:05:46.000000 tif_to_zarr-0.1/tif_to_zarr.egg-info/requires.txt
--rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:05:46.000000 tif_to_zarr-0.1/tif_to_zarr.egg-info/top_level.txt
+drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1518 2024-04-29 20:35:53.000000 tif_to_zarr-0.2/LICENSE
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1319 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/PKG-INFO
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      924 2024-04-29 20:13:11.000000 tif_to_zarr-0.2/README.md
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      516 2024-04-29 20:13:11.000000 tif_to_zarr-0.2/pyproject.toml
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)       38 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/setup.cfg
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      717 2024-04-29 21:35:14.000000 tif_to_zarr-0.2/setup.py
+drwxr-xr-x   0 zubovy   (65918) cellmap   (1127)        0 2024-04-29 21:35:17.568539 tif_to_zarr-0.2/tif_to_zarr.egg-info/
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)     1319 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)      215 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)       45 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/requires.txt
+-rw-r--r--   0 zubovy   (65918) cellmap   (1127)        1 2024-04-29 21:35:17.000000 tif_to_zarr-0.2/tif_to_zarr.egg-info/top_level.txt
```

### Comparing `tif_to_zarr-0.1/LICENSE` & `tif_to_zarr-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.1/PKG-INFO` & `tif_to_zarr-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tif_to_zarr
-Version: 0.1
+Version: 0.2
 Summary: Simple package to convert small tif files to zarr format.
 Home-page: https://github.com/yuriyzubov/tif-to-zarr.git
 Author: Yurii Zubov
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: imagecodecs
 Requires-Dist: click
```

### Comparing `tif_to_zarr-0.1/README.md` & `tif_to_zarr-0.2/README.md`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.1/pyproject.toml` & `tif_to_zarr-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tif_to_zarr-0.1/setup.py` & `tif_to_zarr-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_directory, 'README.md'),
           encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tif_to_zarr',
-    version=0.1,
+    version=0.2,
     url='https://github.com/yuriyzubov/tif-to-zarr.git',
     author='Yurii Zubov',
     description='Simple package to convert small tif files to zarr format.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tif_to_zarr-0.1/tif_to_zarr.egg-info/PKG-INFO` & `tif_to_zarr-0.2/tif_to_zarr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tif_to_zarr
-Version: 0.1
+Version: 0.2
 Summary: Simple package to convert small tif files to zarr format.
 Home-page: https://github.com/yuriyzubov/tif-to-zarr.git
 Author: Yurii Zubov
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: imagecodecs
 Requires-Dist: click
```

