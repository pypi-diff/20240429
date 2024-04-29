# Comparing `tmp/napari-conidie-0.0.1.tar.gz` & `tmp/napari_conidie-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-conidie-0.0.1.tar", last modified: Thu Dec 15 13:01:56 2022, max compression
+gzip compressed data, was "napari_conidie-1.0.0.tar", last modified: Mon Apr 29 12:34:05 2024, max compression
```

## Comparing `napari-conidie-0.0.1.tar` & `napari_conidie-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 13:01:56.354609 napari-conidie-0.0.1/
--rw-rw-rw-   0        0        0     1520 2022-10-06 12:07:34.000000 napari-conidie-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      101 2022-10-06 12:07:34.000000 napari-conidie-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4278 2022-12-15 13:01:56.359607 napari-conidie-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2991 2022-12-15 08:23:19.000000 napari-conidie-0.0.1/README.md
--rw-rw-rw-   0        0        0      192 2022-10-06 12:07:34.000000 napari-conidie-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1796 2022-12-15 13:01:56.361609 napari-conidie-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1348 2022-12-15 08:37:15.000000 napari-conidie-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-15 13:01:56.321606 napari-conidie-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-12-15 13:01:56.337609 napari-conidie-0.0.1/src/napari_conidie/
--rw-rw-rw-   0        0        0      235 2022-10-06 12:10:16.000000 napari-conidie-0.0.1/src/napari_conidie/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 13:01:56.353608 napari-conidie-0.0.1/src/napari_conidie/_tests/
--rw-rw-rw-   0        0        0        0 2022-10-06 12:07:34.000000 napari-conidie-0.0.1/src/napari_conidie/_tests/__init__.py
--rw-rw-rw-   0        0        0       84 2022-12-15 07:53:24.000000 napari-conidie-0.0.1/src/napari_conidie/_tests/test_widget.py
--rw-rw-rw-   0        0        0    18127 2022-12-15 12:14:49.000000 napari-conidie-0.0.1/src/napari_conidie/_widget.py
--rw-rw-rw-   0        0        0      839 2022-12-15 07:38:23.000000 napari-conidie-0.0.1/src/napari_conidie/napari.yaml
--rw-rw-rw-   0        0        0      273 2022-10-06 12:10:53.000000 napari-conidie-0.0.1/src/napari_conidie/path.py
-drwxrwxrwx   0        0        0        0 2022-12-15 13:01:56.350607 napari-conidie-0.0.1/src/napari_conidie.egg-info/
--rw-rw-rw-   0        0        0     4278 2022-12-15 13:01:56.000000 napari-conidie-0.0.1/src/napari_conidie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2022-12-15 13:01:56.000000 napari-conidie-0.0.1/src/napari_conidie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 13:01:56.000000 napari-conidie-0.0.1/src/napari_conidie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-12-15 13:01:56.000000 napari-conidie-0.0.1/src/napari_conidie.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2022-12-15 13:01:56.000000 napari-conidie-0.0.1/src/napari_conidie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-12-15 13:01:56.000000 napari-conidie-0.0.1/src/napari_conidie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.229738 napari_conidie-1.0.0/
+-rw-rw-rw-   0        0        0     1520 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5445 2024-04-29 12:34:05.229738 napari_conidie-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2024-04-29 12:31:10.000000 napari_conidie-1.0.0/README.md
+-rw-rw-rw-   0        0        0      192 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1796 2024-04-29 12:34:05.231737 napari_conidie-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2024-04-29 12:33:31.000000 napari_conidie-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.186457 napari_conidie-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.207803 napari_conidie-1.0.0/src/napari_conidie/
+-rw-rw-rw-   0        0        0      191 2024-04-29 12:33:42.000000 napari_conidie-1.0.0/src/napari_conidie/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.225737 napari_conidie-1.0.0/src/napari_conidie/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/src/napari_conidie/_tests/__init__.py
+-rw-rw-rw-   0        0        0       84 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/src/napari_conidie/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    20449 2024-04-29 12:31:10.000000 napari_conidie-1.0.0/src/napari_conidie/_widget.py
+-rw-rw-rw-   0        0        0     1191 2024-04-29 08:03:42.000000 napari_conidie-1.0.0/src/napari_conidie/ilastik_search.py
+-rw-rw-rw-   0        0        0      591 2024-04-29 12:31:10.000000 napari_conidie-1.0.0/src/napari_conidie/napari.yaml
+-rw-rw-rw-   0        0        0      413 2024-04-29 08:04:52.000000 napari_conidie-1.0.0/src/napari_conidie/path.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.227736 napari_conidie-1.0.0/src/napari_conidie.egg-info/
+-rw-rw-rw-   0        0        0     5445 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/top_level.txt
```

### Comparing `napari-conidie-0.0.1/LICENSE` & `napari_conidie-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-conidie-0.0.1/PKG-INFO` & `napari_conidie-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-conidie
-Version: 0.0.1
+Version: 1.0.0
 Summary: A segmentation tool to get conidie and hyphe
 Home-page: https://github.com/hereariim/napari-conidie
 Author: Herearii Metuarea
 Author-email: herearii.metuarea@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hereariim/napari-conidie/issues
 Project-URL: Documentation, https://github.com/hereariim/napari-conidie#README.md
