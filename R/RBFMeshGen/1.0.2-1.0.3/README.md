# Comparing `tmp/rbfmeshgen-1.0.2.tar.gz` & `tmp/rbfmeshgen-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfmeshgen-1.0.2.tar", last modified: Fri Apr 26 19:04:06 2024, max compression
+gzip compressed data, was "rbfmeshgen-1.0.3.tar", last modified: Mon Apr 29 17:13:53 2024, max compression
```

## Comparing `rbfmeshgen-1.0.2.tar` & `rbfmeshgen-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/RBFMeshGen/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/mesh_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/RBFMeshGen/visualization_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 19:04:06.000000 rbfmeshgen-1.0.2/RBFMeshGen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:04:06.911209 rbfmeshgen-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-26 19:03:56.000000 rbfmeshgen-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:13:53.318396 rbfmeshgen-1.0.3/RBFMeshGen/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/mesh_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/visualization_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/setup.py
```

### Comparing `rbfmeshgen-1.0.2/PKG-INFO` & `rbfmeshgen-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RBFMeshGen
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for generating random meshes based on radial basis functions.
 Home-page: https://github.com/LDBreton/RBFMeshGen
 Author: Louis Breton
 Author-email: louis.breton@ciencias.unam.mx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 ```
 
 
 ## Usage
 
 ```python
 import numpy as np
-from RBFMeshGen import RandomMesh, plot_mesh, Border
+from RBFMeshGen import RBFMesh, plot_mesh, Border
 
 
 # Define a parametric function for a circle
 def circle_parametric_function(radius, t):
     return radius * np.cos(t), radius * np.sin(t)
 
 
@@ -54,15 +54,15 @@
                        t_end=np.pi)
 border_outer2 = Border(parametric_function=lambda t: circle_parametric_function(outer_radius, t), label=1,
                        t_start=np.pi, t_end=2 * np.pi)
 border_inner1 = Border(parametric_function=lambda t: circle_parametric_function(inner_radius, t), label=1, t_start=0,
                        t_end=2 * np.pi)
 
 # Generate a random mesh
-random_mesh = RandomMesh(border_outer1(100), border_outer2(200), border_inner1(-100))
+random_mesh = RBFMesh(border_outer1(100), border_outer2(200), border_inner1(-100))
 
 # Generate points
 num_points = 10000
 random_mesh.generate_points(num_points)
 
 # Plot the points
 plot_mesh(random_mesh)
```

### Comparing `rbfmeshgen-1.0.2/RBFMeshGen/geometry_utils.py` & `rbfmeshgen-1.0.3/RBFMeshGen/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.2/RBFMeshGen/mesh_generation.py` & `rbfmeshgen-1.0.3/RBFMeshGen/mesh_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .geometry_utils import MeshPoint, calculate_orientation, find_polygons, Border
 from shapely.geometry import Polygon, Point
 from shapely.ops import unary_union
 from shapely import prepare
 import random
 
 
-class RandomMesh:
+class RBFMesh:
     """
-    RandomMesh class for generating random points within polygons.
+    RBFMesh class for generating random points within polygons.
 
     Args:
         *borders: Variable length argument list of Border objects representing the borders of the polygons.
         abs_tol (float, optional): Absolute tolerance for geometric calculations. Defaults to 1e-04.
 
     Attributes:
         borders (list): List of Border objects representing the borders of the polygons.
```

### Comparing `rbfmeshgen-1.0.2/RBFMeshGen/visualization_tools.py` & `rbfmeshgen-1.0.3/RBFMeshGen/visualization_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from .mesh_generation import RandomMesh
+from .mesh_generation import RBFMesh
 from .geometry_utils import MeshPoint
 
 
 def plot_each_polygon_separately(polygons):
     """
     Plot each polygon separately in a new figure.
 
