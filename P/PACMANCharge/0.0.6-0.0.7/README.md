# Comparing `tmp/PACMANCharge-0.0.6.tar.gz` & `tmp/PACMANCharge-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMANCharge-0.0.6.tar", last modified: Mon Apr 29 04:09:31 2024, max compression
+gzip compressed data, was "PACMANCharge-0.0.7.tar", last modified: Mon Apr 29 04:23:34 2024, max compression
```

## Comparing `PACMANCharge-0.0.6.tar` & `PACMANCharge-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.356053 PACMANCharge-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMANCharge-0.0.6/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.230294 PACMANCharge-0.0.6/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)    27663 2024-04-29 04:09:09.000000 PACMANCharge-0.0.6/PACMANCharge/PACMaN.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2024-04-27 15:01:51.000000 PACMANCharge-0.0.6/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMANCharge-0.0.6/PACMANCharge/atom_init.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.297294 PACMANCharge-0.0.6/PACMANCharge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      327 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-29 04:09:31.000000 PACMANCharge-0.0.6/PACMANCharge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:09:31.354054 PACMANCharge-0.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4400 2024-04-29 03:12:47.000000 PACMANCharge-0.0.6/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 04:09:31.356053 PACMANCharge-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1037 2024-04-29 04:09:20.000000 PACMANCharge-0.0.6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:09:31.339041 PACMANCharge-0.0.6/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-04-27 15:49:55.000000 PACMANCharge-0.0.6/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMANCharge-0.0.6/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      146 2024-04-29 04:05:35.000000 PACMANCharge-0.0.6/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:23:34.726253 PACMANCharge-0.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMANCharge-0.0.7/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:23:34.608729 PACMANCharge-0.0.7/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)    27598 2024-04-29 04:22:48.000000 PACMANCharge-0.0.7/PACMANCharge/PACMaN.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2024-04-27 15:01:51.000000 PACMANCharge-0.0.7/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMANCharge-0.0.7/PACMANCharge/atom_init.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:23:34.676620 PACMANCharge-0.0.7/PACMANCharge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:23:34.000000 PACMANCharge-0.0.7/PACMANCharge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      327 2024-04-29 04:23:34.000000 PACMANCharge-0.0.7/PACMANCharge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 04:23:34.000000 PACMANCharge-0.0.7/PACMANCharge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-04-29 04:23:34.000000 PACMANCharge-0.0.7/PACMANCharge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-29 04:23:34.000000 PACMANCharge-0.0.7/PACMANCharge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     4774 2024-04-29 04:23:34.724254 PACMANCharge-0.0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4400 2024-04-29 03:12:47.000000 PACMANCharge-0.0.7/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 04:23:34.727254 PACMANCharge-0.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1037 2024-04-29 04:23:24.000000 PACMANCharge-0.0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 04:23:34.710253 PACMANCharge-0.0.7/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-04-29 04:22:08.000000 PACMANCharge-0.0.7/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMANCharge-0.0.7/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      145 2024-04-29 04:22:05.000000 PACMANCharge-0.0.7/test/test.py
```

### Comparing `PACMANCharge-0.0.6/LICENSE` & `PACMANCharge-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.6/PACMANCharge/PACMaN.py` & `PACMANCharge-0.0.7/PACMANCharge/PACMaN.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,47 +14,47 @@
 from torch.autograd import Variable
 from pymatgen.core import Structure
 from pymatgen.io.cif import CifParser
 from pymatgen.io.ase import AseAtomsAdaptor
 from torch.utils.data import Dataset,DataLoader
 from collections import defaultdict
 
-package_directory = os.path.abspath(__file__).replace("PACMaN.py/","")
-
+package_directory = os.path.abspath(__file__).replace("PACMaN.py","")
 files_to_download = {
                     'mof-cm5.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/cm5.pth',
                     'mof-cm5.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/normalizer-cm5.pkl',
                     'mof-bader.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/bader.pth',
                     'mof-bader.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/normalizer-bader.pkl',
                     'mof-ddec.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/ddec.pth',
                     'mof-ddec.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/normalizer-ddec.pkl',
                     'cof.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_COF/ddec.pth',
                     'cof.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_COF/normalizer-ddec.pkl',
                     }
 
 for file_name, url in files_to_download.items():
     file_path = os.path.join(package_directory, file_name)
-    response = requests.get(url)
-    if response.status_code == 200:
-        with open(file_path, 'wb') as f:
-            f.write(response.content)
-        print(f"Downloaded {file_name} to {file_path}")
+    if not os.path.exists(file_path):
+        response = requests.get(url)
+        if response.status_code == 200:
+            with open(file_path, 'wb') as f:
+                f.write(response.content)
+            print(f"Downloaded {file_name} to {file_path}")
+        else:
+            print(f"Failed to download {file_name} from {url}")
     else:
-        print(f"Failed to download {file_name} from {url}")
+        pass
 
 import importlib
 import sys
 source = importlib.import_module('PACMANCharge')
 sys.modules['GCNCharge'] = source
-
-class CustomUnpickler(pickle.Unpickler):
-    def find_class(self, module, name):
-        if module == "model.utils":
-            return globals().get(name)
-        return super().find_class(module, name)
+sys.modules['source'] = source
+sys.modules['model.utils'] = source
+sys.modules['source.utils'] = source
+sys.modules['model'] = source
     
 
 periodic_table_symbols = [
     'H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg',
     'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr',
     'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr',
     'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd',
@@ -514,17 +514,15 @@
         elif charge_type == "Bader":
             charge_model_name = resource_filename('PACMANCharge', 'mof-bader.pth')
             nor_name = resource_filename('PACMANCharge', 'mof-bader.pkl')
         elif charge_type == "CM5":
             charge_model_name = resource_filename('PACMANCharge', 'mof-cm5.pth')
             nor_name = resource_filename('PACMANCharge', 'mof-cm5.pkl')
     with open(nor_name, 'rb') as f:
-        unpickler = CustomUnpickler(f)
-        charge_nor = unpickler.load()
-        # charge_nor = pickle.load(f)
+        charge_nor = pickle.load(f)
     f.close()
     try:
         struc = ase_format(cif_file)
         crystal_data = CIF2json(struc,cif_file)
         cell,pos=pre4pre(cif_file)
         dataset = CIFData(crystal_data,pos,cell,6,0,0.2)
         loader= get_data_loader(dataset=dataset, batch_size=1, num_workers=0, collate_fn=collate_pool, pin_memory=False)
```

### Comparing `PACMANCharge-0.0.6/PACMANCharge/atom_init.json` & `PACMANCharge-0.0.7/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.6/PACMANCharge.egg-info/PKG-INFO` & `PACMANCharge-0.0.7/PACMANCharge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMANCharge
-Version: 0.0.6
+Version: 0.0.7
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMANCharge-0.0.6/PKG-INFO` & `PACMANCharge-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMANCharge
-Version: 0.0.6
+Version: 0.0.7
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMANCharge-0.0.6/README.md` & `PACMANCharge-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.6/setup.py` & `PACMANCharge-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMANCharge",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMANCharge-0.0.6/test/Cu-BTC.cif` & `PACMANCharge-0.0.7/test/Cu-BTC.cif`

 * *Files identical despite different names*

