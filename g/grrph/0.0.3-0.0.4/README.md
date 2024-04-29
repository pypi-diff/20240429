# Comparing `tmp/grrph-0.0.3.tar.gz` & `tmp/grrph-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrph-0.0.3.tar", last modified: Tue Feb 13 09:02:10 2024, max compression
+gzip compressed data, was "grrph-0.0.4.tar", last modified: Mon Apr 29 11:07:19 2024, max compression
```

## Comparing `grrph-0.0.3.tar` & `grrph-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-02-13 09:02:10.390388 grrph-0.0.3/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     1069 2024-01-07 08:04:06.000000 grrph-0.0.3/LICENSE
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1042 2024-02-13 09:02:10.390388 grrph-0.0.3/PKG-INFO
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      476 2024-02-13 08:33:17.000000 grrph-0.0.3/README.md
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-02-13 09:02:10.390388 grrph-0.0.3/grrph/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)        0 2024-02-13 06:43:57.000000 grrph-0.0.3/grrph/__init__.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     1736 2024-02-13 08:59:53.000000 grrph-0.0.3/grrph/converter.py
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-02-13 09:02:10.390388 grrph-0.0.3/grrph/datasets/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     5330 2024-02-13 08:40:12.000000 grrph-0.0.3/grrph/datasets/RIGIDDataset.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)        0 2024-02-13 08:42:32.000000 grrph-0.0.3/grrph/fast_wl.py
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-02-13 09:02:10.390388 grrph-0.0.3/grrph/sklearn/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      647 2024-02-13 08:43:47.000000 grrph-0.0.3/grrph/sklearn/ensembling.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     1498 2024-02-13 08:43:47.000000 grrph-0.0.3/grrph/sklearn/preprocessing.py
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-02-13 09:02:10.390388 grrph-0.0.3/grrph.egg-info/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1042 2024-02-13 09:02:10.000000 grrph-0.0.3/grrph.egg-info/PKG-INFO
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      320 2024-02-13 09:02:10.000000 grrph-0.0.3/grrph.egg-info/SOURCES.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)        1 2024-02-13 09:02:10.000000 grrph-0.0.3/grrph.egg-info/dependency_links.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       21 2024-02-13 09:02:10.000000 grrph-0.0.3/grrph.egg-info/requires.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)        6 2024-02-13 09:02:10.000000 grrph-0.0.3/grrph.egg-info/top_level.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      539 2024-02-13 09:00:20.000000 grrph-0.0.3/pyproject.toml
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       38 2024-02-13 09:02:10.390388 grrph-0.0.3/setup.cfg
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-04-29 11:07:19.509191 grrph-0.0.4/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     1069 2024-01-07 08:04:06.000000 grrph-0.0.4/LICENSE
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1061 2024-04-29 11:07:19.509191 grrph-0.0.4/PKG-INFO
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      476 2024-02-13 08:33:17.000000 grrph-0.0.4/README.md
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-04-29 11:07:19.509191 grrph-0.0.4/grrph/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)        0 2024-02-13 06:43:57.000000 grrph-0.0.4/grrph/__init__.py
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-04-29 11:07:19.509191 grrph-0.0.4/grrph/connectors/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     6367 2024-04-02 07:58:17.000000 grrph-0.0.4/grrph/connectors/outerplanarity.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     2387 2024-04-02 14:56:43.000000 grrph-0.0.4/grrph/converter.py
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-04-29 11:07:19.509191 grrph-0.0.4/grrph/datasets/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     5330 2024-02-13 08:40:12.000000 grrph-0.0.4/grrph/datasets/RIGIDDataset.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     8219 2024-04-29 10:58:44.000000 grrph-0.0.4/grrph/distance.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     8177 2024-04-10 10:10:59.000000 grrph-0.0.4/grrph/fast_wl.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)    11961 2024-04-17 13:37:54.000000 grrph-0.0.4/grrph/inductive_wl.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      580 2024-04-17 13:01:51.000000 grrph-0.0.4/grrph/kernel.py
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-04-29 11:07:19.509191 grrph-0.0.4/grrph/sklearn/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      647 2024-02-13 08:43:47.000000 grrph-0.0.4/grrph/sklearn/ensembling.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     1498 2024-02-13 08:43:47.000000 grrph-0.0.4/grrph/sklearn/preprocessing.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      928 2024-04-10 12:10:27.000000 grrph-0.0.4/grrph/util.py
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2024-04-29 11:07:19.509191 grrph-0.0.4/grrph.egg-info/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1061 2024-04-29 11:07:19.000000 grrph-0.0.4/grrph.egg-info/PKG-INFO
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      425 2024-04-29 11:07:19.000000 grrph-0.0.4/grrph.egg-info/SOURCES.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)        1 2024-04-29 11:07:19.000000 grrph-0.0.4/grrph.egg-info/dependency_links.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       25 2024-04-29 11:07:19.000000 grrph-0.0.4/grrph.egg-info/requires.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)        6 2024-04-29 11:07:19.000000 grrph-0.0.4/grrph.egg-info/top_level.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      609 2024-04-29 11:00:00.000000 grrph-0.0.4/pyproject.toml
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       38 2024-04-29 11:07:19.509191 grrph-0.0.4/setup.cfg
```

### Comparing `grrph-0.0.3/LICENSE` & `grrph-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grrph-0.0.3/PKG-INFO` & `grrph-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: grrph
-Version: 0.0.3
+Version: 0.0.4
 Summary: grrph -- Pascals Python Graph Library 
 Author-email: Pascal Welke <pascal.welke@tuwien.ac.at>
 Project-URL: Homepage, https://github.com/pwelke/grrph
 Project-URL: Issues, https://github.com/pwelke/grrph/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: networkx
