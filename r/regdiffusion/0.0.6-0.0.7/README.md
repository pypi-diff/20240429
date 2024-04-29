# Comparing `tmp/regdiffusion-0.0.6.tar.gz` & `tmp/regdiffusion-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regdiffusion-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "regdiffusion-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `regdiffusion-0.0.6.tar` & `regdiffusion-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11341 2023-11-05 15:52:36.085365 regdiffusion-0.0.6/LICENSE
--rw-r--r--   0        0        0     3809 2024-03-29 20:40:52.313815 regdiffusion-0.0.6/README.md
--rw-r--r--   0        0        0      786 2024-04-20 04:02:47.110287 regdiffusion-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py
--rw-r--r--   0        0        0    18237 2024-04-05 04:43:37.672632 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py
--rw-r--r--   0        0        0     5120 2024-01-25 21:19:10.168299 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py
--rw-r--r--   0        0        0    11432 2024-03-14 17:20:42.308017 regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py
--rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.6/regdiffusion/__init__.py
--rw-r--r--   0        0        0      149 2024-03-02 14:07:24.969670 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     4272 2024-02-01 03:02:39.297276 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py
--rw-r--r--   0        0        0     2654 2024-03-07 17:17:15.538130 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py
--rw-r--r--   0        0        0      567 2024-01-25 21:19:10.293030 regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0        0        0      366 2024-03-29 20:40:52.511868 regdiffusion-0.0.6/regdiffusion/data/__init__.py
--rw-r--r--   0        0        0     3697 2024-03-29 20:40:52.521726 regdiffusion-0.0.6/regdiffusion/data/beeline.py
--rw-r--r--   0        0        0     4278 2024-03-29 20:40:52.535236 regdiffusion-0.0.6/regdiffusion/data/microglia.py
--rw-r--r--   0        0        0      567 2024-01-25 21:19:10.333274 regdiffusion-0.0.6/regdiffusion/data/utils.py
--rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.6/regdiffusion/evaluator.py
--rw-r--r--   0        0        0    18097 2024-04-16 15:03:49.420584 regdiffusion-0.0.6/regdiffusion/grn.py
--rw-r--r--   0        0        0     5906 2024-03-27 03:46:34.074272 regdiffusion-0.0.6/regdiffusion/logger.py
--rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.6/regdiffusion/models/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     6363 2024-03-22 04:52:28.581539 regdiffusion-0.0.6/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py
--rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.6/regdiffusion/models/__init__.py
--rw-r--r--   0        0        0     6331 2024-03-29 20:40:52.560257 regdiffusion-0.0.6/regdiffusion/models/regdiffusion.py
--rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.6/regdiffusion/plot/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.6/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py
--rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.6/regdiffusion/plot/__init__.py
--rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.6/regdiffusion/plot/pyvis.py
--rw-r--r--   0        0        0    17126 2024-04-16 15:03:49.445516 regdiffusion-0.0.6/regdiffusion/trainer.py
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 regdiffusion-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-11-05 15:52:36.085365 regdiffusion-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3910 2024-04-29 14:28:13.415126 regdiffusion-0.0.7/README.md
+-rw-r--r--   0        0        0      786 2024-04-29 14:10:50.881907 regdiffusion-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py
+-rw-r--r--   0        0        0    18237 2024-04-05 04:43:37.672632 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py
+-rw-r--r--   0        0        0     5120 2024-01-25 21:19:10.168299 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py
+-rw-r--r--   0        0        0    11432 2024-03-14 17:20:42.308017 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py
+-rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.7/regdiffusion/__init__.py
+-rw-r--r--   0        0        0      149 2024-03-02 14:07:24.969670 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     4272 2024-02-01 03:02:39.297276 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py
+-rw-r--r--   0        0        0     2654 2024-03-07 17:17:15.538130 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py
+-rw-r--r--   0        0        0      567 2024-01-25 21:19:10.293030 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py
+-rw-r--r--   0        0        0      366 2024-03-29 20:40:52.511868 regdiffusion-0.0.7/regdiffusion/data/__init__.py
+-rw-r--r--   0        0        0     3697 2024-03-29 20:40:52.521726 regdiffusion-0.0.7/regdiffusion/data/beeline.py
+-rw-r--r--   0        0        0     4278 2024-03-29 20:40:52.535236 regdiffusion-0.0.7/regdiffusion/data/microglia.py
+-rw-r--r--   0        0        0      567 2024-01-25 21:19:10.333274 regdiffusion-0.0.7/regdiffusion/data/utils.py
+-rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.7/regdiffusion/evaluator.py
+-rw-r--r--   0        0        0    18097 2024-04-16 15:03:49.420584 regdiffusion-0.0.7/regdiffusion/grn.py
+-rw-r--r--   0        0        0     5906 2024-03-27 03:46:34.074272 regdiffusion-0.0.7/regdiffusion/logger.py
+-rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.7/regdiffusion/models/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     6363 2024-03-22 04:52:28.581539 regdiffusion-0.0.7/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py
+-rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.7/regdiffusion/models/__init__.py
+-rw-r--r--   0        0        0     6331 2024-03-29 20:40:52.560257 regdiffusion-0.0.7/regdiffusion/models/regdiffusion.py
+-rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.7/regdiffusion/plot/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.7/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py
+-rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.7/regdiffusion/plot/__init__.py
+-rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.7/regdiffusion/plot/pyvis.py
+-rw-r--r--   0        0        0    17126 2024-04-16 15:03:49.445516 regdiffusion-0.0.7/regdiffusion/trainer.py
+-rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 regdiffusion-0.0.7/PKG-INFO
```

### Comparing `regdiffusion-0.0.6/LICENSE` & `regdiffusion-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/README.md` & `regdiffusion-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 ```
 From Noise to Knowledge: Probabilistic Diffusion-Based Neural Inference of Gene Regulatory Networks
 Hao Zhu, Donna K. Slonim
 bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/2023.11.05.565675
 ```
 
