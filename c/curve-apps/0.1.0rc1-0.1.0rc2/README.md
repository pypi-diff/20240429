# Comparing `tmp/curve_apps-0.1.0rc1.tar.gz` & `tmp/curve_apps-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curve_apps-0.1.0rc1.tar", max compression
+gzip compressed data, was "curve_apps-0.1.0rc2.tar", max compression
```

## Comparing `curve_apps-0.1.0rc1.tar` & `curve_apps-0.1.0rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      564 2024-04-28 03:43:27.707525 curve_apps-0.1.0rc1/curve_apps/__init__.py
--rw-r--r--   0        0        0     3120 2024-04-23 21:07:08.257218 curve_apps-0.1.0rc1/curve_apps/driver.py
--rw-r--r--   0        0        0      120 2024-04-23 21:07:08.257218 curve_apps-0.1.0rc1/curve_apps/edge_detection/__init__.py
--rw-r--r--   0        0        0     6983 2024-04-23 21:07:08.258300 curve_apps-0.1.0rc1/curve_apps/edge_detection/driver.py
--rw-r--r--   0        0        0     2433 2024-04-23 21:07:08.258361 curve_apps-0.1.0rc1/curve_apps/edge_detection/params.py
--rw-r--r--   0        0        0      712 2024-04-23 21:07:08.258361 curve_apps-0.1.0rc1/curve_apps/params.py
--rw-r--r--   0        0        0      120 2024-04-23 21:07:08.258897 curve_apps-0.1.0rc1/curve_apps/trend_lines/__init__.py
--rw-r--r--   0        0        0     5509 2024-04-23 21:07:08.259478 curve_apps-0.1.0rc1/curve_apps/trend_lines/driver.py
--rw-r--r--   0        0        0     1961 2024-04-23 21:07:08.259478 curve_apps-0.1.0rc1/curve_apps/trend_lines/params.py
--rw-r--r--   0        0        0      120 2024-04-27 20:32:11.993663 curve_apps-0.1.0rc1/curve_apps-assets/__init__.py
--rw-r--r--   0        0        0  4876334 2024-04-23 21:07:09.232019 curve_apps-0.1.0rc1/curve_apps-assets/curve_apps_demo.geoh5
--rw-r--r--   0        0        0     3045 2024-04-23 21:07:08.256066 curve_apps-0.1.0rc1/curve_apps-assets/uijson/edge_detection.ui.json
--rw-r--r--   0        0        0     2999 2024-04-23 21:07:08.256066 curve_apps-0.1.0rc1/curve_apps-assets/uijson/trend_lines.ui.json
--rw-r--r--   0        0        0     1098 2024-04-23 21:07:36.644208 curve_apps-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     3868 2024-04-28 03:44:23.797495 curve_apps-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5944 2024-04-23 21:07:07.585841 curve_apps-0.1.0rc1/README.rst
--rw-r--r--   0        0        0     7216 1970-01-01 00:00:00.000000 curve_apps-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      564 2024-04-29 05:06:55.962611 curve_apps-0.1.0rc2/curve_apps/__init__.py
+-rw-r--r--   0        0        0     3120 2024-04-23 21:07:08.257218 curve_apps-0.1.0rc2/curve_apps/driver.py
+-rw-r--r--   0        0        0      120 2024-04-23 21:07:08.257218 curve_apps-0.1.0rc2/curve_apps/edge_detection/__init__.py
+-rw-r--r--   0        0        0     6983 2024-04-23 21:07:08.258300 curve_apps-0.1.0rc2/curve_apps/edge_detection/driver.py
+-rw-r--r--   0        0        0     2393 2024-04-28 22:43:00.991203 curve_apps-0.1.0rc2/curve_apps/edge_detection/params.py
+-rw-r--r--   0        0        0      675 2024-04-28 22:43:00.991203 curve_apps-0.1.0rc2/curve_apps/params.py
+-rw-r--r--   0        0        0      120 2024-04-23 21:07:08.258897 curve_apps-0.1.0rc2/curve_apps/trend_lines/__init__.py
+-rw-r--r--   0        0        0     5509 2024-04-23 21:07:08.259478 curve_apps-0.1.0rc2/curve_apps/trend_lines/driver.py
+-rw-r--r--   0        0        0     1908 2024-04-28 22:43:00.992309 curve_apps-0.1.0rc2/curve_apps/trend_lines/params.py
+-rw-r--r--   0        0        0      120 2024-04-27 20:32:11.993663 curve_apps-0.1.0rc2/curve_apps-assets/__init__.py
+-rw-r--r--   0        0        0  4876334 2024-04-23 21:07:09.232019 curve_apps-0.1.0rc2/curve_apps-assets/curve_apps_demo.geoh5
+-rw-r--r--   0        0        0     3045 2024-04-23 21:07:08.256066 curve_apps-0.1.0rc2/curve_apps-assets/uijson/edge_detection.ui.json
+-rw-r--r--   0        0        0     2999 2024-04-23 21:07:08.256066 curve_apps-0.1.0rc2/curve_apps-assets/uijson/trend_lines.ui.json
+-rw-r--r--   0        0        0     1098 2024-04-23 21:07:36.644208 curve_apps-0.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     4095 2024-04-29 11:09:40.890018 curve_apps-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5944 2024-04-23 21:07:07.585841 curve_apps-0.1.0rc2/README.rst
+-rw-r--r--   0        0        0     7511 1970-01-01 00:00:00.000000 curve_apps-0.1.0rc2/PKG-INFO
```

### Comparing `curve_apps-0.1.0rc1/curve_apps/__init__.py` & `curve_apps-0.1.0rc2/curve_apps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #  All rights reserved.
 
 from __future__ import annotations
 
 from pathlib import Path
 
