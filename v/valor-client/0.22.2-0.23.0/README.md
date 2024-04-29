# Comparing `tmp/valor_client-0.22.2.tar.gz` & `tmp/valor_client-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.22.2.tar", last modified: Tue Apr 23 16:16:39 2024, max compression
+gzip compressed data, was "valor_client-0.23.0.tar", last modified: Mon Apr 29 18:05:46 2024, max compression
```

## Comparing `valor_client-0.22.2.tar` & `valor_client-0.23.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.314195 valor_client-0.22.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 16:16:34.000000 valor_client-0.22.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 16:16:39.310195 valor_client-0.22.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 16:16:34.000000 valor_client-0.22.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:16:39.314195 valor_client-0.22.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 16:16:34.000000 valor_client-0.22.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54413 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.713965 valor_client-0.23.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 18:05:42.000000 valor_client-0.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-29 18:05:46.713965 valor_client-0.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 18:05:42.000000 valor_client-0.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:05:46.713965 valor_client-0.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 18:05:42.000000 valor_client-0.23.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.705965 valor_client-0.23.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.705965 valor_client-0.23.0/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-29 18:05:42.000000 valor_client-0.23.0/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53919 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.709965 valor_client-0.23.0/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-29 18:05:42.000000 valor_client-0.23.0/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:05:46.713965 valor_client-0.23.0/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-29 18:05:46.000000 valor_client-0.23.0/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 18:05:46.000000 valor_client-0.23.0/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:05:46.000000 valor_client-0.23.0/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-29 18:05:46.000000 valor_client-0.23.0/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 18:05:46.000000 valor_client-0.23.0/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.22.2/LICENSE` & `valor_client-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/PKG-INFO` & `valor_client-0.23.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.22.2
+Version: 0.23.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.22.2/pyproject.toml` & `valor_client-0.23.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/conftest.py` & `valor_client-0.23.0/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/coretypes/test_core.py` & `valor_client-0.23.0/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.23.0/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/coretypes/test_filtering.py` & `valor_client-0.23.0/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/schemas/test_filters.py` & `valor_client-0.23.0/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/schemas/test_geojson.py` & `valor_client-0.23.0/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/schemas/test_label.py` & `valor_client-0.23.0/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.23.0/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.23.0/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.23.0/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/symbolic/test_operators.py` & `valor_client-0.23.0/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.23.0/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.23.0/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/test_client.py` & `valor_client-0.23.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/unit-tests/test_viz.py` & `valor_client-0.23.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/__init__.py` & `valor_client-0.23.0/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/client.py` & `valor_client-0.23.0/valor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from packaging import version
 
 from valor import __version__ as client_version
 from valor.enums import TableStatus
 from valor.exceptions import (
     ClientAlreadyConnectedError,
     ClientConnectionFailed,
-    ClientException,
     ClientNotConnectedError,
+    raise_client_exception,
 )
 from valor.schemas import EvaluationRequest
 
 T = TypeVar("T")
 
 
 def wait_for_predicate(
@@ -299,18 +299,15 @@
                     resp.status_code in [401, 403]
                     and self._using_username_password
                     and not tried
                     and not ignore_auth
                 ):
                     self._get_access_token_from_username_and_password()
                 else:
-                    try:
-                        raise ClientException(resp)
-                    except (requests.exceptions.JSONDecodeError, KeyError):
-                        resp.raise_for_status()
+                    raise_client_exception(resp)
             else:
                 break
             tried = True
 
         return resp
 
     def _requests_post_rel_host(self, endpoint: str, *args, **kwargs):
@@ -656,15 +653,15 @@
             The UID of the datum.
         Returns
         -------
         dict
             A dictionary describing a datum.
         """
         return self._requests_get_rel_host(
-            f"/data/dataset/{dataset_name}/uid/{uid}"
+            f"data/dataset/{dataset_name}/uid/{uid}"
         ).json()
 
     def create_model(self, model: dict) -> None:
         """
         Creates a model.
 
         `CREATE` endpoint.
```

### Comparing `valor_client-0.22.2/valor/coretypes.py` & `valor_client-0.23.0/valor/coretypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import json
 import time
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from valor.client import ClientConnection, connect, get_connection
 from valor.enums import AnnotationType, EvaluationStatus, TableStatus, TaskType
