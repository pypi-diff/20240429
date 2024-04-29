# Comparing `tmp/bridgescaler-0.6.0.tar.gz` & `tmp/bridgescaler-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgescaler-0.6.0.tar", last modified: Fri Mar 29 23:29:34 2024, max compression
+gzip compressed data, was "bridgescaler-0.7.0.tar", last modified: Mon Apr 29 15:24:43 2024, max compression
```

## Comparing `bridgescaler-0.6.0.tar` & `bridgescaler-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:29:34.094856 bridgescaler-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-03-29 23:29:34.094856 bridgescaler-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:29:34.090856 bridgescaler-0.6.0/bridgescaler/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/bridgescaler/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/bridgescaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/bridgescaler/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/bridgescaler/deep.py
--rw-r--r--   0 runner    (1001) docker     (127)    33492 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/bridgescaler/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/bridgescaler/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:29:34.094856 bridgescaler-0.6.0/bridgescaler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-03-29 23:29:34.000000 bridgescaler-0.6.0/bridgescaler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-29 23:29:34.000000 bridgescaler-0.6.0/bridgescaler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 23:29:34.000000 bridgescaler-0.6.0/bridgescaler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-29 23:29:34.000000 bridgescaler-0.6.0/bridgescaler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 23:29:34.000000 bridgescaler-0.6.0/bridgescaler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 23:29:34.000000 bridgescaler-0.6.0/bridgescaler.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-29 23:29:34.094856 bridgescaler-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 23:29:29.000000 bridgescaler-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:24:43.378943 bridgescaler-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-29 15:24:43.378943 bridgescaler-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:24:43.378943 bridgescaler-0.7.0/bridgescaler/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/bridgescaler/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/bridgescaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/bridgescaler/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/bridgescaler/deep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29210 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/bridgescaler/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/bridgescaler/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:24:43.378943 bridgescaler-0.7.0/bridgescaler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-29 15:24:43.000000 bridgescaler-0.7.0/bridgescaler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-29 15:24:43.000000 bridgescaler-0.7.0/bridgescaler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:24:43.000000 bridgescaler-0.7.0/bridgescaler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 15:24:43.000000 bridgescaler-0.7.0/bridgescaler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 15:24:43.000000 bridgescaler-0.7.0/bridgescaler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:24:43.000000 bridgescaler-0.7.0/bridgescaler.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-29 15:24:43.378943 bridgescaler-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 15:24:38.000000 bridgescaler-0.7.0/setup.py
```

### Comparing `bridgescaler-0.6.0/LICENSE` & `bridgescaler-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bridgescaler-0.6.0/PKG-INFO` & `bridgescaler-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgescaler
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tool to automagically save scikit-learn scaler properties to a portable, readable format.
 Home-page: https://github.com/NCAR/bridgescaler
 Author: David John Gagne
 Author-email: dgagne@ucar.edu
 License: MIT
 Keywords: machine learning
 Platform: any
@@ -18,18 +18,17 @@
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.0
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: crick
 Requires-Dist: scipy
 Requires-Dist: xarray
+Requires-Dist: numba
 Requires-Dist: sphinx
 Requires-Dist: sphinx-book-theme
-Requires-Dist: pytdigest
-Requires-Dist: numba-stats
 
 # bridgescaler
 Bridge your scikit-learn-style scaler parameters between Python sessions and users.
 Bridgescaler allows you to save the properties of a scikit-learn-style scaler object
 to a json file, and then repopulate a new scaler object with the same properties.
```

### Comparing `bridgescaler-0.6.0/README.md` & `bridgescaler-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bridgescaler-0.6.0/bridgescaler/backend.py` & `bridgescaler-0.7.0/bridgescaler/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sklearn.preprocessing import (StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler, QuantileTransformer,
                                    SplineTransformer, PowerTransformer)
 from bridgescaler.group import GroupStandardScaler, GroupRobustScaler, GroupMinMaxScaler
 from bridgescaler.deep import DeepStandardScaler, DeepMinMaxScaler, DeepQuantileTransformer
