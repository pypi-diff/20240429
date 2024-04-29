# Comparing `tmp/sctm-0.1.1.tar.gz` & `tmp/sctm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sctm-0.1.1.tar", last modified: Tue Aug 22 01:47:40 2023, max compression
+gzip compressed data, was "sctm-0.1.3.tar", last modified: Mon Apr 29 04:48:03 2024, max compression
```

## Comparing `sctm-0.1.1.tar` & `sctm-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rwxr-xr-x   0        0        0     1618 2023-08-17 04:54:32.860751 sctm-0.1.1/README.rst
--rw-r--r--   0        0        0     1125 2023-08-22 01:47:19.376886 sctm-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0      245 2023-07-17 04:19:45.794470 sctm-0.1.1/sctm/__init__.py
--rwxr-xr-x   0        0        0     5909 2023-08-17 06:04:01.126201 sctm-0.1.1/sctm/analysis.py
--rwxr-xr-x   0        0        0     2494 2023-08-18 01:42:36.815914 sctm-0.1.1/sctm/data.py
--rwxr-xr-x   0        0        0     4163 2023-07-11 14:18:18.710696 sctm-0.1.1/sctm/metrics.py
--rwxr-xr-x   0        0        0    20409 2023-08-22 01:46:21.497310 sctm-0.1.1/sctm/model.py
--rwxr-xr-x   0        0        0    33875 2023-08-22 01:46:21.917307 sctm-0.1.1/sctm/pl.py
--rwxr-xr-x   0        0        0     1113 2023-08-17 06:07:21.512732 sctm-0.1.1/sctm/pp.py
--rwxr-xr-x   0        0        0    17529 2023-08-21 15:14:15.311277 sctm-0.1.1/sctm/stamp.py
--rw-r--r--   0        0        0     1903 2023-08-20 15:23:04.836636 sctm-0.1.1/sctm/utils.py
--rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 sctm-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1618 2023-08-17 04:54:32.860751 sctm-0.1.3/README.rst
+-rw-r--r--   0        0        0     1859 2024-04-29 04:48:02.978544 sctm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-10-18 13:47:32.430057 sctm-0.1.3/sctm/.vscode/settings.json
+-rwxr-xr-x   0        0        0      259 2024-03-26 02:14:45.648763 sctm-0.1.3/sctm/__init__.py
+-rw-r--r--   0        0        0     8364 2023-12-12 14:18:57.322103 sctm-0.1.3/sctm/__pycache__/dist.cpython-39.pyc.139925693191984
+-rw-r--r--   0        0        0        0 2024-02-20 12:38:34.876995 sctm-0.1.3/sctm/__pycache__/model.cpython-39.pyc.139648853430960
+-rw-r--r--   0        0        0    10610 2023-11-03 05:54:43.388051 sctm-0.1.3/sctm/__pycache__/model.cpython-39.pyc.140246342949296
+-rwxr-xr-x   0        0        0     5907 2024-03-26 02:26:42.298790 sctm-0.1.3/sctm/analysis.py
+-rwxr-xr-x   0        0        0      552 2023-12-21 00:08:12.884745 sctm-0.1.3/sctm/data.py
+-rw-r--r--   0        0        0    11295 2024-04-29 02:17:11.893913 sctm-0.1.3/sctm/dist.py
+-rw-r--r--   0        0        0     4384 2024-04-29 01:49:08.331634 sctm-0.1.3/sctm/layers.py
+-rwxr-xr-x   0        0        0     7968 2024-04-27 10:33:24.958102 sctm-0.1.3/sctm/metrics.py
+-rwxr-xr-x   0        0        0    30877 2024-04-29 04:19:25.685750 sctm-0.1.3/sctm/model.py
+-rwxr-xr-x   0        0        0    35592 2024-04-23 07:27:11.528153 sctm-0.1.3/sctm/pl.py
+-rwxr-xr-x   0        0        0     3417 2024-03-26 02:26:42.314790 sctm-0.1.3/sctm/pp.py
+-rw-r--r--   0        0        0     9329 2024-03-26 02:26:42.314790 sctm-0.1.3/sctm/rbo.py
+-rw-r--r--   0        0        0      333 2024-03-26 02:26:42.318790 sctm-0.1.3/sctm/seed.py
+-rwxr-xr-x   0        0        0    29672 2024-04-29 04:14:42.710542 sctm-0.1.3/sctm/stamp.py
+-rw-r--r--   0        0        0     3890 2024-04-29 04:15:41.330378 sctm-0.1.3/sctm/utils.py
+-rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 sctm-0.1.3/PKG-INFO
```

### Comparing `sctm-0.1.1/README.rst` & `sctm-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `sctm-0.1.1/sctm/analysis.py` & `sctm-0.1.3/sctm/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import gseapy as gp
 import discotoolkit as dt
+import gseapy as gp
 from joblib import Parallel, delayed
 
 
 def get_enrichr_geneset(organism="Human"):
     avail_organisms = ["Human", "Mouse", "Yeast", "Fly", "Fish", "Worm"]
     if organism not in avail_organisms:
         raise ValueError(f"available organism are {avail_organisms}")
@@ -29,15 +29,14 @@
         )
         if topic not in enrichr:
             enrichr[topic] = topic_enrichr.results
     return enrichr
 
 
 def get_topic_ora(beta, geneset, topics="all", topn_genes=20, n_jobs=20):
-
     if topics == "all":
         topics = beta.columns
     elif not isinstance(topics, list):
         topics = [topics]
     for topic in topics:
         if topic not in beta.columns:
             raise KeyError(f"{topic} not Found")
@@ -117,18 +116,17 @@
 
 
 def get_topic_gsea(
     beta,
     geneset,
     topics="all",
     geneset_size=[5, 500],
-    n_jobs=1,
     permutations=1000,
+    n_jobs=20,
 ):
-
     if topics == "all":
         topics = beta.columns
     elif not isinstance(topics, list):
         topics = [topics]
     for topic in topics:
         if topic not in beta.columns:
             raise KeyError(f"{topic} not found")
@@ -155,15 +153,14 @@
     gsea = Parallel(n_jobs=n_jobs)(
         delayed(process_topic)(beta, topic, geneset) for topic in topics
     )
     # results["Name"] = geneset
 
     # if topic not in gsea.keys():
     #     gsea[topic] = results
-
     gseas = {}
     for i in range(len(topics)):
         gseas[topics[i]] = gsea[i]
 
     return gseas
```

