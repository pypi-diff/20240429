# Comparing `tmp/octree_creation_app-0.1.0a5.tar.gz` & `tmp/octree_creation_app-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octree_creation_app-0.1.0a5.tar", max compression
+gzip compressed data, was "octree_creation_app-0.1.0rc1.tar", max compression
```

## Comparing `octree_creation_app-0.1.0a5.tar` & `octree_creation_app-0.1.0rc1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1093 2024-01-31 20:07:52.083349 octree_creation_app-0.1.0a5/LICENSE
--rw-r--r--   0        0        0      549 2024-03-15 18:40:12.640049 octree_creation_app-0.1.0a5/octree_creation_app/__init__.py
--rw-r--r--   0        0        0     5226 2024-01-31 20:07:52.119802 octree_creation_app-0.1.0a5/octree_creation_app/constants.py
--rw-r--r--   0        0        0    12030 2024-01-31 20:07:52.119802 octree_creation_app-0.1.0a5/octree_creation_app/driver.py
--rw-r--r--   0        0        0     4858 2024-01-31 20:07:52.120803 octree_creation_app-0.1.0a5/octree_creation_app/params.py
--rw-r--r--   0        0        0    10575 2024-01-31 20:07:52.120803 octree_creation_app-0.1.0a5/octree_creation_app/utils.py
--rw-r--r--   0        0        0      129 2024-01-02 21:13:20.166437 octree_creation_app-0.1.0a5/octree_creation_app-assets/__init__.py
--rw-r--r--   0        0        0     5835 2024-01-31 20:07:52.118802 octree_creation_app-0.1.0a5/octree_creation_app-assets/uijson/octree_mesh.ui.json
--rw-r--r--   0        0        0     3548 2024-03-15 18:40:12.640049 octree_creation_app-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     6757 2024-03-14 21:19:30.027180 octree_creation_app-0.1.0a5/README.rst
--rw-r--r--   0        0        0     8000 1970-01-01 00:00:00.000000 octree_creation_app-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-23 22:39:47.968398 octree_creation_app-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      546 2024-04-28 22:08:16.725627 octree_creation_app-0.1.0rc1/octree_creation_app/__init__.py
+-rw-r--r--   0        0        0     5941 2024-04-23 22:39:48.020389 octree_creation_app-0.1.0rc1/octree_creation_app/constants.py
+-rw-r--r--   0        0        0    12658 2024-04-23 22:39:48.021396 octree_creation_app-0.1.0rc1/octree_creation_app/driver.py
+-rw-r--r--   0        0        0     7387 2024-04-23 22:39:48.021396 octree_creation_app-0.1.0rc1/octree_creation_app/params.py
+-rw-r--r--   0        0        0    10575 2024-04-23 22:39:48.021396 octree_creation_app-0.1.0rc1/octree_creation_app/utils.py
+-rw-r--r--   0        0        0      257 2024-04-27 20:33:15.394101 octree_creation_app-0.1.0rc1/octree_creation_app-assets/__init__.py
+-rw-r--r--   0        0        0     7887 2024-04-23 22:39:48.019158 octree_creation_app-0.1.0rc1/octree_creation_app-assets/uijson/octree_mesh.ui.json
+-rw-r--r--   0        0        0     3966 2024-04-28 22:08:16.738775 octree_creation_app-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6757 2024-04-23 22:39:47.969567 octree_creation_app-0.1.0rc1/README.rst
+-rw-r--r--   0        0        0     4928 2024-04-23 22:39:47.969567 octree_creation_app-0.1.0rc1/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 octree_creation_app-0.1.0rc1/PKG-INFO
```

### Comparing `octree_creation_app-0.1.0a5/LICENSE` & `octree_creation_app-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `octree_creation_app-0.1.0a5/octree_creation_app/__init__.py` & `octree_creation_app-0.1.0rc1/octree_creation_app/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 
 from __future__ import annotations
 
 from pathlib import Path
 
 from geoapps_utils.importing import assets_path as assets_path_impl
 
-__version__ = "0.1.0-alpha.5"
+__version__ = "0.1.0-rc.1"
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
 
     return assets_path_impl(__file__)
```

