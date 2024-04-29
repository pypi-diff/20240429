# Comparing `tmp/napari_smlmlab-0.0.5.tar.gz` & `tmp/napari_smlmlab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-cnp7eo9l\napari_smlmlab-0.0.5.tar", last modified: Mon Apr 29 10:12:57 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-666jea7q\napari_smlmlab-0.0.6.tar", last modified: Mon Apr 29 11:26:09 2024, max compression
```

## Comparing `napari_smlmlab-0.0.5.tar` & `napari_smlmlab-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.5/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-29 10:12:57.739798 napari_smlmlab-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.670807 napari_smlmlab-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.702049 napari_smlmlab-0.0.5/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-29 10:12:30.000000 napari_smlmlab-0.0.5/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.717671 napari_smlmlab-0.0.5/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.5/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.5/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0     9916 2024-04-29 07:54:07.000000 napari_smlmlab-0.0.5/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    36453 2024-04-29 09:50:44.000000 napari_smlmlab-0.0.5/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.5/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    27637 2024-04-29 08:31:32.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    21212 2024-04-29 07:50:18.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/undrift_utils.py
--rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.600597 napari_smlmlab-0.0.6/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4645 2024-04-29 11:26:09.599600 napari_smlmlab-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1819 2024-04-29 11:26:09.603396 napari_smlmlab-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.535225 napari_smlmlab-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.597606 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4645 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      731 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 11:26:09.000000 napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.566468 napari_smlmlab-0.0.6/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-04-29 11:26:03.000000 napari_smlmlab-0.0.6/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.566468 napari_smlmlab-0.0.6/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.6/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.6/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    12984 2024-04-29 11:24:47.000000 napari_smlmlab-0.0.6/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    36584 2024-04-29 11:00:01.000000 napari_smlmlab-0.0.6/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.6/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-29 11:26:09.594613 napari_smlmlab-0.0.6/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    27637 2024-04-29 08:31:32.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    21212 2024-04-29 07:50:18.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/undrift_utils.py
+-rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.6/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.5/LICENSE` & `napari_smlmlab-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/PKG-INFO` & `napari_smlmlab-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.5
+Version: 0.0.6
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.5/README.md` & `napari_smlmlab-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/pyproject.toml` & `napari_smlmlab-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/setup.cfg` & `napari_smlmlab-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.5
+Version: 0.0.6
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.0.6/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.0.6/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/_widget.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/compute_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,251 +1,282 @@
+from qtpy.QtCore import QObject
+from qtpy.QtCore import QRunnable
+from PyQt5.QtCore import pyqtSignal, pyqtSlot
 import traceback
-from functools import partial
-from multiprocessing import Manager
-from typing import TYPE_CHECKING
-
-import matplotlib.colors as mcolors
-import matplotlib.pyplot as plt
+import sys
+from multiprocessing import Process, shared_memory, Pool
 import numpy as np
-import pyqtgraph as pg
-from qtpy.QtCore import QThreadPool
-from qtpy.QtWidgets import (QVBoxLayout, QWidget, )
-from scipy.ndimage import map_coordinates
-
-if TYPE_CHECKING:
-    import napari
-
-from smlmlab.gui import Ui_Frame as gui
-from smlmlab.utils.compute_utils import _utils_compute
-from smlmlab.utils.events_utils import _events_utils
-from smlmlab.utils.import_utils import _import_utils
-from smlmlab.utils.loc_utils import _loc_utils
-from smlmlab.utils.picasso_utils import _picasso_detect_utils
-from smlmlab.utils.viewer_utils import _viewer_utils
-from smlmlab.utils.undrift_utils import _undrift_utils
-
-
-class smlmlabWidget(QWidget, gui,
-    _import_utils, _events_utils,
-    _picasso_detect_utils, _loc_utils,
-    _viewer_utils, _utils_compute,
-    _undrift_utils):
+import napari
 
-    def __init__(self, viewer: "napari.viewer.Viewer"):
-        super().__init__()
-        self.viewer = viewer
+class _utils_compute:
 
-        self.gui = gui()
-        self.gui.setupUi(self)
+    def create_shared_images(self, dataset_list = None, channel_list = None):
 
-        # create pyqt graph container
-        self.graph_container = self.gui.graph_container
-        self.graph_container.setLayout(QVBoxLayout())
+        if self.verbose:
+            print("Creating shared images")
 
