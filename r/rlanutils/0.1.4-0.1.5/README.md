# Comparing `tmp/rlanutils-0.1.4.tar.gz` & `tmp/rlanutils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlanutils-0.1.4.tar", last modified: Sun Apr 28 13:18:59 2024, max compression
+gzip compressed data, was "rlanutils-0.1.5.tar", last modified: Mon Apr 29 01:46:21 2024, max compression
```

## Comparing `rlanutils-0.1.4.tar` & `rlanutils-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.674444 rlanutils-0.1.4/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 13:18:59.674303 rlanutils-0.1.4/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.4/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.670235 rlanutils-0.1.4/rlanutils/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.4/rlanutils/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.671403 rlanutils-0.1.4/rlanutils/cv/
--rw-r--r--   0 rlan       (501) staff       (20)      315 2024-04-28 08:49:41.000000 rlanutils-0.1.4/rlanutils/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     3423 2024-04-28 13:11:21.000000 rlanutils-0.1.4/rlanutils/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.4/rlanutils/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.671841 rlanutils-0.1.4/rlanutils/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.4/rlanutils/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.4/rlanutils/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.673533 rlanutils-0.1.4/rlanutils/io/
--rw-r--r--   0 rlan       (501) staff       (20)      569 2024-04-28 07:17:32.000000 rlanutils-0.1.4/rlanutils/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.4/rlanutils/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.4/rlanutils/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.4/rlanutils/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.4/rlanutils/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.673916 rlanutils-0.1.4/rlanutils/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.4/rlanutils/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.4/rlanutils/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.670787 rlanutils-0.1.4/rlanutils.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      519 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-28 13:18:59.674493 rlanutils-0.1.4/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-28 09:49:59.000000 rlanutils-0.1.4/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.195932 rlanutils-0.1.5/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 01:46:21.195770 rlanutils-0.1.5/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.5/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.191318 rlanutils-0.1.5/rlanutils/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.5/rlanutils/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.192441 rlanutils-0.1.5/rlanutils/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)      315 2024-04-28 08:49:41.000000 rlanutils-0.1.5/rlanutils/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     3430 2024-04-29 01:45:40.000000 rlanutils-0.1.5/rlanutils/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.5/rlanutils/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.193050 rlanutils-0.1.5/rlanutils/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.5/rlanutils/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.5/rlanutils/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.194772 rlanutils-0.1.5/rlanutils/io/
+-rw-r--r--   0 rlan       (501) staff       (20)      569 2024-04-28 07:17:32.000000 rlanutils-0.1.5/rlanutils/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.5/rlanutils/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.5/rlanutils/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.5/rlanutils/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.5/rlanutils/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.195352 rlanutils-0.1.5/rlanutils/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.5/rlanutils/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.5/rlanutils/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 01:46:21.191855 rlanutils-0.1.5/rlanutils.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 01:46:21.000000 rlanutils-0.1.5/rlanutils.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      519 2024-04-29 01:46:21.000000 rlanutils-0.1.5/rlanutils.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-29 01:46:21.000000 rlanutils-0.1.5/rlanutils.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-29 01:46:21.000000 rlanutils-0.1.5/rlanutils.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-29 01:46:21.000000 rlanutils-0.1.5/rlanutils.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-29 01:46:21.195976 rlanutils-0.1.5/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-29 01:45:49.000000 rlanutils-0.1.5/setup.py
```

### Comparing `rlanutils-0.1.4/rlanutils/cv/geometry.py` & `rlanutils-0.1.5/rlanutils/cv/geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Union, Tuple
 
 import numpy as np
-from scipy.spatial.transform import Rotation as R
+from scipy.spatial.transform import Rotation
 
 
 def xyzq2mat(
     x: float, y: float, z: float, qx: float, qy: float, qz: float, qw: float, as_homo: bool = False
 ) -> np.ndarray:
     """A helper function that convert xyzq (7 values) representation to transformation matrix representation.
 
@@ -29,15 +29,15 @@
         if true, the matrix will be saved as homogeneous (4x4), otherwise, it will be saved as 3x4
 
     Returns
     -------
     np.ndarray
         of shape (3, 4) if as_homo == False, otherwise, (4, 4)
     """
