# Comparing `tmp/nap-plot-tools-0.0.4.tar.gz` & `tmp/nap-plot-tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nap-plot-tools-0.0.4.tar", last modified: Thu Apr 11 11:50:15 2024, max compression
+gzip compressed data, was "nap-plot-tools-0.1.0.tar", last modified: Mon Apr 29 08:45:44 2024, max compression
```

## Comparing `nap-plot-tools-0.0.4.tar` & `nap-plot-tools-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.507884 nap-plot-tools-0.0.4/
--rw-rw-rw-   0        0        0     1526 2023-07-03 07:56:44.000000 nap-plot-tools-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3526 2024-04-11 11:50:15.506885 nap-plot-tools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1866 2023-11-28 14:37:34.000000 nap-plot-tools-0.0.4/README.md
--rw-rw-rw-   0        0        0     1670 2024-04-11 11:50:15.511497 nap-plot-tools-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-10-27 08:08:29.000000 nap-plot-tools-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.463002 nap-plot-tools-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.481003 nap-plot-tools-0.0.4/src/nap_plot_tools/
--rw-rw-rw-   0        0        0      246 2024-04-11 11:44:22.000000 nap-plot-tools-0.0.4/src/nap_plot_tools/__init__.py
--rw-rw-rw-   0        0        0     7604 2024-04-03 08:59:43.000000 nap-plot-tools-0.0.4/src/nap_plot_tools/cmap.py
--rw-rw-rw-   0        0        0    15426 2024-04-05 12:15:17.000000 nap-plot-tools-0.0.4/src/nap_plot_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:50:15.503883 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/
--rw-rw-rw-   0        0        0     3526 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 11:50:15.000000 nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:45:44.933094 nap-plot-tools-0.1.0/
+-rw-rw-rw-   0        0        0     1526 2023-07-03 07:56:44.000000 nap-plot-tools-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3553 2024-04-29 08:45:44.932095 nap-plot-tools-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1866 2023-11-28 14:37:34.000000 nap-plot-tools-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1683 2024-04-29 08:45:44.936093 nap-plot-tools-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-10-27 08:08:29.000000 nap-plot-tools-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:45:44.886934 nap-plot-tools-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 08:45:44.907344 nap-plot-tools-0.1.0/src/nap_plot_tools/
+-rw-rw-rw-   0        0        0      251 2024-04-29 08:27:41.000000 nap-plot-tools-0.1.0/src/nap_plot_tools/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-29 08:19:58.000000 nap-plot-tools-0.1.0/src/nap_plot_tools/cmap.py
+-rw-rw-rw-   0        0        0    15393 2024-04-29 08:20:43.000000 nap-plot-tools-0.1.0/src/nap_plot_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:45:44.930094 nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/
+-rw-rw-rw-   0        0        0     3553 2024-04-29 08:45:44.000000 nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-29 08:45:44.000000 nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:45:44.000000 nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-29 08:45:44.000000 nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 08:45:44.000000 nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/top_level.txt
```

### Comparing `nap-plot-tools-0.0.4/LICENSE` & `nap-plot-tools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.4/PKG-INFO` & `nap-plot-tools-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nap-plot-tools
-Version: 0.0.4
+Version: 0.1.0
 Summary: A NAPari PLOTter TOOLbar and tools for additional functionalities.
 Home-page: https://github.com/zoccoler/nap-plot-tools
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/zoccoler/nap-plot-tools/issues
 Project-URL: Documentation, https://github.com/zoccoler/nap-plot-tools#README.md
@@ -25,14 +25,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: qtpy
 Requires-Dist: cmap
 Requires-Dist: deprecated
+Requires-Dist: matplotlib
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
 Requires-Dist: deprecated; extra == "testing"
