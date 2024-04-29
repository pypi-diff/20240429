# Comparing `tmp/phdu-2.3.7.tar.gz` & `tmp/phdu-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.3.7.tar", last modified: Tue Apr  9 08:40:31 2024, max compression
+gzip compressed data, was "phdu-2.3.8.tar", last modified: Mon Apr 29 12:09:18 2024, max compression
```

## Comparing `phdu-2.3.7.tar` & `phdu-2.3.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.919629 phdu-2.3.7/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.7/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:40:31.919629 phdu-2.3.7/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.7/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.867626 phdu-2.3.7/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.7/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.7/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.7/phdu/analysis.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.7/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.7/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.7/phdu/geometry.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.7/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.3.7/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.887627 phdu-2.3.7/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.7/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.7/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.7/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    22968 2024-04-09 08:40:09.000000 phdu-2.3.7/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.7/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.907628 phdu-2.3.7/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.7/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.7/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.7/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.7/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    32282 2024-04-05 11:52:28.000000 phdu-2.3.7/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.7/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.7/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.911628 phdu-2.3.7/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.7/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.7/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.7/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.919629 phdu-2.3.7/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.7/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.7/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.7/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.7/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:40:31.879627 phdu-2.3.7/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:40:31.000000 phdu-2.3.7/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-04-09 08:40:31.000000 phdu-2.3.7/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-04-09 08:40:31.000000 phdu-2.3.7/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-04-09 08:40:31.000000 phdu-2.3.7/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-04-09 08:40:31.000000 phdu-2.3.7/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-04-09 08:40:31.923629 phdu-2.3.7/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-04-09 08:40:18.000000 phdu-2.3.7/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-07-31 18:53:26.000000 phdu-2.3.8/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2024-04-29 12:09:18.389218 phdu-2.3.8/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-07-31 18:53:26.000000 phdu-2.3.8/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.385885 phdu-2.3.8/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      590 2024-02-24 02:21:10.000000 phdu-2.3.8/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1948 2023-09-21 17:52:42.000000 phdu-2.3.8/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2484 2024-02-04 05:18:27.000000 phdu-2.3.8/phdu/analysis.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3664 2023-10-17 21:07:41.000000 phdu-2.3.8/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1333 2023-12-05 04:36:26.000000 phdu-2.3.8/phdu/geometry.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3183 2024-01-23 06:00:25.000000 phdu-2.3.8/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     6214 2024-04-07 07:28:04.000000 phdu-2.3.8/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4011 2023-12-05 02:04:31.000000 phdu-2.3.8/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    23237 2024-04-29 12:08:17.000000 phdu-2.3.8/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    32282 2024-01-18 07:19:52.000000 phdu-2.3.8/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4437 2024-02-24 02:19:42.000000 phdu-2.3.8/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2864 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      786 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        5 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2024-04-29 12:09:18.389218 phdu-2.3.8/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1659 2024-04-29 12:08:50.000000 phdu-2.3.8/setup.py
```

### Comparing `phdu-2.3.7/LICENSE.md` & `phdu-2.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/PKG-INFO` & `phdu-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.7
+Version: 2.3.8
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.7/README.md` & `phdu-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/__init__.py` & `phdu-2.3.8/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/_helper.py` & `phdu-2.3.8/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/analysis.py` & `phdu-2.3.8/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/clustering.py` & `phdu-2.3.8/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/decomposition.py` & `phdu-2.3.8/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/geometry.py` & `phdu-2.3.8/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/np_utils.py` & `phdu-2.3.8/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/pd_utils.py` & `phdu-2.3.8/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/plots/base.py` & `phdu-2.3.8/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/plots/plotly_utils.py` & `phdu-2.3.8/phdu/plots/plotly_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     fig.update_layout(xaxis=dict(tickmode='array', ticktext=ticktext, tickvals=np.arange(ss.size)))
 
     fig.update_layout(plot_bgcolor='white', yaxis=dict(showline=True, linecolor='black', linewidth=2.4),
                       xaxis=dict(showline=True, linecolor='black', linewidth=2.4))
     fig.add_hline(y=0, line=dict(color='black', width=1, dash='dash'))
     return fig
 
-def CI_bar_plot(df, *, x, group, base, y_label, group_order=None, x_order=None, width=0.5, y_range=[0, 1], baseline_in_legend=True, default_x_order='descending', default_group_order='descending', format_label=True):
+def CI_bar_plot(df, *, x, group, base, y_label, color=None, group_order=None, x_order=None, width=0.5, y_range=[0, 1], baseline_in_legend=True, default_x_order='descending', default_group_order='descending', format_label=True):
     """
     This function creates a bar plot with confidence intervals (CI) for a given DataFrame. For each 'x' value, the plot shows a bar for each 'group' value, with the height of the bar representing the sample statistic and the CI represented by the error bars. The baseline value is also plotted as a gray bar.
 
     Parameters:
     df (pandas.DataFrame): The DataFrame containing the data to be plotted. Must have columns for 'x', 'group', 'sample_stat', 'CI', and 'base'.
     x (str): The column name in df to be used as the x-axis.
     group (str): The column name in df to be used for grouping the data.
@@ -293,19 +293,25 @@
     assert set(df[x].values) >= set(x_order), f"x_order must be a subset of the unique values in df['{x}']"
 
     X = np.arange(df.index.size)
     num_groups = len(group_order)
     width /= num_groups
     X0 = X - (num_groups-1)*width
 
-    if num_groups > 2:
-        color_gen = plotly_default_colors()
+    if color is not None:
+        if isinstance(color, str) and color in df.columns:
+            colors = df.set_index(group_order)[color].to_dict()
+        else:
+            colors = {g: c for g, c in zip(group_order, color)}
     else:
-        color_gen = plotly_default_colors(4)[1:]
-    colors = {k: c for k, c in zip(group_order, color_gen)}
+        if num_groups > 2:
+            color_gen = plotly_default_colors()
+        else:
+            color_gen = plotly_default_colors(4)[1:]
+        colors = {k: c for k, c in zip(group_order, color_gen)}
 
     fig = get_figure(xaxis_title=label_fmt(x), yaxis_title=label_fmt(y_label))
     xaxis_ticktext = []
     for i, idx in enumerate(x_order):
         df_i = df[df[x] == idx]
         xaxis_ticktext.append(idx)
         for j, g in enumerate(group_order):
```

### Comparing `phdu-2.3.7/phdu/script_fmt.py` & `phdu-2.3.8/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/_integration.py` & `phdu-2.3.8/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/_plots.py` & `phdu-2.3.8/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/bootstrap.py` & `phdu-2.3.8/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/conf_interval.py` & `phdu-2.3.8/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/corr.py` & `phdu-2.3.8/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/rtopy/_helper.py` & `phdu-2.3.8/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/rtopy/resample.py` & `phdu-2.3.8/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/stats/test/permutation.py` & `phdu-2.3.8/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu/storage.py` & `phdu-2.3.8/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/phdu.egg-info/PKG-INFO` & `phdu-2.3.8/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.7
+Version: 2.3.8
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.7/phdu.egg-info/SOURCES.txt` & `phdu-2.3.8/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.3.7/setup.py` & `phdu-2.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.3.7',
+    version='2.3.8',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