### Comparing `octree_creation_app-0.1.0a5/octree_creation_app/constants.py` & `octree_creation_app-0.1.0rc1/octree_creation_app/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,15 @@
     "u_cell_size": 25.0,
     "v_cell_size": 25.0,
     "w_cell_size": 25.0,
     "horizontal_padding": 1000.0,
     "vertical_padding": 1000.0,
     "depth_core": 500.0,
     "ga_group_name": "Octree_Mesh",
-    "generate_sweep": False,
-    "run_command": "geoapps.octree_creation_app.driver",
+    "run_command": "octree_creation_app.driver",
     "monitoring_directory": None,
     "workspace_geoh5": None,
     "conda_environment": "geoapps",
     "conda_environment_boolean": False,
 }
 
 default_ui_json = deepcopy(base_ui_json)
@@ -79,59 +78,59 @@
         },
         "horizontal_padding": {
             "enabled": True,
             "group": "3- Padding distance",
             "label": "Horizontal (m)",
             "main": True,
             "value": 1000.0,
+            "tooltip": "Horizontal distance added around the 'Core hull extent'.",
         },
         "vertical_padding": {
             "enabled": True,
             "group": "3- Padding distance",
             "label": "Vertical (m)",
             "main": True,
             "value": 1000.0,
+            "tooltip": "Vertical distance of the mesh added above and below "
+            "the 'Core hull extent'.",
         },
         "depth_core": {
             "enabled": True,
             "group": "1- Core",
             "label": "Minimum Depth (m)",
             "main": True,
             "value": 500.0,
+            "tooltip": "Depth of the mesh below the core hull extent.",
         },
         "diagonal_balance": {
             "group": "Basic",
-            "label": "UBC Compatible",
+            "label": "Diagonal Balance",
             "main": True,
             "value": True,
+            "tooltip": "Assure single octree level change on corner neighbours. "
+            "Makes a UBC compatible mesh.",
         },
         "minimum_level": {
             "enabled": True,
             "group": "Basic",
             "label": "Minimum refinement level.",
             "main": True,
             "min": 1,
-            "tooltip": "Minimum refinement in padding region: 2**(n-1) x base_cell.",
+            "tooltip": "Minimum refinement in padding region: 2**(n-1) x 'core cell size'.",
             "value": 4,
         },
         "ga_group_name": {
             "enabled": True,
             "group": None,
             "label": "Name:",
             "value": "Octree_Mesh",
         },
-        "generate_sweep": {
-            "label": "Generate sweep file",
-            "group": "Python run preferences",
-            "main": True,
-            "value": False,
-        },
         "conda_environment": "geoapps",
         "workspace_geoh5": None,
-        "run_command": "geoapps.octree_creation_app.driver",
+        "run_command": "octree_creation_app.driver",
     }
 )
 
 template_dict: dict[str, dict] = {
     "object": {
         "groupOptional": True,
         "enabled": False,
@@ -143,28 +142,37 @@
             "{F26FEBA3-ADED-494B-B9E9-B2BBCBE298E1}",
             "{b99bd6e5-4fe1-45a5-bd2f-75fc31f91b38}",
             "{0b639533-f35b-44d8-92a8-f70ecff3fd26}",
             "{9b08bb5a-300c-48fe-9007-d206f971ea92}",
             "{19730589-fd28-4649-9de0-ad47249d9aba}",
         ],
         "value": None,
+        "tooltip": "Object used to refine the mesh. Refinement strategy varies "
+        "depending on the object type. See documentation for details.",
     },
     "levels": {
-        "enabled": False,
+        "enabled": True,
         "group": "Refinement A",
         "label": "Levels",
         "value": "4, 4, 4",
+        "tooltip": "Number of consecutive cells requested at each octree level. "
+        "See documentation for details.",
     },
-    "type": {
-        "choiceList": ["surface", "radial"],
-        "enabled": False,
+    "horizon": {
+        "enabled": True,
         "group": "Refinement A",
-        "label": "Type",
-        "value": "radial",
+        "label": "Use as horizon",
+        "tooltip": "Object vertices are triangulated. Refinement levels are "
+        "applied as depth layers.",
+        "value": False,
     },
     "distance": {
         "enabled": False,
         "group": "Refinement A",
+        "dependency": "horizon",
+        "dependencyType": "enabled",
         "label": "Distance",
+        "tooltip": "Radial horizontal distance to extend the refinement "
+        "around each vertex.",
         "value": 1000.0,
     },
 }