+![](https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/regdiffusion_structure.png)
 
 ## Installation
 
 RegDiffusion is on pypi.
 
 ```
 pip install regdiffusion
@@ -36,15 +37,15 @@
 - `GRN`: The `GRN` class provides a container to save the inferred adjacency
   matrix and the corresponding gene names. You can save the `GRN` object to 
   a local `HDF5` file using the `.to_hdf5()` method and reload the saved file 
   using the `read_hdf5()` function. It also comes with functionalities to 
   export or visualize local regions. For example, you can use the 
   `.visualize_local_neighborhood()` to generate a similar plot as used in 
   the RegDiffusion paper. You can also extract the underlying adjacency list 
-  using the `.extract_node_2hop_neighborhood()` method.
+  using the `.extract_local_neighborhood()` method.
 - `GRNEvaluator`: The ground truth of regulatory relationship often exist as 
   list of edges but the values to be evaluated are often in adjacency matrix. 
   The `GRNEvaluator` class is designed to fill the gap. Right now it supports
   common metrics such as AUROC, AUPR, AUPR Ratio, EP, and EPR. 
 - `data` module: Right now, the `data` module includes quick access to BEELINE 
   benchmarks and our preprocessed single cell datasets on mouse microglia. 
 
@@ -53,15 +54,15 @@
 `adjacency` matrix. When you have thousands or tens of thousands of genes, 
 it's getting difficult to analyze matrix at that scale. In our paper, we 
 propose a way to analyze the local network by focusing on the genes you care 
 the most. Check out the tutorials on the left side for how to perform a similar 
 network analysis like the one we did in the paper. We are also working on an 
 interactive tool to analyze saved GRN object. 
 
-![](https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/apoe_reg.png)
+![](https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/apoe_net.png)
 
 ## Inference Speed
 Inference on networks with 15,000 genes takes under 5 minutes on an A100 GPU. 
 In contrast, previous VAE based models would take more than 4 hours on the same 
 device. Even if you don't have access to those fancy GPU cards, RegDiffusion 
 still works. Inference on the same large network takes roughly 3 hours on a 
 mid-range 12-core CPU.
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
 # RegDiffusion _[_l_o_g_o_]RegDiffusion is a very fast regulatory network inference
 algorithm based on probabilistic diffusion model. It works well on genes and is
 capable to rapidly (<5min) predict biologically verifiable links from large
 single cell RNA-seq data with 14,000+ genes. ``` From Noise to Knowledge:
 Probabilistic Diffusion-Based Neural Inference of Gene Regulatory Networks Hao
 Zhu, Donna K. Slonim bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/