+Requires-Dist: POT
 
 # grrph -- Pascals Python Graph Library 
 
 Currently does nothing but is supposed to collect various useful helpers for loading, transforming, mining, and learning (on) graphs.
 
 
 ## Installation Advice
```

### Comparing `grrph-0.0.3/grrph/converter.py` & `grrph-0.0.4/grrph/converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import networkx as nx
+import numpy as np
 
 import torch
 
 import torch_geometric
 from torch_geometric.data import Data
 from torch_geometric.utils.convert import from_networkx
 
+import scipy.sparse
 
 def graph6_to_pyg(x):
     '''convert graph6 format to pytorch_geometric object
     source: https://github.com/GraphPKU/BREC/blob/Release/base/BRECDataset_v3.py
     '''
     return from_networkx(nx.from_graph6_bytes(x))
 
@@ -47,8 +49,23 @@
 
         data = dict()
         data['edge_index'] = torch.tensor(g['edges'], dtype=torch.int64).T
 
         G = Data.from_dict(data)
         G.num_nodes = g['n']
         
-        return G
+        return G
+
+
+def edge_index_to_csr_matrix(edge_index, n, edge_weights=None):
+    '''
+    returns scipy.sparse.csr_matrix for given edge_index list as used by pytorch geometric.
+    arguments: 
+        edge_index: (m, 2) shape array 
+        edge_weights: (m,) shape array of weights of the adjacency matrix. (optional. default weight 1)
+    '''
+    if edge_weights is None:
+        edge_weights = np.ones(edge_index.shape[0])
+    if edge_weights.shape[0] == 0:
+        return scipy.sparse.csr_matrix((n, n))
+    else:
+        return scipy.sparse.csr_matrix((edge_weights, (edge_index[:,0], edge_index[:,1])), shape=(n,n))
```

### Comparing `grrph-0.0.3/grrph/datasets/RIGIDDataset.py` & `grrph-0.0.4/grrph/datasets/RIGIDDataset.py`

 * *Files identical despite different names*

### Comparing `grrph-0.0.3/grrph/sklearn/ensembling.py` & `grrph-0.0.4/grrph/sklearn/ensembling.py`

 * *Files identical despite different names*

### Comparing `grrph-0.0.3/grrph/sklearn/preprocessing.py` & `grrph-0.0.4/grrph/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `grrph-0.0.3/grrph.egg-info/PKG-INFO` & `grrph-0.0.4/grrph.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: grrph
-Version: 0.0.3
+Version: 0.0.4
 Summary: grrph -- Pascals Python Graph Library 
 Author-email: Pascal Welke <pascal.welke@tuwien.ac.at>
 Project-URL: Homepage, https://github.com/pwelke/grrph
 Project-URL: Issues, https://github.com/pwelke/grrph/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: networkx
+Requires-Dist: POT
 
 # grrph -- Pascals Python Graph Library 
 
 Currently does nothing but is supposed to collect various useful helpers for loading, transforming, mining, and learning (on) graphs.
 
 
 ## Installation Advice
```