```

### Comparing `octree_creation_app-0.1.0a5/octree_creation_app/driver.py` & `octree_creation_app-0.1.0rc1/octree_creation_app/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys
 
 import numpy as np
 from discretize import TreeMesh
 from discretize.utils import mesh_builder_xyz
 from geoapps_utils.driver.driver import BaseDriver
 from geoapps_utils.locations import get_locations
-from geoh5py.objects import Curve, ObjectBase, Octree, Surface
+from geoh5py.objects import Curve, ObjectBase, Octree, Points, Surface
 from geoh5py.shared.utils import fetch_active_workspace
 from geoh5py.ui_json import utils
 from scipy import interpolate
 from scipy.spatial import Delaunay, cKDTree
 
 from octree_creation_app.params import OctreeParams
 from octree_creation_app.utils import densify_curve, treemesh_2_octree
@@ -75,44 +75,44 @@
             refinement_object = getattr(params, value["object"])
             levels = utils.str2list(getattr(params, value["levels"]))
             if not isinstance(refinement_object, ObjectBase):
                 continue
 
             print(f"Applying {label} on: {getattr(params, value['object']).name}")
 
-            if isinstance(refinement_object, Curve):
+            if getattr(params, value["horizon"]):
+                mesh = OctreeDriver.refine_tree_from_surface(
+                    mesh,
+                    refinement_object,
+                    levels,
+                    params.diagonal_balance,
+                    max_distance=getattr(params, value["distance"]),
+                )
+
+            elif isinstance(refinement_object, Curve):
                 mesh = OctreeDriver.refine_tree_from_curve(
                     mesh, refinement_object, levels, params.diagonal_balance
                 )
 
             elif isinstance(refinement_object, Surface):
                 mesh = OctreeDriver.refine_tree_from_triangulation(
                     mesh, refinement_object, levels, params.diagonal_balance
                 )
 
-            elif getattr(params, value["type"]) == "surface":
-                mesh = OctreeDriver.refine_tree_from_surface(
-                    mesh,
-                    refinement_object,
-                    levels,
-                    params.diagonal_balance,
-                    max_distance=getattr(params, value["distance"]),
-                )
-
-            elif getattr(params, value["type"]) == "radial":
+            elif isinstance(refinement_object, Points):
                 mesh = OctreeDriver.refine_tree_from_points(
                     mesh,
                     refinement_object,
                     levels,
                     diagonal_balance=params.diagonal_balance,
                 )
 
             else:
                 raise NotImplementedError(
-                    f"Refinement type {value['type']} is not implemented."
+                    f"Refinement for object {type(refinement_object)} is not implemented."
                 )
 
         print("Finalizing . . .")
         mesh.finalize()
         octree = treemesh_2_octree(params.geoh5, mesh, name=params.ga_group_name)
 
         return octree
@@ -228,17 +228,14 @@
         if isinstance(levels, list):
             levels = np.array(levels)
 
         xyz = get_locations(surface.workspace, surface)
         triang = Delaunay(xyz[:, :2])
         tree = cKDTree(xyz[:, :2])
 
-        if isinstance(surface, Surface):
-            triang.simplices = surface.cells
-
         interp = interpolate.LinearNDInterpolator(triang, xyz[:, -1])
         levels = np.array(levels)
 
         depth = 0
         # Cycle through the Tree levels backward
         for ind, n_cells in enumerate(levels):
             if n_cells == 0:
@@ -297,34 +294,49 @@
         :param finalize: Finalize the tree mesh after refinement.
 
         :return: Refined tree mesh.
         """
         if not isinstance(surface, Surface):
             raise TypeError("Refinement object must be a Surface.")
 
+        if surface.vertices is None or surface.cells is None:
+            raise ValueError("Surface object must have vertices and cells.")
+
         if isinstance(levels, list):
             levels = np.array(levels)
 
-        ind = np.where(np.r_[levels] > 0)[0]
+        vertices = surface.vertices.copy()
+        normals = np.cross(
+            vertices[surface.cells[:, 1], :] - vertices[surface.cells[:, 0], :],
+            vertices[surface.cells[:, 2], :] - vertices[surface.cells[:, 0], :],
+        )
+        average_normals = np.zeros((surface.n_vertices, 3))
+
+        for vert_ids in surface.cells.T:
+            average_normals[vert_ids, :] += normals
+
+        average_normals /= np.linalg.norm(average_normals, axis=1)[:, None]
+
+        base_cells = np.r_[mesh.h[0][0], mesh.h[1][0], mesh.h[2][0]]
+        for level, n_cells in enumerate(levels):
+            if n_cells == 0:
+                continue
+
+            for _ in range(int(n_cells)):
+                mesh.refine_surface(
+                    (vertices, surface.cells),
+                    level=-level - 1,
+                    diagonal_balance=diagonal_balance,
+                    finalize=False,
+                )
+                vertices -= average_normals * base_cells * 2.0**level
+
+        if finalize:
+            mesh.finalize()
 
-        if any(ind):
-            paddings = []
-            for n_cells in levels[ind[0] :]:
-                if n_cells == 0:
-                    continue
-
-                paddings.append([n_cells] * 3)
-
-            mesh.refine_surface(
-                (surface.vertices, surface.cells),
-                -ind[0] - 1,
-                paddings,
-                diagonal_balance=diagonal_balance,
-                finalize=finalize,
-            )
         return mesh
 
     @staticmethod
     def cell_size_from_level(octree, level: int, axis: int = 0):
         """
         Computes the cell size at a given level of refinement for a given tree mesh.
