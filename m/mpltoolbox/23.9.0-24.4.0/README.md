# Comparing `tmp/mpltoolbox-23.9.0.tar.gz` & `tmp/mpltoolbox-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltoolbox-23.9.0.tar", last modified: Wed Sep 20 13:17:46 2023, max compression
+gzip compressed data, was "mpltoolbox-24.4.0.tar", last modified: Mon Apr 29 09:33:32 2024, max compression
```

## Comparing `mpltoolbox-23.9.0.tar` & `mpltoolbox-24.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.000709 mpltoolbox-23.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.000709 mpltoolbox-23.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.000709 mpltoolbox-23.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/callbacks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/ellipses.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    75876 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    95767 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/lines.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/polygons.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/programmatic-control.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/rectangles.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/docs/spans.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.000709 mpltoolbox-23.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/src/mpltoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/hspans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/rectangles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/src/mpltoolbox/vspans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/src/mpltoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-09-20 13:17:45.000000 mpltoolbox-23.9.0/src/mpltoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-09-20 13:17:45.000000 mpltoolbox-23.9.0/src/mpltoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 13:17:45.000000 mpltoolbox-23.9.0/src/mpltoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-20 13:17:45.000000 mpltoolbox-23.9.0/src/mpltoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-20 13:17:45.000000 mpltoolbox-23.9.0/src/mpltoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:17:46.004709 mpltoolbox-23.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/tests/lines_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-09-20 13:15:53.000000 mpltoolbox-23.9.0/tests/points_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.301115 mpltoolbox-24.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/callbacks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/ellipses.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95767 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/lines.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/polygons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/programmatic-control.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/rectangles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/spans.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/src/mpltoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/hspans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/rectangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/vspans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/tests/lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/tests/points_test.py
```

### Comparing `mpltoolbox-23.9.0/.github/workflows/ci.yml` & `mpltoolbox-24.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/LICENSE` & `mpltoolbox-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/PKG-INFO` & `mpltoolbox-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 23.9.0
+Version: 24.4.0
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-23.9.0/README.md` & `mpltoolbox-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/callbacks.ipynb` & `mpltoolbox-24.4.0/docs/callbacks.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/conf.py` & `mpltoolbox-24.4.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 import os
 import sys
 
 src = os.path.abspath("../src")
 os.environ["PYTHONPATH"] = src
 sys.path.insert(0, src)
```

### Comparing `mpltoolbox-23.9.0/docs/demo.ipynb` & `mpltoolbox-24.4.0/docs/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/ellipses.ipynb` & `mpltoolbox-24.4.0/docs/ellipses.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/images/favicon.ico` & `mpltoolbox-24.4.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/images/logo.png` & `mpltoolbox-24.4.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/images/logo.svg` & `mpltoolbox-24.4.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/index.rst` & `mpltoolbox-24.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/lines.ipynb` & `mpltoolbox-24.4.0/docs/lines.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/points.ipynb` & `mpltoolbox-24.4.0/docs/points.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/polygons.ipynb` & `mpltoolbox-24.4.0/docs/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/programmatic-control.ipynb` & `mpltoolbox-24.4.0/docs/programmatic-control.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/rectangles.ipynb` & `mpltoolbox-24.4.0/docs/rectangles.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/docs/spans.ipynb` & `mpltoolbox-24.4.0/docs/spans.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/setup.cfg` & `mpltoolbox-24.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/ellipses.py` & `mpltoolbox-24.4.0/src/mpltoolbox/ellipses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .patch import Patch
 from .tool import Tool
 from functools import partial
 from matplotlib import patches as mp
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/hspans.py` & `mpltoolbox-24.4.0/src/mpltoolbox/hspans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .patch import Patch
 from .tool import Tool
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 from typing import Tuple
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/lines.py` & `mpltoolbox-24.4.0/src/mpltoolbox/lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .tool import Tool
 from .utils import parse_kwargs
 import numpy as np
 from functools import partial
 from matplotlib.pyplot import Artist, Axes
 from matplotlib.backend_bases import Event
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/patch.py` & `mpltoolbox-24.4.0/src/mpltoolbox/patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .utils import parse_kwargs
 from matplotlib.pyplot import Axes, Artist
 from matplotlib.backend_bases import Event
 from matplotlib.colors import to_rgb
 from typing import Dict
 import uuid
@@ -36,14 +36,17 @@
         self._vertices.parent = self
         self._patch.parent = self
         self.id = uuid.uuid1().hex
 
     def __str__(self):
         return repr(self)
 
+    def __eq__(self, other):
+        return self.id == other.id
+
     def _update_vertices(self):
         self._vertices.set_data(*self._make_vertices())
 
     @property
     def width(self) -> float:
         return self._patch.get_width()
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/points.py` & `mpltoolbox-24.4.0/src/mpltoolbox/points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .lines import Line
 from .tool import Tool
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/polygons.py` & `mpltoolbox-24.4.0/src/mpltoolbox/polygons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .tool import Tool
 from .utils import parse_kwargs
 import numpy as np
 from functools import partial
 from matplotlib.pyplot import Artist, Axes
 from matplotlib.backend_bases import Event
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/rectangles.py` & `mpltoolbox-24.4.0/src/mpltoolbox/rectangles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .patch import Patch
 from .tool import Tool
 from functools import partial
 from matplotlib import patches as mp
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/tool.py` & `mpltoolbox-24.4.0/src/mpltoolbox/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .event import DummyEvent
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 from typing import Callable, List, Tuple, Union
 
@@ -240,17 +240,19 @@
     def _finalize_owner(self):
         child = self.children[-1]
         child.set_picker(5.0)
         if self.on_create is not None:
             self.call_on_create(child)
 
     def _on_pick(self, event: Event):
-        mev = event.mouseevent
         if self._get_active_tool():
             return
+        if event.artist.parent not in self.children:
+            return
+        mev = event.mouseevent
         if mev.inaxes != self._ax:
             return
         art = event.artist
         if (mev.button == 1) and ("ctrl" not in mev.modifiers):
             if not art.parent.is_moveable(art):
                 return
             self._pick_lock = True
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox/vspans.py` & `mpltoolbox-24.4.0/src/mpltoolbox/vspans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 from .patch import Patch
 from .tool import Tool
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 from typing import Tuple
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox.egg-info/PKG-INFO` & `mpltoolbox-24.4.0/src/mpltoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 23.9.0
+Version: 24.4.0
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-23.9.0/src/mpltoolbox.egg-info/SOURCES.txt` & `mpltoolbox-24.4.0/src/mpltoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpltoolbox-23.9.0/tests/conftest.py` & `mpltoolbox-24.4.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 import matplotlib
 import matplotlib.pyplot as plt
 import pytest
 
 
 @pytest.fixture(autouse=True)
```

### Comparing `mpltoolbox-23.9.0/tests/lines_test.py` & `mpltoolbox-24.4.0/tests/lines_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 import mpltoolbox as tbx
```

### Comparing `mpltoolbox-23.9.0/tests/points_test.py` & `mpltoolbox-24.4.0/tests/points_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) Scipp contributors (https://github.com/scipp)
 
 import matplotlib.pyplot as plt
 
 import mpltoolbox as tbx
 
 
 def test_points_creation():
```

