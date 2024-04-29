# Comparing `tmp/fse_baro-0.1.1.tar.gz` & `tmp/fse_baro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.1.tar", last modified: Thu Apr 25 06:32:42 2024, max compression
+gzip compressed data, was "fse_baro-0.1.2.tar", last modified: Mon Apr 29 11:51:08 2024, max compression
```

## Comparing `fse_baro-0.1.1.tar` & `fse_baro-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 06:32:31.000000 fse_baro-0.1.1/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.574864 fse_baro-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-25 06:32:31.000000 fse_baro-0.1.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 06:32:31.000000 fse_baro-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-25 06:32:31.000000 fse_baro-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-25 06:32:31.000000 fse_baro-0.1.1/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-25 06:32:31.000000 fse_baro-0.1.1/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 06:32:31.000000 fse_baro-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-25 06:32:42.578864 fse_baro-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-25 06:32:31.000000 fse_baro-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 06:32:31.000000 fse_baro-0.1.1/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 06:32:31.000000 fse_baro-0.1.1/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 06:32:31.000000 fse_baro-0.1.1/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-25 06:32:31.000000 fse_baro-0.1.1/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-25 06:32:31.000000 fse_baro-0.1.1/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 06:32:31.000000 fse_baro-0.1.1/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 06:32:31.000000 fse_baro-0.1.1/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-25 06:32:31.000000 fse_baro-0.1.1/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-25 06:32:42.000000 fse_baro-0.1.1/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-25 06:32:42.000000 fse_baro-0.1.1/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:32:42.000000 fse_baro-0.1.1/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 06:32:42.000000 fse_baro-0.1.1/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 06:32:42.000000 fse_baro-0.1.1/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 06:32:31.000000 fse_baro-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:32:42.578864 fse_baro-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-25 06:32:31.000000 fse_baro-0.1.1/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:32:42.578864 fse_baro-0.1.1/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-25 06:32:31.000000 fse_baro-0.1.1/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.593746 fse_baro-0.1.2/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.593746 fse_baro-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.593746 fse_baro-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 11:51:03.000000 fse_baro-0.1.2/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 11:51:03.000000 fse_baro-0.1.2/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 11:51:03.000000 fse_baro-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 11:51:08.597746 fse_baro-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 11:51:03.000000 fse_baro-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 11:51:03.000000 fse_baro-0.1.2/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 11:51:03.000000 fse_baro-0.1.2/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 11:51:03.000000 fse_baro-0.1.2/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 11:51:03.000000 fse_baro-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:51:08.597746 fse_baro-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 11:51:03.000000 fse_baro-0.1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 11:51:03.000000 fse_baro-0.1.2/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 11:51:03.000000 fse_baro-0.1.2/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.1/.circleci/config.yml` & `fse_baro-0.1.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/.github/workflows/build-and-test.yml` & `fse_baro-0.1.2/.github/workflows/build-and-test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     branches: [ "main" ]
 
 jobs:
   build-linux:
 
     runs-on: ubuntu-latest
     strategy:
-      fail-fast: false
+      fail-fast: true
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
@@ -32,17 +32,17 @@
       run: |
         pytest tests/test.py
 
   build-windows:
 
     runs-on: windows-latest
     strategy:
