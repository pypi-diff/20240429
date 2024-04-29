# Comparing `tmp/torch_model_manager-0.0.8.dev2.tar.gz` & `tmp/torch_model_manager-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.8.dev2.tar", last modified: Sun Apr 28 10:02:59 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev1.tar", last modified: Mon Apr 29 11:59:28 2024, max compression
```

## Comparing `torch_model_manager-0.0.8.dev2.tar` & `torch_model_manager-0.1.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.229512 torch_model_manager-0.0.8.dev2/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-28 10:02:59.225512 torch_model_manager-0.0.8.dev2/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-28 10:02:59.229512 torch_model_manager-0.0.8.dev2/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-04-28 10:02:53.000000 torch_model_manager-0.0.8.dev2/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.217512 torch_model_manager-0.0.8.dev2/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.217512 torch_model_manager-0.0.8.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.221511 torch_model_manager-0.0.8.dev2/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.221511 torch_model_manager-0.0.8.dev2/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22780 2024-04-28 10:02:30.000000 torch_model_manager-0.0.8.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.0.8.dev2/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.225512 torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-28 10:02:59.000000 torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-28 10:02:59.000000 torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-28 10:02:59.000000 torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-04-28 10:02:59.000000 torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-28 10:02:59.000000 torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-28 10:02:59.225512 torch_model_manager-0.0.8.dev2/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.8.dev2/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.0.8.dev2/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-04-29 11:58:58.000000 torch_model_manager-0.1.0.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.490263 torch_model_manager-0.1.0.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.490263 torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.490263 torch_model_manager-0.1.0.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.494263 torch_model_manager-0.1.0.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23303 2024-04-29 11:52:37.000000 torch_model_manager-0.1.0.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev1/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.498263 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-29 11:59:28.000000 torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-29 11:59:28.494263 torch_model_manager-0.1.0.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.8.dev2/PKG-INFO` & `torch_model_manager-0.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.8.dev2
+Version: 0.1.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.8.dev2/README.md` & `torch_model_manager-0.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.8.dev2/setup.py` & `torch_model_manager-0.1.0.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.0.8.dev2'
+version = '0.1.0.dev1'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.0.8.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.8.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.8.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev1/torch_model_manager/neptune_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from torchviz import make_dot
 from torchcam.methods import LayerCAM, GradCAM, GradCAMpp, SmoothGradCAMpp, ScoreCAM, SSCAM, ISCAM, XGradCAM 
 import sys
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 from utils import helpers
 import torch_model_manager as tmm
 from torchcam.utils import overlay_mask
+import pickle
+import tempfile
 
 
 class NeptuneManager:
     """
     A class for managing Neptune projects and runs.
     """
     # Define static attributes
@@ -206,15 +208,15 @@
                 extension (str, optional): The extension of the file. Defaults to None.
             """
             try:
                 if from_path is not None:
                     self.run[namespace].upload(File.from_path(from_path, extension=extension))
                 else:
                     self.run[namespace].upload(File.as_pickle(data))
-                print(Fore.GREEN+"The data are successfully loaded to Neptune.")
+                print(Fore.GREEN+"The data are successfully loaded to Neptune."+Fore.WHITE)
             except:
                 print(Fore.RED+"The data are not loaded to Neptune. Please check the path or the data format.\
                     This also might due to the existence of the same path in the namespace which risks to be overweighted."+Fore.WHITE)
         
         def log_dataframe(self, 
                           dataframe: pd.DataFrame, 
                           namespace: str, 
@@ -501,15 +503,29 @@
                 self.log_tensors(tensors=res_row, 
                                 names = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
                                 namespace=namespace,
                                 on_series=True)
                     
             print(Fore.GREEN+"The hidden conv2d layer outputs are successfully logged to Neptune.", Fore.WHITE)
             return result, row_index, col_index
+        
+        def fetch_pkl_data(self, namespace: str):
+            
+            tmp_file = tempfile.NamedTemporaryFile(delete=True)
+            try :
+                self.run[namespace].download(tmp_file.name)
+                with open(tmp_file.name, 'rb') as f:
+                    data = pickle.load(f)
             
+                print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
+                return data
+                
+            except:
+                print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
+
 
 
 # nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
 #                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
 #                     run_ids_path="run_ids.json")
 
 # from torchvision import models
@@ -520,11 +536,10 @@
 #     "n_classes": 10,
 #     "model_filename": "basemodel",
 #     "device": torch.device("cuda" if torch.cuda.is_available() else "cpu"),
 #     "epochs": 2,
 # }
 
 
-# run = nm.Run(name="Test2")
-
-# model= models.vgg16()
-# run.log_hidden_conv2d(model, torch.randn(1, 3, 224, 224), indexes=[["features", 0], ["features", 1]], namespace="hidden_conv2d", method="layercam")
+# run = nm.Run(name="Image GAT Message Passing")
+# data = run.fetch_pkl_data("embeddings")
+# print(data)
```

### Comparing `torch_model_manager-0.0.8.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.8.dev2
+Version: 0.1.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.8.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.8.dev2/utils/helpers.py` & `torch_model_manager-0.1.0.dev1/utils/helpers.py`

 * *Files identical despite different names*

