# Comparing `tmp/meni-0.1.1.tar.gz` & `tmp/meni-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meni-0.1.1.tar", max compression
+gzip compressed data, was "meni-0.1.2.tar", max compression
```

## Comparing `meni-0.1.1.tar` & `meni-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,27 @@
--rw-r--r--   0        0        0     1490 2024-03-19 20:22:26.653713 meni-0.1.1/LICENSE
--rw-r--r--   0        0        0     2046 2024-04-18 18:18:05.428346 meni-0.1.1/README.md
--rw-r--r--   0        0        0      150 2024-04-18 03:56:58.735096 meni-0.1.1/meni/__init__.py
--rw-r--r--   0        0        0      848 2024-04-18 04:08:29.075515 meni-0.1.1/meni/__main__.py
--rw-r--r--   0        0        0     2439 2024-04-18 17:37:25.930094 meni-0.1.1/meni/app.py
--rw-r--r--   0        0        0     4853 2024-04-18 16:53:49.295581 meni-0.1.1/meni/assets_rc.py
--rw-r--r--   0        0        0      340 2024-04-02 04:35:25.159956 meni-0.1.1/meni/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    21314 2024-04-18 04:08:17.459374 meni-0.1.1/meni/model/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0    10717 2024-04-18 04:08:13.451325 meni-0.1.1/meni/model/model.py
--rw-r--r--   0        0        0     4818 2024-04-18 16:32:55.229720 meni-0.1.1/meni/rc_assets.py
--rw-r--r--   0        0        0     4766 2024-04-18 02:58:30.122771 meni-0.1.1/meni/theme.py
--rw-r--r--   0        0        0      464 2024-04-02 04:42:03.681225 meni-0.1.1/meni/ui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7522 2024-04-01 08:43:57.085799 meni-0.1.1/meni/ui/__pycache__/collectioninfo.cpython-311.pyc
--rw-r--r--   0        0        0     6891 2024-04-12 05:43:35.293614 meni-0.1.1/meni/ui/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0     3385 2024-03-21 04:25:42.345689 meni-0.1.1/meni/ui/__pycache__/filecontextmenu.cpython-311.pyc
--rw-r--r--   0        0        0     3887 2024-04-01 02:34:44.346849 meni-0.1.1/meni/ui/__pycache__/fileinfo.cpython-311.pyc
--rw-r--r--   0        0        0     6143 2024-03-21 19:51:59.722286 meni-0.1.1/meni/ui/__pycache__/filesgrid.cpython-311.pyc
--rw-r--r--   0        0        0    18045 2024-04-18 04:09:50.188590 meni-0.1.1/meni/ui/__pycache__/filestable.cpython-311.pyc
--rw-r--r--   0        0        0     6351 2024-03-18 19:31:02.485498 meni-0.1.1/meni/ui/__pycache__/flowlayout.cpython-311.pyc
--rw-r--r--   0        0        0     6352 2024-03-21 19:21:47.400790 meni-0.1.1/meni/ui/__pycache__/flowlayout1.cpython-311.pyc
--rw-r--r--   0        0        0     1880 2024-03-18 18:19:21.375000 meni-0.1.1/meni/ui/__pycache__/iconlabel.cpython-311.pyc
--rw-r--r--   0        0        0    16952 2024-03-31 20:44:04.542919 meni-0.1.1/meni/ui/__pycache__/importdialog.cpython-311.pyc
--rw-r--r--   0        0        0     6592 2024-03-19 00:35:17.369593 meni-0.1.1/meni/ui/__pycache__/labelist.cpython-311.pyc
--rw-r--r--   0        0        0     4273 2024-03-18 22:21:28.391667 meni-0.1.1/meni/ui/__pycache__/labeltree.cpython-311.pyc
--rw-r--r--   0        0        0     8295 2024-04-01 03:26:04.142594 meni-0.1.1/meni/ui/__pycache__/mainwindow.cpython-311.pyc
--rw-r--r--   0        0        0     2017 2024-03-31 19:58:00.764989 meni-0.1.1/meni/ui/__pycache__/menusettings.cpython-311.pyc
--rw-r--r--   0        0        0     3407 2024-03-08 08:05:34.174495 meni-0.1.1/meni/ui/__pycache__/modeltable.cpython-311.pyc
--rw-r--r--   0        0        0     6831 2024-04-18 04:08:17.719377 meni-0.1.1/meni/ui/__pycache__/propertyrowwithapply.cpython-311.pyc
--rw-r--r--   0        0        0     3203 2024-03-20 23:46:20.505581 meni-0.1.1/meni/ui/__pycache__/searchinput.cpython-311.pyc
--rw-r--r--   0        0        0     3209 2024-04-18 04:08:17.723377 meni-0.1.1/meni/ui/__pycache__/tagrow.cpython-311.pyc
--rw-r--r--   0        0        0     3008 2024-03-21 03:19:16.647927 meni-0.1.1/meni/ui/__pycache__/viewer.cpython-311.pyc
--rw-r--r--   0        0        0     8193 2024-03-21 18:18:11.355728 meni-0.1.1/meni/ui/__pycache__/welcome.cpython-311.pyc
--rw-r--r--   0        0        0     2898 2024-04-12 05:43:18.249392 meni-0.1.1/meni/ui/common.py
--rw-r--r--   0        0        0     4377 2024-04-13 04:18:53.257391 meni-0.1.1/meni/ui/docks/__pycache__/baseproperties.cpython-311.pyc
--rw-r--r--   0        0        0    21947 2024-04-18 04:08:17.727377 meni-0.1.1/meni/ui/docks/__pycache__/browser.cpython-311.pyc
--rw-r--r--   0        0        0     6246 2024-04-11 19:13:12.192675 meni-0.1.1/meni/ui/docks/__pycache__/collectioninfo.cpython-311.pyc
--rw-r--r--   0        0        0     7786 2024-04-18 04:08:17.719377 meni-0.1.1/meni/ui/docks/__pycache__/collectionproperties.cpython-311.pyc
--rw-r--r--   0        0        0     7681 2024-04-18 04:08:17.723377 meni-0.1.1/meni/ui/docks/__pycache__/fileproperties.cpython-311.pyc
--rw-r--r--   0        0        0     6963 2024-04-11 19:57:18.916545 meni-0.1.1/meni/ui/docks/__pycache__/filters.cpython-311.pyc
--rw-r--r--   0        0        0    15431 2024-04-13 03:52:14.413250 meni-0.1.1/meni/ui/docks/__pycache__/properties.cpython-311.pyc
--rw-r--r--   0        0        0     7046 2024-04-18 04:08:17.723377 meni-0.1.1/meni/ui/docks/__pycache__/viewer.cpython-311.pyc
--rw-r--r--   0        0        0    12600 2024-04-18 04:07:35.742865 meni-0.1.1/meni/ui/docks/browser.py
--rw-r--r--   0        0        0     3580 2024-04-18 04:08:13.659327 meni-0.1.1/meni/ui/docks/collectionproperties.py
--rw-r--r--   0        0        0     3279 2024-04-18 04:08:13.667328 meni-0.1.1/meni/ui/docks/fileproperties.py
--rw-r--r--   0        0        0     3521 2024-04-18 04:07:35.746865 meni-0.1.1/meni/ui/docks/viewer.py
--rw-r--r--   0        0        0     7827 2024-04-18 04:09:43.996508 meni-0.1.1/meni/ui/filestable.py
--rw-r--r--   0        0        0     4817 2024-03-18 19:30:42.929259 meni-0.1.1/meni/ui/flowlayout.py
--rw-r--r--   0        0        0      292 2024-04-02 04:42:03.685225 meni-0.1.1/meni/ui/menus/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4361 2024-04-11 04:47:31.003373 meni-0.1.1/meni/ui/menus/__pycache__/filecontextmenu.cpython-311.pyc
--rw-r--r--   0        0        0     2023 2024-04-01 04:14:26.174050 meni-0.1.1/meni/ui/menus/__pycache__/menusettings.cpython-311.pyc
--rw-r--r--   0        0        0     2019 2024-04-11 04:47:29.287356 meni-0.1.1/meni/ui/menus/filecontextmenu.py
--rw-r--r--   0        0        0      799 2024-03-30 20:38:13.916159 meni-0.1.1/meni/ui/menus/menusettings.py
--rw-r--r--   0        0        0     3168 2024-04-18 04:08:13.531326 meni-0.1.1/meni/ui/propertyrowwithapply.py
--rw-r--r--   0        0        0     1219 2024-03-20 23:46:17.629549 meni-0.1.1/meni/ui/searchinput.py
--rw-r--r--   0        0        0     1341 2024-04-18 04:07:35.446862 meni-0.1.1/meni/ui/tagrow.py
--rw-r--r--   0        0        0     3226 2024-04-18 04:08:17.727377 meni-0.1.1/meni/ui/toolbars/__pycache__/maintoolbar.cpython-311.pyc
--rw-r--r--   0        0        0     1258 2024-04-18 04:07:35.766866 meni-0.1.1/meni/ui/toolbars/maintoolbar.py
--rw-r--r--   0        0        0      345 2024-04-02 04:42:03.761226 meni-0.1.1/meni/ui/windows/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16991 2024-04-18 04:08:17.455374 meni-0.1.1/meni/ui/windows/__pycache__/importdialog.cpython-311.pyc
--rw-r--r--   0        0        0     6619 2024-04-18 04:07:41.194932 meni-0.1.1/meni/ui/windows/__pycache__/mainwindow.cpython-311.pyc
--rw-r--r--   0        0        0     8374 2024-04-18 16:53:56.339690 meni-0.1.1/meni/ui/windows/__pycache__/welcome.cpython-311.pyc
--rw-r--r--   0        0        0     7500 2024-04-18 04:08:13.639327 meni-0.1.1/meni/ui/windows/importdialog.py
--rw-r--r--   0        0        0     3535 2024-04-18 04:07:37.326885 meni-0.1.1/meni/ui/windows/mainwindow.py
--rw-r--r--   0        0        0     4683 2024-04-18 16:50:57.376840 meni-0.1.1/meni/ui/windows/welcome.py
--rw-r--r--   0        0        0     1148 2024-04-18 16:32:37.093507 meni-0.1.1/meni/utils.py
--rw-r--r--   0        0        0      880 2024-03-08 07:40:56.969488 meni-0.1.1/meni/worker.py
--rw-r--r--   0        0        0     1133 2024-04-18 18:19:08.873610 meni-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 meni-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1490 2024-03-19 20:22:26.653713 meni-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2046 2024-04-18 18:18:05.428346 meni-0.1.2/README.md
+-rw-r--r--   0        0        0      150 2024-04-18 03:56:58.735096 meni-0.1.2/meni/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-28 23:42:55.444189 meni-0.1.2/meni/__main__.py
+-rw-r--r--   0        0        0     2439 2024-04-27 03:58:58.344925 meni-0.1.2/meni/app.py
+-rw-r--r--   0        0        0    10717 2024-04-27 04:00:10.714310 meni-0.1.2/meni/model/model.py
+-rw-r--r--   0        0        0     4699 2024-04-27 04:02:08.300488 meni-0.1.2/meni/rc_assets.py
+-rw-r--r--   0        0        0     4766 2024-04-27 03:59:03.609027 meni-0.1.2/meni/theme.py
+-rw-r--r--   0        0        0     3017 2024-04-27 03:59:57.822066 meni-0.1.2/meni/ui/common.py
+-rw-r--r--   0        0        0    12600 2024-04-27 03:59:43.493793 meni-0.1.2/meni/ui/docks/browser.py
+-rw-r--r--   0        0        0     3580 2024-04-27 03:59:45.393829 meni-0.1.2/meni/ui/docks/collectionproperties.py
+-rw-r--r--   0        0        0     3279 2024-04-27 03:59:46.609852 meni-0.1.2/meni/ui/docks/fileproperties.py
+-rw-r--r--   0        0        0     4363 2024-04-27 03:59:47.845876 meni-0.1.2/meni/ui/docks/viewer.py
+-rw-r--r--   0        0        0     7768 2024-04-27 03:59:58.830085 meni-0.1.2/meni/ui/filestable.py
+-rw-r--r--   0        0        0     4817 2024-04-27 04:00:00.386114 meni-0.1.2/meni/ui/flowlayout.py
+-rw-r--r--   0        0        0     2019 2024-04-27 03:59:49.117900 meni-0.1.2/meni/ui/menus/filecontextmenu.py
+-rw-r--r--   0        0        0      799 2024-04-27 03:59:51.205940 meni-0.1.2/meni/ui/menus/menusettings.py
+-rw-r--r--   0        0        0     3168 2024-04-27 15:05:41.987610 meni-0.1.2/meni/ui/propertyrowwithapply.py
+-rw-r--r--   0        0        0     1219 2024-04-27 04:00:04.394190 meni-0.1.2/meni/ui/searchinput.py
+-rw-r--r--   0        0        0     1341 2024-04-27 04:00:05.746216 meni-0.1.2/meni/ui/tagrow.py
+-rw-r--r--   0        0        0     7500 2024-04-27 03:59:53.969992 meni-0.1.2/meni/ui/windows/importdialog.py
+-rw-r--r--   0        0        0     7901 2024-04-27 03:59:55.014012 meni-0.1.2/meni/ui/windows/mainwindow.py
+-rw-r--r--   0        0        0     4683 2024-04-27 03:59:56.626043 meni-0.1.2/meni/ui/windows/welcome.py
+-rw-r--r--   0        0        0     1148 2024-04-27 03:59:06.161076 meni-0.1.2/meni/utils.py
+-rw-r--r--   0        0        0      880 2024-04-27 03:59:08.129114 meni-0.1.2/meni/worker.py
+-rw-r--r--   0        0        0     1178 2024-04-28 23:47:15.739864 meni-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 meni-0.1.2/PKG-INFO
```

### Comparing `meni-0.1.1/LICENSE` & `meni-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/README.md` & `meni-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/__main__.py` & `meni-0.1.2/meni/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from meni.ui.windows.mainwindow import MainWindow
 from meni.ui.windows.welcome import WelcomeWindow
 from meni.app import AppMeni
 import sys
 import argparse
 
 