-      fail-fast: false
+      fail-fast: true
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `fse_baro-0.1.1/.github/workflows/python-publish.yml` & `fse_baro-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/.gitignore` & `fse_baro-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/INSTALL.md` & `fse_baro-0.1.2/INSTALL.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Installation
 
-We assume the users already satisfy the [REQUIREMENTS.md](REQUIREMENTS.md) and have Python 3.10 installed ([Section 1](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#1-install-python310)). Then, users can install BARO from PyPI ([Section 2](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#2-install-baro-from-pypi)) or build BARO from source ([Section 3](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#3-install-baro-from-source)). In addition, users who familiar with Continuous Integration (CI) can take a look at our [build-and-test.yml](https://github.com/phamquiluan/baro/blob/main/.github/workflows/build-and-test.yml) configuration to see how we test our BARO on Linux and Windows machine with Python 3.10, 3.11, and 3.12.
+We assume the users already satisfy the [REQUIREMENTS.md](REQUIREMENTS.md) and have Python 3.10 installed ([Section 1](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#1-install-python310)). Then, users can install BARO from PyPI ([Section 2](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#2-install-baro-from-pypi)) or build BARO from source ([Section 3](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#3-install-baro-from-source)). In addition, users who familiar with Continuous Integration (CI) can take a look at our [build-and-test.yml](https://github.com/phamquiluan/baro/blob/main/.github/workflows/build-and-test.yml) configuration to see how we test our BARO on Linux and Windows machine from Python 3.7 to 3.12.
 
 
 ## 1. Install Python 3.10
 
 ```bash
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt update -y
```

### Comparing `fse_baro-0.1.1/LICENSE` & `fse_baro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/PKG-INFO` & `fse_baro-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.1
+Version: 0.1.2
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -68,20 +68,30 @@
 
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
+import pandas as pd 
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
+from baro.utility import download_data, read_csv
 
-anomalies = bocpd(data)  # the data and its visualization are presented in the Google Colab above.
+# download a sample data to data.csv
+download_data()
+
+# read data, perform anomaly detection and rca using bocpd and robust_scorer
+data = read_csv("data.csv")
+anomalies = bocpd(data)  # data format and visualization are described in the Colab notebook above.
 root_causes = robust_scorer(data, anomalies=anomalies)
 print(root_causes)
+
+# reproducibility
+TODO: add reproducibility
 ```
 
 ## Download Paper
 
 TBD
 
 ## Download Datasets
```

### Comparing `fse_baro-0.1.1/README.md` & `fse_baro-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,20 +29,30 @@
 
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
+import pandas as pd 
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
+from baro.utility import download_data, read_csv
 
-anomalies = bocpd(data)  # the data and its visualization are presented in the Google Colab above.
+# download a sample data to data.csv
+download_data()
+
+# read data, perform anomaly detection and rca using bocpd and robust_scorer
+data = read_csv("data.csv")
+anomalies = bocpd(data)  # data format and visualization are described in the Colab notebook above.
 root_causes = robust_scorer(data, anomalies=anomalies)
 print(root_causes)
+
+# reproducibility
+TODO: add reproducibility
 ```
 
 ## Download Paper
 
 TBD
 
 ## Download Datasets
```

### Comparing `fse_baro-0.1.1/REQUIREMENTS.md` & `fse_baro-0.1.2/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/STATUS.md` & `fse_baro-0.1.2/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/baro/_bocpd.py` & `fse_baro-0.1.2/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/baro/anomaly_detection.py` & `fse_baro-0.1.2/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/baro/root_cause_analysis.py` & `fse_baro-0.1.2/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.2/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.1/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.1.2/fse_baro.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.1
+Version: 0.1.2
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -68,20 +68,30 @@
 
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
+import pandas as pd 
 from baro.anomaly_detection import bocpd
 from baro.root_cause_analysis import robust_scorer
+from baro.utility import download_data, read_csv
 
-anomalies = bocpd(data)  # the data and its visualization are presented in the Google Colab above.
+# download a sample data to data.csv
+download_data()
+
+# read data, perform anomaly detection and rca using bocpd and robust_scorer
+data = read_csv("data.csv")
+anomalies = bocpd(data)  # data format and visualization are described in the Colab notebook above.
 root_causes = robust_scorer(data, anomalies=anomalies)
 print(root_causes)
+
+# reproducibility
+TODO: add reproducibility
 ```
 
 ## Download Paper
 
 TBD
 
 ## Download Datasets
```

### Comparing `fse_baro-0.1.1/pyproject.toml` & `fse_baro-0.1.2/pyproject.toml`

 * *Files identical despite different names*