-from bridgescaler.distributed import DStandardScaler, DMinMaxScaler, DQuantileTransformer, DQuantileScaler
+from bridgescaler.distributed import DStandardScaler, DMinMaxScaler, DQuantileScaler
 import numpy as np
 import json
 import pandas as pd
 from numpy.lib.format import descr_to_dtype, dtype_to_descr
 from base64 import b64decode, b64encode
 from typing import Any
 
@@ -23,15 +23,15 @@
                "GroupMinMaxScaler": GroupMinMaxScaler,
                "DeepStandardScaler": DeepStandardScaler,
                "DeepMinMaxScaler": DeepMinMaxScaler,
                "DeepQuantileTransformer": DeepQuantileTransformer,
                "DStandardScaler": DStandardScaler,
                "DMinMaxScaler": DMinMaxScaler,
                "DQuantileScaler": DQuantileScaler,
-               "DQuantileTransformer": DQuantileTransformer}
+               }
 
 
 def save_scaler(scaler, scaler_file):
     """
     Save a scikit-learn or bridgescaler scaler object to json format.
 
     Args:
@@ -56,15 +56,15 @@
         str representation of object in json format
     """
     scaler_params = scaler.__dict__
     scaler_params["type"] = str(type(scaler))[1:-2].split(".")[-1]
     return json.dumps(scaler_params, indent=4, sort_keys=True, cls=NumpyEncoder)
 
 
-def object_hook(dct: dict[Any, Any]) -> dict[Any, Any] | np.ndarray | np.generic:
+def object_hook(dct: dict[Any, Any]):
     if "__numpy__" in dct:
         np_obj = np.frombuffer(
             b64decode(dct["__numpy__"]), descr_to_dtype(dct["dtype"])
         )
         return np_obj.reshape(shape) if (shape := dct["shape"]) else np_obj[0]
     return dct
 
@@ -147,8 +147,8 @@
     scales = np.array([1.0, 10, 0.1, 5000.0])
     names = ["A", "B", "C", "D"]
     num_examples = 205
     x_data_dict = {}
     for l in range(locs.shape[0]):
         x_data_dict[names[l]] = np.random.normal(loc=locs[l], scale=scales[l], size=num_examples)
     x_data = pd.DataFrame(x_data_dict)
-    return x_data
+    return x_data
```

### Comparing `bridgescaler-0.6.0/bridgescaler/deep.py` & `bridgescaler-0.7.0/bridgescaler/deep.py`

 * *Files identical despite different names*

### Comparing `bridgescaler-0.6.0/bridgescaler/distributed.py` & `bridgescaler-0.7.0/bridgescaler/distributed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import numpy as np
 from numpy.lib.recfunctions import structured_to_unstructured, unstructured_to_structured
 from copy import deepcopy
 from crick import TDigest as CTDigest
-from numba_stats import norm
+from scipy.special import ndtr, ndtri
 import pandas as pd
 import xarray as xr
-from pytdigest import TDigest
 from functools import partial
 from scipy.stats import logistic
 from warnings import warn
-
+from numba import guvectorize, float32, float64, void
 CENTROID_DTYPE = np.dtype([('mean', np.float64), ('weight', np.float64)])
 
 class DBaseScaler(object):
     """
     Base distributed scaler class. Used only to store attributes and methods shared across all distributed
     scaler subclasses.
     """
@@ -351,35 +350,139 @@
     else:
         td_obj.update(xv[:, var_index].ravel())
     return td_obj
 
 
 def transform_variable(td_obj, xv,
                        min_val=0.000001, max_val=0.9999999, distribution="normal"):