-__version__ = "0.1.0-rc.1"
+__version__ = "0.1.0-rc.2"
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
 
     parent = Path(__file__).parent
     folder_name = f"{parent.name}-assets"
```

### Comparing `curve_apps-0.1.0rc1/curve_apps/driver.py` & `curve_apps-0.1.0rc2/curve_apps/driver.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/curve_apps/edge_detection/driver.py` & `curve_apps-0.1.0rc2/curve_apps/edge_detection/driver.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/curve_apps/edge_detection/params.py` & `curve_apps-0.1.0rc2/curve_apps/edge_detection/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 #  This file is part of curve-apps.
 #
 #  curve-apps is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 
 from __future__ import annotations
 
-from typing import Optional
-
 from geoapps_utils.driver.data import BaseData
 from geoh5py.data import FloatData
 from geoh5py.objects import Grid2D
 from geoh5py.ui_json import InputFile
 from pydantic import BaseModel, ConfigDict
 
 from curve_apps import assets_path
@@ -54,31 +52,31 @@
     :param merge_length: Minimum length between nodes that should be merged.
     """
 
     line_length: int = 1
     line_gap: int = 1
     sigma: float = 10
     threshold: int = 1
-    window_size: Optional[int] = None
-    merge_length: Optional[int] = None
+    window_size: int | None = None
+    merge_length: int | None = None
 
 
 class Parameters(BaseData):
     """
     Edge detection input parameters.
 
     :param detection: Detection parameters expected for the edge detection.
     :param source: Parameters for the source object and data.
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     _name: str = NAME
 
