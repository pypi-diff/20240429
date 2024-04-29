# Comparing `tmp/trellisplot-0.0.2.tar.gz` & `tmp/trellisplot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trellisplot-0.0.2.tar", last modified: Tue Mar  5 04:25:40 2024, max compression
+gzip compressed data, was "trellisplot-0.0.3.tar", last modified: Mon Apr 29 16:52:01 2024, max compression
```

## Comparing `trellisplot-0.0.2.tar` & `trellisplot-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 04:25:40.647440 trellisplot-0.0.2/
--rw-rw-rw-   0        0        0      527 2024-03-05 04:25:40.637927 trellisplot-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-05 04:25:40.647440 trellisplot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      811 2024-03-05 04:19:14.000000 trellisplot-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-05 04:25:40.615591 trellisplot-0.0.2/trellisplot/
--rw-rw-rw-   0        0        0       22 2024-01-09 20:12:41.000000 trellisplot-0.0.2/trellisplot/__init__.py
--rw-rw-rw-   0        0        0    13626 2024-01-09 20:15:30.000000 trellisplot-0.0.2/trellisplot/plot.py
--rw-rw-rw-   0        0        0      942 2024-03-05 04:09:21.000000 trellisplot-0.0.2/trellisplot/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-05 04:25:40.637927 trellisplot-0.0.2/trellisplot.egg-info/
--rw-rw-rw-   0        0        0      527 2024-03-05 04:25:38.000000 trellisplot-0.0.2/trellisplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-03-05 04:25:40.000000 trellisplot-0.0.2/trellisplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 04:25:38.000000 trellisplot-0.0.2/trellisplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-03-05 04:25:38.000000 trellisplot-0.0.2/trellisplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-05 04:25:38.000000 trellisplot-0.0.2/trellisplot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 16:52:01.862307 trellisplot-0.0.3/
+-rw-rw-rw-   0        0        0      604 2024-04-29 16:52:01.857357 trellisplot-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:52:01.862307 trellisplot-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-04-29 16:50:36.000000 trellisplot-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:52:01.818674 trellisplot-0.0.3/trellisplot/
+-rw-rw-rw-   0        0        0       22 2024-01-09 20:12:41.000000 trellisplot-0.0.3/trellisplot/__init__.py
+-rw-rw-rw-   0        0        0    13677 2024-04-29 16:46:53.000000 trellisplot-0.0.3/trellisplot/plot.py
+-rw-rw-rw-   0        0        0     9178 2024-04-29 16:38:40.000000 trellisplot-0.0.3/trellisplot/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:52:01.855269 trellisplot-0.0.3/trellisplot.egg-info/
+-rw-rw-rw-   0        0        0      604 2024-04-29 16:51:59.000000 trellisplot-0.0.3/trellisplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-29 16:52:01.000000 trellisplot-0.0.3/trellisplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:51:59.000000 trellisplot-0.0.3/trellisplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-29 16:51:59.000000 trellisplot-0.0.3/trellisplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 16:51:59.000000 trellisplot-0.0.3/trellisplot.egg-info/top_level.txt
```

### Comparing `trellisplot-0.0.2/PKG-INFO` & `trellisplot-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trellisplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trellis plot tool
 Author: Ethan S. Lee
 Author-email: <sukraelee@gmail.com>
 Keywords: python,trellisplot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: scipy
 
-Package to plot trellis functionality
+Package to plot trellis functionality. Updated with width normalization, new default colormap, and reduced boxplot
```

### Comparing `trellisplot-0.0.2/setup.py` & `trellisplot-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Trellis plot tool'
-LONG_DESCRIPTION = 'Package to plot trellis functionality'
+LONG_DESCRIPTION = 'Package to plot trellis functionality. Updated with width normalization, new default colormap, and reduced boxplot'
 
 # Setting up
 setup(
         name="trellisplot", 
         version=VERSION,
         author="Ethan S. Lee",
         author_email="<sukraelee@gmail.com>",
```

### Comparing `trellisplot-0.0.2/trellisplot/plot.py` & `trellisplot-0.0.3/trellisplot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from .utils import jitter
+from .utils import parula_map
 from matplotlib.patches import Rectangle
 from matplotlib.patches import Patch
 import pandas as pd
 
 
-def plot(data, parameter, trellis, UL=None, LL=None, filters=None, color=None, plot='violin', cmap="viridis", norm=None, yscale="linear", ylim=None, ylabel=None, width=9, height=5, fontsize=6, markersize=1, linewidth=1):
+def plot(data, parameter, trellis, UL=None, LL=None, filters=None, color=None, plot='violin', cmap=parula_map, norm=None, yscale="linear", ylim=None, ylabel=None, width=9, height=5, fontsize=6, markersize=1, linewidth=1):
     """Plots trellis of a given parameter on split conditions.
     
     Parameters
     ----------
     data : pd.DataFrame
         Summarized dataframe from which to plot parameters from.
     parameter : str
@@ -124,16 +125,16 @@
         mean.append(data_slice[parameter].mean())
         median.append(data_slice[parameter].median())
         std.append(data_slice[parameter].std())
         n_sample.append(data_slice[parameter].count())
         count += 1
         
     if plot =='violin':      
-        sns.boxplot(x=x, y=y, ax=ax, color='0.99', linewidth=0.5, zorder=200, notch=True)
-        sns.violinplot(x=x, y=y, ax=ax, color='0.95', inner=None, zorder=198)
+        sns.boxplot(x=x, y=y, ax=ax, color='0.99', zorder=200, notch=False, width=0.1)
+        sns.violinplot(x=x, y=y, ax=ax, color='0.95', inner=None, zorder=198, density_norm='width')
     elif plot =='box':
         sns.boxplot(x=x, y=y, ax=ax, color='0.95', zorder=200, notch=True)
     
     if color is None:
         # sns.stripplot(x=x, y=y, size=10,ax=ax)
         ax.scatter(x=jitter(x,y), y=y, s=6*ms, zorder=202)
     else:
```

### Comparing `trellisplot-0.0.2/trellisplot.egg-info/PKG-INFO` & `trellisplot-0.0.3/trellisplot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trellisplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trellis plot tool
 Author: Ethan S. Lee
 Author-email: <sukraelee@gmail.com>
 Keywords: python,trellisplot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: scipy
 
-Package to plot trellis functionality
+Package to plot trellis functionality. Updated with width normalization, new default colormap, and reduced boxplot
```

