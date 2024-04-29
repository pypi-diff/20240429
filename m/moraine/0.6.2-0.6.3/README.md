# Comparing `tmp/moraine-0.6.2.tar.gz` & `tmp/moraine-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moraine-0.6.2.tar", last modified: Mon Apr 29 03:57:28 2024, max compression
+gzip compressed data, was "moraine-0.6.3.tar", last modified: Mon Apr 29 04:17:13 2024, max compression
```

## Comparing `moraine-0.6.2.tar` & `moraine-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.504676 moraine-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 03:56:33.000000 moraine-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 03:56:33.000000 moraine-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:57:28.500676 moraine-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 03:56:33.000000 moraine-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.500676 moraine-0.6.2/moraine/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.500676 moraine-0.6.2/moraine/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/co.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/shp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/cli/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/co.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/coord_.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/rtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/shp.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 03:56:33.000000 moraine-0.6.2/moraine/utils_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:57:28.500676 moraine-0.6.2/moraine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:57:26.000000 moraine-0.6.2/moraine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 03:57:28.000000 moraine-0.6.2/moraine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 03:56:33.000000 moraine-0.6.2/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:57:28.504676 moraine-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 03:56:33.000000 moraine-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 04:16:19.000000 moraine-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 04:16:19.000000 moraine-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 04:17:13.121941 moraine-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 04:16:19.000000 moraine-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/moraine/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/moraine/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/coord_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/moraine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:17:11.000000 moraine-0.6.3/moraine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 04:16:19.000000 moraine-0.6.3/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:17:13.121941 moraine-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 04:16:19.000000 moraine-0.6.3/setup.py
```

### Comparing `moraine-0.6.2/LICENSE` & `moraine-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/PKG-INFO` & `moraine-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.6.2
+Version: 0.6.3
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moraine-0.6.2/README.md` & `moraine-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/_modidx.py` & `moraine-0.6.3/moraine/_modidx.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/co.py` & `moraine-0.6.3/moraine/cli/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/load.py` & `moraine-0.6.3/moraine/cli/load.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/logging.py` & `moraine-0.6.3/moraine/cli/logging.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/math.py` & `moraine-0.6.3/moraine/cli/math.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/pc.py` & `moraine-0.6.3/moraine/cli/pc.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/pl.py` & `moraine-0.6.3/moraine/cli/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/plot.py` & `moraine-0.6.3/moraine/cli/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/ps.py` & `moraine-0.6.3/moraine/cli/ps.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/shp.py` & `moraine-0.6.3/moraine/cli/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/cli/transform.py` & `moraine-0.6.3/moraine/cli/transform.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/co.py` & `moraine-0.6.3/moraine/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/coord_.py` & `moraine-0.6.3/moraine/coord_.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/pc.py` & `moraine-0.6.3/moraine/pc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/API/pc.ipynb.
 
 # %% auto 0
 __all__ = ['pc2ras', 'pc_hix', 'pc_sort', 'pc_union', 'pc_intersect', 'pc_diff']
 
 # %% ../nbs/API/pc.ipynb 7
 import numpy as np
-from typing import Union
 from numba import prange
 import math
 try:
     import cupy as cp
     from cupy._sorting.search import _exists_kernel
 except:
     pass
 from .utils_ import ngjit, ngpjit
 from .coord_ import Coord
 
 # %% ../nbs/API/pc.ipynb 9