```

### Comparing `nap-plot-tools-0.0.4/README.md` & `nap-plot-tools-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nap-plot-tools-0.0.4/setup.cfg` & `nap-plot-tools-0.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -72,34 +72,35 @@
 00000470: 7562 2e63 6f6d 2f7a 6f63 636f 6c65 722f  ub.com/zoccoler/
 00000480: 6e61 702d 706c 6f74 2d74 6f6f 6c73 2f69  nap-plot-tools/i
 00000490: 7373 7565 730d 0a0d 0a5b 6f70 7469 6f6e  ssues....[option
 000004a0: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
 000004b0: 696e 643a 0d0a 696e 7374 616c 6c5f 7265  ind:..install_re
 000004c0: 7175 6972 6573 203d 200d 0a09 6e75 6d70  quires = ...nump
 000004d0: 790d 0a09 7174 7079 0d0a 0963 6d61 700d  y...qtpy...cmap.
-000004e0: 0a09 6465 7072 6563 6174 6564 0d0a 7079  ..deprecated..py
-000004f0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000500: 3e3d 332e 380d 0a69 6e63 6c75 6465 5f70  >=3.8..include_p
-00000510: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-00000520: 7565 0d0a 7061 636b 6167 655f 6469 7220  ue..package_dir 
-00000530: 3d20 0d0a 093d 7372 630d 0a0d 0a5b 6f70  = ...=src....[op
-00000540: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000550: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000560: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  c....[options.ex
-00000570: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
-00000580: 6573 7469 6e67 203d 200d 0a09 746f 780d  esting = ...tox.
-00000590: 0a09 7079 7465 7374 2020 2320 6874 7470  ..pytest  # http
-000005a0: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
-000005b0: 6f72 672f 656e 2f6c 6174 6573 742f 636f  org/en/latest/co
-000005c0: 6e74 656e 7473 2e68 746d 6c0d 0a09 7079  ntents.html...py
-000005d0: 7465 7374 2d63 6f76 2020 2320 6874 7470  test-cov  # http
-000005e0: 733a 2f2f 7079 7465 7374 2d63 6f76 2e72  s://pytest-cov.r
-000005f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000600: 2f6c 6174 6573 742f 0d0a 0970 7974 6573  /latest/...pytes
-00000610: 742d 7174 2020 2320 6874 7470 733a 2f2f  t-qt  # https://
-00000620: 7079 7465 7374 2d71 742e 7265 6164 7468  pytest-qt.readth
-00000630: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000640: 7374 2f0d 0a09 7079 7174 350d 0a09 6465  st/...pyqt5...de
-00000650: 7072 6563 6174 6564 0d0a 0d0a 5b65 6767  precated....[egg
-00000660: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000670: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000680: 2030 0d0a 0d0a                            0....
+000004e0: 0a09 6465 7072 6563 6174 6564 0d0a 096d  ..deprecated...m
+000004f0: 6174 706c 6f74 6c69 620d 0a70 7974 686f  atplotlib..pytho
+00000500: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000510: 2e38 0d0a 696e 636c 7564 655f 7061 636b  .8..include_pack
+00000520: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+00000530: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000540: 0a09 3d73 7263 0d0a 0d0a 5b6f 7074 696f  ..=src....[optio
+00000550: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000560: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000570: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
+00000580: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
+00000590: 696e 6720 3d20 0d0a 0974 6f78 0d0a 0970  ing = ...tox...p
+000005a0: 7974 6573 7420 2023 2068 7474 7073 3a2f  ytest  # https:/
+000005b0: 2f64 6f63 732e 7079 7465 7374 2e6f 7267  /docs.pytest.org
+000005c0: 2f65 6e2f 6c61 7465 7374 2f63 6f6e 7465  /en/latest/conte
+000005d0: 6e74 732e 6874 6d6c 0d0a 0970 7974 6573  nts.html...pytes
+000005e0: 742d 636f 7620 2023 2068 7474 7073 3a2f  t-cov  # https:/
+000005f0: 2f70 7974 6573 742d 636f 762e 7265 6164  /pytest-cov.read
+00000600: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000610: 7465 7374 2f0d 0a09 7079 7465 7374 2d71  test/...pytest-q
+00000620: 7420 2023 2068 7474 7073 3a2f 2f70 7974  t  # https://pyt
+00000630: 6573 742d 7174 2e72 6561 6474 6865 646f  est-qt.readthedo
+00000640: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000650: 0d0a 0970 7971 7435 0d0a 0964 6570 7265  ...pyqt5...depre
+00000660: 6361 7465 640d 0a0d 0a5b 6567 675f 696e  cated....[egg_in
+00000670: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000680: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000690: 0a0d 0a                                  ...
```

### Comparing `nap-plot-tools-0.0.4/src/nap_plot_tools/cmap.py` & `nap-plot-tools-0.1.0/src/nap_plot_tools/cmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from deprecated import deprecated
 
-def make_cat10_mod_cmap(first_color_transparent=True):
+def make_cat10_mod_cmap(first_color_transparent=False):
     """Make a modified version of the cat10 colormap.
 
     Parameters
     ----------
     first_color_transparent : bool, optional
-        Whether to make the first color transparent. The default is True.
+        Whether to make the first color transparent. The default is False.
 
     Returns
     -------
     matplotlib.colors.ListedColormap
         Matplotlib colormap.
     """
     return make_cmap_from_list(get_cat10_mod_hex_colors(), first_color_transparent)
 
-def make_cmap_from_list(colors, first_transparent=True):
+def make_cmap_from_list(colors, first_transparent=False):
     """Make a matplotlib colormap from a list of colors.
 
     Parameters
     ----------
     colors : list
         List of colors in hex or rgb format.
     first_transparent : bool, optional
-        Whether to make the first color transparent. The default is True.
+        Whether to make the first color transparent. The default is False.
 
     Returns
     -------
     matplotlib.colors.ListedColormap
         Matplotlib colormap.
     """    
     from cmap import Colormap, Color
+    name = 'cat10_modified'
     if first_transparent:
         first_color_as_list = list(Color(colors[0]))
         # Set transparency to 0
         first_color_as_list[-1] = 0
         colors[0] = tuple(first_color_as_list)
-    return Colormap(colors).to_mpl()
+        name = name + '_first_transparent'
+    return Colormap(value=colors, name=name).to_mpl()
 
 @deprecated("get_custom_cat10based_cmap_list() is deprecated. Use make_cat10_mod_cmap() instead (turn into list if needed).")
 def get_custom_cat10based_cmap_list():
     from cmap import Colormap
     import warnings
     warnings.warn("get_custom_cat10based_cmap_list() is deprecated. Use make_cat10_mod_cmap() instead (turn into list if needed).", DeprecationWarning)
     cat10_cmap = Colormap(get_cat10_mod_hex_colors()).lut()[1:]
@@ -314,9 +316,9 @@
         "#5c4a56",
         "#735647",
         "#bcbcbc",
     ]
 
     return colors_hex
 
-cat10_mod_cmap = make_cat10_mod_cmap()
-cat10_mod_cmap_first_opaque = make_cat10_mod_cmap(first_color_transparent=False)
+cat10_mod_cmap = make_cat10_mod_cmap() # Default is first color opaque
+cat10_mod_cmap_first_transparent = make_cat10_mod_cmap(first_color_transparent=True)
```

### Comparing `nap-plot-tools-0.0.4/src/nap_plot_tools/tools.py` & `nap-plot-tools-0.1.0/src/nap_plot_tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nap_plot_tools.cmap import make_cat10_mod_cmap, get_custom_cat10based_cmap_list
+from nap_plot_tools.cmap import make_cat10_mod_cmap
 from qtpy.QtCore import Qt, QSize, QRect, Signal
 from qtpy.QtGui import QColor, QPainter, QPixmap
 from qtpy.QtWidgets import QSpinBox, QToolButton, QToolBar, QVBoxLayout, QWidget, QHBoxLayout, QSizePolicy
 
 import numpy as np
 
 class QtColorBox(QWidget):
```

### Comparing `nap-plot-tools-0.0.4/src/nap_plot_tools.egg-info/PKG-INFO` & `nap-plot-tools-0.1.0/src/nap_plot_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nap-plot-tools
-Version: 0.0.4
+Version: 0.1.0
 Summary: A NAPari PLOTter TOOLbar and tools for additional functionalities.
 Home-page: https://github.com/zoccoler/nap-plot-tools
 Author: Marcelo Leomil Zoccoler
 Author-email: marzoccoler@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/zoccoler/nap-plot-tools/issues
 Project-URL: Documentation, https://github.com/zoccoler/nap-plot-tools#README.md
@@ -25,14 +25,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: qtpy
 Requires-Dist: cmap
 Requires-Dist: deprecated
+Requires-Dist: matplotlib
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
 Requires-Dist: deprecated; extra == "testing"
```

