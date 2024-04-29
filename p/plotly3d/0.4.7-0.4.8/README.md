# Comparing `tmp/plotly3d-0.4.7.tar.gz` & `tmp/plotly3d-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.4.7.tar", last modified: Thu Apr 25 23:14:34 2024, max compression
+gzip compressed data, was "plotly3d-0.4.8.tar", last modified: Mon Apr 29 14:39:06 2024, max compression
```

## Comparing `plotly3d-0.4.7.tar` & `plotly3d-0.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:14:34.003493 plotly3d-0.4.7/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.7/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:14:34.003024 plotly3d-0.4.7/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      118 2024-04-25 22:33:15.000000 plotly3d-0.4.7/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:14:34.000658 plotly3d-0.4.7/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.7/plotly3d/__init__.py
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     9167 2024-04-25 23:14:09.000000 plotly3d-0.4.7/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-25 23:14:34.002548 plotly3d-0.4.7/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      328 2024-04-25 23:14:33.000000 plotly3d-0.4.7/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-25 23:14:33.000000 plotly3d-0.4.7/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-25 23:14:33.000000 plotly3d-0.4.7/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-25 23:14:33.000000 plotly3d-0.4.7/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-25 23:14:33.000000 plotly3d-0.4.7/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-25 23:14:34.003820 plotly3d-0.4.7/setup.cfg
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      422 2024-04-25 23:14:16.000000 plotly3d-0.4.7/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-29 14:39:06.155554 plotly3d-0.4.8/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.8/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     2896 2024-04-29 14:39:06.154674 plotly3d-0.4.8/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     2430 2024-04-29 14:37:32.000000 plotly3d-0.4.8/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-29 14:39:06.149876 plotly3d-0.4.8/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.8/plotly3d/__init__.py
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9227 2024-04-29 14:37:32.000000 plotly3d-0.4.8/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-29 14:39:06.153817 plotly3d-0.4.8/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     2896 2024-04-29 14:39:05.000000 plotly3d-0.4.8/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-29 14:39:05.000000 plotly3d-0.4.8/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-29 14:39:05.000000 plotly3d-0.4.8/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-29 14:39:05.000000 plotly3d-0.4.8/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-29 14:39:05.000000 plotly3d-0.4.8/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-29 14:39:06.155734 plotly3d-0.4.8/setup.cfg
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      680 2024-04-29 14:38:45.000000 plotly3d-0.4.8/setup.py
```

### Comparing `plotly3d-0.4.7/LICENSE` & `plotly3d-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.4.7/plotly3d/plot.py` & `plotly3d-0.4.8/plotly3d/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 import pandas as pd
 import os
 import plotly.express as px
 import matplotlib.cm as cm
 
 
 def scatter(points, colors=None, **kwargs):
-    """
+    '''
     Plots 3D scatter plot with optional rescaling, coloring, and customization.
-    
+
     Parameters:
     - points: Array of points to plot.
     - colors: Optional array of colors for each point.
     - scaler: Optional scaler object to rescale points. If None and rescaling is enabled, MinMaxScaler is used.
     - **kwargs: Additional optional arguments:
         - s (float): Size of the markers.
         - alpha (float): Opacity of the markers.
         - force_continuous (bool): Force treating colors as continuous even if they seem categorical.
         - title (str): Title of the plot.
         - filename (str): If provided, saves the plot to this file.
         - rescale (bool): If True, rescales points using the provided or default scaler.
         - fig (go.Figure): Plotly figure object to which the scatter plot will be added. If None, a new figure is created.
         - xtitle (str), ytitle (str), ztitle (str): Titles for the X, Y, and Z axes.
-    """
+
+    Returns:
+    - Plotly figure containing the scatter points plotted in 3D space.
+    '''
+
     is_3d = points.shape[1] == 3
     plot_func = go.Scatter3d if is_3d else lambda z, **kwargs: go.Scatter(**kwargs)
     scaler = kwargs.get('scaler', None)
     s = kwargs.get('s', 1)
     alpha = kwargs.get('alpha', 1)
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
@@ -83,15 +87,15 @@
         fig.add_trace(plot_func(
             x=points_s[:, 0],
             y=points_s[:, 1],
             z=points_s[:, 2] if is_3d else None,
             mode='markers',
             marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
         ))
-    
+
     fig.data[0].marker.colorscale = colorscale
     scene=dict(xaxis_title=xtitle, yaxis_title=ytitle)
     if is_3d:
         scene['zaxis_title'] = ztitle
     fig.update_layout(
         title=title,
         scene=scene,
@@ -107,37 +111,38 @@
     if figsize is not None:
         assert len(figsize) == 2
         fig.update_layout(width=figsize[0] * 100, height=figsize[1] * 100)  # width and height in pixels
 
     if white_bkgrnd:
         fig.update_layout(
             paper_bgcolor='white',  # Color of the whole background
-            plot_bgcolor='white'        # Color of the plotting area
+            plot_bgcolor='white'    # Color of the plotting area
         )
 
     if filename is not None:
         fig.write_html(filename)
 
     return fig
 
 # for compatability with previous versions
 plot_3d = scatter
 scatter3d = scatter
 
 def trajectories(trajs, colors=None, **kwargs):
-    """
+    '''
     Plots trajectories in 3D space using Plotly, with unique colors for each category and a single legend entry per category.
 
     Parameters:
     - trajs: numpy array of shape (a, b, c), where
       a: time bins, b: trajectory index, c: space dimension (c=3 for 3D).
 
     Returns:
     - Plotly figure containing the trajectories plotted in 3D space.
-    """
+    '''
+
     is_3d = trajs.shape[2] == 3
     plot_func = go.Scatter3d if is_3d else lambda z, **kwargs: go.Scatter(**kwargs)
     s = kwargs.get('s', 1)
     s_end = kwargs.get('s_end', 1)
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
     rescale = kwargs.get('rescale', False)
@@ -160,27 +165,27 @@
     if rescale and scaler is None:
         scaler = MinMaxScaler()
         scaler.fit(trajs.reshape(-1, trajs.shape[2]))
     trajs_s = scaler.transform(trajs.reshape(-1, trajs.shape[2])).reshape(trajs.shape) if rescale else trajs
 
     color_map, categories = pd.factorize(colors, sort=True)
     cmap = cm.get_cmap(cmap, len(categories))  # Get a colormap with as many colors as categories
-    
+
     # color_map = color_map % len(color_palette)  # Ensure we use the color palette cyclically if not enough colors
 
     for i, color in enumerate(categories):
         category_color = cmap(i % 20)[:3]  # Get color from colormap, repeat if more than 20 categories
         category_color = 'rgb' + str(tuple(int(c*255) for c in category_color))  # Convert to RGB string for Plotly
         idx = color_map == i
         first_idx = np.where(idx)[0][0]
         for j in np.where(idx)[0]:
             trajectory = trajs_s[:, j, :]
             showlegend = (j == first_idx)  # Compare indices to determine if it's the first trajectory
             showlegend = bool(showlegend)  # Explicitly convert to Python bool
-            
+
             # Add the trace for the trajectory
             fig.add_trace(plot_func(
                 x=trajectory[:, 0],
                 y=trajectory[:, 1],
                 z=trajectory[:, 2] if is_3d else None,
                 mode= 'lines',  # Add markers only for the first trajectory
                 line=dict(width=s, color=category_color),
@@ -221,7 +226,8 @@
             plot_bgcolor='white'        # Color of the plotting area
         )
 
     if filename is not None:
         fig.write_html(filename)
 
     return fig
+
```