@@ -103,20 +103,20 @@
     ax.set_xlabel('X Coordinate')
     ax.set_ylabel('Y Coordinate')
     plt.title(title)
     plt.axis('equal')  # Set equal scaling by changing axis limits
     plt.show()
 
 
-def plot_mesh(mesh: RandomMesh, border_size=5, interior_size=2, title='Random Mesh Points by Label'):
+def plot_mesh(mesh: RBFMesh, border_size=5, interior_size=2, title='Random Mesh Points by Label'):
     """
     Plot points with different labels and border status.
 
     Args:
-        mesh (list): A RandomMesh object.
+        mesh (list): A RBFMesh object.
         title (str): Title of the plot.
         border_size (int): Size of border points.
         interior_size (int): Size of interior points.
 
     Returns:
         None
     """
```

### Comparing `rbfmeshgen-1.0.2/RBFMeshGen.egg-info/PKG-INFO` & `rbfmeshgen-1.0.3/RBFMeshGen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RBFMeshGen
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for generating random meshes based on radial basis functions.
 Home-page: https://github.com/LDBreton/RBFMeshGen
 Author: Louis Breton
 Author-email: louis.breton@ciencias.unam.mx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 ```
 
 
 ## Usage
 
 ```python
 import numpy as np
-from RBFMeshGen import RandomMesh, plot_mesh, Border
+from RBFMeshGen import RBFMesh, plot_mesh, Border
 
 
 # Define a parametric function for a circle
 def circle_parametric_function(radius, t):
     return radius * np.cos(t), radius * np.sin(t)
 
 
@@ -54,15 +54,15 @@
                        t_end=np.pi)
 border_outer2 = Border(parametric_function=lambda t: circle_parametric_function(outer_radius, t), label=1,
                        t_start=np.pi, t_end=2 * np.pi)
 border_inner1 = Border(parametric_function=lambda t: circle_parametric_function(inner_radius, t), label=1, t_start=0,
                        t_end=2 * np.pi)
 
 # Generate a random mesh
-random_mesh = RandomMesh(border_outer1(100), border_outer2(200), border_inner1(-100))
+random_mesh = RBFMesh(border_outer1(100), border_outer2(200), border_inner1(-100))
 
 # Generate points
 num_points = 10000
 random_mesh.generate_points(num_points)
 
 # Plot the points
 plot_mesh(random_mesh)
```

### Comparing `rbfmeshgen-1.0.2/README.md` & `rbfmeshgen-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```
 
 
 ## Usage
 
 ```python
 import numpy as np
-from RBFMeshGen import RandomMesh, plot_mesh, Border
+from RBFMeshGen import RBFMesh, plot_mesh, Border
 
 
 # Define a parametric function for a circle
 def circle_parametric_function(radius, t):
     return radius * np.cos(t), radius * np.sin(t)
 
 
@@ -38,15 +38,15 @@
                        t_end=np.pi)
 border_outer2 = Border(parametric_function=lambda t: circle_parametric_function(outer_radius, t), label=1,
                        t_start=np.pi, t_end=2 * np.pi)
 border_inner1 = Border(parametric_function=lambda t: circle_parametric_function(inner_radius, t), label=1, t_start=0,
                        t_end=2 * np.pi)
 
 # Generate a random mesh
-random_mesh = RandomMesh(border_outer1(100), border_outer2(200), border_inner1(-100))
+random_mesh = RBFMesh(border_outer1(100), border_outer2(200), border_inner1(-100))
 
 # Generate points
 num_points = 10000
 random_mesh.generate_points(num_points)
 
 # Plot the points
 plot_mesh(random_mesh)
```

### Comparing `rbfmeshgen-1.0.2/setup.py` & `rbfmeshgen-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RBFMeshGen",
-    version="1.0.2",
+    version="1.0.3",
     author="Louis Breton",
     author_email="louis.breton@ciencias.unam.mx",
     description="A Python package for generating random meshes based on radial basis functions.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/LDBreton/RBFMeshGen",
     packages=find_packages(),
```