-        self.graph_canvas = pg.GraphicsLayoutWidget()
-        self.graph_container.layout().addWidget(self.graph_canvas)
+        if dataset_list is None:
+            dataset_list = list(self.dataset_dict.keys())
+        else:
+            dataset_list = [dataset for dataset in dataset_list if dataset in self.dataset_dict.keys()]
 
-        self.gui.import_data.clicked.connect(self.import_image_data)
+        self.shared_images = []
 
-        self.viewer.dims.events.current_step.connect(partial(self.draw_molecules, update_vis=False))
+        for dataset_name in dataset_list:
 
-        self.gui.picasso_detect.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=False))
-        self.gui.picasso_fit.clicked.connect(partial(self.pixseq_picasso, detect=False, fit=True))
-        self.gui.picasso_detectfit.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=True))
-        self.gui.picasso_render.clicked.connect(self.picasso_render)
-        self.gui.export_locs.clicked.connect(self.initialise_export_locs)
+            if channel_list is None:
+                channel_names = list(self.dataset_dict[dataset_name].keys())
+            else:
+                channel_names = [channel for channel in channel_list if channel in self.dataset_dict[dataset_name].keys()]
 
-        self.gui.picasso_undrift.clicked.connect(self.initialise_undrift)
+            for channel_name in channel_names:
 
-        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
-        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
-        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
-        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
+                if channel_name in self.dataset_dict[dataset_name].keys():
 
-        self.gui.plot_mode.currentIndexChanged.connect(self.draw_line_plot)
-        self.gui.plot_dataset.currentIndexChanged.connect(self.draw_line_plot)
-        self.gui.plot_channel.currentIndexChanged.connect(self.draw_line_plot)
+                    channel_dict = self.dataset_dict[dataset_name][channel_name]
 
-        self.verbose = False
+                    image = channel_dict.pop("data")
 
-        self.dataset_dict = {}
-        self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
-        self.traces_dict = {}
-        self.plot_dict = {}
-        self.contrast_dict = {}
+                    shared_mem = shared_memory.SharedMemory(create=True, size=image.nbytes)
+                    shared_memory_name = shared_mem.name
+                    shared_image = np.ndarray(image.shape, dtype=image.dtype, buffer=shared_mem.buf)
+                    shared_image[:] = image[:]
 
-        self.active_dataset = None
-        self.active_channel = None
+                    n_frames = image.shape[0]
 
-        self.threadpool = QThreadPool()
+                    self.shared_images.append({"dataset": dataset_name,
+                                               "channel": channel_name,
+                                               "gap_label": channel_dict["gap_label"],
+                                               "sequence_label": channel_dict["sequence_label"],
+                                               "n_frames": n_frames,
+                                               "shape": image.shape,
+                                               "dtype": image.dtype,
+                                               "shared_mem": shared_mem,
+                                               "shared_memory_name": shared_memory_name})
 
-        manager = Manager()
-        self.stop_event = manager.Event()
+        return self.shared_images
 
-        self.worker = None
-        self.multiprocessing_active = False
+    def restore_shared_images(self):
 
-        self.viewer.layers.events.inserted.connect(self.on_add_layer)
+        if self.verbose:
+            print("Restoring shared images")
 
-    def on_add_layer(self, event):
-        if event.value.name == "Shapes":
-            self.shapes_layer = self.viewer.layers["Shapes"]
+        if hasattr(self, "shared_images"):
 
-            self.shapes_layer.events.data.connect(self.shapes_layer_updated)
+            for dat in self.shared_images:
+                try:
+                    shared_mem = dat["shared_mem"]
 
