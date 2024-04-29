# Comparing `tmp/bomcheckgui-1.9.6.tar.gz` & `tmp/bomcheckgui-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomcheckgui-1.9.6.tar", last modified: Thu Mar  7 04:04:30 2024, max compression
+gzip compressed data, was "bomcheckgui-1.9.7.tar", last modified: Mon Apr 29 03:07:05 2024, max compression
```

## Comparing `bomcheckgui-1.9.6.tar` & `bomcheckgui-1.9.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-03-07 04:04:29.603508 bomcheckgui-1.9.6/
--rwxrwx---   0 root         (0) vboxsf     (999)    35149 2022-01-21 03:48:35.000000 bomcheckgui-1.9.6/LICENSE.txt
--rwxrwx---   0 root         (0) vboxsf     (999)      164 2022-03-04 02:02:43.000000 bomcheckgui-1.9.6/MANIFEST.in
--rwxrwx---   0 root         (0) vboxsf     (999)     2508 2024-03-07 04:04:29.599602 bomcheckgui-1.9.6/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)     1695 2023-09-24 01:37:14.000000 bomcheckgui-1.9.6/README.md
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-03-07 04:04:29.523767 bomcheckgui-1.9.6/help_files/
--rwxrwx---   0 root         (0) vboxsf     (999)     2692 2024-01-08 03:37:22.000000 bomcheckgui-1.9.6/help_files/bomcheckgui_help.html
--rwxrwx---   0 root         (0) vboxsf     (999)       48 2024-03-06 03:03:02.000000 bomcheckgui-1.9.6/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       38 2024-03-07 04:04:29.604486 bomcheckgui-1.9.6/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1214 2024-03-07 04:01:27.000000 bomcheckgui-1.9.6/setup.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-03-07 04:04:29.535487 bomcheckgui-1.9.6/src/
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2023-01-28 21:55:32.000000 bomcheckgui-1.9.6/src/__init__.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-03-07 04:04:29.594739 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)     2508 2024-03-07 04:04:28.000000 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      363 2024-03-07 04:04:28.000000 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2024-03-07 04:04:28.000000 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       51 2024-03-07 04:04:28.000000 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/entry_points.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       43 2024-03-07 04:04:28.000000 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       12 2024-03-07 04:04:28.000000 bomcheckgui-1.9.6/src/bomcheckgui.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (999)    48012 2024-03-07 04:01:27.000000 bomcheckgui-1.9.6/src/bomcheckgui.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-29 03:07:04.293911 bomcheckgui-1.9.7/
+-rwxrwx---   0 root         (0) vboxsf     (999)    35149 2022-01-21 03:48:35.000000 bomcheckgui-1.9.7/LICENSE.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)      164 2022-03-04 02:02:43.000000 bomcheckgui-1.9.7/MANIFEST.in
+-rwxrwx---   0 root         (0) vboxsf     (999)     2524 2024-04-29 03:07:04.289026 bomcheckgui-1.9.7/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)     1695 2023-09-24 01:37:14.000000 bomcheckgui-1.9.7/README.md
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-29 03:07:04.230466 bomcheckgui-1.9.7/help_files/
+-rwxrwx---   0 root         (0) vboxsf     (999)     2441 2024-04-27 23:28:32.000000 bomcheckgui-1.9.7/help_files/bomcheckgui_help.html
+-rwxrwx---   0 root         (0) vboxsf     (999)       48 2024-03-06 03:03:02.000000 bomcheckgui-1.9.7/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       38 2024-04-29 03:07:04.294892 bomcheckgui-1.9.7/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1237 2024-04-27 20:41:28.000000 bomcheckgui-1.9.7/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-29 03:07:04.246069 bomcheckgui-1.9.7/src/
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2023-01-28 21:55:32.000000 bomcheckgui-1.9.7/src/__init__.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-29 03:07:04.284147 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)     2524 2024-04-29 03:07:03.000000 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      363 2024-04-29 03:07:03.000000 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2024-04-29 03:07:03.000000 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       51 2024-04-29 03:07:03.000000 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/entry_points.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       43 2024-04-29 03:07:03.000000 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       12 2024-04-29 03:07:03.000000 bomcheckgui-1.9.7/src/bomcheckgui.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)    47995 2024-04-27 23:28:13.000000 bomcheckgui-1.9.7/src/bomcheckgui.py
```

### Comparing `bomcheckgui-1.9.6/LICENSE.txt` & `bomcheckgui-1.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bomcheckgui-1.9.6/PKG-INFO` & `bomcheckgui-1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: bomcheckgui
-Version: 1.9.6
+Version: 1.9.7
 Summary: gui for bomcheck
 Home-page: https://github.com/kcarlton55/bomcheckgui
 Author: Kenneth Edward Carlton
 Author-email: kencarlton55@gmail.com
