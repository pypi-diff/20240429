# Comparing `tmp/ansys_simai_core-0.1.5.tar.gz` & `tmp/ansys_simai_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_simai_core-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_simai_core-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_simai_core-0.1.5.tar` & `ansys_simai_core-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1089 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/LICENSE
--rw-r--r--   0        0        0     5009 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/README.rst
--rw-r--r--   0        0        0     4796 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1532 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/__init__.py
--rw-r--r--   0        0        0     1146 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/client.py
--rw-r--r--   0        0        0     2397 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/design_of_experiments.py
--rw-r--r--   0        0        0     5852 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/geometry.py
--rw-r--r--   0        0        0    10158 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/mixin.py
--rw-r--r--   0        0        0     1975 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/optimization.py
--rw-r--r--   0        0        0     4901 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/post_processing.py
--rw-r--r--   0        0        0     2650 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/prediction.py
--rw-r--r--   0        0        0     3749 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/project.py
--rw-r--r--   0        0        0     6030 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/sse.py
--rw-r--r--   0        0        0     2903 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data.py
--rw-r--r--   0        0        0     2456 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data_part.py
--rw-r--r--   0        0        0     3818 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/workspace.py
--rw-r--r--   0        0        0    13489 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/client.py
--rw-r--r--   0        0        0     1146 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/__init__.py
--rw-r--r--   0        0        0    12193 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/base.py
--rw-r--r--   0        0        0     3158 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/design_of_experiments.py
--rw-r--r--   0        0        0     2638 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/downloads.py
--rw-r--r--   0        0        0    22009 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometries.py
--rw-r--r--   0        0        0    11257 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometry_utils.py
--rw-r--r--   0        0        0     4766 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/lists.py
--rw-r--r--   0        0        0     4318 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/models.py
--rw-r--r--   0        0        0    10813 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/optimizations.py
--rw-r--r--   0        0        0    30612 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/post_processings.py
--rw-r--r--   0        0        0     9794 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/predictions.py
--rw-r--r--   0        0        0     6826 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/projects.py
--rw-r--r--   0        0        0     7571 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/selection_post_processings.py
--rw-r--r--   0        0        0     9701 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/selections.py
--rw-r--r--   0        0        0    11040 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data.py
--rw-r--r--   0        0        0     2137 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data_parts.py
--rw-r--r--   0        0        0     9460 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/types.py
--rw-r--r--   0        0        0     6541 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/workspaces.py
--rw-r--r--   0        0        0     4108 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/errors.py
--rw-r--r--   0        0        0        0 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/py.typed
--rw-r--r--   0        0        0     1146 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/__init__.py
--rw-r--r--   0        0        0     9373 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/auth.py
--rw-r--r--   0        0        0     4522 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/config_file.py
--rw-r--r--   0        0        0     5970 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/configuration.py
--rw-r--r--   0        0        0     2761 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/files.py
--rw-r--r--   0        0        0     5041 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/grouping.py
--rw-r--r--   0        0        0     1627 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/misc.py
--rw-r--r--   0        0        0     4132 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/numerical.py
--rw-r--r--   0        0        0     3903 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/requests.py
--rw-r--r--   0        0        0     3084 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/sse_client.py
--rw-r--r--   0        0        0     1643 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/typing.py
--rw-r--r--   0        0        0     2118 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/validation.py
--rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ansys_simai_core-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-29 16:23:44.826218 ansys_simai_core-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5009 2024-04-29 16:23:44.826218 ansys_simai_core-0.1.6/README.rst
+-rw-r--r--   0        0        0     4796 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1532 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/__init__.py
+-rw-r--r--   0        0        0     1146 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/client.py
+-rw-r--r--   0        0        0     2397 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/design_of_experiments.py
+-rw-r--r--   0        0        0     5852 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/geometry.py
+-rw-r--r--   0        0        0    10158 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/mixin.py
+-rw-r--r--   0        0        0     1975 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/optimization.py
+-rw-r--r--   0        0        0     4901 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/post_processing.py
+-rw-r--r--   0        0        0     2650 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/prediction.py
+-rw-r--r--   0        0        0     3749 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/project.py
+-rw-r--r--   0        0        0     6030 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/sse.py
+-rw-r--r--   0        0        0     3134 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data.py
+-rw-r--r--   0        0        0     2456 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data_part.py
+-rw-r--r--   0        0        0     3818 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/api/workspace.py
+-rw-r--r--   0        0        0    13489 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/client.py
+-rw-r--r--   0        0        0     1146 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/__init__.py
+-rw-r--r--   0        0        0    12193 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/base.py
+-rw-r--r--   0        0        0     3158 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/design_of_experiments.py
+-rw-r--r--   0        0        0     2638 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/downloads.py
+-rw-r--r--   0        0        0    22009 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometries.py
+-rw-r--r--   0        0        0    11257 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometry_utils.py
+-rw-r--r--   0        0        0     4766 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/lists.py
+-rw-r--r--   0        0        0     4318 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/models.py
+-rw-r--r--   0        0        0    10812 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/optimizations.py
+-rw-r--r--   0        0        0    30612 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/post_processings.py
+-rw-r--r--   0        0        0     9794 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/predictions.py
+-rw-r--r--   0        0        0     6826 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/projects.py
+-rw-r--r--   0        0        0     7571 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/selection_post_processings.py
+-rw-r--r--   0        0        0     9701 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/selections.py
+-rw-r--r--   0        0        0    11994 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data.py
+-rw-r--r--   0        0        0     2137 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data_parts.py
+-rw-r--r--   0        0        0     9611 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/types.py
+-rw-r--r--   0        0        0     6541 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/data/workspaces.py
+-rw-r--r--   0        0        0     4108 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/errors.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/py.typed
+-rw-r--r--   0        0        0     1146 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/__init__.py
+-rw-r--r--   0        0        0     9476 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/auth.py
+-rw-r--r--   0        0        0     4522 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/config_file.py
+-rw-r--r--   0        0        0     5970 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/configuration.py
+-rw-r--r--   0        0        0     2761 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/files.py
+-rw-r--r--   0        0        0     5041 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/grouping.py
+-rw-r--r--   0        0        0     1627 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/misc.py
+-rw-r--r--   0        0        0     4132 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/numerical.py
+-rw-r--r--   0        0        0     3903 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/requests.py
+-rw-r--r--   0        0        0     3084 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/sse_client.py
+-rw-r--r--   0        0        0     1643 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/typing.py
+-rw-r--r--   0        0        0     2118 2024-04-29 16:23:44.830218 ansys_simai_core-0.1.6/src/ansys/simai/core/utils/validation.py
+-rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ansys_simai_core-0.1.6/PKG-INFO
```

### Comparing `ansys_simai_core-0.1.5/LICENSE` & `ansys_simai_core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/README.rst` & `ansys_simai_core-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/pyproject.toml` & `ansys_simai_core-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Using PDM with flit backend
 [build-system]
 requires = ["flit_core>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-simai-core"
-version = "0.1.5"
+version = "0.1.6"
 description = "A python wrapper for Ansys SimAI"
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
```

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/__init__.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/__init__.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/client.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/design_of_experiments.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/design_of_experiments.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/geometry.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/geometry.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/mixin.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/mixin.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/optimization.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/optimization.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/post_processing.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/post_processing.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/prediction.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/prediction.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/project.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/project.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/sse.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/sse.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,7 +61,12 @@
         )
 
     def compute_training_data(self, training_data_id: str) -> None:
         self._post(f"training_data/{training_data_id}/compute")
 
     def get_training_data_subset(self, project_id: str, training_data_id: str) -> Dict[str, Any]:
         return self._get(f"projects/{project_id}/data/{training_data_id}/subset")
+
+    def put_training_data_subset(self, project_id: str, training_data_id: str, subset: str) -> None:
+        return self._put(
+            f"projects/{project_id}/data/{training_data_id}/subset", json={"subset": subset}
+        )
```

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data_part.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/training_data_part.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/api/workspace.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/api/workspace.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/client.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/__init__.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/base.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/base.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/design_of_experiments.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/design_of_experiments.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/downloads.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometries.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometries.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometry_utils.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/lists.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/lists.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/models.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/models.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/optimizations.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/optimizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                 boundary_conditions={"VelocityX": 10.5},
                 outcome_constraints=["TotalForceX <= 10"],
                 n_iters=100,
             )
 
             print(results)
         """
-        workspace_id = get_id_from_identifiable(workspace, False, self._client._current_workspace)
+        workspace_id = get_id_from_identifiable(workspace, True, self._client._current_workspace)
         if not minimize and not maximize:
             raise InvalidArguments("No global coefficient to optimize.")
         objective = {}
         if minimize:
             for global_coefficient in minimize:
                 objective[global_coefficient] = {"minimize": True}
         if maximize:
```

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/post_processings.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/post_processings.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/predictions.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/predictions.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/projects.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/projects.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/selection_post_processings.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/selection_post_processings.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/selections.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/selections.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from ansys.simai.core.data.base import ComputableDataModel, Directory
 from ansys.simai.core.data.types import (
     Identifiable,
     MonitorCallback,
     NamedFile,
     Path,
+    SubsetEnum,
     get_id_from_identifiable,
     unpack_named_file,
 )
 from ansys.simai.core.errors import InvalidArguments
 
 if TYPE_CHECKING:
     from ansys.simai.core.data.projects import Project
@@ -71,26 +72,44 @@
         objects in the training data.
         """
         return [
             self._client.training_data_parts._model_from(training_data_part)
             for training_data_part in self.fields["parts"]
         ]
 