-2023.11.05.565675 ``` ## Installation RegDiffusion is on pypi. ``` pip install
-regdiffusion ``` Check out the [this tutorial](https://tuftsbcb.github.io/
-RegDiffusion/quick_tour.html) for a quick tour of how to use RegDiffusion for
-your research! ## Quick Tour This package `regdiffusion` provides the official
-implementation of the RegDiffusion algorithm and a set of easy-to-use companion
-tools to evaluate, analyze, and visualize the inferred network. We also provide
-access tools to GRN benchmarks and preprocessed single cell datasets for
-evaluation. We tried to keep the top level interface straightforward. Right
-now, it only consists of 4 components: the `RegDiffusionTrainer` class, the
-`GRN` class, the `GRNEvaluator` class, and the `data` module. -
-`RegDiffusionTrainer`: You can use it to train a `RegDiffusion` model by
-providing log transformed expression data in a `numpy` array. The training
-process could be either started or continued using the `.train()` method. You
-can export the inferred `GRN` using the `.get_grn()` method. - `GRN`: The `GRN`
-class provides a container to save the inferred adjacency matrix and the
-corresponding gene names. You can save the `GRN` object to a local `HDF5` file
-using the `.to_hdf5()` method and reload the saved file using the `read_hdf5()`
-function. It also comes with functionalities to export or visualize local
-regions. For example, you can use the `.visualize_local_neighborhood()` to
-generate a similar plot as used in the RegDiffusion paper. You can also extract
-the underlying adjacency list using the `.extract_node_2hop_neighborhood()`
-method. - `GRNEvaluator`: The ground truth of regulatory relationship often
-exist as list of edges but the values to be evaluated are often in adjacency
-matrix. The `GRNEvaluator` class is designed to fill the gap. Right now it
-supports common metrics such as AUROC, AUPR, AUPR Ratio, EP, and EPR. - `data`
-module: Right now, the `data` module includes quick access to BEELINE
-benchmarks and our preprocessed single cell datasets on mouse microglia. ##
-Understanding the Inferred Networks After the `RegDiffusion` model converges,
-what you get is simply an `adjacency` matrix. When you have thousands or tens
-of thousands of genes, it's getting difficult to analyze matrix at that scale.
-In our paper, we propose a way to analyze the local network by focusing on the
-genes you care the most. Check out the tutorials on the left side for how to
-perform a similar network analysis like the one we did in the paper. We are
-also working on an interactive tool to analyze saved GRN object. ![](https://
-raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/apoe_reg.png)
-## Inference Speed Inference on networks with 15,000 genes takes under 5
-minutes on an A100 GPU. In contrast, previous VAE based models would take more
-than 4 hours on the same device. Even if you don't have access to those fancy
-GPU cards, RegDiffusion still works. Inference on the same large network takes
-roughly 3 hours on a mid-range 12-core CPU.
+2023.11.05.565675 ``` ![](https://raw.githubusercontent.com/TuftsBCB/
+RegDiffusion/master/resources/regdiffusion_structure.png) ## Installation
+RegDiffusion is on pypi. ``` pip install regdiffusion ``` Check out the [this
+tutorial](https://tuftsbcb.github.io/RegDiffusion/quick_tour.html) for a quick
+tour of how to use RegDiffusion for your research! ## Quick Tour This package
+`regdiffusion` provides the official implementation of the RegDiffusion
+algorithm and a set of easy-to-use companion tools to evaluate, analyze, and
+visualize the inferred network. We also provide access tools to GRN benchmarks
+and preprocessed single cell datasets for evaluation. We tried to keep the top
+level interface straightforward. Right now, it only consists of 4 components:
+the `RegDiffusionTrainer` class, the `GRN` class, the `GRNEvaluator` class, and
+the `data` module. - `RegDiffusionTrainer`: You can use it to train a
+`RegDiffusion` model by providing log transformed expression data in a `numpy`
+array. The training process could be either started or continued using the
+`.train()` method. You can export the inferred `GRN` using the `.get_grn()`
+method. - `GRN`: The `GRN` class provides a container to save the inferred
+adjacency matrix and the corresponding gene names. You can save the `GRN`
+object to a local `HDF5` file using the `.to_hdf5()` method and reload the
+saved file using the `read_hdf5()` function. It also comes with functionalities
+to export or visualize local regions. For example, you can use the
+`.visualize_local_neighborhood()` to generate a similar plot as used in the
+RegDiffusion paper. You can also extract the underlying adjacency list using
+the `.extract_local_neighborhood()` method. - `GRNEvaluator`: The ground truth
+of regulatory relationship often exist as list of edges but the values to be
+evaluated are often in adjacency matrix. The `GRNEvaluator` class is designed
+to fill the gap. Right now it supports common metrics such as AUROC, AUPR, AUPR
+Ratio, EP, and EPR. - `data` module: Right now, the `data` module includes
+quick access to BEELINE benchmarks and our preprocessed single cell datasets on
+mouse microglia. ## Understanding the Inferred Networks After the
+`RegDiffusion` model converges, what you get is simply an `adjacency` matrix.
+When you have thousands or tens of thousands of genes, it's getting difficult
+to analyze matrix at that scale. In our paper, we propose a way to analyze the
+local network by focusing on the genes you care the most. Check out the
+tutorials on the left side for how to perform a similar network analysis like
+the one we did in the paper. We are also working on an interactive tool to
+analyze saved GRN object. ![](https://raw.githubusercontent.com/TuftsBCB/
+RegDiffusion/master/resources/apoe_net.png) ## Inference Speed Inference on
+networks with 15,000 genes takes under 5 minutes on an A100 GPU. In contrast,
+previous VAE based models would take more than 4 hours on the same device. Even
+if you don't have access to those fancy GPU cards, RegDiffusion still works.
+Inference on the same large network takes roughly 3 hours on a mid-range 12-
+core CPU.
```

### Comparing `regdiffusion-0.0.6/pyproject.toml` & `regdiffusion-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     { name = "Donna Slonim", email="donna.slonim@tufts.edu"}
 ]
 maintainers = [
     { name = "Hao Zhu", email = "haozhu233@gmail.com" }
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.0.6"
+version = "0.0.7"
 description = "Gene Regulatory Networks Inference using diffusion model"
 
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 
 dependencies = [
     "numpy>=1.16.5",
     "pandas>=1.1.1",
```

### Comparing `regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/data/beeline.py` & `regdiffusion-0.0.7/regdiffusion/data/beeline.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/data/microglia.py` & `regdiffusion-0.0.7/regdiffusion/data/microglia.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/data/utils.py` & `regdiffusion-0.0.7/regdiffusion/data/utils.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/evaluator.py` & `regdiffusion-0.0.7/regdiffusion/evaluator.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/grn.py` & `regdiffusion-0.0.7/regdiffusion/grn.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/logger.py` & `regdiffusion-0.0.7/regdiffusion/logger.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/models/regdiffusion.py` & `regdiffusion-0.0.7/regdiffusion/models/regdiffusion.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py` & `regdiffusion-0.0.7/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/plot/pyvis.py` & `regdiffusion-0.0.7/regdiffusion/plot/pyvis.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/regdiffusion/trainer.py` & `regdiffusion-0.0.7/regdiffusion/trainer.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.6/PKG-INFO` & `regdiffusion-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regdiffusion
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gene Regulatory Networks Inference using diffusion model
 Author-email: Hao Zhu <haozhu233@gmail.com>, Donna Slonim <donna.slonim@tufts.edu>
 Maintainer-email: Hao Zhu <haozhu233@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: numpy>=1.16.5
 Requires-Dist: pandas>=1.1.1
@@ -22,14 +22,15 @@
 
 ```
 From Noise to Knowledge: Probabilistic Diffusion-Based Neural Inference of Gene Regulatory Networks
 Hao Zhu, Donna K. Slonim
 bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/2023.11.05.565675
 ```
 
+![](https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/regdiffusion_structure.png)
 
 ## Installation
 
 RegDiffusion is on pypi.
 
 ```
 pip install regdiffusion
@@ -54,15 +55,15 @@
 - `GRN`: The `GRN` class provides a container to save the inferred adjacency
   matrix and the corresponding gene names. You can save the `GRN` object to 
   a local `HDF5` file using the `.to_hdf5()` method and reload the saved file 
   using the `read_hdf5()` function. It also comes with functionalities to 
   export or visualize local regions. For example, you can use the 
   `.visualize_local_neighborhood()` to generate a similar plot as used in 
   the RegDiffusion paper. You can also extract the underlying adjacency list 
-  using the `.extract_node_2hop_neighborhood()` method.
+  using the `.extract_local_neighborhood()` method.
 - `GRNEvaluator`: The ground truth of regulatory relationship often exist as 
   list of edges but the values to be evaluated are often in adjacency matrix. 
   The `GRNEvaluator` class is designed to fill the gap. Right now it supports
   common metrics such as AUROC, AUPR, AUPR Ratio, EP, and EPR. 
 - `data` module: Right now, the `data` module includes quick access to BEELINE 
   benchmarks and our preprocessed single cell datasets on mouse microglia. 
 
@@ -71,15 +72,15 @@
 `adjacency` matrix. When you have thousands or tens of thousands of genes, 
 it's getting difficult to analyze matrix at that scale. In our paper, we 
 propose a way to analyze the local network by focusing on the genes you care 
 the most. Check out the tutorials on the left side for how to perform a similar 
 network analysis like the one we did in the paper. We are also working on an 
 interactive tool to analyze saved GRN object. 
 
-![](https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/apoe_reg.png)
+![](https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/apoe_net.png)
 
 ## Inference Speed
 Inference on networks with 15,000 genes takes under 5 minutes on an A100 GPU. 
 In contrast, previous VAE based models would take more than 4 hours on the same 
 device. Even if you don't have access to those fancy GPU cards, RegDiffusion 
 still works. Inference on the same large network takes roughly 3 hours on a 
 mid-range 12-core CPU.
```

#### html2text {}

```diff
@@ -1,55 +1,57 @@
-Metadata-Version: 2.1 Name: regdiffusion Version: 0.0.6 Summary: Gene
+Metadata-Version: 2.1 Name: regdiffusion Version: 0.0.7 Summary: Gene
 Regulatory Networks Inference using diffusion model Author-email: Hao Zhu
 gmail.com>, Donna Slonim
 tufts.edu> Maintainer-email: Hao Zhu
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: Apache Software License Requires-Dist: numpy>=1.16.5 Requires-Dist:
 pandas>=1.1.1 Requires-Dist: torch Requires-Dist: tqdm Requires-Dist: scanpy
 Requires-Dist: scikit-learn Requires-Dist: h5py Requires-Dist: pyvis Project-
 URL: Home, https://github.com/TuftsBCB/RegDiffusion # RegDiffusion
 _[_l_o_g_o_]RegDiffusion is a very fast regulatory network inference algorithm based
 on probabilistic diffusion model. It works well on genes and is capable to
 rapidly (<5min) predict biologically verifiable links from large single cell
 RNA-seq data with 14,000+ genes. ``` From Noise to Knowledge: Probabilistic
 Diffusion-Based Neural Inference of Gene Regulatory Networks Hao Zhu, Donna K.
 Slonim bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/
-2023.11.05.565675 ``` ## Installation RegDiffusion is on pypi. ``` pip install
-regdiffusion ``` Check out the [this tutorial](https://tuftsbcb.github.io/
-RegDiffusion/quick_tour.html) for a quick tour of how to use RegDiffusion for
-your research! ## Quick Tour This package `regdiffusion` provides the official
-implementation of the RegDiffusion algorithm and a set of easy-to-use companion
-tools to evaluate, analyze, and visualize the inferred network. We also provide
-access tools to GRN benchmarks and preprocessed single cell datasets for
-evaluation. We tried to keep the top level interface straightforward. Right
-now, it only consists of 4 components: the `RegDiffusionTrainer` class, the
-`GRN` class, the `GRNEvaluator` class, and the `data` module. -
-`RegDiffusionTrainer`: You can use it to train a `RegDiffusion` model by
-providing log transformed expression data in a `numpy` array. The training
-process could be either started or continued using the `.train()` method. You
-can export the inferred `GRN` using the `.get_grn()` method. - `GRN`: The `GRN`
-class provides a container to save the inferred adjacency matrix and the
-corresponding gene names. You can save the `GRN` object to a local `HDF5` file
-using the `.to_hdf5()` method and reload the saved file using the `read_hdf5()`
-function. It also comes with functionalities to export or visualize local
-regions. For example, you can use the `.visualize_local_neighborhood()` to
-generate a similar plot as used in the RegDiffusion paper. You can also extract
-the underlying adjacency list using the `.extract_node_2hop_neighborhood()`
-method. - `GRNEvaluator`: The ground truth of regulatory relationship often
-exist as list of edges but the values to be evaluated are often in adjacency
-matrix. The `GRNEvaluator` class is designed to fill the gap. Right now it
-supports common metrics such as AUROC, AUPR, AUPR Ratio, EP, and EPR. - `data`
-module: Right now, the `data` module includes quick access to BEELINE
-benchmarks and our preprocessed single cell datasets on mouse microglia. ##
-Understanding the Inferred Networks After the `RegDiffusion` model converges,
-what you get is simply an `adjacency` matrix. When you have thousands or tens
-of thousands of genes, it's getting difficult to analyze matrix at that scale.
-In our paper, we propose a way to analyze the local network by focusing on the
-genes you care the most. Check out the tutorials on the left side for how to
-perform a similar network analysis like the one we did in the paper. We are
-also working on an interactive tool to analyze saved GRN object. ![](https://
-raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/apoe_reg.png)
-## Inference Speed Inference on networks with 15,000 genes takes under 5
-minutes on an A100 GPU. In contrast, previous VAE based models would take more
-than 4 hours on the same device. Even if you don't have access to those fancy
-GPU cards, RegDiffusion still works. Inference on the same large network takes
-roughly 3 hours on a mid-range 12-core CPU.
+2023.11.05.565675 ``` ![](https://raw.githubusercontent.com/TuftsBCB/
+RegDiffusion/master/resources/regdiffusion_structure.png) ## Installation
+RegDiffusion is on pypi. ``` pip install regdiffusion ``` Check out the [this
+tutorial](https://tuftsbcb.github.io/RegDiffusion/quick_tour.html) for a quick
+tour of how to use RegDiffusion for your research! ## Quick Tour This package
+`regdiffusion` provides the official implementation of the RegDiffusion
+algorithm and a set of easy-to-use companion tools to evaluate, analyze, and
+visualize the inferred network. We also provide access tools to GRN benchmarks
+and preprocessed single cell datasets for evaluation. We tried to keep the top
+level interface straightforward. Right now, it only consists of 4 components:
+the `RegDiffusionTrainer` class, the `GRN` class, the `GRNEvaluator` class, and
+the `data` module. - `RegDiffusionTrainer`: You can use it to train a
+`RegDiffusion` model by providing log transformed expression data in a `numpy`
+array. The training process could be either started or continued using the
+`.train()` method. You can export the inferred `GRN` using the `.get_grn()`
+method. - `GRN`: The `GRN` class provides a container to save the inferred
+adjacency matrix and the corresponding gene names. You can save the `GRN`
+object to a local `HDF5` file using the `.to_hdf5()` method and reload the
+saved file using the `read_hdf5()` function. It also comes with functionalities
+to export or visualize local regions. For example, you can use the
+`.visualize_local_neighborhood()` to generate a similar plot as used in the
+RegDiffusion paper. You can also extract the underlying adjacency list using
+the `.extract_local_neighborhood()` method. - `GRNEvaluator`: The ground truth
+of regulatory relationship often exist as list of edges but the values to be
+evaluated are often in adjacency matrix. The `GRNEvaluator` class is designed
+to fill the gap. Right now it supports common metrics such as AUROC, AUPR, AUPR
+Ratio, EP, and EPR. - `data` module: Right now, the `data` module includes
+quick access to BEELINE benchmarks and our preprocessed single cell datasets on
+mouse microglia. ## Understanding the Inferred Networks After the
+`RegDiffusion` model converges, what you get is simply an `adjacency` matrix.
+When you have thousands or tens of thousands of genes, it's getting difficult
+to analyze matrix at that scale. In our paper, we propose a way to analyze the
+local network by focusing on the genes you care the most. Check out the
+tutorials on the left side for how to perform a similar network analysis like
+the one we did in the paper. We are also working on an interactive tool to
+analyze saved GRN object. ![](https://raw.githubusercontent.com/TuftsBCB/
+RegDiffusion/master/resources/apoe_net.png) ## Inference Speed Inference on
+networks with 15,000 genes takes under 5 minutes on an A100 GPU. In contrast,
+previous VAE based models would take more than 4 hours on the same device. Even
+if you don't have access to those fancy GPU cards, RegDiffusion still works.
+Inference on the same large network takes roughly 3 hours on a mid-range 12-
+core CPU.
```