-            self.shapes_layer.current_edge_color = list(mcolors.to_rgb("green"))
-            self.shapes_layer.current_face_color = [0, 0, 0, 0]
-            self.shapes_layer.current_edge_width = 1
+                    np_array = np.ndarray(dat["shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
 
-    def shapes_layer_updated(self, event):
-        try:
-            if event.action in ["added", "changed", "removed"]:
-                shapes_layer = self.viewer.layers["Shapes"]
-                shapes = shapes_layer.data
+                    self.dataset_dict[dat["dataset"]][dat["channel"]]["data"] = np_array.copy()
 
-                if len(shapes) > 0:
-                    shape_type = shapes_layer.shape_type[-1]
+                    shared_mem.close()
+                    shared_mem.unlink()
 
-                    if shapes_layer.ndim == 3:
-                        if self.verbose:
-                            print("reformatting shapes to ndim=2")
+                except:
+                    print(traceback.format_exc())
+                    pass
 
-                        shapes = shapes_layer.data.copy()
-                        shapes = [shape[:, -2:] for shape in shapes]
-                        shapes_layer.data = []
-                        shapes_layer.add(shapes, shape_type=shape_type)
+    def create_shared_frames(self, dataset_list = None, channel_list = None):
 
-                    # if event.action == "added":
-                    #     shapes = shapes[-1]
-                    #     shapes_layer.data = shapes
+        if self.verbose:
+            print("Creating shared frames")
 
-                    if shape_type == "line":
-                        self.gui.plot_mode.setCurrentIndex(0)
+        if dataset_list is None:
+            dataset_list = list(self.dataset_dict.keys())
+        else:
+            dataset_list = [dataset for dataset in dataset_list if dataset in self.dataset_dict.keys()]
 
-                    if shape_type == "rectangle":
-                        self.gui.plot_mode.setCurrentIndex(1)
+        self.shared_frames = []
 
-                self.draw_line_plot()
+        for dataset_name in dataset_list:
 
-        except:
-            print(traceback.format_exc())
+            if channel_list is None:
+                channel_names = list(self.dataset_dict[dataset_name].keys())
+            else:
+                channel_names = [channel for channel in channel_list if channel in self.dataset_dict[dataset_name].keys()]
 
-    def get_plot_data(self):
-        plot_dataset = {}
+            for channel_name in channel_names:
 
-        try:
-            layer_names = [layer.name for layer in self.viewer.layers]
+                if channel_name in self.dataset_dict[dataset_name].keys():
 
-            if "Shapes" in layer_names:
-                shapes_layer = self.viewer.layers["Shapes"]
-                shapes = shapes_layer.data.copy()
-                shape_types = shapes_layer.shape_type.copy()
+                    channel_dict = self.dataset_dict[dataset_name][channel_name]
 
-                plot_mode = self.gui.plot_mode.currentIndex()
-                dataset = self.gui.plot_dataset.currentText()
+                    image = channel_dict.pop("data")
 
-                current_frame = self.viewer.dims.current_step[0]
+                    image_dict = {"dataset": dataset_name,
+                                  "channel": channel_name,
+                                  "gap_label": channel_dict["gap_label"],
+                                  "sequence_label": channel_dict["sequence_label"],
+                                  "n_frames": image.shape[0],
+                                  "shape": image.shape,
+                                  "dtype": image.dtype,
+                                  "frame_dict":{},
+                                  }
 
-                for channel in self.dataset_dict[dataset].keys():
-                    if channel not in plot_dataset:
-                        plot_dataset[channel] = {}
+                    for frame_index, frame in enumerate(image):
 
-                    for shape_index, (shape, shape_type) in enumerate(zip(shapes, shape_types)):
-                        if shape_type == "line" and plot_mode == 0:
-                            if shape.shape[-1] == 3:
-                                dat = shape[:, 1:]
-                            else:
-                                dat = shape
+                        if frame_index not in image_dict["frame_dict"]:
+                            image_dict["frame_dict"][frame_index] = {}
 
-                            [[x1, y1], [x2, y2]] = dat
+                        shared_mem = shared_memory.SharedMemory(create=True, size=frame.nbytes)
+                        shared_memory_name = shared_mem.name
+                        shared_frame = np.ndarray(frame.shape, dtype=frame.dtype, buffer=shared_mem.buf)
+                        shared_frame[:] = frame[:]
 
-                            x1, y1 = int(x1), int(y1)
-                            x2, y2 = int(x2), int(y2)
+                        image_dict["frame_dict"][frame_index] = {"frame_index": frame_index,
+                                                                 "dataset": dataset_name,
+                                                                 "channel": channel_name,
+                                                                 "shared_mem": shared_mem,
+                                                                 "shared_memory_name": shared_memory_name,
+                                                                 "shape": frame.shape,
+                                                                 "dtype": frame.dtype,
+                                                                 }
 
-                            num = int(np.hypot(x2 - x1, y2 - y1))
+                self.shared_frames.append(image_dict)
 
-                            img = self.dataset_dict[dataset][channel]["data"][current_frame]
+        return self.shared_frames
 
-                            x, y = np.linspace(x1, x2, num), np.linspace(y1, y2, num)
-                            coords = np.vstack((x, y))
+    def restore_shared_frames(self):
 
-                            line_profile = map_coordinates(img, coords, order=1, mode="nearest")
+        if self.verbose:
+            print("Restoring shared frames")
 
-                            plot_dataset[channel][shape_index] = line_profile
+        if hasattr(self, "shared_frames"):
 
-                        if shape_type == "rectangle" and plot_mode == 1:
-                            if shape.shape[-1] == 3:
-                                dat = shape[:, 1:]
-                            else:
-                                dat = shape
+            for image_dict in self.shared_frames:
 
-                            x1, y1, x2, y2 = (dat[0, 1], dat[0, 0], dat[2, 1], dat[2, 0],)
-                            x1, y1 = int(x1), int(y1)
-                            x2, y2 = int(x2), int(y2)
+                try:
 
-                            img = self.dataset_dict[dataset][channel]["data"]
+                    frame_dict = image_dict["frame_dict"]
 
-                            box_data = img[:, y1:y2, x1:x2]
+                    image = []
 
-                            line_profile = np.mean(box_data, axis=(1, 2))
+                    for frame_index, frame_dict in frame_dict.items():
 
-                            plot_dataset[channel][shape_index] = line_profile
+                        shared_mem = frame_dict["shared_mem"]
 
-                    if set(["donor", "acceptor"]).issubset(plot_dataset.keys()):
-                        plot_dataset = self.calculate_fret(plot_dataset)
+                        frame = np.ndarray(frame_dict["shape"], dtype=frame_dict["dtype"], buffer=shared_mem.buf)
 
-        except:
-            print(traceback.format_exc())
+                        image.append(frame.copy())
+
+                        shared_mem.close()
+                        shared_mem.unlink()
 
-        return plot_dataset
+                    image = np.stack(image, axis=0)
+
+                    self.dataset_dict[image_dict["dataset"]][image_dict["channel"]]["data"] = image
+
+                    shared_mem.close()
+                    shared_mem.unlink()
+
+                except:
+                    print(traceback.format_exc())
+                    pass
+
+    def clear_live_images(self):
 
-    def calculate_fret(self, plot_dataset):
         try:
-            donor_data = plot_dataset["donor"]
-            acceptor_data = plot_dataset["acceptor"]
 
-            for shape_index, (donor, acceptor) in enumerate(zip(donor_data.values(), acceptor_data.values())):
-                if "fret" not in plot_dataset.keys():
-                    plot_dataset["fret"] = {}
+            if self.verbose:
+                print("Clearing live images")
 
-                fret = acceptor / (donor + acceptor)
-                plot_dataset["fret"][shape_index] = fret
+            image_layers = [layer for layer in self.viewer.layers if isinstance(layer, napari.layers.Image)]
+
+            for layer in image_layers:
+
+                # self.viewer.layers.remove(layer)
+
+                frame_shape = layer.data.shape[1:]
+                empty_frame = np.zeros(frame_shape, dtype=layer.data.dtype)
+                layer.data = empty_frame
 
         except:
             print(traceback.format_exc())
+            pass
 
-        return plot_dataset
 
-    def draw_line_plot(self):
-        try:
-            plot_mode = self.gui.plot_mode.currentIndex()
-            plot_channel = self.gui.plot_channel.currentText()
 
-            if "efficiency" in plot_channel.lower():
-                plot_channel = "fret"
 
-            plot_dataset = self.get_plot_data()
 
-            self.graph_canvas.clear()
 
-            if plot_channel.lower() in plot_dataset.keys():
-                plot_data = plot_dataset[plot_channel.lower()]
+class WorkerSignals(QObject):
+    """
+    Defines the signals available from a running worker thread.
 
-                if plot_data != {}:
-                    if plot_mode == 0:
-                        plot_title = "Line profile(s)"
-                    if plot_mode == 1:
-                        plot_title = "Single Molecule Time Series"
+    Supported signals are:
 
-                    ax = self.graph_canvas.addPlot(title=plot_title)
+    finished
+        No data
 
-                    for data in plot_data.values():
-                        ax.plot(data, pen=(255, 0, 0))
+    error
+        tuple (exctype, value, traceback.format_exc() )
 
-                    plt.show()
+    result
+        object data returned from processing, anything
 
+    progress
+        int indicating % progress
+
+    """
+
+    finished = pyqtSignal()
+    error = pyqtSignal(tuple)
+    result = pyqtSignal(object)
+    progress = pyqtSignal(int)
+
+class Worker(QRunnable):
+    """
+    Worker thread
+
+    Inherits from QRunnable to handler worker thread setup, signals and wrap-up.
+
+    :param callback: The function callback to run on this worker thread. Supplied args and
+                     kwargs will be passed through to the runner.
+    :type callback: function
+    :param args: Arguments to pass to the callback function
+    :param kwargs: Keywords to pass to the callback function
+
+    """
+
+    def __init__(self, fn, *args, **kwargs):
+        super().__init__()
+
+        # Store constructor arguments (re-used for processing)
+        self.fn = fn
+        self.args = args
+        self.kwargs = kwargs
+        self.signals = WorkerSignals()
+
+        # Add the callback to our kwargs
+        self.kwargs["progress_callback"] = self.signals.progress
+
+        self._is_stopped = False  # Stop flag
+
+    @pyqtSlot()
+    def run(self):
+        """
+        Initialise the runner function with passed args, kwargs.
+        """
+
+        # Retrieve args/kwargs here; and fire processing using them
+        try:
+
+            while not self._is_stopped:
+                result = self.fn(*self.args, **self.kwargs)
+                self.signals.result.emit(result)  # Emit the result
+                self._is_stopped = True
         except:
-            print(traceback.format_exc())
+            traceback.print_exc()
+            exctype, value = sys.exc_info()[:2]
+            self.signals.error.emit((exctype, value, traceback.format_exc()))
+        finally:
+            self.signals.finished.emit()  # Done
+
+    def result(self):
+        return self.fn(*self.args, **self.kwargs)
+
+    def stop(self):
+
+        self._is_stopped = True
+        self.signals.finished.emit()
```

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/gui.py` & `napari_smlmlab-0.0.6/src/smlmlab/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,14 +386,15 @@
         self.label_16 = QtWidgets.QLabel(self.tab_6)
         self.label_16.setObjectName("label_16")
         self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_16)
         self.plot_mode = QtWidgets.QComboBox(self.tab_6)
         self.plot_mode.setObjectName("plot_mode")
         self.plot_mode.addItem("")
         self.plot_mode.addItem("")
+        self.plot_mode.addItem("")
         self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.plot_mode)
         self.label_17 = QtWidgets.QLabel(self.tab_6)
         self.label_17.setObjectName("label_17")
         self.formLayout_5.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_17)
         self.plot_dataset = QtWidgets.QComboBox(self.tab_6)
         self.plot_dataset.setObjectName("plot_dataset")
         self.formLayout_5.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.plot_dataset)
@@ -570,13 +571,14 @@
         self.picasso_vis_edge_width.setItemText(7, _translate("Frame", "0.8"))
         self.picasso_vis_edge_width.setItemText(8, _translate("Frame", "0.9"))
         self.picasso_vis_edge_width.setItemText(9, _translate("Frame", "1.0"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_4), _translate("Frame", "Visualisation Settings"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Frame", "SMLM"))
         self.label_16.setText(_translate("Frame", "Plot Mode"))
         self.plot_mode.setItemText(0, _translate("Frame", "Line Profiles"))
-        self.plot_mode.setItemText(1, _translate("Frame", "Single Molecule Time Series"))
+        self.plot_mode.setItemText(1, _translate("Frame", "Line Profiles With Gaussian Fit"))
+        self.plot_mode.setItemText(2, _translate("Frame", "Single Molecule Time Series"))
         self.label_17.setText(_translate("Frame", "Plot Dataset"))
         self.label_18.setText(_translate("Frame", "Plot Channel"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Plots"))
         self.label_12.setText(_translate("Frame", "Display Mode"))
         self.label_14.setText(_translate("Frame", "Dataset [PageUp/PageDown]"))
```

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/picasso_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/utils/undrift_utils.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/undrift_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.5/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.0.6/src/smlmlab/utils/viewer_utils.py`

 * *Files identical despite different names*