-if __name__ == "__main__":
-
+def main():
     parser = argparse.ArgumentParser(description="Meni: Library manager for 3D models and assets.")
     parser.add_argument("-l", "--library", help="Path to the library directory.")
     args = parser.parse_args()
 
     app = AppMeni(sys.argv, library=args.library)
 
     # app.setStyleSheet(qdarkstyle.load_stylesheet_pyside6())
@@ -21,7 +20,11 @@
     # apply_stylesheet(app, theme="dark_teal.xml")
     # extra = {"density_scale": "-3"}
     # apply_stylesheet(app, "dark_teal.xml", invert_secondary=False, extra=extra, save_as="stylesheet.css")
 
     app.startup()
 
     app.exec()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `meni-0.1.1/meni/app.py` & `meni-0.1.2/meni/app.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/assets_rc.py` & `meni-0.1.2/meni/rc_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.6.2
+# Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x0c&\
 <\
@@ -202,30 +202,24 @@
 541,-0.17195 z\x22\x0a\
        id=\x22path3\
 65\x22 />\x0a  </g>\x0a</\
 svg>\x0a\
 "
 
 qt_resource_name = b"\
-\x00\x06\
-\x06\x8a\x9c\xb3\
-\x00a\
-\x00s\x00s\x00e\x00t\x00s\
 \x00\x08\
 \x05\xe2T\xa7\
 \x00l\
 \x00o\x00g\x00o\x00.\x00s\x00v\x00g\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x8e\xf2\x10\xc3\x8b\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `meni-0.1.1/meni/model/model.py` & `meni-0.1.2/meni/model/model.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/theme.py` & `meni-0.1.2/meni/theme.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/common.py` & `meni-0.1.2/meni/ui/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,35 +13,37 @@
     def __init__(self):
         super(QVLine, self).__init__()
         self.setFrameShape(QtWidgets.QFrame.VLine)
         self.setFrameShadow(QtWidgets.QFrame.Sunken)
 
 
 class DockTitleBar(QtWidgets.QWidget):