### Comparing `sctm-0.1.1/sctm/pl.py` & `sctm-0.1.3/sctm/pl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,44 @@
+from typing import (
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
+
 import anndata as ad
-import scanpy as sc
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 
 # import textwrap
 import numpy as np
-from matplotlib.axes import Axes
-
-# import pandas as pd
-from matplotlib.patches import Patch
+import scanpy as sc
 
 # import seaborn as sns
 from matplotlib import rcParams
-import matplotlib as mpl
+from matplotlib.axes import Axes
 
 # import matplotlib.pyplot as plt
 # import numpy as np
 from matplotlib.colors import ListedColormap
 from matplotlib.gridspec import GridSpec
 
+# import pandas as pd
+from matplotlib.patches import Patch
+
 # from upsetplot import plot, from_contents
 # from itertools import chain
-
-
-from scanpy._utils import _empty, Empty
+from scanpy._utils import Empty, _empty
 from scanpy.pl._tools.scatterplots import (
-    _check_spatial_data,
-    _check_img,
-    _check_spot_size,
-    _check_scale_factor,
     _check_crop_coord,
+    _check_img,
     _check_na_color,
-)
-from typing import (
-    Union,
-    Optional,
-    List,
-    Tuple,
+    _check_scale_factor,
+    _check_spatial_data,
+    _check_spot_size,
 )
 from scanpy.pl._utils import (
     ColorLike,
 )
 
 
 def heatmap_topic(adata, groupby=None, topics=None, figsize=(10, 5), cmap=None):
@@ -463,43 +462,44 @@
 
 #         return ax
 
 
 def draw_pie(dist, xpos, ypos, size, colors, figsize, ax=None):
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize)
-
     # for incremental pie slices
+
     cumsum = np.cumsum(dist)
+    # normalize
     cumsum = cumsum / cumsum[-1]
     pie = [0] + cumsum.tolist()
     c = 0
     for r1, r2 in zip(pie[:-1], pie[1:]):