@@ -20,16 +20,30 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: pandas
+Requires-Dist: h5py
+Requires-Dist: scikit-image
+Requires-Dist: napari
+Requires-Dist: matplotlib
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: napari; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
 
 # napari-conidie
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-conidie.svg?color=green)](https://github.com/hereariim/napari-conidie/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-conidie.svg?color=green)](https://pypi.org/project/napari-conidie)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-conidie.svg?color=green)](https://python.org)
 [![tests](https://github.com/hereariim/napari-conidie/workflows/tests/badge.svg)](https://github.com/hereariim/napari-conidie/actions)
@@ -56,19 +70,48 @@
 
 This private tool cannot be found in the built-in napari. The installation therefore follows two steps:
 
 1 - Install latest development version :
 
     git clone https://github.com/hereariim/napari-conidie.git
 
-Or:
+## Getting started
+
+As prerequisite, user must have installed ilastik in its computer.
+
+Before using the plugin, you must have two data:
+
+- The ilastik model
+- The compressed file contained your images structured as followed :
+
+```
+└── Compressed file
+    ├── Folder1
+    │   ├── img0_1.jpg
+    │   ├── img0_2.jpg
+    │   ...
+    │   └── img0_n.jpg
+    │ 
+    ├── Folder2
+    │   ├── img1_1.jpg
+    │   ├── img1_2.jpg
+    │   ...
+    │   └── img1_n.jpg
+    ...
+    │
+    └──  Foldern
+        ├── imgn_1.jpg
+        ├── imgn_2.jpg
+        ...
+        └── imgn_n.jpg
+```
 
-    Download napari-conidie zip file
+## Plugin
 
-2 - Drag and drop napari-conidie file into the built-in
+![here](https://github.com/hereariim/napari-conidie/assets/93375163/07cf6bc3-3d55-4ae1-94ac-8e8b33193963)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari-conidie-0.0.1/README.md` & `napari_conidie-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -27,19 +27,48 @@
 
 This private tool cannot be found in the built-in napari. The installation therefore follows two steps:
 
 1 - Install latest development version :
 
     git clone https://github.com/hereariim/napari-conidie.git
 
-Or:
+## Getting started
 
-    Download napari-conidie zip file
+As prerequisite, user must have installed ilastik in its computer.
 
-2 - Drag and drop napari-conidie file into the built-in
+Before using the plugin, you must have two data:
+
+- The ilastik model
+- The compressed file contained your images structured as followed :
+
+```
+└── Compressed file
+    ├── Folder1
+    │   ├── img0_1.jpg
+    │   ├── img0_2.jpg
+    │   ...
+    │   └── img0_n.jpg
+    │ 
+    ├── Folder2
+    │   ├── img1_1.jpg
+    │   ├── img1_2.jpg
+    │   ...
+    │   └── img1_n.jpg
+    ...
+    │
+    └──  Foldern
+        ├── imgn_1.jpg
+        ├── imgn_2.jpg
+        ...
+        └── imgn_n.jpg
+```
+
+## Plugin
+
+![here](https://github.com/hereariim/napari-conidie/assets/93375163/07cf6bc3-3d55-4ae1-94ac-8e8b33193963)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari-conidie-0.0.1/setup.cfg` & `napari_conidie-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 636f 6e69 6469   = napari-conidi
-00000020: 650d 0a76 6572 7369 6f6e 203d 2030 2e30  e..version = 0.0
-00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
+00000020: 650d 0a76 6572 7369 6f6e 203d 2031 2e30  e..version = 1.0
+00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 7365 676d 656e 7461 7469 6f6e  = A segmentation
 00000050: 2074 6f6f 6c20 746f 2067 6574 2063 6f6e   tool to get con
 00000060: 6964 6965 2061 6e64 2068 7970 6865 0d0a  idie and hyphe..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 000000a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

### Comparing `napari-conidie-0.0.1/setup.py` & `napari_conidie-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh: 
      long_description = fh.read() 
 setup(    
     author="Herearii Metuarea",    
     author_email="herearii.metuarea@gmail.com",
     name='napari-conidie', 
     description='A segmentation tool to get conidie and hyphe',  
-    version="0.0.1",    
+    version="1.0.0",    
     long_description=long_description, 
     long_description_content_type="text/markdown",  
     url='https://github.com/hereariim/napari-conidie', 
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=['numpy',
     'magicgui',
```

### Comparing `napari-conidie-0.0.1/src/napari_conidie/_widget.py` & `napari_conidie-1.0.0/src/napari_conidie/_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import subprocess
 import pathlib
 import tempfile
 from zipfile import ZipFile
 import os
 import napari_conidie.path as paths
-
+import napari_conidie.ilastik_search as il_sh
+import typing
 import re
 import PIL
 
 import h5py
 from collections import Counter
 from pandas import DataFrame
 import shutil
@@ -42,45 +43,49 @@
 from napari.utils.notifications import show_info
 from magicgui import magic_factory
 from magicgui import magicgui
 from magicgui.widgets import Table
 from magicgui.tqdm import trange
 from qtpy.QtWidgets import QTableWidget, QTableWidgetItem, QGridLayout, QFileDialog, QListWidget, QHBoxLayout, QPushButton, QWidget
 from qtpy.QtCore import Qt
-
+import pandas as pd
 # from ilastik.experimental.api import from_project_file
 
+il_sh.ilastik_txt_search()
 
+iter_ = 0
 colormap = cu.label_colormap()
 colors = colormap.colors
 color_dict = {}
 color_dict[0] = colors[0]
 color_dict[1] = colors[1]
 
 zip_dir = tempfile.TemporaryDirectory()
+os.mkdir(os.path.join(zip_dir.name,'data'))
 
 def function_central(filepath,modelname):
     
     path_image = str(filepath).replace('\\','/')
   
     donner = '--raw_data="'+path_image+'"'
     output_dir = tempfile.TemporaryDirectory()
     recevoir = '--output_filename_format="'+os.path.join(output_dir.name,path_image.split('/')[-1][:-4])+'_result_type.jpg"'
     # projet_path = '--project="'+os.path.join(paths.get_models_dir(),'NEW_RETRAIN.ilp')+'"'
     projet_path = '--project='+str(modelname).replace('\\','/')
     
-    check_version = [ix for ix in os.listdir('C:/Program Files') if ix.find('ilastik')!=-1]
-    if len(check_version)==0:
-        show_info('ILASTIK NOT INSTALLED')
-    else:
-        ilastik_version = check_version[0]
-        show_info('ILASTIK VERSION:'+ilastik_version)
-    
-        
-    path_to_run = os.path.join("C:/Program Files",os.path.join(ilastik_version,"ilastik.exe"))
+    # check_version = [ix for ix in os.listdir('C:/Program Files') if ix.find('ilastik')!=-1]
+    # if len(check_version)==0:
+    #     show_info('ILASTIK NOT INSTALLED')
+    # else:
+    #     ilastik_version = check_version[0]
+    #     show_info('ILASTIK VERSION:'+ilastik_version)
+        
+    df = pd.read_csv(paths.get_ilastik_exe(),header=None)
+    path_to_run = df.iloc[0][0]
+    # path_to_run = os.path.join("C:/Program Files",os.path.join(ilastik_version,"ilastik.exe"))
     
     subprocess.run([path_to_run,
                     '--headless',
                     projet_path,
                     '--export_source=Simple Segmentation',
                     donner,
                     recevoir])
@@ -305,100 +310,118 @@
     widget.layout().addWidget(copy_button)
     widget.layout().addWidget(save_button)
     widget.layout().addWidget(view.native)
     widget.layout().addWidget(save_images_button)
 
     return widget
 
-def get_quantitative_data(image, napari_viewer):
-    img=image
-    seuil=25
-
-    connidie=np.where(img==1)
-    hyphe=np.where(img==2)
-    img[connidie]=0
-
-    labels_mask = measure.label(img, background=0) # Solution venant de stackoverflow, Mesure les differents elements                       
-    regions = measure.regionprops(labels_mask)
-    regions.sort(key=lambda x: x.area, reverse=False) 
-
-    print(">",len(hyphe[0]))
-    print(">",len(connidie[0]))
-    
-    minus=0
-    for rg in regions:
-        if len(rg.coords[:,0])>seuil:
-            print(">",len(regions)-minus)
-            break
-        else: 
-            minus+=1    
-    d = {'nombre dhyphes': [len(regions)-minus], 'hyphe': [len(hyphe[0])], 'connidie': [len(connidie[0])]}
-
-    dock_widget = table_to_widget(d)
-    napari_viewer.window.add_dock_widget(dock_widget, area='right')
-    
-def quantitative_data_for_all(dictionnaire,napari_viewer):
-    A = [] #sous dossier
-    B = [] #nom image
-    C = []
-    D = []
-    E = []
-    for ix in dictionnaire.keys():
-        img=dictionnaire[ix]
-        seuil=25
-
-        connidie=np.where(img==1)
-        hyphe=np.where(img==2)
-        img[connidie]=0
-
-        labels_mask = measure.label(img, background=0) # Solution venant de stackoverflow, Mesure les differents elements                       
-        regions = measure.regionprops(labels_mask)
-        regions.sort(key=lambda x: x.area, reverse=False) 
-
-        print(">",len(hyphe[0]))
-        print(">",len(connidie[0]))
-        
-        minus=0
-        for rg in regions:
-            if len(rg.coords[:,0])>seuil:
-                print(">",len(regions)-minus)
-                name_xx = ix.split('xx')
-                A.append(name_xx[0])
-                B.append(name_xx[1])
-                C.append(len(regions)-minus)
-                D.append(len(hyphe[0]))
-                E.append(len(connidie[0]))
-                break
-            else: 
-                minus+=1    
-
-    d = {'sous dossier':A,'nom image':B,'nombre dhyphes': C, 'hyphe': D, 'connidie': E}
-    dock_widget = table_to_widget(d)
-    napari_viewer.window.add_dock_widget(dock_widget, area='right')
+# def get_quantitative_data(image, napari_viewer):
+#     img=image
+#     seuil=25
+
+#     connidie=np.where(img==1)
+#     hyphe=np.where(img==2)
+#     img[connidie]=0
+
+#     labels_mask = measure.label(img, background=0) # Solution venant de stackoverflow, Mesure les differents elements                       
+#     regions = measure.regionprops(labels_mask)
+#     regions.sort(key=lambda x: x.area, reverse=False) 
+
+#     print(">",len(hyphe[0]))
+#     print(">",len(connidie[0]))
+    
+#     minus=0
+#     for rg in regions:
+#         if len(rg.coords[:,0])>seuil:
+#             print(">",len(regions)-minus)
+#             break
+#         else: 
+#             minus+=1    
+#     d = {'nombre dhyphes': [len(regions)-minus], 'hyphe': [len(hyphe[0])], 'connidie': [len(connidie[0])]}
+
+#     dock_widget = table_to_widget(d)
+#     napari_viewer.window.add_dock_widget(dock_widget, area='right')
+    
+# def quantitative_data_for_all(dictionnaire,napari_viewer):
+#     A = [] #sous dossier
+#     B = [] #nom image
+#     C = []
+#     D = []
+#     E = []
+#     for ix in dictionnaire.keys():
+#         img=dictionnaire[ix]
+#         seuil=25
+
+#         connidie=np.where(img==1)
+#         hyphe=np.where(img==2)
+#         img[connidie]=0
+
+#         labels_mask = measure.label(img, background=0) # Solution venant de stackoverflow, Mesure les differents elements                       
+#         regions = measure.regionprops(labels_mask)
+#         regions.sort(key=lambda x: x.area, reverse=False) 
+
+#         print(">",len(hyphe[0]))
+#         print(">",len(connidie[0]))
+        
+#         minus=0
+#         for rg in regions:
+#             if len(rg.coords[:,0])>seuil:
+#                 print(">",len(regions)-minus)
+#                 name_xx = ix.split('xx')
+#                 A.append(name_xx[0])
+#                 B.append(name_xx[1])
+#                 C.append(len(regions)-minus)
+#                 D.append(len(hyphe[0]))
+#                 E.append(len(connidie[0]))
+#                 break
+#             else: 
+#                 minus+=1    
+
+#     d = {'sous dossier':A,'nom image':B,'nombre dhyphes': C, 'hyphe': D, 'connidie': E}
+#     dock_widget = table_to_widget(d)
+#     napari_viewer.window.add_dock_widget(dock_widget, area='right')
+    
+    
+    
+def get_quantitative_data_all_for_csv(dossier_des_images,napari_viewer,image_raw,image_seg):
+    print(image_raw.name)
+    dfl = pd.read_csv(zip_dir.name+'\\'+'data'+'\\'+image_raw.name+'.csv')
+    A_im = np.array(dfl["Image"])
+    A_sb = np.array(dfl["Folder"])
+    print("A_im",A_im)
+    print("A_sb",A_sb)
     
+    n = len(image_raw.data.shape)
     
+    dictionnaire = {}
+    if n==4:
+        msk_stack = image_seg.data
+        total_img,_,_,_ = image_raw.data.shape
+        for ix in range(total_img):
+            dictionnaire[ix]=msk_stack[ix,...]
+    else:
+        dictionnaire[0]=image_seg.data
     
-def get_quantitative_data_all_for_csv(dossier_des_images,napari_viewer):
     A = [] 
     B = []
     C = []
     D = []
     E = []
     
-    dictionnaire = {}
+    # dictionnaire = {}
     
-    for ix in os.listdir(dossier_des_images):
-        chemin_dans_sousdossier = os.path.join(dossier_des_images,ix)
-        print(f'path to {ix} :',chemin_dans_sousdossier)
-        if len(os.listdir(chemin_dans_sousdossier))!=0:
-            for iy in os.listdir(chemin_dans_sousdossier):
-                if iy.find("result")!=-1:
-                    data_dico=imread(os.path.join(chemin_dans_sousdossier,iy))
-                    print("chemin sous dossier",os.path.join(chemin_dans_sousdossier,iy))
-                    dictionnaire[iy]=data_dico
+    # for ix in os.listdir(dossier_des_images):
+    #     chemin_dans_sousdossier = os.path.join(dossier_des_images,ix)
+    #     print(f'path to {ix} :',chemin_dans_sousdossier)
+    #     if len(os.listdir(chemin_dans_sousdossier))!=0:
+    #         for iy in os.listdir(chemin_dans_sousdossier):
+    #             if iy.find("result")!=-1:
+    #                 data_dico=imread(os.path.join(chemin_dans_sousdossier,iy))
+    #                 print("chemin sous dossier",os.path.join(chemin_dans_sousdossier,iy))
+    #                 dictionnaire[iy]=data_dico
 
     for ix in dictionnaire.keys():
         print('ix',ix)
         img=dictionnaire[ix]
         seuil=25
         
         print('before',Counter(img.flatten()))
@@ -410,97 +433,124 @@
         labels_mask = measure.label(img, background=0) # Solution venant de stackoverflow, Mesure les differents elements                       
         regions = measure.regionprops(labels_mask)
         regions.sort(key=lambda x: x.area, reverse=False) 
         
         minus=0
         for rg in regions:
             if len(rg.coords[:,0])>seuil:
-                name_xx = ix.split('xx')
-                A.append(name_xx[0])
-                B.append(name_xx[1][:-4])
+                # name_xx = ix.split('xx')
+                # A.append(name_xx[0])
+                # B.append(name_xx[1][:-4])
+    
+                A.append(A_sb[ix])
+                B.append(A_im[ix])
                 C.append(len(regions)-minus)
                 D.append(len(hyphe[0]))
                 E.append(len(connidie[0]))
                 break
             else: 
                 minus+=1    
 
     d = {'sous dossier':A,'nom image':B,'nombre dhyphes': C, 'hyphe': D, 'connidie': E}
 
     dock_widget = table_to_widget(d)
     napari_viewer.window.add_dock_widget(dock_widget, area='right',name="Save")
     
-    
+
 @magic_factory(call_button="Run segmentation",filename={"label": "Zip file (.zip):"},modelname={"label": "Ilastik model (.ilp):"})
-def process_function_segmentation(napari_viewer : Viewer,filename=pathlib.Path.cwd(),modelname=pathlib.Path.cwd()): 
+def process_function_segmentation(napari_viewer : Viewer,filename=pathlib.Path.cwd(),modelname=pathlib.Path.cwd()) -> typing.List[napari.types.LayerDataTuple]:
+    global iter_
+    iter_+=1
     
     dico = {}
+    print(napari_viewer.add_image)
+    Mask_ = []
+    Imgs_ = []
+    A_folder = []
+    A_name = []
     with ZipFile(filename,'r') as zipObject:
     
         listOfFileNames = zipObject.namelist()
         
         for i in trange(len(listOfFileNames)):
             
             zipObject.extract(listOfFileNames[i],path=zip_dir.name)            
             temp_i = listOfFileNames[i].replace('/','xx').replace(" ","")       
             temp_i_jpg = listOfFileNames[i].replace('/','xx')[:-4].replace(" ","")
+            
+            folder_ = temp_i.split('xx')[0]
+            images_ = temp_i.split('xx')[1]
+            A_folder.append(folder_)
+            A_name.append(images_)            
             os.mkdir(zip_dir.name+'\\'+temp_i_jpg)
+            print(listOfFileNames[i].replace('/','\\'))
             shutil.move(zip_dir.name+'\\'+listOfFileNames[i].replace('/','\\'),zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i)
+            # shutil.copy(zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i,zip_dir.name+'\\'+'data'+'\\'+temp_i)
+            
+            Imgs_.append(imread(zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i))
             image_segm = function_central(zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i,modelname)
+            Mask_.append(image_segm)
             # imsave(zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i_jpg+'_result.png', img_as_uint(image_segm))
-            imsave(zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i_jpg+'_result.png', img_as_ubyte(image_segm))
-            dico[temp_i_jpg+'_result.png'] = image_segm
+            # imsave(zip_dir.name+'\\'+temp_i_jpg+'\\'+temp_i_jpg+'_result.png', img_as_ubyte(image_segm))
+            # imsave(os.path.join(zip_dir.name,'data',temp_i_jpg+'_result.png'), img_as_ubyte(image_segm))
+            # dico[temp_i_jpg+'_result.png'] = image_segm
+    
+    # napari_viewer.add_image(np.array(Imgs_))
+    # napari_viewer.add_labels(np.array(Mask_))
+    dfd = pd.DataFrame({"Folder":A_folder,"Image":A_name})
+    dfd.to_csv(zip_dir.name+'\\'+'data'+'\\'+'Image '+str(iter_)+'.csv',index=False)
+    return [(np.array(Imgs_),{"name":"Image "+str(iter_)},"Image"),(np.array(Mask_),{"name":"Mask"},"Labels")]
             
-    print("Extraction done located into",zip_dir.name)
+    # print("Extraction done located into",zip_dir.name)
         
-    names = []
-    for ix in os.listdir(zip_dir.name):
-        if len(os.listdir(os.path.join(zip_dir.name,ix)))!=0:
-            names.append(ix)
-
-    def open_name(item):
-        
-        name = item.text()
-        name_folder = name[:-4]
-        
-        print('Loading', name, '...')
-
-        napari_viewer.layers.select_all()
-        napari_viewer.layers.remove_selected()    
-        fname = f'{zip_dir.name}\{name}'
-        for fname_i in os.listdir(fname):
-            if fname_i.find('result')!=-1:
-                data_label = imread(f'{fname}\{fname_i}')
-                data_label1 = np.array(data_label)
-                print("Image_count :",Counter(data_label.flatten()))
-                tache=np.where(data_label1==0)
-                condide=np.where(data_label1==257)
-                hyphe=np.where(data_label1==514)
-                data_label1[tache]=0
-                data_label1[hyphe]=2
-                data_label1[condide]=1                
-                napari_viewer.add_labels(data_label1,name=f'{fname_i[:-4]}')
-            else:
-                napari_viewer.add_image(imread(f'{fname}\{fname_i}'),name=f'{fname_i[:-4]}')
-
-        print('... done.')
-
-
-    list_widget = QListWidget()
-    for n in names:
-        list_widget.addItem(n)    
-    list_widget.currentItemChanged.connect(open_name)
-    napari_viewer.window.add_dock_widget([list_widget], area='right',name="Images")
-    list_widget.setCurrentRow(0)
-    
-@magic_factory(call_button="save modification", layout="vertical")
-def save_modification(image_seg : napari.layers.Labels, image_raw : ImageData, napari_viewer : Viewer):
-    data_label = image_seg.data
-    sousdossier = image_seg.name.split('_result')[0]
-    nom_image = image_seg.name.split('xx')[1]
-    os.remove(f'{zip_dir.name}\{sousdossier}\{image_seg}.png')
-    imsave(f'{zip_dir.name}\{sousdossier}\{image_seg}.png', img_as_ubyte(data_label))
+    # names = []
+    # for ix in os.listdir(zip_dir.name):
+    #     if len(os.listdir(os.path.join(zip_dir.name,ix)))!=0:
+    #         names.append(ix)
+
+    # def open_name(item):
+        
+    #     name = item.text()
+    #     name_folder = name[:-4]
+        
+    #     print('Loading', name, '...')
+
+    #     napari_viewer.layers.select_all()
+    #     napari_viewer.layers.remove_selected()    
+    #     fname = f'{zip_dir.name}\{name}'
+    #     for fname_i in os.listdir(fname):
+    #         if fname_i.find('result')!=-1:
+    #             data_label = imread(f'{fname}\{fname_i}')
+    #             data_label1 = np.array(data_label)
+    #             print("Image_count :",Counter(data_label.flatten()))
+    #             tache=np.where(data_label1==0)
+    #             condide=np.where(data_label1==257)
+    #             hyphe=np.where(data_label1==514)
+    #             data_label1[tache]=0
+    #             data_label1[hyphe]=2
+    #             data_label1[condide]=1                
+    #             napari_viewer.add_labels(data_label1,name=f'{fname_i[:-4]}')
+    #         else:
+    #             napari_viewer.add_image(imread(f'{fname}\{fname_i}'),name=f'{fname_i[:-4]}')
+
+    #     print('... done.')
+
+
+    # list_widget = QListWidget()
+    # for n in names:
+    #     list_widget.addItem(n)    
+    # list_widget.currentItemChanged.connect(open_name)
+    # napari_viewer.window.add_dock_widget([list_widget], area='right',name="Images")
+    # list_widget.setCurrentRow(0)
+    
+# @magic_factory(call_button="save modification", layout="vertical")
+# def save_modification(image_seg : napari.layers.Labels, image_raw : ImageData, napari_viewer : Viewer):
+#     data_label = image_seg.data
+#     sousdossier = image_seg.name.split('_result')[0]
+#     nom_image = image_seg.name.split('xx')[1]
+#     os.remove(f'{zip_dir.name}\{sousdossier}\{image_seg}.png')
+#     imsave(f'{zip_dir.name}\{sousdossier}\{image_seg}.png', img_as_ubyte(data_label))
    
 
 @magic_factory(call_button="execute", layout="vertical")
-def quantitative_data_for_all(napari_viewer : Viewer):
-    return get_quantitative_data_all_for_csv(zip_dir.name,napari_viewer)
+def quantitative_data_for_all(napari_viewer : Viewer,image_seg : napari.layers.Labels, image_raw : napari.layers.Image):
+    return get_quantitative_data_all_for_csv(zip_dir.name,napari_viewer,image_raw,image_seg)
```

### Comparing `napari-conidie-0.0.1/src/napari_conidie.egg-info/PKG-INFO` & `napari_conidie-1.0.0/src/napari_conidie.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-conidie
-Version: 0.0.1
+Version: 1.0.0
 Summary: A segmentation tool to get conidie and hyphe
 Home-page: https://github.com/hereariim/napari-conidie
 Author: Herearii Metuarea
 Author-email: herearii.metuarea@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hereariim/napari-conidie/issues
 Project-URL: Documentation, https://github.com/hereariim/napari-conidie#README.md
@@ -20,16 +20,30 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: pandas
+Requires-Dist: h5py
+Requires-Dist: scikit-image
+Requires-Dist: napari
+Requires-Dist: matplotlib
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: napari; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
 
 # napari-conidie
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-conidie.svg?color=green)](https://github.com/hereariim/napari-conidie/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-conidie.svg?color=green)](https://pypi.org/project/napari-conidie)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-conidie.svg?color=green)](https://python.org)
 [![tests](https://github.com/hereariim/napari-conidie/workflows/tests/badge.svg)](https://github.com/hereariim/napari-conidie/actions)
@@ -56,19 +70,48 @@
 
 This private tool cannot be found in the built-in napari. The installation therefore follows two steps:
 
 1 - Install latest development version :
 
     git clone https://github.com/hereariim/napari-conidie.git
 
-Or:
+## Getting started
+
+As prerequisite, user must have installed ilastik in its computer.
+
+Before using the plugin, you must have two data:
+
+- The ilastik model
+- The compressed file contained your images structured as followed :
+
+```
+└── Compressed file
+    ├── Folder1
+    │   ├── img0_1.jpg
+    │   ├── img0_2.jpg
+    │   ...
+    │   └── img0_n.jpg
+    │ 
+    ├── Folder2
+    │   ├── img1_1.jpg
+    │   ├── img1_2.jpg
+    │   ...
+    │   └── img1_n.jpg
+    ...
+    │
+    └──  Foldern
+        ├── imgn_1.jpg
+        ├── imgn_2.jpg
+        ...
+        └── imgn_n.jpg
+```
 
-    Download napari-conidie zip file
+## Plugin
 
-2 - Drag and drop napari-conidie file into the built-in
+![here](https://github.com/hereariim/napari-conidie/assets/93375163/07cf6bc3-3d55-4ae1-94ac-8e8b33193963)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari-conidie-0.0.1/src/napari_conidie.egg-info/SOURCES.txt` & `napari_conidie-1.0.0/src/napari_conidie.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/napari_conidie/__init__.py
 src/napari_conidie/_widget.py
+src/napari_conidie/ilastik_search.py
 src/napari_conidie/napari.yaml
 src/napari_conidie/path.py
 src/napari_conidie.egg-info/PKG-INFO
 src/napari_conidie.egg-info/SOURCES.txt
 src/napari_conidie.egg-info/dependency_links.txt
 src/napari_conidie.egg-info/entry_points.txt
 src/napari_conidie.egg-info/requires.txt
```

