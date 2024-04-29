# Comparing `tmp/napari_smlmlab-0.0.4.tar.gz` & `tmp/napari_smlmlab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-sjockx7h\napari_smlmlab-0.0.4.tar", last modified: Fri Apr 26 21:40:52 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-cnp7eo9l\napari_smlmlab-0.0.5.tar", last modified: Mon Apr 29 10:12:57 2024, max compression
```

## Comparing `napari_smlmlab-0.0.4.tar` & `napari_smlmlab-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 21:40:52.622081 napari_smlmlab-0.0.4/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-26 21:40:52.622081 napari_smlmlab-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.4/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-26 21:40:52.625250 napari_smlmlab-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 21:40:52.570037 napari_smlmlab-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 21:40:52.619089 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-26 21:40:52.000000 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2024-04-26 21:40:52.000000 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 21:40:52.000000 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-26 21:40:52.000000 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-26 21:40:52.000000 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 21:40:52.000000 napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 21:40:52.603130 napari_smlmlab-0.0.4/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-26 21:40:10.000000 napari_smlmlab-0.0.4/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 21:40:52.606124 napari_smlmlab-0.0.4/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.4/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.4/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0     9749 2024-04-26 21:31:44.000000 napari_smlmlab-0.0.4/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    33082 2024-04-26 16:20:20.000000 napari_smlmlab-0.0.4/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.4/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-26 21:40:52.617094 napari_smlmlab-0.0.4/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    27413 2024-04-26 21:39:16.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    20955 2024-04-26 15:44:32.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.4/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4645 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1819 2024-04-29 10:12:57.739798 napari_smlmlab-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.670807 napari_smlmlab-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4645 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      731 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      148 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 10:12:57.000000 napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.702049 napari_smlmlab-0.0.5/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-04-29 10:12:30.000000 napari_smlmlab-0.0.5/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.717671 napari_smlmlab-0.0.5/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.5/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.5/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     9916 2024-04-29 07:54:07.000000 napari_smlmlab-0.0.5/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    36453 2024-04-29 09:50:44.000000 napari_smlmlab-0.0.5/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.5/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-29 10:12:57.724174 napari_smlmlab-0.0.5/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    27637 2024-04-29 08:31:32.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    21212 2024-04-29 07:50:18.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/undrift_utils.py
+-rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.5/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.4/LICENSE` & `napari_smlmlab-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/PKG-INFO` & `napari_smlmlab-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.4
+Version: 0.0.5
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.4/README.md` & `napari_smlmlab-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/pyproject.toml` & `napari_smlmlab-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/setup.cfg` & `napari_smlmlab-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.4
+Version: 0.0.5
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
```

### Comparing `napari_smlmlab-0.0.4/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.0.5/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 src/smlmlab/_tests/test_widget.py
 src/smlmlab/utils/__init__.py
 src/smlmlab/utils/compute_utils.py
 src/smlmlab/utils/events_utils.py
 src/smlmlab/utils/import_utils.py
 src/smlmlab/utils/loc_utils.py
 src/smlmlab/utils/picasso_utils.py
+src/smlmlab/utils/undrift_utils.py
 src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.0.5/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/_widget.py` & `napari_smlmlab-0.0.5/src/smlmlab/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 from smlmlab.gui import Ui_Frame as gui
 from smlmlab.utils.compute_utils import _utils_compute
 from smlmlab.utils.events_utils import _events_utils
 from smlmlab.utils.import_utils import _import_utils
 from smlmlab.utils.loc_utils import _loc_utils
 from smlmlab.utils.picasso_utils import _picasso_detect_utils
 from smlmlab.utils.viewer_utils import _viewer_utils
+from smlmlab.utils.undrift_utils import _undrift_utils
 
 
-class smlmlabWidget(QWidget, gui, _import_utils, _events_utils, _picasso_detect_utils, _loc_utils, _viewer_utils, _utils_compute, ):
+class smlmlabWidget(QWidget, gui,
+    _import_utils, _events_utils,
+    _picasso_detect_utils, _loc_utils,
+    _viewer_utils, _utils_compute,
+    _undrift_utils):
 
     def __init__(self, viewer: "napari.viewer.Viewer"):
         super().__init__()
         self.viewer = viewer
 
         self.gui = gui()
         self.gui.setupUi(self)
@@ -45,14 +50,16 @@
 
         self.gui.picasso_detect.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=False))
         self.gui.picasso_fit.clicked.connect(partial(self.pixseq_picasso, detect=False, fit=True))
         self.gui.picasso_detectfit.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=True))
         self.gui.picasso_render.clicked.connect(self.picasso_render)
         self.gui.export_locs.clicked.connect(self.initialise_export_locs)
 
+        self.gui.picasso_undrift.clicked.connect(self.initialise_undrift)
+
         self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
         self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
         self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