-        # if r2 - r1 > 0.01:
-        angles = np.linspace(2 * np.pi * r1, 2 * np.pi * r2, num=10)
-        x = [0] + np.cos(angles).tolist() + [0]
-        y = [0] + np.sin(angles).tolist() + [0]
-
-        xy = np.column_stack([x, y])
-        # print(xy.shape)
-        ax.plot(
-            [xpos],
-            [ypos],
-            marker=xy,
-            markersize=np.abs(xy).max() * np.array(np.sqrt(size)),
-            c=colors[c],
-        )
+        if r2 - r1 > 0.01:
+            angles = np.linspace(2 * np.pi * r1, 2 * np.pi * r2, num=100)
+            x = [0] + np.cos(angles).tolist() + [0]
+            y = [0] + np.sin(angles).tolist() + [0]
+            xy = np.column_stack([x, y])
+            # print(xy.shape)
+            ax.plot(
+                [xpos],
+                [ypos],
+                marker=xy,
+                markersize=np.abs(xy).max() * np.array(np.sqrt(size)),
+                c=colors[c],
+            )
         c += 1
 
     return ax
 
 
 def spatialpie(
     adata,
-    topic_prop,
+    color,
+    N=2,
     *,
     basis: str = "spatial",
     img: Union[np.ndarray, None] = None,
     img_key: Union[str, None, Empty] = _empty,
     library_id: Union[str, Empty] = _empty,
     crop_coord: Tuple[int, int, int, int] = None,
     alpha_img: float = 1.0,
@@ -562,45 +562,47 @@
     if scale_factor is not None:
         circle_radius = size * scale_factor * spot_size * 0.5
     else:
         circle_radius = spot_size * 0.5
 
     if figsize is None:
         figsize = (rcParams["figure.figsize"][0], rcParams["figure.figsize"][1])
-    topic_names = topic_prop.columns
-    topic_prop = topic_prop.to_numpy()
+
+    topic_prop = adata.obs[color]
+    topic_prop = topic_prop.mask(
+        topic_prop.rank(axis=1, method="min", ascending=False) > N, 0
+    )
+    topic_prop = topic_prop.values
 
     n_cells = topic_prop.shape[0]
     axs = None
     spatial_coords = adata.obsm[basis]
     n = 0
     colors = plt.get_cmap(cmap)
     colors = colors.colors
 
     for i in range(n_cells):
         n = n + 1
         if (n % 20000) == 0:
             print(f"{i} number of cells done")
         axs = draw_pie(
-            topic_prop[
-                i,
-            ],
+            topic_prop[i,],
             xpos=spatial_coords[i, 0] * scale_factor,
             ypos=spatial_coords[i, 1] * scale_factor,
             figsize=figsize,
             size=circle_radius,
             ax=axs,
             colors=colors,
         )
 
     if legend:
         legend_elements = []
-        for i in range(len(topic_names)):
+        for i in range(len(colors)):
             legend_elements.append(
-                Patch(facecolor=colors[i], edgecolor="w", label=topic_names[i])
+                Patch(facecolor=colors[i], edgecolor="w", label=color[i])
             )
 
         axs.legend(
             handles=legend_elements,
             bbox_to_anchor=(1, 0.5),
             loc="center left",
             labelspacing=0.5,
@@ -1083,9 +1085,72 @@
         value_df=topic_prop,
         labels=topic_prop.columns,
         circle_radius=circle_radius,
         figsize=figsize,
         display_zeros=display_zeros,
         **kwargs,
     )  # cell abundance values
+    plt.gca().invert_yaxis()
 
     return fig
+
+
+def spatial(
+    adata,
+    color=None,
+    cmap=None,
+    frameon=None,
+    title=None,
+    wspace=None,
+    hspace=0.25,
+    palette=None,
+    colorbar_loc="right",
+    size=1,
+    basis="spatial",
+    vmax=None,
+    ncols=4,
+    layer=None,
+    show=True,
+    *args,
+    **kwargs,
+):
+    """A faster simple function that uses sc.pl.embedding to plot for non-visium data
+    so it dont take too long. ~sleep. Very inflexible.
+
+    Args:
+        adata (_type_): Annotated data matrix.
+        color (_type_): Keys for annotations of observations/cells or variables/genes
+        size (int, optional): size of spots. Defaults to 1.
+        basis (str, optional): basis in obsm. Defaults to "spatial".
+        vmax (str, optional): The value representing the upper limit of the color scale. Defaults to "p99".
+        show (bool, optional): Show the plot, do not return axis. Defaults to True.
+
+    Returns:
+        _type_: A plot
+    """
+    ax = sc.pl.embedding(
+        adata,
+        basis=basis,
+        show=False,
+        color=color,
+        wspace=wspace,
+        hspace=hspace,
+        palette=palette,
+        vmax=vmax,
+        size=size,
+        ncols=ncols,
+        cmap=cmap,
+        frameon=frameon,
+        colorbar_loc=colorbar_loc,
+        title=title,
+        layer=layer,
+        *args,
+        **kwargs,
+    )
+    if isinstance(ax, list):
+        [axs.invert_yaxis() for axs in ax]
+        [axs.set_aspect("equal") for axs in ax]
+    else:
+        ax.invert_yaxis()
+        ax.set_aspect("equal")
+    if show is False:
+        return ax
```

### Comparing `sctm-0.1.1/PKG-INFO` & `sctm-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: scTM
-Version: 0.1.1
+Version: 0.1.3
 Summary: A toolbox for single cell topic models
 Author-Email: chengwei94 <chengwei8@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: scanpy>=1.9.3
 Requires-Dist: anndata>=0.9.1
 Requires-Dist: gseapy>=1.0.4
 Requires-Dist: pyro-ppl>=1.8.4
-Requires-Dist: torch-geometric>=2.3.1
 Requires-Dist: squidpy>=1.2.2
 Requires-Dist: torch>=2.0.1
 Requires-Dist: torchinfo>=1.8.0
 Requires-Dist: discotoolkit>=1.0.0.1
 Requires-Dist: scikit-misc>=0.2.0
 Description-Content-Type: text/x-rst
```

