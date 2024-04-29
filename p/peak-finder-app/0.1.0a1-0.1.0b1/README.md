# Comparing `tmp/peak_finder_app-0.1.0a1.tar.gz` & `tmp/peak_finder_app-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak_finder_app-0.1.0a1.tar", max compression
+gzip compressed data, was "peak_finder_app-0.1.0b1.tar", max compression
```

## Comparing `peak_finder_app-0.1.0a1.tar` & `peak_finder_app-0.1.0b1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1093 2024-04-18 17:39:16.334754 peak_finder_app-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      971 2024-04-18 17:39:18.605355 peak_finder_app-0.1.0a1/peak_finder/__init__.py
--rw-r--r--   0        0        0      866 2024-04-18 17:39:18.605355 peak_finder_app-0.1.0a1/peak_finder/anomaly.py
--rw-r--r--   0        0        0     8372 2024-04-18 17:39:18.605355 peak_finder_app-0.1.0a1/peak_finder/anomaly_group.py
--rw-r--r--   0        0        0    78823 2024-04-18 17:39:18.610430 peak_finder_app-0.1.0a1/peak_finder/application.py
--rw-r--r--   0        0        0     1785 2024-04-18 17:39:18.610430 peak_finder_app-0.1.0a1/peak_finder/constants.py
--rw-r--r--   0        0        0    15078 2024-04-18 17:39:18.610430 peak_finder_app-0.1.0a1/peak_finder/driver.py
--rw-r--r--   0        0        0   356591 2023-09-29 15:03:01.660768 peak_finder_app-0.1.0a1/peak_finder/images/peak_finder_app.png
--rw-r--r--   0        0        0    15808 2024-04-18 17:39:18.610430 peak_finder_app-0.1.0a1/peak_finder/layout.py
--rw-r--r--   0        0        0    10882 2024-04-18 17:39:18.610430 peak_finder_app-0.1.0a1/peak_finder/line_anomaly.py
--rw-r--r--   0        0        0    11584 2024-04-18 17:39:18.613944 peak_finder_app-0.1.0a1/peak_finder/line_data.py
--rw-r--r--   0        0        0    11849 2024-04-18 17:39:18.613944 peak_finder_app-0.1.0a1/peak_finder/line_group.py
--rw-r--r--   0        0        0    11812 2024-04-18 17:39:18.613944 peak_finder_app-0.1.0a1/peak_finder/line_position.py
--rw-r--r--   0        0        0    13241 2024-04-18 17:39:18.615492 peak_finder_app-0.1.0a1/peak_finder/params.py
--rw-r--r--   0        0        0     1106 2024-04-18 17:39:18.615492 peak_finder_app-0.1.0a1/peak_finder/utils.py
--rw-r--r--   0        0        0      117 2024-04-18 17:39:18.605355 peak_finder_app-0.1.0a1/peak_finder-assets/__init__.py
--rw-r--r--   0        0        0  1983716 2024-04-18 17:39:20.557576 peak_finder_app-0.1.0a1/peak_finder-assets/FlinFlon_tem_aoi.geoh5
--rw-r--r--   0        0        0     6444 2024-04-18 17:39:18.605355 peak_finder_app-0.1.0a1/peak_finder-assets/uijson/peak_finder.ui.json
--rw-r--r--   0        0        0     3332 2024-04-18 18:47:20.625094 peak_finder_app-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     5595 2024-04-18 17:39:16.334754 peak_finder_app-0.1.0a1/README.rst
--rw-r--r--   0        0        0     7164 1970-01-01 00:00:00.000000 peak_finder_app-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 peak_finder_app-0.1.0b1/LICENSE
+-rw-r--r--   0        0        0      970 2024-04-29 02:59:24.685914 peak_finder_app-0.1.0b1/peak_finder/__init__.py
+-rw-r--r--   0        0        0      866 2024-04-23 22:39:24.314550 peak_finder_app-0.1.0b1/peak_finder/anomaly.py
+-rw-r--r--   0        0        0     8372 2024-04-23 22:39:24.314612 peak_finder_app-0.1.0b1/peak_finder/anomaly_group.py
+-rw-r--r--   0        0        0    78823 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b1/peak_finder/application.py
+-rw-r--r--   0        0        0     1785 2024-04-23 22:39:24.315729 peak_finder_app-0.1.0b1/peak_finder/constants.py
+-rw-r--r--   0        0        0    15078 2024-04-23 22:39:24.316280 peak_finder_app-0.1.0b1/peak_finder/driver.py
+-rw-r--r--   0        0        0   356591 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b1/peak_finder/images/peak_finder_app.png
+-rw-r--r--   0        0        0    15808 2024-04-23 22:39:24.319046 peak_finder_app-0.1.0b1/peak_finder/layout.py
+-rw-r--r--   0        0        0    10882 2024-04-23 22:39:24.319593 peak_finder_app-0.1.0b1/peak_finder/line_anomaly.py
+-rw-r--r--   0        0        0    11584 2024-04-23 22:39:24.320130 peak_finder_app-0.1.0b1/peak_finder/line_data.py
+-rw-r--r--   0        0        0    11849 2024-04-23 22:39:24.320197 peak_finder_app-0.1.0b1/peak_finder/line_group.py
+-rw-r--r--   0        0        0    11812 2024-04-23 22:39:24.320728 peak_finder_app-0.1.0b1/peak_finder/line_position.py
+-rw-r--r--   0        0        0    13241 2024-04-23 22:39:24.321386 peak_finder_app-0.1.0b1/peak_finder/params.py
+-rw-r--r--   0        0        0     1106 2024-04-23 22:39:24.321970 peak_finder_app-0.1.0b1/peak_finder/utils.py
+-rw-r--r--   0        0        0      117 2024-04-23 22:39:24.312898 peak_finder_app-0.1.0b1/peak_finder-assets/__init__.py
+-rw-r--r--   0        0        0  1983716 2024-04-23 22:39:24.854255 peak_finder_app-0.1.0b1/peak_finder-assets/FlinFlon_tem_aoi.geoh5
+-rw-r--r--   0        0        0     6444 2024-04-23 22:39:24.313523 peak_finder_app-0.1.0b1/peak_finder-assets/uijson/peak_finder.ui.json
+-rw-r--r--   0        0        0     5083 2024-04-29 13:15:47.874294 peak_finder_app-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6280 2024-04-28 20:57:34.791039 peak_finder_app-0.1.0b1/README.rst
+-rw-r--r--   0        0        0     6573 2024-04-23 22:39:23.613401 peak_finder_app-0.1.0b1/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     8168 1970-01-01 00:00:00.000000 peak_finder_app-0.1.0b1/PKG-INFO
```

### Comparing `peak_finder_app-0.1.0a1/LICENSE` & `peak_finder_app-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/__init__.py` & `peak_finder_app-0.1.0b1/peak_finder/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) 2024 Mira Geoscience Ltd.
 #
 #  This file is part of peak-finder-app project.
 #
 #  All rights reserved.
 #
 
