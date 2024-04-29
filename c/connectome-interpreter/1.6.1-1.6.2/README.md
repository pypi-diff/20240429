# Comparing `tmp/connectome_interpreter-1.6.1.tar.gz` & `tmp/connectome_interpreter-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.6.1.tar", last modified: Sun Apr 28 18:55:03 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.6.2.tar", last modified: Sun Apr 28 19:50:37 2024, max compression
```

## Comparing `connectome_interpreter-1.6.1.tar` & `connectome_interpreter-1.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.939546 connectome_interpreter-1.6.1/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.1/LICENSE
--rw-rw-rw-   0        0        0     1088 2024-04-28 18:55:03.939546 connectome_interpreter-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.894189 connectome_interpreter-1.6.1/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.1/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.6.1/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.1/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16141 2024-04-28 10:55:54.000000 connectome_interpreter-1.6.1/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.1/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.935559 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1088 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-28 18:55:03.000000 connectome_interpreter-1.6.1/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 18:55:03.939546 connectome_interpreter-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1695 2024-04-28 18:51:25.000000 connectome_interpreter-1.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 18:55:03.937552 connectome_interpreter-1.6.1/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.1/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.692154 connectome_interpreter-1.6.2/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0     1095 2024-04-28 19:50:37.692154 connectome_interpreter-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.667269 connectome_interpreter-1.6.2/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.6.2/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.6.2/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    21563 2024-04-28 18:29:19.000000 connectome_interpreter-1.6.2/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.6.2/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.6.2/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.686540 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1095 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-28 19:50:37.000000 connectome_interpreter-1.6.2/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 19:50:37.692154 connectome_interpreter-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1702 2024-04-28 19:48:44.000000 connectome_interpreter-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 19:50:37.690161 connectome_interpreter-1.6.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.6.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.6.2/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.6.2/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.6.1/LICENSE` & `connectome_interpreter-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/PKG-INFO` & `connectome_interpreter-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.6.1
+Version: 1.6.2
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: torch
+Requires-Dist: torch>=1.7.1
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
```

### Comparing `connectome_interpreter-1.6.1/README.md` & `connectome_interpreter-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.6.2/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.6.2/connectome_interpreter/compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.6.2/connectome_interpreter/path_finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,21 @@
       top_n (int, optional): The number of top connections to consider based on direct connectivity from inprop_csc. If top_n = -1, all connections are considered.
       threshold (float, optional): The threshold of the direct connectivity from inidx to an average outidx.
 
     Returns:
       np.ndarray: An array of neuron indices in the previous layer that have significant connectivity, connecting between the `inidx` and `outidx`.
     """
 
-    inidx = to_nparray(inidx)
-    outidx = to_nparray(outidx)
-    # make sure they are integers as well
+    # make sure they are integers
     inidx = [int(i) for i in inidx]
     outidx = [int(i) for i in outidx]
 
+    inidx = to_nparray(inidx)
+    outidx = to_nparray(outidx)
+
     if target_layer_number == 1:
         # if the target layer is 1, we are looking at the direct synaptic connectivity
         # so we just need to find the indices of the non-zero values in the inprop_csc matrix
         # that correspond to the outidx, and intersect those with the inidx we are interested in.
         colidx = inidx
     else:
         # first get the neurons that effectively connect to inidx, at layer number target_layer_number - 1.
```

### Comparing `connectome_interpreter-1.6.1/connectome_interpreter/utils.py` & `connectome_interpreter-1.6.2/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.6.2/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.6.1
+Version: 1.6.2
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
-Requires-Dist: torch
+Requires-Dist: torch>=1.7.1
 Requires-Dist: tqdm
 Requires-Dist: plotly
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
```

### Comparing `connectome_interpreter-1.6.1/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.6.2/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/setup.py` & `connectome_interpreter-1.6.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.6.1',
+    version='1.6.2',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
-        'torch',
+        'torch>=1.7.1',
         'tqdm',
         'plotly',
         'matplotlib',
         'networkx',
         'seaborn',
         'ipywidgets',
         'IPython',
```

### Comparing `connectome_interpreter-1.6.1/tests/test_compress_paths.py` & `connectome_interpreter-1.6.2/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.6.1/tests/test_utils.py` & `connectome_interpreter-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

