# Comparing `tmp/fse_baro-0.1.2.tar.gz` & `tmp/fse_baro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.1.2.tar", last modified: Mon Apr 29 11:51:08 2024, max compression
+gzip compressed data, was "fse_baro-0.1.3.tar", last modified: Mon Apr 29 11:54:13 2024, max compression
```

## Comparing `fse_baro-0.1.2.tar` & `fse_baro-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.593746 fse_baro-0.1.2/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.593746 fse_baro-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.593746 fse_baro-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 11:51:03.000000 fse_baro-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 11:51:03.000000 fse_baro-0.1.2/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 11:51:03.000000 fse_baro-0.1.2/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 11:51:03.000000 fse_baro-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 11:51:08.597746 fse_baro-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 11:51:03.000000 fse_baro-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 11:51:03.000000 fse_baro-0.1.2/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 11:51:03.000000 fse_baro-0.1.2/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-29 11:51:03.000000 fse_baro-0.1.2/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 11:51:03.000000 fse_baro-0.1.2/docs/running_time_and_instrumentation_cost.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 11:51:08.000000 fse_baro-0.1.2/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 11:51:03.000000 fse_baro-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:51:08.597746 fse_baro-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 11:51:03.000000 fse_baro-0.1.2/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:51:08.597746 fse_baro-0.1.2/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 11:51:03.000000 fse_baro-0.1.2/tutorials/reproduce_multivariate_bocpd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 11:51:03.000000 fse_baro-0.1.2/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.457786 fse_baro-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 11:54:08.000000 fse_baro-0.1.3/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.449786 fse_baro-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-29 11:54:08.000000 fse_baro-0.1.3/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 11:54:08.000000 fse_baro-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-29 11:54:08.000000 fse_baro-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 11:54:08.000000 fse_baro-0.1.3/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-29 11:54:08.000000 fse_baro-0.1.3/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 11:54:08.000000 fse_baro-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 11:54:13.453786 fse_baro-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-29 11:54:08.000000 fse_baro-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 11:54:08.000000 fse_baro-0.1.3/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 11:54:08.000000 fse_baro-0.1.3/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 11:54:08.000000 fse_baro-0.1.3/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-29 11:54:08.000000 fse_baro-0.1.3/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 11:54:08.000000 fse_baro-0.1.3/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-29 11:54:08.000000 fse_baro-0.1.3/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-29 11:54:08.000000 fse_baro-0.1.3/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 11:54:08.000000 fse_baro-0.1.3/docs/running_time_and_instrumentation_cost.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 11:54:13.000000 fse_baro-0.1.3/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 11:54:13.000000 fse_baro-0.1.3/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:54:13.000000 fse_baro-0.1.3/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 11:54:13.000000 fse_baro-0.1.3/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 11:54:13.000000 fse_baro-0.1.3/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 11:54:08.000000 fse_baro-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:54:13.457786 fse_baro-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-29 11:54:08.000000 fse_baro-0.1.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:54:13.453786 fse_baro-0.1.3/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-29 11:54:08.000000 fse_baro-0.1.3/tutorials/reproduce_multivariate_bocpd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-29 11:54:08.000000 fse_baro-0.1.3/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.1.2/.circleci/config.yml` & `fse_baro-0.1.3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/.github/workflows/build-and-test.yml` & `fse_baro-0.1.3/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/.github/workflows/python-publish.yml` & `fse_baro-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/.gitignore` & `fse_baro-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/INSTALL.md` & `fse_baro-0.1.3/INSTALL.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/LICENSE` & `fse_baro-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/PKG-INFO` & `fse_baro-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.2
+Version: 0.1.3
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fse_baro-0.1.2/README.md` & `fse_baro-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/REQUIREMENTS.md` & `fse_baro-0.1.3/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/STATUS.md` & `fse_baro-0.1.3/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/baro/_bocpd.py` & `fse_baro-0.1.3/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/baro/anomaly_detection.py` & `fse_baro-0.1.3/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/baro/root_cause_analysis.py` & `fse_baro-0.1.3/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/baro/utility.py` & `fse_baro-0.1.3/baro/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -166,8 +166,18 @@
     # cut the data into 10 mins
     data_length = 300
     with open(join(data_dir, "inject_time.txt")) as f:
         inject_time = int(f.readlines()[0].strip())
     normal_df = data[data["time"] < inject_time].tail(data_length)
     anomal_df = data[data["time"] >= inject_time].head(data_length)
     data = pd.concat([normal_df, anomal_df], ignore_index=True)    
-    return data
+    return data
+
+def to_service_ranks(ranks):
+    """Convert fine-grained ranking to service ranks"""
+    _service_ranks = [r.split("_")[0] for r in ranks]
+    service_ranks = []
+    # remove duplicates
+    for s in _service_ranks:
+        if s not in service_ranks:
+            service_ranks.append(s)
+    return service_ranks
```

### Comparing `fse_baro-0.1.2/docs/running_time_and_instrumentation_cost.md` & `fse_baro-0.1.3/docs/running_time_and_instrumentation_cost.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.1.3/fse_baro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.1.2
+Version: 0.1.3
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fse_baro-0.1.2/fse_baro.egg-info/SOURCES.txt` & `fse_baro-0.1.3/fse_baro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/pyproject.toml` & `fse_baro-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/tests/test.py` & `fse_baro-0.1.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/tutorials/reproduce_multivariate_bocpd.ipynb` & `fse_baro-0.1.3/tutorials/reproduce_multivariate_bocpd.ipynb`

 * *Files identical despite different names*

### Comparing `fse_baro-0.1.2/tutorials/reproducibility.ipynb` & `fse_baro-0.1.3/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*