-__version__ = "0.1.0-alpha.1"
+__version__ = "0.1.0-beta.1"
 import os
 import warnings
 from pathlib import Path
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
```

### Comparing `peak_finder_app-0.1.0a1/peak_finder/anomaly.py` & `peak_finder_app-0.1.0b1/peak_finder/anomaly.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/anomaly_group.py` & `peak_finder_app-0.1.0b1/peak_finder/anomaly_group.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/application.py` & `peak_finder_app-0.1.0b1/peak_finder/application.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/constants.py` & `peak_finder_app-0.1.0b1/peak_finder/constants.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/driver.py` & `peak_finder_app-0.1.0b1/peak_finder/driver.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/images/peak_finder_app.png` & `peak_finder_app-0.1.0b1/peak_finder/images/peak_finder_app.png`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/layout.py` & `peak_finder_app-0.1.0b1/peak_finder/layout.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/line_anomaly.py` & `peak_finder_app-0.1.0b1/peak_finder/line_anomaly.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/line_data.py` & `peak_finder_app-0.1.0b1/peak_finder/line_data.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/line_group.py` & `peak_finder_app-0.1.0b1/peak_finder/line_group.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/line_position.py` & `peak_finder_app-0.1.0b1/peak_finder/line_position.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/params.py` & `peak_finder_app-0.1.0b1/peak_finder/params.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder/utils.py` & `peak_finder_app-0.1.0b1/peak_finder/utils.py`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder-assets/FlinFlon_tem_aoi.geoh5` & `peak_finder_app-0.1.0b1/peak_finder-assets/FlinFlon_tem_aoi.geoh5`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/peak_finder-assets/uijson/peak_finder.ui.json` & `peak_finder_app-0.1.0b1/peak_finder-assets/uijson/peak_finder.ui.json`

 * *Files identical despite different names*

### Comparing `peak_finder_app-0.1.0a1/PKG-INFO` & `peak_finder_app-0.1.0b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: peak-finder-app
-Version: 0.1.0a1
+Version: 0.1.0b1
 Summary: Peak Finder App
-Home-page: https://mirageoscience.com
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
+Maintainer: Dominique Fournier
+Maintainer-email: dominiquef@mirageoscience.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -17,34 +19,37 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: dash
-Requires-Dist: Pillow (>=10.0.1,<11.0.0)
-Requires-Dist: curve-apps (>=0.1.0-alpha.1,<0.2.0)
+Requires-Dist: Pillow (>=10.1.0,<10.2.0)
+Requires-Dist: curve-apps (>=0.1.0rc2,<0.2.0)
 Requires-Dist: dash (>=2.12,<2.13) ; extra == "dash"