-    def get_subset(self, project: Identifiable["Project"]) -> Optional[str]:
+    def get_subset(self, project: Identifiable["Project"]) -> Optional[SubsetEnum]:
         """Get the subset that the training data belongs to, in relation to the given project.
 
         Args:
             project: ID or :class:`model <.projects.Project>` of the project to check
                 the :class:`~.projects.Project` object for, or its ID.
 
         Returns:
-            Name of the subset that the training data belongs to in the given project.
+            SubsetEnum of the subset that the training data belongs to in the given project.
+                (e.g. <SubsetEnum.VALIDATION: 'Validation'>)
         """
         project_id = get_id_from_identifiable(project, default=self._client._current_project)
-        return self._client._api.get_training_data_subset(project_id, self.id).get("subset")
+        subset_value = self._client._api.get_training_data_subset(project_id, self.id).get("subset")
+        return SubsetEnum(subset_value) if subset_value else None
+
+    def assign_subset(self, project: Identifiable["Project"], subset: SubsetEnum) -> None:
+        """Assign the training data subset in relation to a given project.
+
+        Args:
+            project: ID or :class:`model <.projects.Project>`
+            subset: SubsetEnum attribute (e.g. SubsetEnum.TRAINING) or string value (e.g. "Training").
+                Available options: (Training, Validation, Test, Ignored)
+
+        Returns:
+            None
+        """
+        if subset not in SubsetEnum.__members__.values():
+            raise InvalidArguments("Must be one of: Ignored, Training, Test, Validation.")
+        project_id = get_id_from_identifiable(project, default=self._client._current_project)
+        self._client._api.put_training_data_subset(project_id, self.id, subset)
 
     @property
     def extracted_metadata(self) -> Optional[Dict]:
         """Metadata extracted from the training data."""
         return self.fields["extracted_metadata"]
 
     def compute(self) -> None:
```

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data_parts.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/training_data_parts.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/types.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import io
 import os
 import pathlib
 from contextlib import contextmanager
+from enum import Enum
 from numbers import Number
 from typing import Any, BinaryIO, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 from requests import Response
 
 from ansys.simai.core.data.base import DataModel, DataModelType, Directory
 from ansys.simai.core.errors import InvalidArguments
@@ -258,7 +259,14 @@
         return identifiable
     elif isinstance(identifiable, str):
         return directory.get(id=identifiable)
     elif default:
         return get_object_from_identifiable(default, directory)
     else:
         raise InvalidArguments(f"Argument {identifiable} is neither a data model nor an ID string.")
+
+
+class SubsetEnum(str, Enum):
+    IGNORED = "Ignored"
+    TRAINING = "Training"
+    VALIDATION = "Validation"
+    TEST = "Test"
```

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/data/workspaces.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/data/workspaces.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/errors.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/__init__.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/auth.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,24 +174,24 @@
         self._session = session
         self._enabled = not getattr(config, "_disable_authentication", False)
         if not self._enabled:
             logger.debug("Disabling authentication logic.")
             return
         self._url_prefix = config.url
         # HACK: start with a slash to override the /v2/ on the api url
-        realm_url = urljoin(str(config.url), "/auth/realms/simai")
-        self._token_url = f"{realm_url}/protocol/openid-connect/token"
+        self._realm_url = urljoin(str(config.url), "/auth/realms/simai")
+        self._token_url = f"{self._realm_url}/protocol/openid-connect/token"
         self._organization_name = config.organization
         self._refresh_timer = None
         if config.credentials:
             auth = _AuthTokens.from_request_direct_grant(
                 self._session, self._token_url, config.credentials
             )
         else:
-            device_auth_url = f"{realm_url}/protocol/openid-connect/auth/device"
+            device_auth_url = f"{self._realm_url}/protocol/openid-connect/auth/device"
             auth_hash = None if config.disable_cache else config._auth_hash()
             auth = _get_cached_or_request_device_auth(
                 self._session, device_auth_url, self._token_url, auth_hash
             )
         self._authentication = auth
         self._schedule_auth_refresh()
 
@@ -207,15 +207,16 @@
         request_host = request.url.split("://", 1)[-1]  # ignore protocol part
         if self._enabled and request_host.startswith(self._url_prefix.host):
             is_token_expired = self._authentication.is_token_expired()
             # So the token doesn't expire during requests that upload a large amount of data
             is_request_multipart_data = "multipart/form_data" in request.headers.get(
                 "Content-Type", ""
             )
-            if is_token_expired or is_request_multipart_data:
+            is_auth_request = self._realm_url in request.url
+            if not is_auth_request and is_token_expired or is_request_multipart_data:
                 self._refresh_auth()
             request.headers["Authorization"] = f"Bearer {self._authentication.access_token}"
             request.headers["X-Org"] = self._organization_name
         return request
 
     def _refresh_auth(self):
         """Refresh the authentication."""
@@ -223,11 +224,11 @@
         self._schedule_auth_refresh()
 
     def _schedule_auth_refresh(self):
         """Schedule authentication refresh to avoids refresh token expiring if the client is idle for a long time."""
         if self._refresh_timer:
             self._refresh_timer.cancel()
         self._refresh_timer = threading.Timer(
-            self._authentication.refresh_expires_in - 30, self._refresh_auth
+            self._authentication.refresh_expires_in - 60, self._refresh_auth
         )
         self._refresh_timer.daemon = True
         self._refresh_timer.start()
```

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/config_file.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/config_file.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/configuration.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/files.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/grouping.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/grouping.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/misc.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/numerical.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/numerical.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/requests.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/requests.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/sse_client.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/typing.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/validation.py` & `ansys_simai_core-0.1.6/src/ansys/simai/core/utils/validation.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.5/PKG-INFO` & `ansys_simai_core-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-simai-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for Ansys SimAI
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