-    input_file: Optional[InputFile] = InputFile.read_ui_json(
+    input_file: InputFile | None = InputFile.read_ui_json(
         DEFAULT_UI_JSON, validate=False
     )
     detection: DetectionParameters
     output: OutputParameters
     run_command: str = f"curve_apps.{NAME}.driver"
     source: SourceParameters
     title: str = NAME.capitalize().replace("_", " ")
```

### Comparing `curve_apps-0.1.0rc1/curve_apps/params.py` & `curve_apps-0.1.0rc2/curve_apps/params.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 #  This file is part of curve-apps.
 #
 #  curve-apps is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 
 from __future__ import annotations
 
-from typing import Optional
-
 from pydantic import BaseModel
 
 
 class OutputParameters(BaseModel):
     """
     Output parameters expected by the ui.json file format.
 
     :param export_as: Name of the output entity.
     :param out_group: Name of the output group.
     """
 
-    export_as: Optional[str] = None
-    out_group: Optional[str] = None
+    export_as: str | None = None
+    out_group: str | None = None
```

### Comparing `curve_apps-0.1.0rc1/curve_apps/trend_lines/driver.py` & `curve_apps-0.1.0rc2/curve_apps/trend_lines/driver.py`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/curve_apps/trend_lines/params.py` & `curve_apps-0.1.0rc2/curve_apps/trend_lines/params.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 #  curve-apps is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 
 # pylint: disable=duplicate-code
 
 from __future__ import annotations
 
-from typing import Optional, Union
-
 from geoapps_utils.driver.data import BaseData
 from geoapps_utils.numerical import DetectionParameters
 from geoh5py.data import Data, ReferencedData
 from geoh5py.objects import Curve, Points
 from geoh5py.ui_json import InputFile
 from pydantic import BaseModel, ConfigDict
 
@@ -38,17 +36,17 @@
     :param entity: A Curve or Points source object.
     :param data: Data values to find edges on.
     :param parts: Optional parts to connect.
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    entity: Union[Curve, Points]
-    data: Optional[ReferencedData] = None
-    parts: Optional[Data] = None
+    entity: Curve | Points
+    data: ReferencedData | None = None
+    parts: Data | None = None
 
 
 class Parameters(BaseData):
     """
     Parts connection input parameters.
 
     :param detection: Detection parameters expected for the parts connection.
@@ -56,14 +54,14 @@
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     _name: str = NAME
 
     detection: DetectionParameters
-    input_file: Optional[InputFile] = InputFile.read_ui_json(
+    input_file: InputFile | None = InputFile.read_ui_json(
         DEFAULT_UI_JSON, validate=False
     )
     output: OutputParameters
     run_command: str = f"curve_apps.{NAME}.driver"
     source: SourceParameters
     title: str = NAME.capitalize().replace("_", " ")
```

### Comparing `curve_apps-0.1.0rc1/curve_apps-assets/curve_apps_demo.geoh5` & `curve_apps-0.1.0rc2/curve_apps-assets/curve_apps_demo.geoh5`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/curve_apps-assets/uijson/edge_detection.ui.json` & `curve_apps-0.1.0rc2/curve_apps-assets/uijson/edge_detection.ui.json`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/curve_apps-assets/uijson/trend_lines.ui.json` & `curve_apps-0.1.0rc2/curve_apps-assets/uijson/trend_lines.ui.json`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/LICENSE` & `curve_apps-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/pyproject.toml` & `curve_apps-0.1.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [tool.poetry]
 name = "curve-apps"
-version = "0.1.0-rc.1"
+version = "0.1.0-rc.2"
 license = "MIT"
 description = "Find edges on 2D grids or vertices."
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
-repository = "https://github.com/MiraGeoscience/curve_apps"
-homepage = "https://mirageoscience.com"
+maintainers = ["Dominique Fournier <dominiquef@mirageoscience.com>"]
+repository = "https://github.com/MiraGeoscience/curve-apps"
+documentation  = "https://mirageoscience-curve-apps.readthedocs-hosted.com/"
+homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
 readme = "README.rst"
 packages = [
      { include = "curve_apps" },
      { include = "curve_apps-assets" },
 ]
 
 include = [
@@ -57,14 +59,19 @@
 #geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
 #---------------------------------------------------------------------------------
 h5py = "^3.2.1"  # from geoh5py
 Pillow = "~10.1.0"  # from geoh5py
 
+# pin down package versions when Conda is behind PyPI
+#----------------------------------------------------
+pywavelets = "~1.4.1"  # from scikit-image
+tifffile = "2024.2.12"  # from scikit-image
+
 ## about pip dependencies
 # to be specified to work with conda-lock
 # - from PyPI: my_package = { version = "1.2.3", source = "pypi" }
 # - from URL:
 #   - for a tags:   my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/tags/VERSION_TAG.zip#sha256=" }
 #   - for a branch: my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/heads/BRANCH.zip#sha256=" }
 # Note - conda-lock does not support the syntax: my_package = { git = ... }
@@ -81,20 +88,15 @@
 tomli = "*"
 
 [tool.conda-lock]
 platforms = ['win-64', 'linux-64']
 channels = ['conda-forge']
 
 [tool.isort]
-# settings for compatibility between ``isort`` and ``black`` formatting
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-line_length = 88
+profile = "black"
 
 [tool.black]
 # defaults are just fine
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
```

### Comparing `curve_apps-0.1.0rc1/README.rst` & `curve_apps-0.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `curve_apps-0.1.0rc1/PKG-INFO` & `curve_apps-0.1.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: curve-apps
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Find edges on 2D grids or vertices.
-Home-page: https://mirageoscience.com
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
+Maintainer: Dominique Fournier
+Maintainer-email: dominiquef@mirageoscience.com
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,18 +26,21 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: Pillow (>=10.1.0,<10.2.0)
 Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
+Requires-Dist: pywavelets (>=1.4.1,<1.5.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
+Requires-Dist: tifffile (==2024.2.12)
 Requires-Dist: tqdm (>=4.66.1,<4.67.0)
-Project-URL: Repository, https://github.com/MiraGeoscience/curve_apps
+Project-URL: Documentation, https://mirageoscience-curve-apps.readthedocs-hosted.com/
+Project-URL: Repository, https://github.com/MiraGeoscience/curve-apps
 Description-Content-Type: text/x-rst
 
 |coverage| |maintainability| |precommit_ci| |docs| |style| |version| |status| |pyversions|
 
 
 .. |docs| image:: https://readthedocs.org/projects/curve-apps/badge/
     :alt: Documentation Status
```

