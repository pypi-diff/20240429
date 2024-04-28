# Comparing `tmp/pssr-1.1.0.tar.gz` & `tmp/pssr-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.1.0.tar", max compression
+gzip compressed data, was "pssr-1.1.1.tar", max compression
```

## Comparing `pssr-1.1.0.tar` & `pssr-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.1.0/LICENSE
--rw-r--r--   0        0        0     1135 2024-04-18 21:41:53.895012 pssr-1.1.0/README.md
--rw-r--r--   0        0        0     4388 2024-04-26 16:18:41.417948 pssr-1.1.0/_pssr.py
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.1.0/pssr/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-26 04:19:02.573621 pssr-1.1.0/pssr/crappifiers.py
--rw-r--r--   0        0        0    32538 2024-04-26 16:07:25.348267 pssr-1.1.0/pssr/data.py
--rw-r--r--   0        0        0     2610 2024-04-26 03:52:46.726742 pssr-1.1.0/pssr/loss.py
--rw-r--r--   0        0        0       60 2024-04-16 23:21:24.747072 pssr-1.1.0/pssr/models/__init__.py
--rw-r--r--   0        0        0     1531 2024-04-23 03:43:56.881543 pssr-1.1.0/pssr/models/_blocks.py
--rw-r--r--   0        0        0     3449 2024-04-23 03:55:21.307775 pssr-1.1.0/pssr/models/resunet.py
--rw-r--r--   0        0        0     6143 2024-04-23 03:46:26.643939 pssr-1.1.0/pssr/models/resuneta.py
--rw-r--r--   0        0        0    11102 2024-04-26 16:28:39.578874 pssr-1.1.0/pssr/predict.py
--rw-r--r--   0        0        0    13012 2024-04-26 03:53:11.755078 pssr-1.1.0/pssr/train.py
--rw-r--r--   0        0        0     1125 2024-04-26 04:20:30.130972 pssr-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pssr-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.1.1/README.md
+-rw-r--r--   0        0        0     4388 2024-04-26 16:18:41.417948 pssr-1.1.1/_pssr.py
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.1.1/pssr/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-26 04:19:02.573621 pssr-1.1.1/pssr/crappifiers.py
+-rw-r--r--   0        0        0    32538 2024-04-26 16:07:25.348267 pssr-1.1.1/pssr/data.py
+-rw-r--r--   0        0        0     2610 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/loss.py
+-rw-r--r--   0        0        0       60 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     3449 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/resunet.py
+-rw-r--r--   0        0        0     6143 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/models/resuneta.py
+-rw-r--r--   0        0        0    11102 2024-04-26 16:28:39.578874 pssr-1.1.1/pssr/predict.py
+-rw-r--r--   0        0        0    13012 2024-04-28 22:15:04.325004 pssr-1.1.1/pssr/train.py
+-rw-r--r--   0        0        0     1125 2024-04-28 22:16:40.978868 pssr-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pssr-1.1.1/PKG-INFO
```

### Comparing `pssr-1.1.0/LICENSE` & `pssr-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/_pssr.py` & `pssr-1.1.1/_pssr.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/crappifiers.py` & `pssr-1.1.1/pssr/crappifiers.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/data.py` & `pssr-1.1.1/pssr/data.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/loss.py` & `pssr-1.1.1/pssr/loss.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/models/_blocks.py` & `pssr-1.1.1/pssr/models/_blocks.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/models/resunet.py` & `pssr-1.1.1/pssr/models/resunet.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/models/resuneta.py` & `pssr-1.1.1/pssr/models/resuneta.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/predict.py` & `pssr-1.1.1/pssr/predict.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pssr/train.py` & `pssr-1.1.1/pssr/train.py`

 * *Files identical despite different names*

### Comparing `pssr-1.1.0/pyproject.toml` & `pssr-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pssr"
-version = "1.1.0"
+version = "1.1.1"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
-repository = "https://github.com/haydenstites/PSSR"
-documentation = "https://haydenstites.github.io/PSSR/"
+repository = "https://github.com/ucsdmanorlab/PSSR"
+documentation = "https://ucsdmanorlab.github.io/PSSR/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Environment :: GPU :: NVIDIA CUDA",
```

### Comparing `pssr-1.1.0/PKG-INFO` & `pssr-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.1.0
+Version: 1.1.1
 Summary: Point-Scanning Super-Resolution
-Home-page: https://github.com/haydenstites/PSSR
+Home-page: https://github.com/ucsdmanorlab/PSSR
 License: MIT
 Author: Hayden Stites
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -23,25 +23,25 @@
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pytorch-msssim (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.23.1,<0.24.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
 Requires-Dist: tifffile (>=2024.4.24,<2025.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
-Project-URL: Documentation, https://haydenstites.github.io/PSSR/
-Project-URL: Repository, https://github.com/haydenstites/PSSR
+Project-URL: Documentation, https://ucsdmanorlab.github.io/PSSR/
+Project-URL: Repository, https://github.com/ucsdmanorlab/PSSR
 Description-Content-Type: text/markdown
 
 # Point-Scanning Super-Resolution (**PSSR**)
 
 **PSSR** is a standardized [PyTorch](https://pytorch.org)-based workflow for super-resolution tasks using microscopy images.
 This is the official reimplementation of the methods described in the original paper: [Deep learning-based point-scanning super-resolution imaging](https://www.nature.com/articles/s41592-021-01080-z),
 containing various improvements and new features.
 
-The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://haydenstites.github.io/PSSR).
+The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://ucsdmanorlab.github.io/PSSR).
 
-If you have never used **PSSR** before, [Getting Started](https://haydenstites.github.io/PSSR/guide/start.html) outlines installation and basic usage.
-Full reference and explanations of all **PSSR** tools is available in [API Reference](https://haydenstites.github.io/PSSR/reference/api.html).
+If you have never used **PSSR** before, [Getting Started](https://ucsdmanorlab.github.io/PSSR/guide/start.html) outlines installation and basic usage.
+Full reference and explanations of all **PSSR** tools is available in [API Reference](https://ucsdmanorlab.github.io/PSSR/reference/api.html).
 
-The package is still in development. All code can be found at [https://github.com/haydenstites/PSSR](https://github.com/haydenstites/PSSR).
-If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to [open a ticket](https://github.com/haydenstites/PSSR/issues).
+The package is still in development. All code can be found at [https://github.com/ucsdmanorlab/PSSR](https://github.com/ucsdmanorlab/PSSR).
+If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to [open a ticket](https://github.com/ucsdmanorlab/PSSR/issues).
```

