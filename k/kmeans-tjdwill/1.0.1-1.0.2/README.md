# Comparing `tmp/kmeans_tjdwill-1.0.1.tar.gz` & `tmp/kmeans_tjdwill-1.0.2.tar.gz`

## Comparing `kmeans_tjdwill-1.0.1.tar` & `kmeans_tjdwill-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,31 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/animate.py
--rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/base_funcs.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/clustering.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/segmentation.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_animate2D.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_animate3D.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_assign_cluster.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_clustering.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_datavalidation.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_gen_means.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/tests/test_segmentation.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/LICENSE
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/.github/workflows/sitebuild.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/api-dev.rst
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/api-user.rst
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/modules.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/animate.py
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/base_funcs.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/clustering.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/segmentation.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_animate2D.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_animate3D.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_assign_cluster.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_clustering.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_datavalidation.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_distances.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_gen_means.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_segmentation.py
+-rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_groups04.jpg
+-rw-r--r--   0        0        0    15340 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_groups10.jpg
+-rw-r--r--   0        0        0    18720 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_rand_groups04.jpg
+-rw-r--r--   0        0        0    25980 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_rand_groups10.jpg
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/README.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/PKG-INFO
```

### Comparing `kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/animate.py` & `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/animate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-"""
-@author: tjdwill 
-@date: 5 April 2024
-@title: K-means Clustering Animation
-@description:
-    Animating k-means for 2-D and 3-D cases.
-"""
+#=============================================================================
+# @author: tjdwill 
+# @date: 5 April 2024
+# @title: K-means Clustering Animation
+# @description: Animating k-means for 2-D and 3-D cases.
+#=============================================================================
 from typing import Union
 #-
 from matplotlib import pyplot as plt
 from matplotlib import colors
 import matplotlib as mpl
 import numpy as np
 #-
 from kmeans.base_funcs import _assign_clusters, _validate, _new_centroids, SMALLEST_THRESH
+from kmeans.clustering import MaxIterationError
 
 
 Clusterable = np.ndarray
 Clusters = dict[int, Clusterable]
