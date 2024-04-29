# Comparing `tmp/moraine-0.6.3.tar.gz` & `tmp/moraine-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moraine-0.6.3.tar", last modified: Mon Apr 29 04:17:13 2024, max compression
+gzip compressed data, was "moraine-0.6.4.tar", last modified: Mon Apr 29 04:27:45 2024, max compression
```

## Comparing `moraine-0.6.3.tar` & `moraine-0.6.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 04:16:19.000000 moraine-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 04:16:19.000000 moraine-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 04:17:13.121941 moraine-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 04:16:19.000000 moraine-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/moraine/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/moraine/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/co.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/shp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/cli/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/co.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/coord_.py
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/rtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/shp.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 04:16:19.000000 moraine-0.6.3/moraine/utils_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:13.121941 moraine-0.6.3/moraine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:17:11.000000 moraine-0.6.3/moraine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 04:17:13.000000 moraine-0.6.3/moraine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 04:16:19.000000 moraine-0.6.3/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:17:13.121941 moraine-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 04:16:19.000000 moraine-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:27:45.289956 moraine-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-04-29 04:26:50.000000 moraine-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 04:26:50.000000 moraine-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 04:27:45.289956 moraine-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-29 04:26:50.000000 moraine-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:27:45.289956 moraine-0.6.4/moraine/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:27:45.289956 moraine-0.6.4/moraine/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/cli/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/coord_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 04:26:50.000000 moraine-0.6.4/moraine/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:27:45.289956 moraine-0.6.4/moraine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-29 04:27:45.000000 moraine-0.6.4/moraine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 04:27:45.000000 moraine-0.6.4/moraine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:27:45.000000 moraine-0.6.4/moraine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 04:27:45.000000 moraine-0.6.4/moraine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:27:43.000000 moraine-0.6.4/moraine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 04:27:45.000000 moraine-0.6.4/moraine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 04:27:45.000000 moraine-0.6.4/moraine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 04:26:50.000000 moraine-0.6.4/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:27:45.289956 moraine-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-29 04:26:50.000000 moraine-0.6.4/setup.py
```

### Comparing `moraine-0.6.3/LICENSE` & `moraine-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/PKG-INFO` & `moraine-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.6.3
+Version: 0.6.4
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moraine-0.6.3/README.md` & `moraine-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/_modidx.py` & `moraine-0.6.4/moraine/_modidx.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/co.py` & `moraine-0.6.4/moraine/cli/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/load.py` & `moraine-0.6.4/moraine/cli/load.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/logging.py` & `moraine-0.6.4/moraine/cli/logging.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/math.py` & `moraine-0.6.4/moraine/cli/math.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/pc.py` & `moraine-0.6.4/moraine/cli/pc.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/pl.py` & `moraine-0.6.4/moraine/cli/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/plot.py` & `moraine-0.6.4/moraine/cli/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/ps.py` & `moraine-0.6.4/moraine/cli/ps.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/shp.py` & `moraine-0.6.4/moraine/cli/shp.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/cli/transform.py` & `moraine-0.6.4/moraine/cli/transform.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/co.py` & `moraine-0.6.4/moraine/co.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/coord_.py` & `moraine-0.6.4/moraine/coord_.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/pc.py` & `moraine-0.6.4/moraine/pc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 # %% ../nbs/API/pc.ipynb 7
 import numpy as np
 from numba import prange
 import math
 try:
     import cupy as cp
-    from cupy._sorting.search import _exists_kernel
 except:
-    pass
+    cp = None
 from .utils_ import ngjit, ngpjit
 from .coord_ import Coord
 
 # %% ../nbs/API/pc.ipynb 9
 def pc2ras(gix:np.ndarray|cp.ndarray, # gix array
            pc_data:np.ndarray|cp.ndarray, # data, 1D or more
            shape:tuple, # image shape
```

### Comparing `moraine-0.6.3/moraine/pl.py` & `moraine-0.6.4/moraine/pl.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/plot.py` & `moraine-0.6.4/moraine/plot.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/ps.py` & `moraine-0.6.4/moraine/ps.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # %% ../nbs/API/ps.ipynb 4
 import numpy as np
 import math
 import numba
 try:
     import cupy as cp
 except:
-    pass
+    cp = None
 
 # %% ../nbs/API/ps.ipynb 5
 @numba.jit(nopython=True, cache=True,parallel=True)
 def _amp_disp_numba(rslc):
     epsilon = np.float32(1e-30)
     nlines, width = rslc.shape[:-1]
     amp_disp = np.empty((nlines,width),dtype=np.float32)
```

### Comparing `moraine-0.6.3/moraine/rtree.py` & `moraine-0.6.4/moraine/rtree.py`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/moraine/shp.py` & `moraine-0.6.4/moraine/shp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # %% auto 0
 __all__ = ['ks_test']
 
 # %% ../nbs/API/shp.ipynb 4
 try:
     import cupy as cp
 except:
-    pass
+    cp = None
 import math
 
 # %% ../nbs/API/shp.ipynb 6
 # It looks cupy do not support pointer to pointer: float** rmli_stack
 # These code are modified from https://dev.thep.lu.se/yat under GPLv3 license.
 _ks_test_kernel = cp.ElementwiseKernel(
     'raw T rmli_stack, int32 nlines, int32 width, int32 nimages, int32 az_half_win, int32 r_half_win',
```

### Comparing `moraine-0.6.3/moraine.egg-info/PKG-INFO` & `moraine-0.6.4/moraine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moraine
-Version: 0.6.3
+Version: 0.6.4
 Summary: Modern Radar Interferometry Environment, A simple, stupid InSAR postprocessing tool in big data era
 Home-page: https://github.com/kanglcn/moraine
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA Deep-learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moraine-0.6.3/moraine.egg-info/SOURCES.txt` & `moraine-0.6.4/moraine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moraine-0.6.3/settings.ini` & `moraine-0.6.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = moraine
 lib_name = moraine
-version = 0.6.3
+version = 0.6.4
 min_python = 3.10
 license = gpl3
 doc_path = _docs
 lib_path = moraine
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `moraine-0.6.3/setup.py` & `moraine-0.6.4/setup.py`

 * *Files identical despite different names*