+License: GPLv3+
 Keywords: BOM,BOMs,compare,bill,materials,SolidWorks,SyteLine,ERP
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `bomcheckgui-1.9.6/README.md` & `bomcheckgui-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `bomcheckgui-1.9.6/help_files/bomcheckgui_help.html` & `bomcheckgui-1.9.7/help_files/bomcheckgui_help.html`

 * *Files 19% similar despite different names*

```diff
@@ -20,42 +20,39 @@
       <li><a href="#intro">Introduction</a></li>
       <li><a href="#run">How to run bomcheckgui</a></li>
       <li><a href="#copy_paste">How to copy & paste from the CAD BOM Table into ERP</a></li>
     </ul>
 
     <h2 id="intro">Introduction</h2>
 
-    <p>The bomcheck program was originally written to be run from a Command
-      Prompt Terminal
+    <p>Bomcheck is a command line interface (cli) program that can
+      be run with the Command Prompt Terminal
       <a href="https://en.wikipedia.org/wiki/Cmd.exe">(cmd.exe)</a>.
-      The program <i>bomcheckgui</i> is actually a wrapper that presents a
-      graphical user interface (gui) for the bomcheck program. That is, bomcheckgui
+      Bomcheckgui is a wrapper of bomcheck that provides
+      graphical user interface (gui) for bomcheck. That is, bomcheckgui
       runs the bomcheck program in the background. </p>
 
 
     <h2 id="run">How to run bomcheckgui:</h2>
 
-    <p>Drag and drop the BOM files that you want to be checked onto the
-      central portion of the gui. File names that do not end with _sw.xlsx or
-      sl_xlsx will be ignored. Files that contain a tilde character, ~, will
-      also be ignored.  Optionally drag and drop a directory that contains the
-      BOM files.</p>
-
-    <p>Press the green check button icon to have your BOMs analyzed. To print
-      results or save results to a csv file, click the boxes located at the
-      bottom of the pop up window containing results.  For more information
-      about csv files, see bomcheck_help.html.</p>
+    <p>Start bomcheckgui and then drag and drop the BOM files that you want to
+      be evaluated onto bomcheckgui's main window. File names that do
+      not end with _sw.xlsx or sl_xlsx will be ignored. Files that contain a
+      tilde character, ~, will also be ignored.  Optionally drag and drop a
+      directory that contains the BOM files.</p>
+
+    <p>Press the green triangle icon to have your BOMs analyzed. Results can be
+      saved to a text file.  For more information about viewing the text files,
+      see bomcheck's help.</p>
 
     <p>To clear the list of files in the drop area, click the clear button, i.e.
-      the windshield wiper icon</p>
+      the eraser icon</p>
 
-    <p>If at some point in your work day you close the folder that contains
-      your BOMs, and later you want to reopen it to make changes, instead of
-      having to search for that folder again, click on the folder icon.
-      Your folder will open.</p>
+    <p>Click on the folder icon to open the folder from which BOM data was last
+      evaluated.</p>
 
 
 
 
   </div>
   <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.10.2/dist/umd/popper.min.js"
     integrity="sha384-7+zCNj/IqJ95wo16oMtfsKbZ9ccEh31eOz1HGyDuCQ6wgnyJNSYdrPa03rtR1zdB"
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
 ************ bboommcchheecckkgguuii hheellpp ************
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _H_o_w_ _t_o_ _r_u_n_ _b_o_m_c_h_e_c_k_g_u_i
     * _H_o_w_ _t_o_ _c_o_p_y_ _&_ _p_a_s_t_e_ _f_r_o_m_ _t_h_e_ _C_A_D_ _B_O_M_ _T_a_b_l_e_ _i_n_t_o_ _E_R_P
 ********** IInnttrroodduuccttiioonn **********
-The bomcheck program was originally written to be run from a Command Prompt
-Terminal _(_c_m_d_._e_x_e_). The program bomcheckgui is actually a wrapper that presents
-a graphical user interface (gui) for the bomcheck program. That is, bomcheckgui
-runs the bomcheck program in the background.
+Bomcheck is a command line interface (cli) program that can be run with the
+Command Prompt Terminal _(_c_m_d_._e_x_e_). Bomcheckgui is a wrapper of bomcheck that
+provides graphical user interface (gui) for bomcheck. That is, bomcheckgui runs
+the bomcheck program in the background.
 ********** HHooww ttoo rruunn bboommcchheecckkgguuii:: **********