```

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/gui.py` & `napari_smlmlab-0.0.5/src/smlmlab/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,14 +173,59 @@
         self.picasso_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.picasso_progressbar.setProperty("value", 0)
         self.picasso_progressbar.setObjectName("picasso_progressbar")
         self.verticalLayout_4.addWidget(self.picasso_progressbar)
         spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_4.addItem(spacerItem1)
         self.tabWidget_2.addTab(self.tab_3, "")
+        self.tab_8 = QtWidgets.QWidget()
+        self.tab_8.setObjectName("tab_8")
+        self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.tab_8)
+        self.verticalLayout_9.setObjectName("verticalLayout_9")
+        self.label_7 = QtWidgets.QLabel(self.tab_8)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_7.setFont(font)
+        self.label_7.setObjectName("label_7")
+        self.verticalLayout_9.addWidget(self.label_7)
+        self.formLayout_6 = QtWidgets.QFormLayout()
+        self.formLayout_6.setObjectName("formLayout_6")
+        self.label_19 = QtWidgets.QLabel(self.tab_8)
+        self.label_19.setObjectName("label_19")
+        self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_19)
+        self.picasso_undrift_dataset = QtWidgets.QComboBox(self.tab_8)
+        self.picasso_undrift_dataset.setObjectName("picasso_undrift_dataset")
+        self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_undrift_dataset)
+        self.label_20 = QtWidgets.QLabel(self.tab_8)
+        self.label_20.setObjectName("label_20")
+        self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_20)
+        self.picasso_undrift_channel = QtWidgets.QComboBox(self.tab_8)
+        self.picasso_undrift_channel.setObjectName("picasso_undrift_channel")
+        self.formLayout_6.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_undrift_channel)
+        self.label_21 = QtWidgets.QLabel(self.tab_8)
+        self.label_21.setObjectName("label_21")
+        self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_21)
+        self.picasso_undrift_segmentation = QtWidgets.QSpinBox(self.tab_8)
+        self.picasso_undrift_segmentation.setMaximum(1000)
+        self.picasso_undrift_segmentation.setProperty("value", 100)
+        self.picasso_undrift_segmentation.setObjectName("picasso_undrift_segmentation")
+        self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_undrift_segmentation)
+        self.verticalLayout_9.addLayout(self.formLayout_6)
+        self.picasso_undrift = QtWidgets.QPushButton(self.tab_8)
+        self.picasso_undrift.setObjectName("picasso_undrift")
+        self.verticalLayout_9.addWidget(self.picasso_undrift)
+        self.undrift_progressbar = QtWidgets.QProgressBar(self.tab_8)
+        self.undrift_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
+        self.undrift_progressbar.setProperty("value", 0)
+        self.undrift_progressbar.setObjectName("undrift_progressbar")
+        self.verticalLayout_9.addWidget(self.undrift_progressbar)
+        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_9.addItem(spacerItem2)
+        self.tabWidget_2.addTab(self.tab_8, "")
         self.tab_5 = QtWidgets.QWidget()
         self.tab_5.setObjectName("tab_5")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.tab_5)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.label_2 = QtWidgets.QLabel(self.tab_5)
         font = QtGui.QFont()
         font.setBold(True)
@@ -220,16 +265,16 @@
         self.picasso_render_min_blur.setSingleStep(0.1)
         self.picasso_render_min_blur.setObjectName("picasso_render_min_blur")
         self.formLayout_4.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.picasso_render_min_blur)
         self.verticalLayout_6.addLayout(self.formLayout_4)
         self.picasso_render = QtWidgets.QPushButton(self.tab_5)
         self.picasso_render.setObjectName("picasso_render")
         self.verticalLayout_6.addWidget(self.picasso_render)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_6.addItem(spacerItem2)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_6.addItem(spacerItem3)
         self.tabWidget_2.addTab(self.tab_5, "")
         self.tab_7 = QtWidgets.QWidget()
         self.tab_7.setObjectName("tab_7")
         self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.tab_7)
         self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.label_74 = QtWidgets.QLabel(self.tab_7)
         self.label_74.setObjectName("label_74")
@@ -248,16 +293,16 @@
         self.locs_export_channel = QtWidgets.QComboBox(self.tab_7)
         self.locs_export_channel.setObjectName("locs_export_channel")
         self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.locs_export_channel)
         self.verticalLayout_8.addLayout(self.formLayout_19)
         self.export_locs = QtWidgets.QPushButton(self.tab_7)
         self.export_locs.setObjectName("export_locs")
         self.verticalLayout_8.addWidget(self.export_locs)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_8.addItem(spacerItem3)
+        spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_8.addItem(spacerItem4)
         self.tabWidget_2.addTab(self.tab_7, "")
         self.tab_4 = QtWidgets.QWidget()
         self.tab_4.setObjectName("tab_4")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.tab_4)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.label_27 = QtWidgets.QLabel(self.tab_4)
         font = QtGui.QFont()
@@ -321,20 +366,20 @@
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_edge_width, 1, 3, 1, 1)
         self.verticalLayout_5.addLayout(self.gridLayout_14)
-        spacerItem4 = QtWidgets.QSpacerItem(20, 215, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_5.addItem(spacerItem4)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 215, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem5)
         self.tabWidget_2.addTab(self.tab_4, "")
         self.verticalLayout_3.addWidget(self.tabWidget_2)
-        spacerItem5 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem5)
+        spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem6)
         self.tabWidget.addTab(self.tab_2, "")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.formLayout_5 = QtWidgets.QFormLayout()
         self.formLayout_5.setObjectName("formLayout_5")
@@ -460,14 +505,20 @@
         self.picasso_remove_overlapping.setText(_translate("Frame", "Remove Overlapping Fiducials/Bounding Boxes (determined by Picaso Box Size)"))
         self.picasso_window_cropping.setText(_translate("Frame", "Remove Localisations Outside Field Of View (FOV)"))
         self.picasso_minimise_ram.setText(_translate("Frame", "Minimise RAM usage"))
         self.picasso_fit.setText(_translate("Frame", "Fit"))
         self.picasso_detect.setText(_translate("Frame", "Detect"))
         self.picasso_detectfit.setText(_translate("Frame", "Detect and Fit"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_3), _translate("Frame", "Detect"))
+        self.label_7.setText(_translate("Frame", "Detect Localisations (Picasso)"))
+        self.label_19.setText(_translate("Frame", "Dataset"))
+        self.label_20.setText(_translate("Frame", "Channel"))
+        self.label_21.setText(_translate("Frame", "Segmentation"))
+        self.picasso_undrift.setText(_translate("Frame", "Undrift Localisations"))
+        self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_8), _translate("Frame", "Undrift"))
         self.label_2.setText(_translate("Frame", "Render Fiducials (Picasso)"))
         self.label_4.setText(_translate("Frame", "Dataset"))
         self.label_9.setText(_translate("Frame", "Channel"))
         self.label_10.setText(_translate("Frame", "Blur Method"))
         self.picasso_render_blur_method.setItemText(0, _translate("Frame", "None"))
         self.picasso_render_blur_method.setItemText(1, _translate("Frame", "One-Pixel-Blur"))
         self.picasso_render_blur_method.setItemText(2, _translate("Frame", "Global Localisation Precision"))
```

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.0.5/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.0.5/src/smlmlab/utils/events_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 
     def update_ui(self, error=None, init=False):
         try:
             if self.verbose:
                 print(f"Updating UI, init = {init}")
 
             controls = ["import_data", "picasso_detect", "picasso_fit",
-                        "picasso_detectfit", "picasso_render", "export_locs"]
+                        "picasso_detectfit", "picasso_render", "export_locs",
+                        "picasso_undrift"]
 