-Requires-Dist: dash-daq (>=0.5.0,<0.6.0)
-Requires-Dist: dask[distributed] (==2022.10.0)
-Requires-Dist: geoapps-utils (>=0.3.0-alpha.3,<0.4.0)
-Requires-Dist: geoh5py (>=0.9.0-alpha.3,<0.10.0)
-Requires-Dist: h5py (>=3.8.0,<3.9.0)
-Requires-Dist: jupyter-server (>=1.23.6,<1.24.0)
-Requires-Dist: notebook (>=6.5.3,<6.6.0)
+Requires-Dist: dash-daq (>=0.5.0,<0.6.0) ; extra == "dash"
+Requires-Dist: dask[distributed] (==2022.10.*)
+Requires-Dist: distributed (==2022.10.*)
+Requires-Dist: flask (>=3.0.3,<3.1.0) ; extra == "dash"
+Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
+Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
+Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Requires-Dist: plotly (>=5.13.1,<5.14.0)
-Requires-Dist: pyqtwebengine (>=5.15,<5.16) ; extra == "dash"
-Requires-Dist: pyside2 (>=5.15,<5.16) ; extra == "dash"
+Requires-Dist: plotly (>=5.19.0,<5.20.0)
+Requires-Dist: pydantic (>=2.5.2,<2.6.0)
+Requires-Dist: pyqtwebengine (>=5.15.2,<5.15.7) ; extra == "dash"
+Requires-Dist: pyside2 (>=5.15.2.1,<5.16.0.0) ; extra == "dash"
+Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Project-URL: Documentation, https://mirageoscience-peak-finder-app.readthedocs-hosted.com/
 Project-URL: Repository, https://github.com/MiraGeoscience/peak-finder-app
 Description-Content-Type: text/x-rst
 
-|coverage| |maintainability| |precommit_ci| |docs| |style| |version| |status| |pyversions|
+|coverage| |precommit_ci| |docs| |style| |version| |status| |pyversions|
 
 
 .. |docs| image:: https://readthedocs.org/projects/peak-finder-app/badge/
     :alt: Documentation Status
     :target: https://peak-finder-app.readthedocs.io/en/latest/?badge=latest
 
 .. |coverage| image:: https://codecov.io/gh/MiraGeoscience/peak-finder-app/branch/develop/graph/badge.svg
@@ -67,37 +72,35 @@
     :alt: Python versions
     :target: https://pypi.python.org/pypi/peak-finder-app/
 
 .. |precommit_ci| image:: https://results.pre-commit.ci/badge/github/MiraGeoscience/peak-finder-app/develop.svg
     :alt: pre-commit.ci status
     :target: https://results.pre-commit.ci/latest/github/MiraGeoscience/peak-finder-app/develop
 
-.. |maintainability| image:: https://api.codeclimate.com/v1/badges/_token_/maintainability
-   :target: https://codeclimate.com/github/MiraGeoscience/peak-finder-app/maintainability
-   :alt: Maintainability
+.. .. |maintainability| image:: https://api.codeclimate.com/v1/badges/_token_/maintainability
+..    :target: https://codeclimate.com/github/MiraGeoscience/peak-finder-app/maintainability
+..    :alt: Maintainability
 
 
-peak-finder-app: # TODO: SHORT DESCRIPTION
-=========================================================================
+Peak-Finder-App
+===============
 **peak-finder-app** is a package for the detection and grouping of time-domain
 electromagnetic (TEM) anomalies measured along flight lines.
 
-.. contents:: Table of Contents
-   :local:
-   :depth: 3
 
 Documentation
 ^^^^^^^^^^^^^
 `Online documentation <https://mirageoscience-peak-finder-app.readthedocs-hosted.com/en/latest/>`_
 
 
 Installation
 ^^^^^^^^^^^^
 **peak-finder-app** is currently written for Python 3.10 or higher.
 
+
 Install Conda
 -------------
 
 To install **peak-finder-app**, you need to install **Conda** first.
 
 We recommend to install **Conda** using `miniforge`_.
 
@@ -164,31 +167,43 @@
 
 Or in **editable mode**, so that you can edit the sources and see the effect immediately at runtime:
 
 .. code-block:: bash
 
     pip install -e -U --force-reinstall path/to/project_folder_with_pyproject_toml
 
-Setup for development
-^^^^^^^^^^^^^^^^^^^^^
-To configure the development environment and tools, please see `README-dev.rst`_.
-
-.. _README-dev.rst: README-dev.rst
 
 License
 ^^^^^^^
-# TODO: ADD LICENSE TERMS
+MIT License
+
+Copyright (c) 2024 Mira Geoscience
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
 
 Third Party Software
 ^^^^^^^^^^^^^^^^^^^^
 The peak-finder-app Software may provide links to third party libraries or code (collectively “Third Party Software”)
 to implement various functions. Third Party Software does not comprise part of the Software.
 The use of Third Party Software is governed by the terms of such software license(s).
 Third Party Software notices and/or additional terms and conditions are located in the
 `THIRD_PARTY_SOFTWARE.rst`_ file.
 
 .. _THIRD_PARTY_SOFTWARE.rst: THIRD_PARTY_SOFTWARE.rst
 
-Copyright
-^^^^^^^^^
-Copyright (c) 2024 Mira Geoscience Ltd.
-
```

