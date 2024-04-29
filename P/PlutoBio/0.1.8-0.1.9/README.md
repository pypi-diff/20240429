# Comparing `tmp/PlutoBio-0.1.8.tar.gz` & `tmp/PlutoBio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlutoBio-0.1.8.tar", last modified: Tue Nov 14 18:28:21 2023, max compression
+gzip compressed data, was "PlutoBio-0.1.9.tar", last modified: Mon Nov 27 21:57:05 2023, max compression
```

## Comparing `PlutoBio-0.1.8.tar` & `PlutoBio-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:28:21.535220 PlutoBio-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-11-14 18:28:21.535220 PlutoBio-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:28:21.531220 PlutoBio-0.1.8/PlutoBio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-11-14 18:28:21.000000 PlutoBio-0.1.8/PlutoBio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-14 18:28:21.000000 PlutoBio-0.1.8/PlutoBio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 18:28:21.000000 PlutoBio-0.1.8/PlutoBio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-14 18:28:21.000000 PlutoBio-0.1.8/PlutoBio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-14 18:28:21.000000 PlutoBio-0.1.8/PlutoBio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:28:21.531220 PlutoBio-0.1.8/plutobio/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/analyses.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/assay_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    20269 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/download_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/plutobio/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 18:28:21.535220 PlutoBio-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-14 18:28:06.000000 PlutoBio-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:57:05.040804 PlutoBio-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-11-27 21:57:05.040804 PlutoBio-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:57:05.040804 PlutoBio-0.1.9/PlutoBio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-11-27 21:57:05.000000 PlutoBio-0.1.9/PlutoBio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-27 21:57:05.000000 PlutoBio-0.1.9/PlutoBio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 21:57:05.000000 PlutoBio-0.1.9/PlutoBio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-27 21:57:05.000000 PlutoBio-0.1.9/PlutoBio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-27 21:57:05.000000 PlutoBio-0.1.9/PlutoBio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:57:05.040804 PlutoBio-0.1.9/plutobio/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/analyses.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/assay_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20245 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/download_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/plutobio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 21:57:05.040804 PlutoBio-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-27 21:56:49.000000 PlutoBio-0.1.9/setup.py
```

### Comparing `PlutoBio-0.1.8/PKG-INFO` & `PlutoBio-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlutoBio
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python SDK for Pluto.bio
 Author: Pluto Team
 Keywords: PlutoBio,SDK,API,Biosciences,Pluto
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `PlutoBio-0.1.8/PlutoBio.egg-info/PKG-INFO` & `PlutoBio-0.1.9/PlutoBio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlutoBio
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python SDK for Pluto.bio
 Author: Pluto Team
 Keywords: PlutoBio,SDK,API,Biosciences,Pluto
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `PlutoBio-0.1.8/PlutoBio.egg-info/SOURCES.txt` & `PlutoBio-0.1.9/PlutoBio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/README.md` & `PlutoBio-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/analyses.py` & `PlutoBio-0.1.9/plutobio/analyses.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/assay_data.py` & `PlutoBio-0.1.9/plutobio/assay_data.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/attachments.py` & `PlutoBio-0.1.9/plutobio/attachments.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/client.py` & `PlutoBio-0.1.9/plutobio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .pipelines import Pipelines
 from .projects import Project
 from .results import Results
 from .experiments import Experiment, Experiments
 from .download_upload import DownloadUploadHandler
 from .settings import DEFAULT_TMP_PATH
 import pandas as pd
-import requests
 from . import utils
 
 
 class PlutoClient:
     """Base class for Pluto API access"""
 
     def __init__(self, token: str, test_client=None) -> None:
@@ -446,15 +445,15 @@
         # Once ExternalAnalysis is created and the file is upload.
         # We need to link the uploaded file to the ExternalAnalysis
         response = self._plot_displays.update(
             experiment_id=experiment_id,
             plot_uuid=plot_uuid,
             display_uuid=display_uuid,
             data={
-                "figure_file": upload_response["experiment_file"]["uuid"],
+                "figure_file": upload_response["experiment_file"],
                 "display_type": "external",
                 "methods": methods,
                 "analysis_id": analysis_uuid,
                 "display_id": display_uuid,
             },
         )
```

### Comparing `PlutoBio-0.1.8/plutobio/download_upload.py` & `PlutoBio-0.1.9/plutobio/download_upload.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/experiments.py` & `PlutoBio-0.1.9/plutobio/experiments.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/pipelines.py` & `PlutoBio-0.1.9/plutobio/pipelines.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/plots.py` & `PlutoBio-0.1.9/plutobio/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pandas as pd
 from typing import TYPE_CHECKING, Union
 import math
 from . import utils
 from .settings import DEFAULT_TMP_PATH
 from . import api_endpoints
 import os
-from . import utils
 
 if TYPE_CHECKING:
     from . import PlutoClient
 
 
 class Plots(list):
     def __init__(self, client: "PlutoClient") -> None:
```

### Comparing `PlutoBio-0.1.8/plutobio/projects.py` & `PlutoBio-0.1.9/plutobio/projects.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/sample_data.py` & `PlutoBio-0.1.9/plutobio/sample_data.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/settings.py` & `PlutoBio-0.1.9/plutobio/settings.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/plutobio/utils.py` & `PlutoBio-0.1.9/plutobio/utils.py`

 * *Files identical despite different names*

### Comparing `PlutoBio-0.1.8/pyproject.toml` & `PlutoBio-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 
 [tool.coverage.run]
-omit = [
-    "*/tests/*",
-    "*/__init__.py",
-]
+omit = ["*/tests/*", "*/__init__.py"]
 
 [tool.coverage.report]
-omit = [
-    "*/tests/*",
-    "*/__init__.py",
-]
+omit = ["*/tests/*", "*/__init__.py"]
 
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PlutoBio"
-version = "0.1.8"
-authors = [
-    { name = "Pluto Team" }
-]
+version = "0.1.9"
+authors = [{ name = "Pluto Team" }]
 description = "A Python SDK for Pluto.bio"
 keywords = ["PlutoBio", "SDK", "API", "Biosciences", "Pluto"]
-readme = "README.md" 
-dependencies = [
-    "requests",
-    "pandas"
-]
+readme = "README.md"
+dependencies = ["requests", "pandas"]
 requires-python = ">=3.10, <4"
 
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "pluto.settings"
 python_files = "tests/*.py"
 addopts = "--reuse-db --cov=plutobio --cov-report term -n 4 --cov-append --cov-config=pyproject.toml --cov-report=lcov:lcov.info"
-env_files = ".env-test.local"
+env_files = ".env-test.local"
```