-from valor.exceptions import ClientException
+from valor.exceptions import (
+    ClientException,
+    DatasetDoesNotExistError,
+    ModelDoesNotExistError,
+)
 from valor.schemas import (
     Annotation,
     Datum,
     Dictionary,
     EvaluationParameters,
     EvaluationRequest,
     Filter,
@@ -1319,26 +1323,21 @@
             The name of the dataset to fetch.
 
         Returns
         -------
         Union[Dataset, None]
             A Dataset with a matching name, or 'None' if one doesn't exist.
         """
-        try:
-            dataset = Dataset.decode_value(
-                {
-                    **self.conn.get_dataset(name),
-                    "connection": self.conn,
-                }
-            )
-            return dataset
-        except ClientException as e:
-            if e.status_code == 404:
-                return None
-            raise e
+        dataset = Dataset.decode_value(
+            {
+                **self.conn.get_dataset(name),
+                "connection": self.conn,
+            }
+        )
+        return dataset
 
     def get_datasets(
         self,
         filter_by: Optional[FilterType] = None,
     ) -> List[Dataset]:
         """
         Get all datasets, with an option to filter results according to some user-defined parameters.
@@ -1405,21 +1404,16 @@
         -------
         valor.Datum
             The requested datum or 'None' if it doesn't exist.
         """
         dataset_name = (
             dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
-        try:
-            resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)
-            return Datum.decode_value(resp)
-        except ClientException as e:
-            if e.status_code == 404:
-                return None
-            raise e
+        resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)
+        return Datum.decode_value(resp)
 
     def get_dataset_status(
         self,
         name: str,
     ) -> Union[TableStatus, None]:
         """
         Get the state of a given dataset.
@@ -1467,18 +1461,19 @@
             The name of the dataset to be deleted.
         timeout : int
             The number of seconds to wait in order to confirm that the dataset was deleted.
         """
         self.conn.delete_dataset(name)
         if timeout:
             for _ in range(timeout):
-                if self.get_dataset(name) is None:
+                try:
+                    self.get_dataset(name)
+                except DatasetDoesNotExistError:
                     break
-                else:
-                    time.sleep(1)
+                time.sleep(1)
             else:
                 raise TimeoutError(
                     "Dataset wasn't deleted within timeout interval"
                 )
 
     def create_model(
         self,
@@ -1552,27 +1547,23 @@
             The matching prediction or 'None' if it doesn't exist.
         """
         dataset_name = (
             dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         model_name = model.get_name() if isinstance(model, Model) else model
         datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
-        try:
-            resp = self.conn.get_prediction(
-                dataset_name=dataset_name,
-                model_name=model_name,
-                datum_uid=datum_uid,
-            )
-            resp.pop("dataset_name")
-            resp.pop("model_name")
-            return Prediction.decode_value(resp)
-        except ClientException as e:
-            if e.status_code == 404:
-                return None
-            raise e
+
+        resp = self.conn.get_prediction(
+            dataset_name=dataset_name,
+            model_name=model_name,
+            datum_uid=datum_uid,
+        )
+        resp.pop("dataset_name")
+        resp.pop("model_name")
+        return Prediction.decode_value(resp)
 
     def finalize_inferences(
         self, dataset: Union[Dataset, str], model: Union[Model, str]
     ) -> None:
         """
         Finalizes a model-dataset pairing such that new predictions cannot be added to it.
         """
@@ -1598,25 +1589,20 @@
             The name of the model to fetch.
 
         Returns
         -------
         Union[valor.Model, None]
             A Model with matching name or 'None' if one doesn't exist.
         """
-        try:
-            return Model.decode_value(
-                {
-                    **self.conn.get_model(name),
-                    "connection": self.conn,
-                }
-            )
-        except ClientException as e:
-            if e.status_code == 404:
-                return None
-            raise e
+        return Model.decode_value(
+            {
+                **self.conn.get_model(name),
+                "connection": self.conn,
+            }
+        )
 
     def get_models(
         self,
         filter_by: Optional[FilterType] = None,
     ) -> List[Model]:
         """
         Get all models using an optional filter.
@@ -1703,18 +1689,19 @@
             The name of the model to be deleted.
         timeout : int
             The number of seconds to wait in order to confirm that the model was deleted.
         """
         self.conn.delete_model(name)
         if timeout:
             for _ in range(timeout):
-                if self.get_model(name) is None:
+                try:
+                    self.get_model(name)
+                except ModelDoesNotExistError:
                     break
-                else:
-                    time.sleep(1)
+                time.sleep(1)
             else:
                 raise TimeoutError(
                     "Model wasn't deleted within timeout interval"
                 )
 
     def get_evaluations(
         self,
```

### Comparing `valor_client-0.22.2/valor/enums.py` & `valor_client-0.23.0/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/metatypes.py` & `valor_client-0.23.0/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/schemas/__init__.py` & `valor_client-0.23.0/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/schemas/evaluation.py` & `valor_client-0.23.0/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/schemas/filters.py` & `valor_client-0.23.0/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/schemas/symbolic/collections.py` & `valor_client-0.23.0/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/schemas/symbolic/operators.py` & `valor_client-0.23.0/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/schemas/symbolic/types.py` & `valor_client-0.23.0/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/type_checks.py` & `valor_client-0.23.0/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor/viz.py` & `valor_client-0.23.0/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.2/valor_client.egg-info/PKG-INFO` & `valor_client-0.23.0/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.22.2
+Version: 0.23.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.22.2/valor_client.egg-info/SOURCES.txt` & `valor_client-0.23.0/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