-class MaxIterationError(Exception):
-    """An exception to be raised when the maximum iteration tolerance is exceeded."""
-    pass
 
 
 colors: list = [color for color in colors.TABLEAU_COLORS.values()]
 WRAP_FACTOR: int = len(colors)
 SZ = 10
 CENTROID_SZ = 2*SZ
 def _draw(
@@ -99,46 +96,39 @@
         initial_means: Union[Clusterable, list[Clusterable], tuple[Clusterable]] = None,
         ndim: int = None,
         tolerance: float = SMALLEST_THRESH,
         max_iterations: int = 250,
 ) -> tuple[Clusters, np.ndarray, mpl.figure.Figure]:
     """Perform and display k-means clustering
     
+    This is the same as :func:`kmeans.cluster`, just with plotting side-effects.
+
     Args:
-        data: The input data
-            This data should be formatted in terms of row vectors.
-            Given a flat numpy array
-            data=np.array([0, 1, 2, 3, 4]), do the following:
-                `data = data.reshape(data.shape[-1], -1)`
-            or  `data = data[..., np.newaxis]`
-            It should make each point a row entry:
-                [[0], [1], [2], [3], [4]]
-            Data of higher dimensions (ex. a multi-channeled image)
-            should be flattened using the number of indices
-            for the deepest dimension. So, for an image with shape
-            (480, 640, 3), run
-                `data = data.reshape(-1, data.shape[-1])`
-        k: Amount of clusters
-        initial_means: The initial cluster centroids
-            Default: None -> Means are randomly selected from data 
-            with uniform probability
-        ndim: Dimension limit for clustering; 
-            Default: None -> selects the ndim based on data length
-        tolerance: Controls the completion criteria. Lower -> more iterations.
-            Default: 20*eps for np.float64
-        max_iterations: The counter timeout. Function raises exception if exceeded.
-            Default: 250
+        data: The input data. Expects data homogeneity (all elements are the
+            same dimension)
+        k: Amount of clusters desired.
+        initial_means: The initial cluster centroids. Means are randomly
+            selected from data with uniform probability by default.
+        ndim: Dimension limit for clustering. If default, the length of a given
+            data element is used (all data dimensions clustered).
+        tolerance: Controls the completion criteria. Lower values -> more
+            iterations. Defaults to 20*eps for np.float64.
+        max_iterations: Max number of iterations before terminating function execution.
 
     Returns:
-        ({int: np.np.ndarray}, np.np.ndarray, matplotlib.figure.Figure): 
-            clustered data, cluster centroids, Matplotlib Figure
+        dict[int, np.ndarray], np.ndarray, matplotlib.figure.Figure: 
+            Clustered Data, Cluster Centroids, Matplotlib Figure
 
     Raises:
-        MaxIterationError: Raise this exception if the clustering doesn't
-            converge before reaching the `max_iterations` count.
+        `ValueError`: if calculated ``ndim`` or provided ``ndim`` is neither 2
+            nor 3.
+        kmeans.MaxIterationError: Raise this exception if the clustering doesn't
+            converge before reaching the ``max_iterations`` count.
+        
+
     """
     data, initial_means, ndim = _validate(
         data,
         k, 
         initial_means=initial_means, 
         ndim=ndim,
         tolerance=tolerance,
```

### Comparing `kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/base_funcs.py` & `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/base_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-"""
-@author: tjdwill 
-@date: 6 April 2024
-@title: k-means base functions
-@description:
-    Functions that assist with the clustering operation
-"""
+#==============================================================================
+# @author: tjdwill 
+# @date: 6 April 2024
+# @title: k-means base functions
+# @description:
+#     Functions that assist with the clustering operation
+#==============================================================================
 from time import perf_counter
 from typing import Callable, Union
 #-
 import numpy as np
 
 Clusterable = np.ndarray 
 Clusters = dict[int, Clusterable]
 
 # A la Peter Corke's spatialmath, this sets the smallest value in which an element can change. 
 _eps = np.finfo(np.float64).eps
 SMALLEST_THRESH =  20*_eps
 
 
-def time_func(func: Callable):
+def time_func(func: Callable) -> Callable:
+    """A decorator to time function execution.
+    
+    Args:
+        func: the function to time.
+
+    Returns: 
+        Callable: The wrapped function
+
+    """
     def wrapper(*args, **kwargs):
         start = perf_counter()
         out = func(*args, **kwargs)
         print(f"{func.__name__} Execution Time (s): {perf_counter() - start}")
         return out
     return wrapper
 
@@ -32,15 +41,16 @@
     """Assigns each data element to a cluster
     
     Args:
         data: The data to be labeled.
         centroids: The given information to use as cluster criteria.
 
     Returns:
-        dict[int: Clusterable]: the clusters 
+        dict[int, np.ndarray]: The Clusters 
+    
     """    
     k, ndim, *_ = centroids.shape
     temp_data = data[..., :ndim]
     vecs = temp_data[:, np.newaxis] - centroids[np.newaxis, ...]
     norms = np.linalg.norm(vecs, axis=-1)
 
     # Handle the case in which a given data point is equivalently close to multiple centroids.
@@ -89,18 +99,19 @@
 
     Args:
         data: The data from which the means are selected
         k: How many means to select
         ndim: Dimensionality of means
 
     Returns:
-        np.ndarray: the initial means    
+        np.ndarray: Initial Cluster Centroids
 
     Raises:
-        ValueError: If can't find unique set of means within the COUNT_OUT
+        ValueError: If can't find unique set of means.
+    
     """
     COUNT_OUT = 1000
     count = 0
 
 
     while count < COUNT_OUT:
         indices = np.random.choice(np.arange(len(data)), size=(k,), replace=False) 
@@ -117,15 +128,16 @@
     """Returns a new set of centroids
     
     Args:
         clusters: the current grouped data
         ndim: Dimension of data we are clustering
 
     Returns:
-        np.ndarray: the new centroids
+        np.ndarray: New Centroids
+    
     """
     # If this becomes a bottleneck, replace the `for` loop with a list comp.
     centroids = []
     for key in clusters:
         cluster = clusters[key]
         avg = np.average(cluster[:, :ndim], axis=0)
         centroids.append(avg)
@@ -142,23 +154,30 @@
         tolerance: float = 0.5,
         max_iterations: int = 100,
 ) -> tuple[Clusterable, np.ndarray, int]:
     """Perform validation checks on cluster arguments
     
     Args:
         data: The input data
-        k: Amount of clusters
+        k: Amount of clusters desired
         initial_means: The initial cluster centroids
-        ndim: Dimension limit for clustering
-        tolerance: How much can a given cluster centroid 
-            move between iterations
-        max_iterations: The counter timeout
+        ndim: Dimension limit for clustering. If default, the length of a given
+            data element is used (all data dimensions clustered).
+        tolerance: Max tolerable distance a centroid can move before requiring
+            another round of clustering
+        max_iterations: Max number of iterations before terminating function
+            execution.
 
     Returns:
-        tuple[np.ndarray, np.ndarray, int]: the validated data, initial means, and ndim
+        np.ndarray, np.ndarray, int: Validated Data, Initial Centroids, ndim
+        
+    Raises:
+        ValueError: if an input argument is incorrect in value
+        TypeError: if an input argument is of the wrong type.
+
     """
     # Check k
     if not isinstance(k, int): 
         raise TypeError("k must be an integer.")
     if k < 1 or k > len(data):
         raise ValueError("k must be positive and can't exceed number of data points.")
     
@@ -218,8 +237,9 @@
         # Check length
         try:
             assert len(filtered_initial_means) == k
         except AssertionError:
             raise ValueError("\nNumber of unique mean points must == number of segments.\n")
     return new_data, temp_means, ndim
 
+validate = _validate
 __all__ = ["_assign_clusters", "_validate", "_new_centroids", "_generate_means"]
```

### Comparing `kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/clustering.py` & `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/clustering.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,75 @@
-"""
-@author: tjdwill 
-@date: 5 April 2024
-@title: K-means Clustering
-@description:
-    A more function-based implementation of my k-means clustering class.
-"""
+#==============================================================================
+# @author: tjdwill 
+# @date: 5 April 2024
+# @title: K-means Clustering
+# @description:
+#     A more function-based implementation of my k-means clustering class.
+#==============================================================================
 from typing import Union
 #-
 import numpy as np
 #-
 from kmeans.base_funcs import _assign_clusters, _validate, _new_centroids, SMALLEST_THRESH
 
 
 Clusterable = np.ndarray
 Clusters = dict[int, Clusterable]
+
 class MaxIterationError(Exception):
     """An exception to be raised when the maximum iteration tolerance is exceeded."""
     pass
 
-
 def cluster(
         data: Union[Clusterable, list[Clusterable], tuple[Clusterable]],
         k: int,*,
         initial_means: Union[Clusterable, list[Clusterable], tuple[Clusterable]] = None,
         ndim: int = None,
         tolerance: float = SMALLEST_THRESH, 
         max_iterations: int = 250,
 ) -> tuple[Clusters, Clusterable]:
     """Perform k-means clustering
+
+    The input data should be formatted in terms of row vectors. Given a flat
+    numpy array ``data=np.array([0, 1, 2, 3, 4])``, do the following::
+
+        data = data.reshape(data.shape[-1], -1)
+        # or 
+        data = data[..., np.newaxis]
+
+    It should make each point a row entry::
+
+        [[0], [1], [2], [3], [4]]
     
+    Data of higher dimensions (ex. a multi-channeled image)
+    should be flattened using the number of indices
+    for the deepest dimension. So, for an image with shape
+    (480, 640, 3), run::
+
+        data = data.reshape(-1, data.shape[-1])
+
     Args:
-        data: The input data
-            This data should be formatted in terms of row vectors.
-            Given a flat numpy array
-            data=np.array([0, 1, 2, 3, 4]), do the following:
-                `data = data.reshape(data.shape[-1], -1)`
-            or  `data = data[..., np.newaxis]`
-            It should make each point a row entry:
-                [[0], [1], [2], [3], [4]]
-            Data of higher dimensions (ex. a multi-channeled image)
-            should be flattened using the number of indices
-            for the deepest dimension. So, for an image with shape
-            (480, 640, 3), run
-                `data = data.reshape(-1, data.shape[-1])`
-        k: Amount of clusters
-        initial_means: The initial cluster centroids
-            Default: None -> Means are randomly selected from data 
-            with uniform probability
-        ndim: Dimension limit for clustering; 
-            Default: None -> selects the ndim based on data length
-        tolerance: Controls the completion criteria. Lower -> more iterations.
-            Default: 20*eps for np.float64
-        max_iterations: The counter timeout. Function raises exception if exceeded.
-            Default: 250
+        data: The input data. Expects data homogeneity (all elements are the
+            same dimension)
+        k: Amount of clusters desired.
+        initial_means: The initial cluster centroids. Means are randomly
+            selected from data with uniform probability by default.
+        ndim: Dimension limit for clustering. If default, the length of a given
+            data element is used (all data dimensions clustered).
+        tolerance: Controls the completion criteria. Lower values -> more
+            iterations. Defaults to 20*eps for np.float64.
+        max_iterations: Max number of iterations before terminating function execution.
 
     Returns:
-        ({int: np.ndarray}, np.ndarray): clustered data, cluster centroids
+        dict[int, np.ndarray], np.ndarray: Clustered Data, Cluster Centroids
 
     Raises:
-        MaxIterationError: Raise this exception if the clustering doesn't
+        kmeans.MaxIterationError: Raise this exception if the clustering doesn't
             converge before reaching the `max_iterations` count.
+
     """
     data, initial_means, ndim = _validate(
         data,
         k, 
         initial_means=initial_means, 
         ndim=ndim,
         tolerance=tolerance,
```

### Comparing `kmeans_tjdwill-1.0.1/src/kmeans-tjdwill/kmeans/segmentation.py` & `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/segmentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""
-@author: tjdwill
-@date: 12 April 2024
-@title: Image segmentation
-@description:
-    Perform semantic segmentation on the provided image.
-"""
+#=============================================================================
+#@author: tjdwill
+#@date: 12 April 2024
+#@title: Image segmentation
+#@description:
+#    Perform semantic segmentation on the provided image.
+#=============================================================================
 import itertools
 #-
 import numpy as np
 #-
 from kmeans import cluster
 
 
-def append_coords(img: np.ndarray) -> np.ndarray:
+def _append_coords(img: np.ndarray) -> np.ndarray:
     """Append each pixel's coordinate to itself.
     
     Args:
         img: The image.
     
     Returns:
-        np.ndarray: The new array with appended indices.
+        np.ndarray: Array with appended indices.
+
     """
     height, width, *rest = img.shape
     indices = list(itertools.product(range(height), range(width)))
     indices = np.array(indices).reshape(height, width, -1)
     return np.concatenate((img, indices), axis=-1)
 
 
 def segment_img(img: np.ndarray, groups: int, random_colors: bool = False) -> np.ndarray:
-    """Segment the image based on RGB color.
+    """Segment the input RGB image by color groups.
     
     Args:
         img: The image to be segmented. Assumes RGB
         groups: How many groups the image is segmented into. Higher numbers -> more detail
         random_colors: Provide each group with a randomized RGB color instead of the average color.
-            Defaults to False
 
     Returns:
-        np.ndarray: The segmented image
+        np.ndarray: Segmented Image
+ 
     """
-    img_w_idxs = append_coords(img)
+    img_w_idxs = _append_coords(img)
     elem_dim = img_w_idxs.shape[-1]
     assert elem_dim == 5  #(R, G, B, y, x)
     color_groups, group_colors, *extra = cluster(img_w_idxs.reshape(-1, elem_dim), k=groups, ndim=3, tolerance=0.01)
 
     # The idea here is to use advanced indexing to change each group's color at once.
     '''
     Example:
```

### Comparing `kmeans_tjdwill-1.0.1/tests/test_assign_cluster.py` & `kmeans_tjdwill-1.0.2/tests/test_assign_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 @author: tjdwill
 @description:
     Test the cluster assignment functions
 """
 import numpy as np
-#-
 from kmeans.base_funcs import _assign_clusters as acs
 from kmeans.base_funcs import _generate_means as gm
 
 # Now I need to come up with test data...
 SEED = 27
 np.random.seed(SEED)
```

### Comparing `kmeans_tjdwill-1.0.1/tests/test_clustering.py` & `kmeans_tjdwill-1.0.2/tests/test_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 @author: tjdwill
 @date: 6 April 2024
 @description:
     Test the k-means clustering function
 """
 
 import numpy as np
-#-
 from kmeans import cluster
 from kmeans.base_funcs import _generate_means as gm
 
 SEED=27
 np.random.seed(SEED)
 SZ = 100000
 NDIM = 3
```

### Comparing `kmeans_tjdwill-1.0.1/tests/test_datavalidation.py` & `kmeans_tjdwill-1.0.2/tests/test_datavalidation.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.1/tests/test_segmentation.py` & `kmeans_tjdwill-1.0.2/tests/test_segmentation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from pathlib import Path
-#-
+
 import numpy as np
 from PIL import Image
-#-
-from kmeans.segmentation import segment_img
 
-
-# Assumes you are in the top-level directory of package
+from kmeans.segmentation import segment_img
+# Assumes your are in the top-level directory of package
 indir = Path("images")
 outdir = Path("tests/output")
 
 with Image.open(indir / "img00.png") as pil:
     img = np.asarray(pil.convert('RGB'))
 num_groups=4
 seg_img = segment_img(img, groups=num_groups)
```

### Comparing `kmeans_tjdwill-1.0.1/LICENSE` & `kmeans_tjdwill-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `kmeans_tjdwill-1.0.1/README.md` & `kmeans_tjdwill-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.1/PKG-INFO` & `kmeans_tjdwill-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: kmeans-tjdwill
-Version: 1.0.1
+Version: 1.0.2
 Summary: A function-based implementation of k-means clustering that maintains data association.
-Project-URL: Homepage, https://github.com/tjdwill/KMeans_Clustering
-Project-URL: Issues, https://github.com/tjdwill/KMeans_Clustering/issues
+Project-URL: Homepage, https://github.com/tjdwill/kmeans
+Project-URL: Issues, https://github.com/tjdwill/kmeans/issues
 Author-email: Terrance Williams <tjdwill.gh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 tjdwill
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,18 +23,25 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
+Keywords: clustering,computer vision,data analysis,data processing,k-means,linear algebra,robotics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
+Requires-Dist: matplotlib
+Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # K-Means Clustering
 
 
 A repository documenting the implementation of k-Means clustering in Python. Usage examples can be found in the `tests` directory.
```

