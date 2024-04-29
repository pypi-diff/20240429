# Comparing `tmp/rok4-2.1.4.tar.gz` & `tmp/rok4-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rok4-2.1.4.tar", last modified: Tue Feb 13 16:02:24 2024, max compression
+gzip compressed data, was "rok4-2.1.5.tar", last modified: Mon Apr 29 13:57:02 2024, max compression
```

## Comparing `rok4-2.1.4.tar` & `rok4-2.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:02:24.275516 rok4-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    21863 2024-02-13 16:01:39.000000 rok4-2.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28385 2024-02-13 16:02:24.275516 rok4-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-13 16:01:39.000000 rok4-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-13 16:01:39.000000 rok4-2.1.4/README.pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-02-13 16:02:02.000000 rok4-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 16:02:24.275516 rok4-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 16:01:39.000000 rok4-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:02:24.271516 rok4-2.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:02:24.275516 rok4-2.1.4/src/rok4/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-13 16:02:02.000000 rok4-2.1.4/src/rok4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    49869 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    37553 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/tile_matrix_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-02-13 16:01:39.000000 rok4-2.1.4/src/rok4/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:02:24.275516 rok4-2.1.4/src/rok4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28385 2024-02-13 16:02:24.000000 rok4-2.1.4/src/rok4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-13 16:02:24.000000 rok4-2.1.4/src/rok4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 16:02:24.000000 rok4-2.1.4/src/rok4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-13 16:02:24.000000 rok4-2.1.4/src/rok4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 16:02:24.000000 rok4-2.1.4/src/rok4.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:02:24.275516 rok4-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)    23118 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    32062 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_tile_matrix_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    13831 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-02-13 16:01:39.000000 rok4-2.1.4/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:02.383305 rok4-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    21863 2024-04-29 13:56:20.000000 rok4-2.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28385 2024-04-29 13:57:02.383305 rok4-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-29 13:56:20.000000 rok4-2.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 13:56:20.000000 rok4-2.1.5/README.pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-29 13:56:44.000000 rok4-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:57:02.383305 rok4-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:56:20.000000 rok4-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:02.375306 rok4-2.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:02.379305 rok4-2.1.5/src/rok4/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 13:56:44.000000 rok4-2.1.5/src/rok4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50043 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37554 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/tile_matrix_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-29 13:56:20.000000 rok4-2.1.5/src/rok4/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:02.379305 rok4-2.1.5/src/rok4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28385 2024-04-29 13:57:02.000000 rok4-2.1.5/src/rok4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-29 13:57:02.000000 rok4-2.1.5/src/rok4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:57:02.000000 rok4-2.1.5/src/rok4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 13:57:02.000000 rok4-2.1.5/src/rok4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 13:57:02.000000 rok4-2.1.5/src/rok4.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:02.379305 rok4-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23118 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32062 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_tile_matrix_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13831 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-29 13:56:20.000000 rok4-2.1.5/tests/test_vector.py
```

### Comparing `rok4-2.1.4/LICENSE.txt` & `rok4-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/PKG-INFO` & `rok4-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rok4
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python core libraries for ROK4 project
 Author-email: Géoportail IGN Developers <tout_rdev@ign.fr>
 License: 
         CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
```

### Comparing `rok4-2.1.4/README.md` & `rok4-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/README.pypi.md` & `rok4-2.1.5/README.pypi.md`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/pyproject.toml` & `rok4-2.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "rok4"
-version = "2.1.4"
+version = "2.1.5"
 
 description = "Python core libraries for ROK4 project"
 readme = "README.pypi.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 
 keywords = ["ROK4", "library", "pyramid", "tile matrix set", "storage"]
```

### Comparing `rok4-2.1.4/src/rok4/enums.py` & `rok4-2.1.5/src/rok4/enums.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/src/rok4/exceptions.py` & `rok4-2.1.5/src/rok4/exceptions.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/src/rok4/layer.py` & `rok4-2.1.5/src/rok4/layer.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/src/rok4/pyramid.py` & `rok4-2.1.5/src/rok4/pyramid.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,52 +368,52 @@
             "max_col": col_max,
             "max_row": row_max,
             "min_col": col_min,
         }
 
 
 class Pyramid:
-
     """A data pyramid, raster or vector
 
     Attributes:
         __name (str): pyramid's name
         __descriptor (str): pyramid's descriptor path
         __list (str): pyramid's list path
         __tms (rok4.tile_matrix_set.TileMatrixSet): Used grid
         __levels (Dict[str, Level]): Pyramid's levels
         __format (str): Data format
         __storage (Dict[str, Union[rok4.enums.StorageType,str,int]]): Pyramid's storage informations (type, root and depth if FILE storage)
         __raster_specifications (Dict): If raster pyramid, raster specifications
-        __content (Dict): Loading status (loaded) and list content (cache).
+        __content (Dict): Loading status (loaded), slab count (count) and list content (cache).
 
             Example (S3 storage):
 
                 {
                     'cache': {
                         (<SlabType.DATA: 'DATA'>, '18', 5424, 7526): {
                             'link': False,
                             'md5': None,
                             'root': 'pyramids@localhost:9000/LIMADM',
                             'slab': 'DATA_18_5424_7526'
                         }
                     },
+                    'count': 1,
                     'loaded': True
                 }
     """
 
     @classmethod
     def from_descriptor(cls, descriptor: str) -> "Pyramid":
         """Create a pyramid from its descriptor
 
         Args:
             descriptor (str): pyramid's descriptor path
 
         Raises:
-            FormatError: Provided path or the TMS is not a well formed JSON
+            FormatError: Provided path or the descriptor is not a well formed JSON
             Exception: Level issue : no one in the pyramid or the used TMS, or level ID not defined in the TMS
             MissingAttributeError: Attribute is missing in the content
             StorageError: Storage read issue (pyramid descriptor or TMS)
             MissingEnvironmentError: Missing object storage informations or TMS root directory
 
         Examples:
 
@@ -544,15 +544,15 @@
         return pyramid
 
     def __init__(self) -> None:
         self.__storage = {}
         self.__levels = {}
         self.__masks = None
 
-        self.__content = {"loaded": False, "cache": {}}
+        self.__content = {"loaded": False, "count": 0, "cache": {}}
 
     def __str__(self) -> str:
         return f"{self.type.name} pyramid '{self.__name}' ({self.__storage['type'].name} storage)"
 
     @property
     def serializable(self) -> Dict:
         """Get the dict version of the pyramid object, descriptor compliant
