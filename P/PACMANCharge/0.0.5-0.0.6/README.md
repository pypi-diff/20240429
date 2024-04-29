# Comparing `tmp/PACMANCharge-0.0.5.tar.gz` & `tmp/PACMANCharge-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMANCharge-0.0.5.tar", last modified: Mon Apr 29 04:03:29 2024, max compression
+gzip compressed data, was "PACMANCharge-0.0.6.tar", last modified: Mon Apr 29 04:09:31 2024, max compression
```

## Comparing `PACMANCharge-0.0.5.tar` & `PACMANCharge-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:03:29.318328 PACMANCharge-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMANCharge-0.0.5/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:03:29.211331 PACMANCharge-0.0.5/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)    27638 2024-04-29 04:03:17.000000 PACMANCharge-0.0.5/PACMANCharge/PACMaN.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2024-04-27 15:01:51.000000 PACMANCharge-0.0.5/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMANCharge-0.0.5/PACMANCharge/atom_init.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:03:29.276329 PACMANCharge-0.0.5/PACMANCharge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:03:29.000000 PACMANCharge-0.0.5/PACMANCharge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      314 2024-04-29 04:03:29.000000 PACMANCharge-0.0.5/PACMANCharge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 04:03:29.000000 PACMANCharge-0.0.5/PACMANCharge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-04-29 04:03:29.000000 PACMANCharge-0.0.5/PACMANCharge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-29 04:03:29.000000 PACMANCharge-0.0.5/PACMANCharge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:03:29.316329 PACMANCharge-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4400 2024-04-29 03:12:47.000000 PACMANCharge-0.0.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 04:03:29.319330 PACMANCharge-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1037 2024-04-29 03:58:49.000000 PACMANCharge-0.0.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:03:29.302330 PACMANCharge-0.0.5/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-04-27 15:49:55.000000 PACMANCharge-0.0.5/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMANCharge-0.0.5/test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.356053 PACMANCharge-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMANCharge-0.0.6/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.230294 PACMANCharge-0.0.6/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)    27663 2024-04-29 04:09:09.000000 PACMANCharge-0.0.6/PACMANCharge/PACMaN.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2024-04-27 15:01:51.000000 PACMANCharge-0.0.6/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMANCharge-0.0.6/PACMANCharge/atom_init.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.297294 PACMANCharge-0.0.6/PACMANCharge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      327 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:09:31.354054 PACMANCharge-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4400 2024-04-29 03:12:47.000000 PACMANCharge-0.0.6/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 04:09:31.356053 PACMANCharge-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1037 2024-04-29 04:09:20.000000 PACMANCharge-0.0.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.339041 PACMANCharge-0.0.6/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-04-27 15:49:55.000000 PACMANCharge-0.0.6/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMANCharge-0.0.6/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      146 2024-04-29 04:05:35.000000 PACMANCharge-0.0.6/test/test.py
```

### Comparing `PACMANCharge-0.0.5/LICENSE` & `PACMANCharge-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.5/PACMANCharge/PACMaN.py` & `PACMANCharge-0.0.6/PACMANCharge/PACMaN.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from torch.autograd import Variable
 from pymatgen.core import Structure
 from pymatgen.io.cif import CifParser
 from pymatgen.io.ase import AseAtomsAdaptor
 from torch.utils.data import Dataset,DataLoader
 from collections import defaultdict
 
-package_directory = os.path.abspath(__file__)
+package_directory = os.path.abspath(__file__).replace("PACMaN.py/","")
 
 files_to_download = {
                     'mof-cm5.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/cm5.pth',
                     'mof-cm5.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/normalizer-cm5.pkl',
                     'mof-bader.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/bader.pth',
                     'mof-bader.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/normalizer-bader.pkl',
                     'mof-ddec.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/ddec.pth',
```

### Comparing `PACMANCharge-0.0.5/PACMANCharge/atom_init.json` & `PACMANCharge-0.0.6/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.5/PACMANCharge.egg-info/PKG-INFO` & `PACMANCharge-0.0.6/PACMANCharge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMANCharge
-Version: 0.0.5
+Version: 0.0.6
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMANCharge-0.0.5/PKG-INFO` & `PACMANCharge-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMANCharge
-Version: 0.0.5
+Version: 0.0.6
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMANCharge-0.0.5/README.md` & `PACMANCharge-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.5/setup.py` & `PACMANCharge-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMANCharge",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMANCharge-0.0.5/test/Cu-BTC.cif` & `PACMANCharge-0.0.6/test/Cu-BTC.cif`

 * *Files identical despite different names*

