# Comparing `tmp/sae_lens-1.0.0.tar.gz` & `tmp/sae_lens-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.0.0.tar", max compression
+gzip compressed data, was "sae_lens-1.1.0.tar", max compression
```

## Comparing `sae_lens-1.0.0.tar` & `sae_lens-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2024-04-27 17:22:41.477072 sae_lens-1.0.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-04-27 17:22:41.477072 sae_lens-1.0.0/README.md
--rw-r--r--   0        0        0     1773 2024-04-27 17:22:42.477070 sae_lens-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-27 17:22:42.477070 sae_lens-1.0.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0     2443 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    18451 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     6645 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    16793 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2849 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     9927 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1528 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8052 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    15324 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    19179 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-27 17:22:41.489072 sae_lens-1.0.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 sae_lens-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-29 11:57:39.783671 sae_lens-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-04-29 11:57:39.783671 sae_lens-1.1.0/README.md
+-rw-r--r--   0        0        0     1811 2024-04-29 11:57:40.751684 sae_lens-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-29 11:57:40.751684 sae_lens-1.1.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    15926 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    18451 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     6645 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    16793 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2849 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     9927 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8052 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    15324 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    19179 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-29 11:57:39.795671 sae_lens-1.1.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 sae_lens-1.1.0/PKG-INFO
```

### Comparing `sae_lens-1.0.0/LICENSE` & `sae_lens-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/README.md` & `sae_lens-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/pyproject.toml` & `sae_lens-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.0.0"
+version = "1.1.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -27,14 +27,15 @@
 mkdocs-section-index = "^0.3.8"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
 safetensors = "^0.4.2"
 typer = "^0.12.3"
 mamba-lens = { version = "^0.0.4", optional = true }
 pyzmq = "26.0.0"
+automated-interpretability = "^0.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "24.4.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
```

### Comparing `sae_lens-1.0.0/sae_lens/__init__.py` & `sae_lens-1.1.0/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.0.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.1.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.1.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.1.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/analysis/tsea.py` & `sae_lens-1.1.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.1.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/activations_store.py` & `sae_lens-1.1.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-1.1.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/config.py` & `sae_lens-1.1.0/sae_lens/training/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/evals.py` & `sae_lens-1.1.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/geometric_median.py` & `sae_lens-1.1.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/lm_runner.py` & `sae_lens-1.1.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/load_model.py` & `sae_lens-1.1.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/optim.py` & `sae_lens-1.1.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/sae_group.py` & `sae_lens-1.1.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/session_loader.py` & `sae_lens-1.1.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.1.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.1.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/toy_models.py` & `sae_lens-1.1.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.1.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.1.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/sae_lens/training/utils.py` & `sae_lens-1.1.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.0.0/PKG-INFO` & `sae_lens-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.0.0
+Version: 1.1.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mamba
+Requires-Dist: automated-interpretability (>=0.0.2,<0.0.3)
 Requires-Dist: babe (>=0.0.7,<0.0.8)
 Requires-Dist: datasets (>=2.17.1,<3.0.0)
 Requires-Dist: ipykernel (>=6.29.2,<7.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: mamba-lens (>=0.0.4,<0.0.5) ; extra == "mamba"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: matplotlib-inline (>=0.1.6,<0.2.0)
```