-    x_transformed = td_obj.cdf(xv)
-    x_transformed[:] = np.minimum(x_transformed, max_val)
-    x_transformed[:] = np.maximum(x_transformed, min_val)
+    td_centroids = td_obj.centroids()
+    x_transformed = np.zeros_like(xv)
+    tdigest_cdf(xv, td_centroids["mean"], td_centroids["weight"],
+                                td_obj.min(), td_obj.max(), x_transformed)
+    x_transformed = np.minimum(x_transformed, max_val)
+    x_transformed = np.maximum(x_transformed, min_val)
     if distribution == "normal":
-        x_transformed[:] = norm.ppf(x_transformed, loc=0, scale=1)
+        x_transformed = ndtri(x_transformed)
     elif distribution == "logistic":
-        x_transformed[:] = logistic.ppf(x_transformed)
+        x_transformed = logistic.ppf(x_transformed)
     return x_transformed
 
 
 def inv_transform_variable(td_obj, xv,
                            distribution="normal"):
-    x_transformed = np.zeros(xv.shape, dtype=xv.dtype)
+    td_centroids = td_obj.centroids()
+    x_transformed = np.zeros_like(xv)
     if distribution == "normal":
-        x_transformed = norm.cdf(xv, loc=0, scale=1)
+        x_transformed = ndtr(xv)
     elif distribution == "logistic":
         x_transformed = logistic.cdf(xv)
-    x_transformed[:] = td_obj.quantile(x_transformed)
+    tdigest_quantile(xv, td_centroids["mean"], td_centroids["weight"],
+                                td_obj.min(), td_obj.max(), x_transformed)
     return x_transformed
 
 