-    def __init__(self, title, clicked=None, parent=None):
+    def __init__(self, title, clicked=None, parent=None, closeable=True, draggable=True):
         super().__init__(parent)
         self.app = QtWidgets.QApplication.instance()
 
         self.layout = QtWidgets.QHBoxLayout()
         self.setLayout(self.layout)
         self.layout.setContentsMargins(3, 3, 3, 3)
         self.layout.setSpacing(3)
 
-        icon = QtWidgets.QLabel()
-        icon.setPixmap(qta.icon("fa5s.grip-vertical", color=self.app.theme.icon_color).pixmap(15))
-        self.layout.addWidget(icon)
+        if draggable:
+            drag_icon = QtWidgets.QLabel()
+            drag_icon.setPixmap(qta.icon("fa5s.grip-vertical", color=self.app.theme.icon_color).pixmap(15))
+            self.layout.addWidget(drag_icon)
 
         label = QtWidgets.QLabel(title)
         label.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         self.layout.addWidget(label)
 
-        close = QtWidgets.QPushButton("", icon=qta.icon("fa5s.times", color=self.app.theme.icon_color), objectName="close", clicked=clicked)
-        close.setFlat(True)
-        close.setMouseTracking(True)
-        self.layout.addWidget(close)
+        if closeable:
+            close = QtWidgets.QPushButton("", icon=qta.icon("fa5s.times", color=self.app.theme.icon_color), objectName="close", clicked=clicked)
+            close.setFlat(True)
+            close.setMouseTracking(True)
+            self.layout.addWidget(close)
         self.setAttribute(QtCore.Qt.WidgetAttribute.WA_StyledBackground, True)
 
         self.setStyleSheet(
             f"""
             DockTitleBar {{
                 background:rgba(0,0,0,0.1);
             }}
```

### Comparing `meni-0.1.1/meni/ui/docks/browser.py` & `meni-0.1.2/meni/ui/docks/browser.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/docks/collectionproperties.py` & `meni-0.1.2/meni/ui/docks/collectionproperties.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/docks/fileproperties.py` & `meni-0.1.2/meni/ui/docks/fileproperties.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/docks/viewer.py` & `meni-0.1.2/meni/ui/docks/viewer.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class ViewerDock(QtWidgets.QDockWidget):
     def __init__(self, parent):
         super().__init__("Viewer", objectName="viewer", parent=parent)
 
         self.app = QtCore.QCoreApplication.instance()
-        self.mesh = None
+        self.mesh_plot = None
+        self.loader = None
+        self.threadpool = QtCore.QThreadPool()
 
         self.setTitleBarWidget(DockTitleBar("Viewer", clicked=self.close))
 
         self.setFeatures(QtWidgets.QDockWidget.DockWidgetFeature.DockWidgetMovable | QtWidgets.QDockWidget.DockWidgetFeature.DockWidgetClosable)
         self.setAllowedAreas(QtCore.Qt.DockWidgetArea.AllDockWidgetAreas)
 
         self.layout = QtWidgets.QVBoxLayout()
@@ -79,17 +81,46 @@
             self.title.setText("")
             self.path.setText("")
             self.collection.setText("")
             self.tagrow.tags = []
             self.show_stl(None)
 
     def show_stl(self, stl):
-        if self.mesh:
-            self.fig.remove_plot(self.mesh)
-
         if stl is None:
             self.fig.update()
             return
 
-        self.mesh = vpl.mesh_plot(Mesh.from_file(stl), color=self.app.theme.model_color, fig=self.fig)
+        if self.loader:
+            self.loader.cancel()
+
+        self.loader = BackgroundLoader(stl)
+        self.threadpool.start(self.loader)
+        self.loader.signals.loaded.connect(self.on_mesh_loaded)
+
+    def on_mesh_loaded(self, mesh):
+        if self.mesh_plot:
+            self.fig.remove_plot(self.mesh_plot)
+        self.mesh_plot = vpl.mesh_plot(mesh, color=self.app.theme.model_color, fig=self.fig)
         vpl.reset_camera(fig=self.fig)
         self.fig.update()
+
+
+class BackgroundLoader(QtCore.QRunnable):
+
+    def __init__(self, path):
+        super(BackgroundLoader, self).__init__()
+        self.path = path
+        self.cancelled = False
+        self.signals = BackgroundLoaderSignals()
+
+    @QtCore.Slot()
+    def run(self):
+        mesh = Mesh.from_file(self.path)
+        if not self.cancelled:
+            self.signals.loaded.emit(mesh)
+
+    def cancel(self):
+        self.cancelled = True
+
+
+class BackgroundLoaderSignals(QtCore.QObject):
+    loaded = QtCore.Signal(Mesh)
```

### Comparing `meni-0.1.1/meni/ui/filestable.py` & `meni-0.1.2/meni/ui/filestable.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         super().__init__()
         self.app = QtCore.QCoreApplication.instance()
         self.delegate = PreviewDelegate()
 
         self.setSelectionMode(QtWidgets.QAbstractItemView.SelectionMode.ExtendedSelection)
         self.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.setModel(TableModel())
-        self.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
 
         self.setItemDelegateForColumn(0, self.delegate)
         self.verticalHeader().setDefaultSectionSize(self.delegate.size)
         self.verticalHeader().hide()
 
         self.selectionModel().selectionChanged.connect(self.on_selection_changed)
         header = self.horizontalHeader()
```

### Comparing `meni-0.1.1/meni/ui/flowlayout.py` & `meni-0.1.2/meni/ui/flowlayout.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/menus/filecontextmenu.py` & `meni-0.1.2/meni/ui/menus/filecontextmenu.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/menus/menusettings.py` & `meni-0.1.2/meni/ui/menus/menusettings.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/propertyrowwithapply.py` & `meni-0.1.2/meni/ui/propertyrowwithapply.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/searchinput.py` & `meni-0.1.2/meni/ui/searchinput.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/tagrow.py` & `meni-0.1.2/meni/ui/tagrow.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/windows/importdialog.py` & `meni-0.1.2/meni/ui/windows/importdialog.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/ui/windows/welcome.py` & `meni-0.1.2/meni/ui/windows/welcome.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/utils.py` & `meni-0.1.2/meni/utils.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/meni/worker.py` & `meni-0.1.2/meni/worker.py`

 * *Files identical despite different names*

### Comparing `meni-0.1.1/pyproject.toml` & `meni-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meni"
-version = "0.1.1"
+version = "0.1.2"
 description = "Software to manage a library of 3d files (stl)"
 authors = ["Diego Pereyra <diego@diegopereyra.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "meni" }]
 homepage = "https://github.com/diesphink/meni"
 repository = "https://github.com/diesphink/meni"
@@ -28,14 +28,17 @@
 numpy-stl = "^3.1.1"
 pyside6 = "^6.7.0"
 qt-material = "^2.14"
 qtawesome = "^1.3.1"
 vtkplotlib = "^2.1.1"
 pyinstaller = "^6.6.0"
 
+[tool.poetry.group.dev.dependencies]
+black = "^21.12b0"
+nuitka = "^2.1.6"
+
+[tool.poetry.scripts]
+meni = "meni.__main__:main"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-#[tool.poetry.scripts]
-#assets = "pyside6-rcc assets.qrc -o meni/rc_assets.py"
-
```

### Comparing `meni-0.1.1/PKG-INFO` & `meni-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meni
-Version: 0.1.1
+Version: 0.1.2
 Summary: Software to manage a library of 3d files (stl)
 Home-page: https://github.com/diesphink/meni
 License: BSD-3-Clause
 Author: Diego Pereyra
 Author-email: diego@diegopereyra.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meni Version: 0.1.1 Summary: Software to manage a
+Metadata-Version: 2.1 Name: meni Version: 0.1.2 Summary: Software to manage a
 library of 3d files (stl) Home-page: https://github.com/diesphink/meni License:
 BSD-3-Clause Author: Diego Pereyra Author-email: diego@diegopereyra.com
 Requires-Python: >=3.9,<3.13 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: X11 Applications :: Qt Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
```