```

### Comparing `octree_creation_app-0.1.0a5/octree_creation_app/utils.py` & `octree_creation_app-0.1.0rc1/octree_creation_app/utils.py`

 * *Files identical despite different names*

### Comparing `octree_creation_app-0.1.0a5/octree_creation_app-assets/uijson/octree_mesh.ui.json` & `octree_creation_app-0.1.0rc1/octree_creation_app-assets/uijson/octree_mesh.ui.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.674404761904762%*

 * *Differences: {"'Refinement A distance'": "{'enabled': False, 'value': 1000.0, 'dependency': 'Refinement A "*

 * *                            "horizon', 'dependencyType': 'enabled', 'tooltip': 'Radial horizontal "*

 * *                            "distance to extend the refinement around each vertex.'}",*

 * * "'Refinement A horizon'": "OrderedDict([('enabled', False), ('group', 'Refinement A'), ('label', "*

 * *                           "'Use as horizon'), ('tooltip', 'Object vertices are triangulated. "*

 * *                           "Refine […]*

```diff
@@ -1,19 +1,30 @@
 {
     "Refinement A distance": {
-        "enabled": true,
+        "dependency": "Refinement A horizon",
+        "dependencyType": "enabled",
+        "enabled": false,
         "group": "Refinement A",
         "label": "Distance",
-        "value": ""
+        "tooltip": "Radial horizontal distance to extend the refinement around each vertex.",
+        "value": 1000.0
+    },
+    "Refinement A horizon": {
+        "enabled": false,
+        "group": "Refinement A",
+        "label": "Use as horizon",
+        "tooltip": "Object vertices are triangulated. Refinement levels are applied as depth layers.",
+        "value": false
     },
     "Refinement A levels": {
         "enabled": true,
         "group": "Refinement A",
         "label": "Levels",
-        "value": ""
+        "tooltip": "Number of consecutive cells requested at each octree level. See documentation for details.",
+        "value": "4,4,4"
     },
     "Refinement A object": {
         "enabled": false,
         "group": "Refinement A",
         "groupOptional": true,
         "label": "Object",
         "meshType": [
@@ -21,37 +32,39 @@
             "{6a057fdc-b355-11e3-95be-fd84a7ffcb88}",
             "{f26feba3-aded-494b-b9e9-b2bbcbe298e1}",
             "{b99bd6e5-4fe1-45a5-bd2f-75fc31f91b38}",
             "{0b639533-f35b-44d8-92a8-f70ecff3fd26}",
             "{9b08bb5a-300c-48fe-9007-d206f971ea92}",
             "{19730589-fd28-4649-9de0-ad47249d9aba}"
         ],
-        "value": ""
-    },
-    "Refinement A type": {
-        "choiceList": [
-            "surface",
-            "radial"
-        ],
-        "enabled": true,
-        "group": "Refinement A",
-        "label": "Type",
+        "tooltip": "Object used to refine the mesh. Refinement strategy varies depending on the object type. See documentation for details.",
         "value": ""
     },
     "Refinement B distance": {
-        "enabled": true,
+        "dependency": "Refinement B horizon",
+        "dependencyType": "enabled",
+        "enabled": false,
         "group": "Refinement B",
         "label": "Distance",
-        "value": ""
+        "tooltip": "Radial horizontal distance to extend the refinement around each vertex.",
+        "value": 1000.0
+    },
+    "Refinement B horizon": {
+        "enabled": false,
+        "group": "Refinement B",
+        "label": "Use as horizon",
+        "tooltip": "Object vertices are triangulated. Refinement levels are applied as depth layers.",
+        "value": false
     },
     "Refinement B levels": {
         "enabled": true,
         "group": "Refinement B",
         "label": "Levels",
-        "value": ""
+        "tooltip": "Number of consecutive cells requested at each octree level. See documentation for details.",
+        "value": "0,0,2"
     },
     "Refinement B object": {
         "enabled": false,
         "group": "Refinement B",
         "groupOptional": true,
         "label": "Object",
         "meshType": [
@@ -59,36 +72,38 @@
             "{6a057fdc-b355-11e3-95be-fd84a7ffcb88}",
             "{f26feba3-aded-494b-b9e9-b2bbcbe298e1}",
             "{b99bd6e5-4fe1-45a5-bd2f-75fc31f91b38}",
             "{0b639533-f35b-44d8-92a8-f70ecff3fd26}",
             "{9b08bb5a-300c-48fe-9007-d206f971ea92}",
             "{19730589-fd28-4649-9de0-ad47249d9aba}"
         ],
-        "value": ""
-    },
-    "Refinement B type": {
-        "choiceList": [
-            "surface",
-            "radial"
-        ],
-        "enabled": true,
-        "group": "Refinement B",
-        "label": "Type",
+        "tooltip": "Object used to refine the mesh. Refinement strategy varies depending on the object type. See documentation for details.",
         "value": ""
     },
     "Refinement C distance": {
-        "enabled": true,
+        "dependency": "Refinement C horizon",
+        "dependencyType": "enabled",
+        "enabled": false,
         "group": "Refinement C",
         "label": "Distance",
-        "value": ""
+        "tooltip": "Radial horizontal distance to extend the refinement around each vertex.",
+        "value": 1000.0
+    },
+    "Refinement C horizon": {
+        "enabled": false,
+        "group": "Refinement C",
+        "label": "Use as horizon",
+        "tooltip": "Object vertices are triangulated. Refinement levels are applied as depth layers.",
+        "value": false
     },
     "Refinement C levels": {
         "enabled": true,
         "group": "Refinement C",
         "label": "Levels",
+        "tooltip": "Number of consecutive cells requested at each octree level. See documentation for details.",
         "value": ""
     },
     "Refinement C object": {
         "enabled": false,
         "group": "Refinement C",
         "groupOptional": true,
         "label": "Object",
@@ -97,55 +112,58 @@
             "{6a057fdc-b355-11e3-95be-fd84a7ffcb88}",
             "{f26feba3-aded-494b-b9e9-b2bbcbe298e1}",
             "{b99bd6e5-4fe1-45a5-bd2f-75fc31f91b38}",
             "{0b639533-f35b-44d8-92a8-f70ecff3fd26}",
             "{9b08bb5a-300c-48fe-9007-d206f971ea92}",
             "{19730589-fd28-4649-9de0-ad47249d9aba}"
         ],
-        "value": ""
-    },
-    "Refinement C type": {
-        "choiceList": [
-            "surface",
-            "radial"
-        ],
-        "enabled": true,
-        "group": "Refinement C",
-        "label": "Type",
+        "tooltip": "Object used to refine the mesh. Refinement strategy varies depending on the object type. See documentation for details.",
         "value": ""
     },
     "conda_environment": "octree_creation_app",
     "conda_environment_boolean": false,
     "depth_core": {
         "enabled": true,
         "group": "1- Core",
         "label": "Minimum Depth (m)",
         "main": true,
+        "tooltip": "Depth of the mesh below the core hull extent.",
         "value": 500.0
     },
+    "diagonal_balance": {
+        "group": "Basic",
+        "label": "Diagonal Balance",
+        "main": true,
+        "tooltip": "Assure single octree level change on corner neighbours. UBC compatible mesh.",
+        "value": true
+    },
     "ga_group_name": {
         "enabled": true,
         "group": "",
         "label": "Name:",
         "value": "Octree_Mesh"
     },
-    "generate_sweep": {
-        "group": "Python run preferences",
-        "label": "Generate sweep file",
-        "main": true,
-        "value": false
-    },
     "geoh5": "",
     "horizontal_padding": {
         "enabled": true,
         "group": "3- Padding distance",
         "label": "Horizontal (m)",
         "main": true,
+        "tooltip": "Horizontal distance added around the 'Core hull extent'.",
         "value": 1000.0
     },
+    "minimum_level": {
+        "enabled": true,
+        "group": "Basic",
+        "label": "Minimum refinement level.",
+        "main": true,
+        "min": 1,
+        "tooltip": "Minimum refinement in padding region: 2**(n-1) x base_cell.",
+        "value": 4
+    },
     "monitoring_directory": "",
     "objects": {
         "enabled": true,
         "group": "1- Core",
         "label": "Core hull extent",
         "main": true,
         "meshType": [
@@ -155,22 +173,22 @@
             "{b99bd6e5-4fe1-45a5-bd2f-75fc31f91b38}",
             "{0b639533-f35b-44d8-92a8-f70ecff3fd26}",
             "{9b08bb5a-300c-48fe-9007-d206f971ea92}",
             "{19730589-fd28-4649-9de0-ad47249d9aba}"
         ],
         "value": ""
     },
-    "run_command": "geoapps.octree_creation.driver",
+    "run_command": "octree_creation_app.driver",
     "run_command_boolean": {
         "label": "Run python module ",
         "main": true,
         "tooltip": "Warning: launches process to run python model on save",
         "value": false
     },
-    "title": "octree Mesh Creator",
+    "title": "Octree Mesh Creator",
     "u_cell_size": {
         "enabled": true,
         "group": "2- Core cell size",
         "label": "Easting (m)",
         "main": true,
         "value": 25.0
     },
@@ -183,14 +201,15 @@
     },
     "version": "0.1.0",
     "vertical_padding": {
         "enabled": true,
         "group": "3- Padding distance",
         "label": "Vertical (m)",
         "main": true,
+        "tooltip": "Vertical distance of the mesh added above and below the 'Core hull extent'.",
         "value": 1000.0
     },
     "w_cell_size": {
         "enabled": true,
         "group": "2- Core cell size",
         "label": "Vertical (m)",
         "main": true,
```

### Comparing `octree_creation_app-0.1.0a5/pyproject.toml` & `octree_creation_app-0.1.0rc1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 [tool.poetry]
 name = "octree-creation-app"
-version = "0.1.0-alpha.5"
+version = "0.1.0-rc.1"
 license = "MIT"
 description = "Octree creation app."
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
+maintainers = ["Dominique Fournier <dominiquef@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/octree-creation-app"
-homepage = "https://mirageoscience-octree-creation-app.readthedocs-hosted.com/en/latest/"
+documentation  = "https://mirageoscience-octree-creation-app.readthedocs-hosted.com/"
+homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
+
 readme = "README.rst"
 
 packages = [
      { include = "octree_creation_app" },
      { include = "octree_creation_app-assets" },
 ]
 
+include = [
+    "COPYING",
+    "COPYING.LESSER",
+    "LICENSE",
+    "README.rst",
+    "THIRD_PARTY_SOFTWARE.rst",
+]
+
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
@@ -27,38 +38,44 @@
     "Natural Language :: English",
 ]
 
 [tool.poetry.scripts]
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.11"
-numpy = "~1.23.5"  # also geoh5py
-scipy = "~1.10.1"
+
 discretize = "~0.10.0"
+numpy = "~1.23.5"  # also in geoh5py
+scipy = "~1.10.1"
 
-## pip dependencies
-geoh5py = {version = "~0.9.0-alpha.1", source = "pypi", allow-prereleases = true}
-#geoh5py = { url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/main.tar.gz#sha256=" }
-#geoapps-utils = { url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.2.0.tar.gz#sha256=" }
-geoapps-utils = { version = "~0.3.0-alpha.1", source = "pypi", allow-prereleases = true}
+## Pip dependencies from Git repositories
+#------------------------------------
+geoh5py = {version = "~0.9.0rc1", source = "pypi", allow-prereleases = true}
+#geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
+#geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
+
+geoapps-utils = { version = "~0.3.0rc1", source = "pypi", allow-prereleases = true}
+#geoapps-utils = { url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.3.0.zip#sha256=" }
+#geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
+#---------------------------------------------------------------------------------
 h5py = "^3.2.1"  # from geoh5py
-Pillow = "^10.0.1"  # from geoh5py
+Pillow = "~10.1.0"  # from geoh5py
 
 ## about pip dependencies
 # to be specified to work with conda-lock
 # - from PyPI: my_package = { version = "1.2.3", source = "pypi" }
 # - from URL:
 #   - for a tags:   my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/tags/VERSION_TAG.zip#sha256=" }
 #   - for a branch: my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/heads/BRANCH.zip#sha256=" }
 # Note - conda-lock does not support the syntax: my_package = { git = ... }
 #        while poetry2conda supports only { git = "...", tag = "..." }, and not { url = ... }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 Pygments = "*"
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 tomli = "*"
 
 [tool.conda-lock]
@@ -81,37 +98,33 @@
 ignore_missing_imports = true
 scripts_are_modules = true
 show_error_context = true
 show_column_numbers = true
 check_untyped_defs = true
 
 plugins = [
-#    'numpy.typing.mypy_plugin'
+    'numpy.typing.mypy_plugin'
 ]
 
 [tool.pytest.ini_options]
-addopts = "--cov octree_creation_app --cov-report html --cov-report term-missing:skip-covered"
+#addopts =
 
 [tool.coverage.run]
 branch = true
 source = ["octree_creation_app"]
-omit = [
-    "octree_creation_app/commands/hello_world.py"
-]
+omit = []
 
 [tool.coverage.report]
 exclude_lines = [
     "raise NotImplementedError",
     "pass",
     "if TYPE_CHECKING",
     "pragma: no cover"
 ]
 
-fail_under = 80
-
 [tool.coverage.html]
 skip_empty = true
 skip_covered = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `octree_creation_app-0.1.0a5/README.rst` & `octree_creation_app-0.1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `octree_creation_app-0.1.0a5/PKG-INFO` & `octree_creation_app-0.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: octree-creation-app
-Version: 0.1.0a5
+Version: 0.1.0rc1
 Summary: Octree creation app.
-Home-page: https://mirageoscience-octree-creation-app.readthedocs-hosted.com/en/latest/
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
+Maintainer: Dominique Fournier
+Maintainer-email: dominiquef@mirageoscience.com
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,21 +20,22 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: Pillow (>=10.0.1,<11.0.0)
+Requires-Dist: Pillow (>=10.1.0,<10.2.0)
 Requires-Dist: discretize (>=0.10.0,<0.11.0)
-Requires-Dist: geoapps-utils (>=0.3.0-alpha.1,<0.4.0)
-Requires-Dist: geoh5py (>=0.9.0-alpha.1,<0.10.0)
+Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
+Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
+Project-URL: Documentation, https://mirageoscience-octree-creation-app.readthedocs-hosted.com/
 Project-URL: Repository, https://github.com/MiraGeoscience/octree-creation-app
 Description-Content-Type: text/x-rst
 
 |coverage| |maintainability| |precommit_ci| |style| |version| |status| |pyversions|
 
 .. |docs| image:: https://readthedocs.org/projects/octree-creation-app/badge/
     :alt: Documentation Status
```