+@guvectorize([void(float64[:], float64[:], float64[:], float64, float64, float64[:]),
+            void(float32[:], float64[:], float64[:], float64, float64, float32[:])], "(m),(n),(n),(),()->(m)")
+def tdigest_cdf(xv, cent_mean, cent_weight, t_min, t_max, out):
+    cent_merged_weight = np.zeros_like(cent_weight)
+    cumulative_weight = 0
+    for i in range(cent_weight.size):
+        cent_merged_weight[i] = cumulative_weight + cent_weight[i] / 2.0
+        cumulative_weight += cent_weight[i]
+    total_weight = cent_weight.sum()
+    for i, x in enumerate(xv):
+        if cent_mean.size == 0:
+            out[i] = np.nan
+            continue
+        # Single centroid
+        if cent_mean.size == 1:
+            if x < t_min:
+                out[i] = 0.0
+            elif x > t_max:
+                out[i] = 1.0
+            elif t_max - t_min < np.finfo(np.float64).eps:
+                out[i] = 0.5
+            else:
+                out[i] = (x - t_min) / (t_max - t_min)
+            continue
+        # Equality checks only apply if > 1 centroid
+        if x >= t_max:
+            out[i] = 1.0
+            continue
+        elif x <= t_min:
+            out[i] = 0.0
+            continue
+
+        # i_l = bisect_left_mean(T->merge_centroids, x, 0, T->ncentroids);
+        i_l = np.searchsorted(cent_mean, x, side="left")
+        if x < cent_mean[0]:
+            # min < x < first centroid
+            x0 = t_min
+            x1 = cent_mean[0]
+            dw = cent_merged_weight[0] / 2.0
+            out[i] = dw * (x - x0) / (x1 - x0) / total_weight
+        elif i_l == cent_mean.size:
+            # last centroid < x < max
+            x0 = cent_mean[i_l - 1]
+            x1 = t_max
+            dw = cent_weight[i_l - 1] / 2.0
+            out[i] = 1.0 - dw * (x1 - x) / (x1 - x0) / total_weight
+        elif cent_mean[i_l] == x:
+            # x is equal to one or more centroids
+            i_r = np.searchsorted(cent_mean, x, side="right")
+            out[i] = cent_merged_weight[i_r] / total_weight
+        else:
+            assert cent_mean[i_l] > x
+            x0 = cent_mean[i_l - 1]
+            x1 = cent_mean[i_l]
+            dw = 0.5 * (cent_weight[i_l - 1] + cent_weight[i_l])
+            out[i] = (cent_merged_weight[i_l - 1] + dw * (x - x0) / (x1 - x0)) / total_weight
+
+
+@guvectorize([void(float64[:], float64[:], float64[:], float64, float64, float64[:]),
+            void(float32[:], float64[:], float64[:], float64, float64, float32[:])], "(m),(n),(n),(),()->(m)")
+def tdigest_quantile(qv, cent_mean, cent_weight, t_min, t_max, out):
+    cent_merged_weight = np.zeros_like(cent_weight)
+    cumulative_weight = 0
+    for i in range(cent_weight.size):
+        cent_merged_weight[i] = cumulative_weight + cent_weight[i] / 2.0
+        cumulative_weight += cent_weight[i]
+    total_weight = cent_weight.sum()
+    for i, q in enumerate(qv):
+        if total_weight == 0:
+            out[i] = np.nan
+            continue
+        if q <= 0:
+            out[i] = t_min
+            continue
+        if q >= 1:
+            out[i] = t_max
+            continue
+        if cent_mean.size == 1:
+            out[i] = cent_mean[0]
+            continue
+
+        index = q * total_weight
+        b = np.searchsorted(cent_merged_weight, index, side="left")
+        if b == 0:
+            x0 = 0
+            y0 = t_min
+        else:
+            x0 = cent_merged_weight[b - 1]
+            y0 = cent_mean[b - 1]
+
+        if b == cent_mean.size:
+            x1 = total_weight
+            y1 = t_max
+        else:
+            x1 = cent_merged_weight[b]
+            y1 = cent_mean[b]
+        out[i] = y0 + (index - x0) * (y1 - y0) / (x1 - x0)
+
+
 class DQuantileScaler(DBaseScaler):
     """
     Distributed Quantile Scaler that uses the crick TDigest Cython library to compute quantiles across multiple
     datasets in parallel. The library can perform fitting, transforms, and inverse transforms across variables
     in parallel using the multiprocessing library. Multidimensional arrays are stored in shared memory across
     processes to minimize inter-process communication.
 
@@ -540,160 +643,7 @@
         x_col_order = current.get_column_order(other.x_columns_)
         assert x_col_order.size > 0, "No matching columns in other DQuantileScaler"
         for i, o in enumerate(x_col_order):
             td_objs[o].merge(other_td_objs[i])
         current.td_objs_to_attributes(td_objs)
         return current
 
-
-class DQuantileTransformer(DBaseScaler):
-    """
-    Distributed quantile transformer that uses the T-Digest algorithm to transform the input data into approximate
-    quantiles. This class stores the centroids and counts from the T-Digest algorithm and calls pytdigest to
-    perform centroid fitting and transforms of data when needed. DQuantileTransformer objects can be added together
-    to create a combined quantile distribution, enabling map-reduce-style distributed calculations of quantiles
-    across large number of files. The same object can also be fit multiple times to compile quantiles serially
-    but with lower memory usage. Scaler supports numpy arrays, pandas dataframes, and xarray DataArrays and
-    will return a transformed array in the same form as the original with column or coordinate names preserved.
-
-    Args:
-        max_merged_centroids (int): Maximum number of centroids in TDigest
-        distribution (str): Output distribution of transform. Options are "uniform" (default), "normal", and "logistic".
-        channels_last (bool): Whether data will use the last dimension (True) as the channels or variable dim
-            or the second dimension (False).
-    """
-    def __init__(self, max_merged_centroids=1000, distribution="uniform", channels_last=True):
-        warn(f'{self.__class__.__name__} will be deprecated in the next version.',
-             DeprecationWarning, stacklevel=2)
-
-        self.max_merged_centroids = max_merged_centroids
-        self.distribution = distribution
-        self.centroids_ = None
-        super().__init__(channels_last=channels_last)
-        return
-
-    def fit(self, x, weight=None):
-        x_columns, is_array = self.extract_x_columns(x, channels_last=self.channels_last)
-        xv = self.extract_array(x)
-        channel_dim = self.set_channel_dim()
-        if not self._fit:
-            self.x_columns_ = x_columns
-            self.is_array_ = is_array
-            # The number of centroids may vary depending on the distribution of each input variable.
-            # The extra spots at the end are padded with nans.
-            self.centroids_ = np.ones((xv.shape[channel_dim], self.max_merged_centroids, 2)) * np.nan
-            if self.channels_last:
-                for i in range(xv.shape[channel_dim]):
-                    td_obj = TDigest.compute(xv[..., i].ravel(), w=weight, compression=self.max_merged_centroids)
-                    self.centroids_[i, :td_obj._num_merged] = td_obj.get_centroids()
-            else:
-                for i in range(xv.shape[channel_dim]):
-                    td_obj = TDigest.compute(xv[:, i].ravel(), w=weight, compression=self.max_merged_centroids)
-                    self.centroids_[i, :td_obj._num_merged] = td_obj.get_centroids()
-        else:
-            assert x.shape[channel_dim] == self.x_columns_.shape[0], "New data has a different number of columns"
-            if is_array:
-                x_col_order = np.arange(x.shape[-1])
-            else:
-                x_col_order = self.get_column_order(x_columns)
-            td_objs = self.to_digests()
-            new_centroids = np.ones((xv.shape[-1], self.max_merged_centroids, 2)) * np.nan
-            if self.channels_last:
-                for i, o in enumerate(x_col_order):
-                    td_obj = td_objs[o]
-                    new_td_obj = TDigest.compute(xv[..., i].ravel(), w=weight, compression=self.max_merged_centroids)
-                    combined_td_obj = td_obj + new_td_obj
-                    new_centroids[i, :combined_td_obj._num_merged] = combined_td_obj.get_centroids()
-            else:
-                for i, o in enumerate(x_col_order):
-                    td_obj = td_objs[o]
-                    new_td_obj = TDigest.compute(xv[:, i].ravel(), w=weight, compression=self.max_merged_centroids)
-                    combined_td_obj = td_obj + new_td_obj
-                    new_centroids[i, :combined_td_obj._num_merged] = combined_td_obj.get_centroids()
-            self.centroids_ = new_centroids
-        self._fit = True
-        return
-
-    def force_merge(self):
-        """
-        Trigger a merger of centroids for each variable.
-        """
-        td_objs = self.to_digests()
-        for td_obj in td_objs:
-            td_obj.force_merge()
-        self.to_centroids(td_objs)
-
-    def to_digests(self):
-        """
-        Converts the centroids for each variable in DQuantileTransformer to a list of TDigest objects.
-
-        Returns:
-            td_objs: list of TDigest objects
-        """
-        assert self._fit, "Must call fit() before calling to_digests()"
-        td_objs = []
-        for i in range(self.centroids_.shape[0]):
-            centroid_len = np.where(np.isnan(self.centroids_[i, :, 0]))[0].min()
-            td_objs.append(TDigest.of_centroids(self.centroids_[i, :centroid_len],
-                                                compression=self.max_merged_centroids))
-        return td_objs
-
-    def to_centroids(self, td_objs):
-        centroids = np.ones((len(td_objs), self.max_merged_centroids, 2)) * np.nan
-        for i in range(len(td_objs)):
-            centroids[i, :td_objs[i]._num_merged] = td_objs[i].get_centroids()
-        return centroids
-
-    def transform(self, x, channels_last=None):
-        xv, x_transformed, channels_last, channel_dim, x_col_order = self.process_x_for_transform(x, channels_last)
-        td_objs = self.to_digests()
-        if channels_last:
-            for i, o in enumerate(x_col_order):
-                xd = xv[..., i].ravel().astype("float64")
-                x_transformed[..., i] = np.reshape(td_objs[o].cdf(xd), xv[..., i].shape)
-        else:
-            for i, o in enumerate(x_col_order):
-                xd = xv[:, i].ravel().astype("float64")
-                x_transformed[:, i] = np.reshape(td_objs[o].cdf(xd), xv[:, i].shape)
-        if self.distribution == "normal":
-            x_transformed = norm.ppf(x_transformed, loc=0, scale=1)
-        elif self.distribution == "logistic":
-            x_transformed = logistic.ppf(x_transformed)
-        x_transformed = self.package_transformed_x(x_transformed, x)
-        return x_transformed
-
-    def inverse_transform(self, x, channels_last=None):
-        xv, x_transformed, channels_last, channel_dim, x_col_order = self.process_x_for_transform(x, channels_last)
-        td_objs = self.to_digests()
-        if self.distribution == "normal":
-            x_transformed = norm.cdf(xv, loc=0, scale=1)
-        elif self.distribution == "logistic":
-            x_transformed = logistic.cdf(xv)
-        if channels_last:
-            for i, o in enumerate(x_col_order):
-                xd = x_transformed[..., i].ravel().astype("float64")
-                x_transformed[..., i] = np.reshape(td_objs[o].inverse_cdf(xd),
-                                                   xv[..., i].shape)
-        else:
-            for i, o in enumerate(x_col_order):
-                xd = x_transformed[:, i].ravel().astype("float64")
-                x_transformed[:, i] = np.reshape(td_objs[o].inverse_cdf(xd),
-                                                 xv[:, i].shape)
-        x_transformed = self.package_transformed_x(x_transformed, x)
-        return x_transformed
-
-    def __add__(self, other):
-        assert type(other) is DQuantileTransformer, "Adding mismatched scaler types."
-        assert self.is_fit() and other.is_fit(), "At least one scaler is not fit."
-        td_objs = self.to_digests()
-        other_td_objs = other.to_digests()
-        assert len(td_objs) == len(other_td_objs), "Number of variables in scalers do not match."
-        max_centroids = np.maximum(self.max_merged_centroids, other.max_merged_centroids)
-        combined_centroids = np.ones((self.centroids_.shape[0], max_centroids, self.centroids_.shape[2])) * np.nan
-        for i in range(len(td_objs)):
-            combined_td_obj = td_objs[i] + other_td_objs[i]
-            combined_td_obj.force_merge()
-            combined_centroids[i, :combined_td_obj._num_merged] = combined_td_obj.get_centroids()
-        new_dquantile = deepcopy(self)
-        new_dquantile.max_merged_centroids = max_centroids
-        new_dquantile.centroids_ = combined_centroids
-        return new_dquantile
```

### Comparing `bridgescaler-0.6.0/bridgescaler/group.py` & `bridgescaler-0.7.0/bridgescaler/group.py`

 * *Files identical despite different names*

### Comparing `bridgescaler-0.6.0/bridgescaler.egg-info/PKG-INFO` & `bridgescaler-0.7.0/bridgescaler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgescaler
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tool to automagically save scikit-learn scaler properties to a portable, readable format.
 Home-page: https://github.com/NCAR/bridgescaler
 Author: David John Gagne
 Author-email: dgagne@ucar.edu
 License: MIT
 Keywords: machine learning
 Platform: any
@@ -18,18 +18,17 @@
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.0
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: crick
 Requires-Dist: scipy
 Requires-Dist: xarray
+Requires-Dist: numba
 Requires-Dist: sphinx
 Requires-Dist: sphinx-book-theme
-Requires-Dist: pytdigest
-Requires-Dist: numba-stats
 
 # bridgescaler
 Bridge your scikit-learn-style scaler parameters between Python sessions and users.
 Bridgescaler allows you to save the properties of a scikit-learn-style scaler object
 to a json file, and then repopulate a new scaler object with the same properties.
```

### Comparing `bridgescaler-0.6.0/setup.cfg` & `bridgescaler-0.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 install_requires = 
 	scikit-learn>=1.0
 	numpy
 	pandas
 	crick
 	scipy
 	xarray
+	numba
 	sphinx
 	sphinx-book-theme
-	pytdigest
-	numba-stats
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