-    rot = R.from_quat([qx, qy, qz, qw]).as_matrix()
+    rot = Rotation.from_quat([qx, qy, qz, qw]).as_matrix()
     T = np.eye(4)
     T[:3, 3] = [x, y, z]
     T[:3, :3] = rot
     if as_homo:
         T = T[:3, :]
     return T
 
@@ -47,34 +47,33 @@
 
 
 def homo_to_points3d(points_homo: np.ndarray) -> np.ndarray:
     return points_homo[:, :3]
 
 
 class Box3d:
-    def __init__(self, position: np.ndarray, scale: np.ndarray, quat: np.ndarray) -> None:
+    def __init__(self, position: np.ndarray, scale: np.ndarray, rotation: Rotation) -> None:
         """_summary_
 
         Parameters
         ----------
         position : np.ndarray
             of shape (3, )
         scale : np.ndarray
             of shape (3, )
-        quat : np.ndarray
-            of shape (4, ), scalar-last (x, y, z, w) format
-
+        rotation : scipy.spatial.transform.Rotation
+            rotation
         Returns
         -------
         _type_
             _description_
         """
         self.position = position
         self.scale = scale
-        self.quat = quat
+        self.rotation = rotation
         self._corners = None
     
     @property
     def corners(self) -> np.ndarray:
         """
         Returns
         -------
@@ -99,20 +98,20 @@
             [0.5, -0.5, 0.5],
             [-0.5, -0.5, -0.5],
             [-0.5, 0.5, -0.5],
             [-0.5, 0.5, 0.5],
             [-0.5, -0.5, 0.5],
         ])
         corners = corners * self.scale[None]
-        corners = corners @ self.quat.as_matrix().T
+        corners = corners @ self.rotation.as_matrix().T
         corners = corners + self.position
         return corners
 
     @classmethod
     def from_pos_scale_euler(cls, pos_x: float, pos_y: float, pos_z: float, scale_x: float, scale_y: float, scale_z: float, rot_euler_x: float, rot_euler_y: float, rot_euler_z: float, degrees: bool = False):
         pos = np.array([pos_x, pos_y, pos_z], dtype=np.float32)
         scale = np.array([scale_x, scale_y, scale_z], dtype=np.float32)
-        quat = R.from_euler("XYZ", [rot_euler_x, rot_euler_y, rot_euler_z], degrees=degrees)
-        return cls(pos, scale, quat)
+        rot = Rotation.from_euler("XYZ", [rot_euler_x, rot_euler_y, rot_euler_z], degrees=degrees)
+        return cls(pos, scale, rot)
 
 
 __all__ = ["xyzq2mat", "points3d_to_homo", "homo_to_points3d", "Box3d"]
```

### Comparing `rlanutils-0.1.4/rlanutils/cv/graphics.py` & `rlanutils-0.1.5/rlanutils/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/data_structure/set.py` & `rlanutils-0.1.5/rlanutils/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/io/__init__.py` & `rlanutils-0.1.5/rlanutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/io/fs.py` & `rlanutils-0.1.5/rlanutils/io/fs.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/io/indices.py` & `rlanutils-0.1.5/rlanutils/io/indices.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/io/network.py` & `rlanutils-0.1.5/rlanutils/io/network.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/io/parallelism.py` & `rlanutils-0.1.5/rlanutils/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils/plot/color.py` & `rlanutils-0.1.5/rlanutils/plot/color.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/rlanutils.egg-info/SOURCES.txt` & `rlanutils-0.1.5/rlanutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.4/setup.py` & `rlanutils-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='rlanutils',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/rlanutils',
```