-def pc2ras(gix:Union[np.ndarray,cp.ndarray], # gix array
-           pc_data:Union[np.ndarray,cp.ndarray], # data, 1D or more
+def pc2ras(gix:np.ndarray|cp.ndarray, # gix array
+           pc_data:np.ndarray|cp.ndarray, # data, 1D or more
            shape:tuple, # image shape
           ):
     '''convert point cloud data to original raster, filled with nan'''
     xp = cp.get_array_module(pc_data)
     raster = xp.empty((*shape,*pc_data.shape[1:]),dtype=pc_data.dtype)
     raster[:] = xp.nan
     raster[gix[0],gix[1]] = pc_data
     return raster
 
 # %% ../nbs/API/pc.ipynb 11
-def _ras_dims(gix1:Union[np.ndarray,cp.ndarray], # int array, grid index of the first point cloud
-              gix2:Union[np.ndarray,cp.ndarray]=None, # int array, grid index of the second point cloud
+def _ras_dims(gix1:np.ndarray|cp.ndarray, # int array, grid index of the first point cloud
+              gix2:np.ndarray|cp.ndarray=None, # int array, grid index of the second point cloud
              )->tuple: # the shape of the original raster image
     '''Get the shape of the original raster image from two index, the shape could be smaller than the truth but it doesn't matter.'''
     xp = cp.get_array_module(gix1)
     if gix2 is None:
         dims_az = gix1[0,-1]+1
         dims_r = int(xp.max(gix1[1,:]))+1
     else:
@@ -184,30 +183,30 @@
     coord = Coord(x0,dx,nx,y0,dy,ny)
     gix = coord.coords2gixs([y,x])
     hix = _distances_from_coordinates(coord.p,gix)
     assert len(np.unique(hix)) == len(hix), "`hix` includes duplicated element. Probably `bbox` is too small or `interval` is too big." 
     return hix
 
 # %% ../nbs/API/pc.ipynb 19
-def pc_sort(idx:Union[np.ndarray,cp.ndarray], # unsorted `gix` (2D) or `hix`(1D)
-           )->Union[np.ndarray,cp.ndarray]: # indices that sort input
+def pc_sort(idx:np.ndarray|cp.ndarray, # unsorted `gix` (2D) or `hix`(1D)
+           )->np.ndarray|cp.ndarray: # indices that sort input
     '''Get the indices that sort the input.'''
     xp = cp.get_array_module(idx)
     if idx.ndim == 2:
         dims_az = int(xp.max(idx[0,:]))+1
         dims_r = int(xp.max(idx[1,:]))+1
         idx_1d = xp.ravel_multi_index(idx,dims=(dims_az,dims_r))
     else:
         idx_1d = idx
     key = xp.argsort(idx_1d,kind='stable')
     return key
 
 # %% ../nbs/API/pc.ipynb 23
-def pc_union(idx1:Union[np.ndarray,cp.ndarray], # int array, grid index or hillbert index of the first point cloud
-             idx2:Union[np.ndarray,cp.ndarray], # int array, grid index or hillbert index of the second point cloud
+def pc_union(idx1:np.ndarray|cp.ndarray, # int array, grid index or hillbert index of the first point cloud
+             idx2:np.ndarray|cp.ndarray, # int array, grid index or hillbert index of the second point cloud
              # the union index `idx`; index of the point in output union index that originally in the first point cloud `inv_iidx`;
              # index of the point in output union index that only exist in the second point cloud `inv_iidx2`;
              # index of the point in the second input index that are not in the first input point cloud
             )->tuple: 
     '''Get the union of two point cloud dataset. For points at their intersection, pc_data1 rather than pc_data2 is copied to the result pc_data.'''
     # this function is modified from np.unique
 
@@ -244,16 +243,16 @@
         idx = xp.stack(xp.unravel_index(idx_1d,dims)).astype(idx1.dtype)
     else:
         idx = idx_1d
 
     return idx, inv_iidx[:n1], inv_iidx[n1:], *xp.where(mask2)
 
 # %% ../nbs/API/pc.ipynb 32
-def pc_intersect(idx1:Union[np.ndarray,cp.ndarray], # int array, grid index or hillbert index of the first point cloud
-                 idx2:Union[np.ndarray,cp.ndarray], # int array, grid index or hillbert index of the second point cloud
+def pc_intersect(idx1:np.ndarray|cp.ndarray, # int array, grid index or hillbert index of the first point cloud
+                 idx2:np.ndarray|cp.ndarray, # int array, grid index or hillbert index of the second point cloud
                  # the intersect index `idx`,
                  # index of the point in first point cloud index that also exist in the second point cloud,
                  # index of the point in second point cloud index that also exist in the first point cloud
                 )->tuple:
     '''Get the intersection of two point cloud dataset.'''
     # Here I do not write the core function by myself since cupy have a different implementation of intersect1d
 
@@ -267,16 +266,16 @@
 
     idx, iidx1, iidx2 = xp.intersect1d(idx1_1d,idx2_1d,assume_unique=True,return_indices=True)
     if idx1.ndim == 2:
         idx = xp.stack(xp.unravel_index(idx,dims)).astype(idx1.dtype)
     return idx, iidx1, iidx2
 
 # %% ../nbs/API/pc.ipynb 35
-def pc_diff(idx1:Union[np.ndarray,cp.ndarray], # int array, grid index or hillbert index of the first point cloud
-            idx2:Union[np.ndarray,cp.ndarray], # int array, grid index or hillbert index of the second point cloud
+def pc_diff(idx1:np.ndarray|cp.ndarray, # int array, grid index or hillbert index of the first point cloud
+            idx2:np.ndarray|cp.ndarray, # int array, grid index or hillbert index of the second point cloud
             # the diff index `idx`,
             # index of the point in first point cloud index that do not exist in the second point cloud,
            )->tuple:
     '''Get the point cloud in `idx1` that are not in `idx2`.'''
     xp = cp.get_array_module(idx1)
     if idx1.ndim == 2:
         dims = _ras_dims(idx1,idx2)
```

### Comparing `moraine-0.6.2/moraine/pl.py` & `moraine-0.6.3/moraine/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/plot.py` & `moraine-0.6.3/moraine/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/ps.py` & `moraine-0.6.3/moraine/ps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/API/ps.ipynb.
 
 # %% auto 0
 __all__ = ['amp_disp']
 
 # %% ../nbs/API/ps.ipynb 4
 import numpy as np
-from typing import Union
 import math
 import numba
 try:
     import cupy as cp
 except:
     pass
 
@@ -55,16 +54,16 @@
     nlines,width,nimages = rmli.shape
     amp_disp = cp.empty((nlines,width),dtype=cp.float32)
     _amp_disp_kernel(rmli,cp.int32(nlines),cp.int32(width),cp.int32(nimages),
                      amp_disp,size=nlines*width,block_size=128)
     return amp_disp
 
 # %% ../nbs/API/ps.ipynb 8
-def amp_disp(rslc:Union[cp.ndarray,np.ndarray], # rslc stack
-            )-> Union[cp.ndarray,np.ndarray]: # dispersion index
+def amp_disp(rslc:cp.ndarray|np.ndarray, # rslc stack
+            )-> cp.ndarray|np.ndarray: # dispersion index
     '''calculation the amplitude dispersion index from SLC stack.'''
     xp = cp.get_array_module(rslc)
     if xp is np:
         return _amp_disp_numba(rslc)
     elif xp is cp:
         return _amp_disp_cp(rslc)
     else:
```

### Comparing `moraine-0.6.2/moraine/rtree.py` & `moraine-0.6.3/moraine/rtree.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine/shp.py` & `moraine-0.6.3/moraine/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/moraine.egg-info/PKG-INFO` & `moraine-0.6.3/moraine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.6.2
+Version: 0.6.3
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moraine-0.6.2/moraine.egg-info/SOURCES.txt` & `moraine-0.6.3/moraine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moraine-0.6.2/settings.ini` & `moraine-0.6.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = moraine
 lib_name = moraine
-version = 0.6.2
+version = 0.6.3
 min_python = 3.10
 license = gpl3
 doc_path = _docs
 lib_path = moraine
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `moraine-0.6.2/setup.py` & `moraine-0.6.3/setup.py`

 * *Files identical despite different names*