-            progressbars = ["import_progressbar", "picasso_progressbar", ]
+            progressbars = ["import_progressbar", "picasso_progressbar",
+                            "undrift_progressbar"]
 
             for progressbar in progressbars:
                 if hasattr(self.gui, progressbar):
                     getattr(self.gui, progressbar).setValue(0)
 
             if init is True:
                 for control in controls:
@@ -343,14 +345,15 @@
             if self.verbose:
                 print("Populating channel selectors")
 
             self.update_channel_selector(dataset_selector="picasso_dataset", channel_selector="picasso_channel", )
             self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel", )
             self.update_channel_selector(dataset_selector="plot_dataset", channel_selector="plot_channel", efficiency=True, )
             self.update_channel_selector(dataset_selector="locs_export_dataset", channel_selector="locs_export_channel")
+            self.update_channel_selector(dataset_selector="picasso_undrift_dataset", channel_selector="picasso_undrift_channel")
 
         except:
             print(traceback.format_exc())
 
     def update_channel_select_buttons(self):
         try:
             datast_name = self.gui.dataset_selector.currentText()
```

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.0.5/src/smlmlab/utils/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,19 @@
             self.gui.plot_dataset.blockSignals(False)
 
             self.gui.locs_export_dataset.blockSignals(True)
             self.gui.locs_export_dataset.clear()
             self.gui.locs_export_dataset.addItems(dataset_names)
             self.gui.locs_export_dataset.blockSignals(False)
 
+            self.gui.picasso_undrift_dataset.blockSignals(True)
+            self.gui.picasso_undrift_dataset.clear()
+            self.gui.picasso_undrift_dataset.addItems(dataset_names)
+            self.gui.picasso_undrift_dataset.blockSignals(False)
+
         except:
             print(traceback.format_exc())
 
     def initialise_localisation_dict(self):
         if hasattr(self, "localisation_dict"):
             self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
```

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.0.5/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.0.5/src/smlmlab/utils/picasso_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.4/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.0.5/src/smlmlab/utils/viewer_utils.py`

 * *Files identical despite different names*