@@ -733,27 +733,30 @@
             PyramidType: RASTER or VECTOR
         """
         if self.__format == "TIFF_PBF_MVT":
             return PyramidType.VECTOR
         else:
             return PyramidType.RASTER
 
-    def load_list(self) -> None:
+    def load_list(self) -> int:
         """Load list content and cache it
 
         If list is already loaded, nothing done
         """
         if self.__content["loaded"]:
-            return
+            return self.__content["count"]
 
         for slab, infos in self.list_generator():
             self.__content["cache"][slab] = infos
+            self.__content["count"] += 1
 
         self.__content["loaded"] = True
 
+        return self.__content["count"]
+
     def list_generator(
         self, level_id: str = None
     ) -> Iterator[Tuple[Tuple[SlabType, str, int, int], Dict]]:
         """Get list content
 
         List is copied as temporary file, roots are read and informations about each slab is returned. If list is already loaded, we yield the cached content
         Args :
```

### Comparing `rok4-2.1.4/src/rok4/raster.py` & `rok4-2.1.5/src/rok4/raster.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/src/rok4/storage.py` & `rok4-2.1.5/src/rok4/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provide functions to use read or write
+"""Provide functions to read or write data
 
 Available storage types are :
 - S3 (path are preffixed with `s3://`)
 - CEPH (path are prefixed with `ceph://`)
 - FILE (path are prefixed with `file://`, but it is the default paths' interpretation)
 - HTTP (path are prefixed with `http://`)
 - HTTPS (path are prefixed with `https://`)
```

### Comparing `rok4-2.1.4/src/rok4/tile_matrix_set.py` & `rok4-2.1.5/src/rok4/tile_matrix_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 The module contains the following classes:
 
 - `TileMatrixSet` - Multi level grid
 - `TileMatrix` - A tile matrix set level
 
 Loading a tile matrix set requires environment variables :
+
 - ROK4_TMS_DIRECTORY
 """
 
 # -- IMPORTS --
 
 # standard library
 import json
@@ -204,14 +205,15 @@
         Args:
             name: TMS's name
 
         Raises:
             MissingEnvironmentError: Missing object storage informations
             Exception: No level in the TMS, CRS not recognized by OSR
             StorageError: Storage read issue
+            FileNotFoundError: TMS file or object does not exist
             FormatError: Provided path is not a well formed JSON
             MissingAttributeError: Attribute is missing in the content
         """
 
         self.name = name
 
         try:
```

### Comparing `rok4-2.1.4/src/rok4/utils.py` & `rok4-2.1.5/src/rok4/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         Tuple[float, float]: X/Y in destination spatial reference
     """
 
     sr_src_inv = sr_src.EPSGTreatsAsLatLong() or sr_src.EPSGTreatsAsNorthingEasting()
     sr_dst_inv = sr_dst.EPSGTreatsAsLatLong() or sr_dst.EPSGTreatsAsNorthingEasting()
 
     if sr_src.IsSame(sr_dst) and sr_src_inv == sr_dst_inv:
-        # Les système sont vraiment les même, avec le même ordre des axes
+        # Les système sont vraiment les mêmes, avec le même ordre des axes
         return (point[0], point[1])
     elif sr_src.IsSame(sr_dst) and sr_src_inv != sr_dst_inv:
         # Les système sont les même pour OSR, mais l'ordre des axes est différent
         return (point[1], point[0])
 
     # Systèmes différents
     ct = osr.CreateCoordinateTransformation(sr_src, sr_dst)
```

### Comparing `rok4-2.1.4/src/rok4/vector.py` & `rok4-2.1.5/src/rok4/vector.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/src/rok4.egg-info/PKG-INFO` & `rok4-2.1.5/src/rok4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rok4
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python core libraries for ROK4 project
 Author-email: Géoportail IGN Developers <tout_rdev@ign.fr>
 License: 
         CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
```

### Comparing `rok4-2.1.4/src/rok4.egg-info/SOURCES.txt` & `rok4-2.1.5/src/rok4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_layer.py` & `rok4-2.1.5/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_pyramid.py` & `rok4-2.1.5/tests/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_raster.py` & `rok4-2.1.5/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_storage.py` & `rok4-2.1.5/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_tile_matrix_set.py` & `rok4-2.1.5/tests/test_tile_matrix_set.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_utils.py` & `rok4-2.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rok4-2.1.4/tests/test_vector.py` & `rok4-2.1.5/tests/test_vector.py`

 * *Files identical despite different names*