-Drag and drop the BOM files that you want to be checked onto the central
-portion of the gui. File names that do not end with _sw.xlsx or sl_xlsx will be
-ignored. Files that contain a tilde character, ~, will also be ignored.
-Optionally drag and drop a directory that contains the BOM files.
-Press the green check button icon to have your BOMs analyzed. To print results
-or save results to a csv file, click the boxes located at the bottom of the pop
-up window containing results. For more information about csv files, see
-bomcheck_help.html.
+Start bomcheckgui and then drag and drop the BOM files that you want to be
+evaluated onto bomcheckgui's main window. File names that do not end with
+_sw.xlsx or sl_xlsx will be ignored. Files that contain a tilde character, ~,
+will also be ignored. Optionally drag and drop a directory that contains the
+BOM files.
+Press the green triangle icon to have your BOMs analyzed. Results can be saved
+to a text file. For more information about viewing the text files, see
+bomcheck's help.
 To clear the list of files in the drop area, click the clear button, i.e. the
-windshield wiper icon
-If at some point in your work day you close the folder that contains your BOMs,
-and later you want to reopen it to make changes, instead of having to search
-for that folder again, click on the folder icon. Your folder will open.
+eraser icon
+Click on the folder icon to open the folder from which BOM data was last
+evaluated.
```

### Comparing `bomcheckgui-1.9.6/setup.py` & `bomcheckgui-1.9.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='bomcheckgui',   # name people will use to pip install
     python_requires='>=3.8',
-    version='1.9.6',
+    version='1.9.7',
     description='gui for bomcheck',
     long_description=long_description,
+    license='GPLv3+',
     long_description_content_type='text/markdown',
     py_modules=['bomcheckgui'],
     package_dir={'': 'src'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
```

### Comparing `bomcheckgui-1.9.6/src/bomcheckgui.egg-info/PKG-INFO` & `bomcheckgui-1.9.7/src/bomcheckgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: bomcheckgui
-Version: 1.9.6
+Version: 1.9.7
 Summary: gui for bomcheck
 Home-page: https://github.com/kcarlton55/bomcheckgui
 Author: Kenneth Edward Carlton
 Author-email: kencarlton55@gmail.com
+License: GPLv3+
 Keywords: BOM,BOMs,compare,bill,materials,SolidWorks,SyteLine,ERP
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `bomcheckgui-1.9.6/src/bomcheckgui.py` & `bomcheckgui-1.9.7/src/bomcheckgui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Wed Jan 20 19:47:41 2021
+Created on Wed Jan 20 19:47:42 2021
 
 @author: ken
 
 A graphical user interface for the bomcheck.py program.
 
 """
 
-__version__ = '1.9.6'
+__version__ = '1.9.7'
 __author__ = 'Kenneth E. Carlton'
 
 #import pdb # use with pdb.set_trace()
 import ast
 import sys
 import os
 sys.path.insert(0, '/media/sf_shared/projects/bomcheck/src')
@@ -32,16 +32,14 @@
 from PyQt5.QtWidgets import (QAction, QApplication, QCheckBox, QComboBox, QDialog,
                              QDialogButtonBox, QFileDialog, QGridLayout,
                              QHBoxLayout, QLabel, QLineEdit, QListWidget, QListWidgetItem,
                              QMainWindow, QMessageBox, QPushButton, QStatusBar,
                              QTableView, QTextEdit, QToolBar, QVBoxLayout,
                              QItemDelegate, QTableWidget, QHeaderView,
                              QTableWidgetItem, QAbstractItemView)
-
-
 printStrs = []
 
 class MainWindow(QMainWindow):
 
     def __init__(self, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         self.setWindowIcon(QIcon('check-mark.png'))
@@ -322,15 +320,15 @@
 
     def _help(self):
         bomcheck.view_help('bomcheck_help', dbdic=self.dbdic)
         # self.dbdic sent so that dictionnary key 'cfgpathname', containing location
         # of bomcheck.cfg file, is sent to function bomcheck.open_help_webpage
 
     def _helpgui(self):
-        bomcheck.view_help('bomcheckgui_help', __version__, dbdic=self.dbdic)  # version here is the bomcheckgui version
+        bomcheck.view_help('bomcheckgui_help', 'main', dbdic=self.dbdic)  # version here is the bomcheckgui version
 
     def _helptroubleshoot(self):
         bomcheck.view_help('bomcheck_troubleshoot', dbdic=self.dbdic)
 
     def _bcgui_license(self):
         bomcheck.view_help('license')
 
@@ -1112,15 +1110,15 @@
     None.
 
     '''
     for x in [f for f in filelst if f[-4:].lower() == '.txt']:
         print(x)
 
 
-def check_latest_version(count, intervals=[0, 1, 4, 10, 20]):
+def check_latest_version(count, intervals=[10,11]):
     '''When bomcheckgui is started, check and see if a later version of
     bomcheckgui and/or bomcheck exist, but don't check every time.  Instead
     check at various intervals.
 
     Parameters
     ----------
     count : int
```

