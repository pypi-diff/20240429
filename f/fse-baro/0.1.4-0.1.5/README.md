# Comparing `tmp/fse_baro-0.1.4.tar.gz` & `tmp/fse_baro-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.4.tar", last modified: Mon Apr 29 12:03:35 2024, max compression
+gzip compressed data, was "fse_baro-0.1.5.tar", last modified: Mon Apr 29 12:53:23 2024, max compression
```

## Comparing `fse_baro-0.1.4.tar` & `fse_baro-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.836348 fse_baro-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.832348 fse_baro-0.1.4/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 12:03:30.000000 fse_baro-0.1.4/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.832348 fse_baro-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.832348 fse_baro-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 12:03:30.000000 fse_baro-0.1.4/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 12:03:30.000000 fse_baro-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 12:03:30.000000 fse_baro-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 12:03:30.000000 fse_baro-0.1.4/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 12:03:30.000000 fse_baro-0.1.4/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 12:03:30.000000 fse_baro-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:03:35.836348 fse_baro-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 12:03:30.000000 fse_baro-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 12:03:30.000000 fse_baro-0.1.4/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 12:03:30.000000 fse_baro-0.1.4/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.836348 fse_baro-0.1.4/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 12:03:30.000000 fse_baro-0.1.4/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 12:03:30.000000 fse_baro-0.1.4/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 12:03:30.000000 fse_baro-0.1.4/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 12:03:30.000000 fse_baro-0.1.4/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-29 12:03:30.000000 fse_baro-0.1.4/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.836348 fse_baro-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 12:03:30.000000 fse_baro-0.1.4/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.836348 fse_baro-0.1.4/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:03:35.000000 fse_baro-0.1.4/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 12:03:35.000000 fse_baro-0.1.4/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:03:35.000000 fse_baro-0.1.4/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 12:03:35.000000 fse_baro-0.1.4/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 12:03:35.000000 fse_baro-0.1.4/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 12:03:30.000000 fse_baro-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:03:35.836348 fse_baro-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.836348 fse_baro-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 12:03:30.000000 fse_baro-0.1.4/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:35.836348 fse_baro-0.1.4/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 12:03:30.000000 fse_baro-0.1.4/tutorials/reproduce_multivariate_bocpd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 12:03:30.000000 fse_baro-0.1.4/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.879968 fse_baro-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 12:53:15.000000 fse_baro-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 12:53:15.000000 fse_baro-0.1.5/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 12:53:15.000000 fse_baro-0.1.5/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 12:53:15.000000 fse_baro-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:53:23.887968 fse_baro-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 12:53:15.000000 fse_baro-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 12:53:15.000000 fse_baro-0.1.5/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 12:53:15.000000 fse_baro-0.1.5/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-29 12:53:15.000000 fse_baro-0.1.5/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.883968 fse_baro-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 12:53:15.000000 fse_baro-0.1.5/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 12:53:23.000000 fse_baro-0.1.5/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 12:53:15.000000 fse_baro-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:53:23.887968 fse_baro-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 12:53:15.000000 fse_baro-0.1.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:23.887968 fse_baro-0.1.5/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 12:53:15.000000 fse_baro-0.1.5/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 12:53:15.000000 fse_baro-0.1.5/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.4/.circleci/config.yml` & `fse_baro-0.1.5/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/.github/workflows/build-and-test.yml` & `fse_baro-0.1.5/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/.github/workflows/python-publish.yml` & `fse_baro-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/.gitignore` & `fse_baro-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/INSTALL.md` & `fse_baro-0.1.5/INSTALL.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/LICENSE` & `fse_baro-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/PKG-INFO` & `fse_baro-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.4
+Version: 0.1.5
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fse_baro-0.1.4/README.md` & `fse_baro-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/REQUIREMENTS.md` & `fse_baro-0.1.5/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/STATUS.md` & `fse_baro-0.1.5/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/baro/_bocpd.py` & `fse_baro-0.1.5/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/baro/anomaly_detection.py` & `fse_baro-0.1.5/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/baro/root_cause_analysis.py` & `fse_baro-0.1.5/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/baro/utility.py` & `fse_baro-0.1.5/baro/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 import os
+import glob 
 import shutil
 import requests
 import json
 import zipfile
-from os.path import join 
+from os.path import join, basename, dirname
 
 import numpy as np
 from tqdm import tqdm
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
 def download_online_boutique_dataset(local_path=None):
+    """
+    Download the Online Boutique dataset from Zenodo.
+    """
     if local_path == None:
         local_path = "data"
     if not os.path.exists(local_path):
         os.makedirs(local_path)
-        
+    if os.path.exists(join(local_path, "fse-ob")):
+        return
     download_data("https://zenodo.org/records/11046533/files/fse-ob.zip?download=1", "fse-ob.zip")
     with zipfile.ZipFile("fse-ob.zip", 'r') as file:
         file.extractall(local_path)
     os.remove("fse-ob.zip")
 
 
 def download_sock_shop_dataset(local_path=None):
+    """
+    Download the Sock Shop dataset from Zenodo. 
+    """
     if local_path == None:
         local_path = "data"
     if not os.path.exists(local_path):
         os.makedirs(local_path)
-        
+    if os.path.exists(join(local_path, "fse-ss")):
+        return   
     download_data("https://zenodo.org/records/11046533/files/fse-ss.zip?download=1", "fse-ss.zip")
     with zipfile.ZipFile("fse-ss.zip", 'r') as file:
         file.extractall(local_path)
     os.remove("fse-ss.zip")
 
 
 def download_train_ticket_dataset(local_path=None):
+    """
+    Download the Train Ticket dataset from Zenodo. 
+    """
     if local_path == None:
         local_path = "data"
     if not os.path.exists(local_path):
         os.makedirs(local_path)
-        
+    if os.path.exists(join(local_path, "fse-tt")):
+        return
     download_data("https://zenodo.org/records/11046533/files/fse-tt.zip?download=1", "fse-tt.zip")
     with zipfile.ZipFile("fse-tt.zip", 'r') as file:
         file.extractall(local_path)
     os.remove("fse-tt.zip")
     
 
 def load_json(filename: str):
@@ -119,15 +132,15 @@
     if remote_url is None:
         remote_url = "https://github.com/phamquiluan/baro/releases/download/0.0.4/simple_data.csv"
     if local_path is None:
         local_path = "data.csv"
 
     response = requests.get(remote_url, stream=True)
     total_size_in_bytes = int(response.headers.get("content-length", 0))
-    block_size = 1024  # 1 Kibibyte
+    block_size = 1024 # 1 Kibibyte
 
     progress_bar = tqdm(
         desc=f"Downloading {local_path}..",
         total=total_size_in_bytes,
         unit="iB",
         unit_scale=True,
     )
```

### Comparing `fse_baro-0.1.4/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.5/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.1.5/fse_baro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.4
+Version: 0.1.5
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fse_baro-0.1.4/pyproject.toml` & `fse_baro-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/tests/test.py` & `fse_baro-0.1.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/tutorials/reproduce_multivariate_bocpd.ipynb` & `fse_baro-0.1.5/tutorials/reproduce_multivariate_bocpd.ipynb`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.4/tutorials/reproducibility.ipynb` & `fse_baro-0.1.5/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

