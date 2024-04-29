# Comparing `tmp/ngautonml_forecasting-0.4.1b1.tar.gz` & `tmp/ngautonml_forecasting-0.4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngautonml_forecasting-0.4.1b1.tar", last modified: Thu Jan  4 16:50:01 2024, max compression
+gzip compressed data, was "ngautonml_forecasting-0.4.1b2.tar", last modified: Mon Apr 29 18:58:25 2024, max compression
```

## Comparing `ngautonml_forecasting-0.4.1b1.tar` & `ngautonml_forecasting-0.4.1b2.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.557189 ngautonml_forecasting-0.4.1b1/
--rw-r--r--   0 root         (0) root         (0)     4285 2024-01-04 16:50:01.557189 ngautonml_forecasting-0.4.1b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3712 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.551189 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.553189 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.555189 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/
--rw-rw-rw-   0 root         (0) root         (0)     3523 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATS.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATS_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6265 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATSx.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATSx_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6398 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NHITS.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NHITS_test.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4363 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_auto_model.py
--rw-rw-rw-   0 root         (0) root         (0)     6921 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3062 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/examples_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.556189 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/splitters/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/splitters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3839 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/splitters/forecasting_splitter.py
--rw-rw-rw-   0 root         (0) root         (0)     3346 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/splitters/forecasting_splitter_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.557189 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/templates/forecasting.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/templates/forecasting_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 16:50:01.557189 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4285 2024-01-04 16:50:01.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1460 2024-01-04 16:50:01.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-04 16:50:01.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      198 2024-01-04 16:50:01.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-04 16:50:01.000000 ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-01-04 16:46:44.000000 ngautonml_forecasting-0.4.1b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-04 16:50:01.558189 ngautonml_forecasting-0.4.1b1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.144156 ngautonml_forecasting-0.4.1b2/
+-rw-r--r--   0 root         (0) root         (0)     4285 2024-04-29 18:58:25.144156 ngautonml_forecasting-0.4.1b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3712 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.137156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/
+-rw-rw-rw-   0 root         (0) root         (0)      888 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.138156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.141156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6159 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATS.py
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATS_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATSx.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATSx_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6742 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NHITS.py
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NHITS_test.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_auto_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7242 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.142156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/config_components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/config_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4803 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/config_components/forecasting_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9806 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/config_components/forecasting_config_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/examples_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.143156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/splitters/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/splitters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/splitters/forecasting_splitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3074 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/splitters/forecasting_splitter_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.143156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/templates/forecasting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/templates/forecasting_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:58:25.144156 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4285 2024-04-29 18:58:25.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-29 18:58:25.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 18:58:25.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-29 18:58:25.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-29 18:58:25.000000 ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-04-29 18:54:58.000000 ngautonml_forecasting-0.4.1b2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-29 18:58:25.144156 ngautonml_forecasting-0.4.1b2/setup.cfg
```

### Comparing `ngautonml_forecasting-0.4.1b1/PKG-INFO` & `ngautonml_forecasting-0.4.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngautonml_forecasting
-Version: 0.4.1b1
+Version: 0.4.1b2
 Summary: a plugin that installs forecasting tools for ngAutonML
 Author-email: "L.H. Piggy Yarroll" <piggy@cmu.edu>, Merritt Kowaleski <merrittk@cmu.edu>, Andrew Williams <awillia2@andrew.cmu.edu>, Jieshi Chen <jieshic@andrew.cmu.edu>
 Keywords: machine learning,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
```

### Comparing `ngautonml_forecasting-0.4.1b1/README.md` & `ngautonml_forecasting-0.4.1b2/README.md`

 * *Files identical despite different names*

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/__init__.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,7 +15,12 @@
     '''Make the plugin algorithms catalog.'''
     return PathedCatalog([Path(__file__).parent / 'algorithms'], **kwargs)
 
 
 def splitters_make_catalog(**kwargs) -> Catalog:
     '''Make the plugin splitters catalog.'''
     return PathedCatalog([Path(__file__).parent / 'splitters'], **kwargs)
+
+
+def config_components_make_catalog(**kwargs) -> Catalog:
+    '''Make the plugin config components catalog.'''
+    return PathedCatalog([Path(__file__).parent / 'config_components'], **kwargs)
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,30 +32,32 @@
     The Neural Hierarchical Interpolation for Time Series (NHITS), is
     an MLP-based deep neural architecture with backward and forward
     residual links. NHITS tackles volatility and memory complexity
     challenges, by locally specializing its sequential predictions
     into the signals frequencies with hierarchical interpolation and
     pooling.
 
-    Required Parameters:
-    `h`: int, Forecast horizon. <br>
+    .. rubric:: Required Parameters:
 
-    Hyperparams:
+    * ``h``: ``int``, Forecast horizon.
 
-    loss: PyTorch module, instantiated train loss class from losses collection.
-    valid_loss: PyTorch module=loss, instantiated valid loss class from losses collection.
-    config: dict, dictionary with ray.tune defined search space.
-    search_alg: ray.tune.search variant, BasicVariantGenerator, HyperOptSearch,
-      DragonflySearch, TuneBOHB for details see tune.search.
-    num_samples: int, number of hyperparameter optimization steps/samples.
-    cpus: int, number of cpus to use during optimization, default all available.
-    gpus: int, number of gpus to use during optimization, default all available.
-    refit_wo_val: bool, number of gpus to use during optimization, default all available.
-    verbose: bool, wether print partial outputs.
-    alias: str, optional, Custom name of the model.
+    .. rubric:: Hyperparams:
+
+    * ``loss``: PyTorch module, instantiated train loss class from ``losses`` collection.
+    * ``valid_loss``: PyTorch module = ``loss``, instantiated valid loss class from ``losses``
+      collection.
+    * ``config``: ``dict``, dictionary with ray.tune defined search space.
+    * ``search_alg``: ``ray.tune.search`` variant, ``BasicVariantGenerator``, ``HyperOptSearch``,
+      ``DragonflySearch``, ``TuneBOHB``. for details see ``tune.search``.
+    * ``num_samples``: ``int`` number of hyperparameter optimization steps/samples.
+    * ``cpus``: ``int``, number of cpus to use during optimization, default all available.
+    * ``gpus``: ``int``, number of gpus to use during optimization, default all available.
+    * ``refit_with_val``: ``bool=False``, whether refit of best model should preserve val size.
+    * ``verbose``: ``bool``, whether to print partial outputs.
+    * ``alias``: ``str``, optional, Custom name of the model.
     '''
     _name = 'neuralforecast.auto.AutoNHITS'
     _basename = 'AutoNHITS'
     _tags = {
         'task': [TaskType.FORECASTING.name],
         'data_type': [DataType.TIMESERIES.name],
         'supports_random_seed': ['true'],
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/AutoNHITS_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NHITS_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-'''Tests for AutoNHITS.py'''
+'''Tests for NHITS.py'''
 # pylint: disable=invalid-name, missing-function-docstring, duplicate-code
 import warnings
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from neuralforecast.utils import AirPassengersDF  # type: ignore[import]
 
 import pandas as pd
 from pytorch_lightning.utilities.warnings import PossibleUserWarning
 import pytest
-import torch
 
-from ngautonml.algorithms.impl.algorithm_instance import DatasetError
+from ngautonml.problem_def.problem_def import ProblemDefinition
 from ngautonml.wrangler.dataset import Column, Dataset, DatasetKeys, Metadata, RoleName
-from .AutoNHITS import AutoNHITSModel
+from .NHITS import NHITSModel
 
 
 def test_sunny_day() -> None:
     warnings.filterwarnings("ignore", category=UserWarning)
     warnings.filterwarnings("ignore", category=PossibleUserWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-    if not torch.cuda.is_available():
-        print('test disabled due to lack of GPU.')
-        return
-
-    model = AutoNHITSModel(num_samples=2)
+    model = NHITSModel()
     dut = model.instantiate()
 
     AirPassengersCovariates = AirPassengersDF[['unique_id', 'ds']]
     AirPassengersTarget = AirPassengersDF[['y']]
 
+    problem_def = ProblemDefinition({
+        'dataset': {
+            'config': 'ignore',
+            'column_roles': {
+                'time': {'name': 'ds'},
+            }
+        },
+        'problem_type': {
+            'task': 'forecasting'
+        },
+        'forecasting': {
+            'horizon': 12,
+            'input_size': 24,
+            'frequency': 'ME'
+        }
+    })
+
     metadata = Metadata(
+        problem_def=problem_def,
         roles={
             RoleName.TIMESERIES_ID: [Column('unique_id')],
             RoleName.TIME: [Column('ds')],
             RoleName.TARGET: [Column('y')]
-        },
-        forecasting={'horizon': 12, 'input_size': 24, 'frequency': 'M'})
+        })
     dataset = Dataset(metadata=metadata, **{
         DatasetKeys.COVARIATES.value: AirPassengersCovariates,
         DatasetKeys.TARGET.value: AirPassengersTarget,
     })
+
     dut.fit(dataset)
 
     got = dut.predict(dataset)
 
     first = got.predictions.head(n=1)
     assert first['ds'][0] == pd.Timestamp('1961-01-31 00:00:00')
-    assert first['y'][0] == pytest.approx(451.5, 0.001)
-
-
-def test_missing_input_size() -> None:
-    warnings.filterwarnings("ignore", category=UserWarning)
-    warnings.filterwarnings("ignore", category=PossibleUserWarning)
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-
-    model = AutoNHITSModel(num_samples=2)
-    dut = model.instantiate()
-
-    AirPassengersCovariates = AirPassengersDF[['unique_id', 'ds']]
-    AirPassengersTarget = AirPassengersDF[['y']]
-
-    metadata = Metadata(
-        roles={
-            RoleName.TIMESERIES_ID: [Column('unique_id')],
-            RoleName.TIME: [Column('ds')],
-            RoleName.TARGET: [Column('y')]
-        },
-        forecasting={'horizon': 12, 'frequency': 'M'})  # Missing input size
-    dataset = Dataset(metadata=metadata, **{
-        DatasetKeys.COVARIATES.value: AirPassengersCovariates,
-        DatasetKeys.TARGET.value: AirPassengersTarget,
-    })
-
-    with pytest.raises(DatasetError, match='input_size'):
-        dut.fit(dataset)
+    assert first['y'][0] == pytest.approx(439.86398, 1e-6)
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATS.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATS.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,82 +27,65 @@
     The Neural Basis Expansion Analysis for Time Series (NBEATS), is a simple and yet effective
     architecture, it is built with a deep stack of MLPs with the doubly residual connections. It
     has a generic and interpretable architecture depending on the blocks it uses. Its
     interpretable architecture is recommended for scarce data settings, as it regularizes its
     predictions through projections unto harmonic and trend basis well-suited for most forecasting
     tasks.
 
-    Required Parameters:
-    `h`: int, Forecast horizon. <br>
-    `input_size`: int, autorregresive inputs size, y=[1,2,3,4] input_size=2 -> y_[t-2:t]=[1,2].<br>
+    .. rubric:: Required Parameters:
 
-    Hyperparams:
-
-    n_harmonics: int, Number of harmonic terms for seasonality stack type. Note that
-      len(n_harmonics) = len(stack_types). Note that it will only be used if a seasonality stack is
-      used.
-
-    n_polynomials: int, polynomial degree for trend stack. Note that len(n_polynomials) =
-      len(stack_types). Note that it will only be used if a trend stack is used.
-
-    stack_types: List[str], List of stack types. Subset from [‘seasonality’, ‘trend’, ‘identity’].
-
-    n_blocks: List[int], Number of blocks for each stack. Note that len(n_blocks) =
-      len(stack_types).
-
-    mlp_units: List[List[int]], Structure of hidden layers for each stack type. Each internal list
-      should contain the number of units of each hidden layer. Note that len(n_hidden) =
-      len(stack_types).
-
-    dropout_prob_theta: float, Float between (0, 1). Dropout for N-BEATS basis.
-
-    shared_weights: bool, If True, all blocks within each stack will share parameters.
-
-    activation: str, activation from [‘ReLU’, ‘Softplus’, ‘Tanh’, ‘SELU’, ‘LeakyReLU’, ‘PReLU’,
-      ‘Sigmoid’].
-
-    loss: PyTorch module, instantiated train loss class from losses collection.
-
-    valid_loss: PyTorch module=loss, instantiated valid loss class from losses collection.
-
-    max_steps: int=1000, maximum number of training steps.
-
-    learning_rate: float=1e-3, Learning rate between (0, 1).
-
-    num_lr_decays: int=3, Number of learning rate decays, evenly distributed across max_steps.
-
-    early_stop_patience_steps: int=-1, Number of validation iterations before early stopping.
-
-    val_check_steps: int=100, Number of training steps between every validation loss check.
-
-    batch_size: int=32, number of different series in each batch.
-
-    valid_batch_size: int=None, number of different series in each validation and test batch, if
-      None uses batch_size.
-
-    windows_batch_size: int=1024, number of windows to sample in each training batch, default uses
-      all.
-
-    inference_windows_batch_size: int=-1, number of windows to sample in each inference batch, -1
-      uses all.
-
-    step_size: int=1, step size between each window of temporal data.
-
-    scaler_type: str=‘identity’, type of scaler for temporal inputs normalization see temporal
-      scalers.
-
-    random_seed: int, random_seed for pytorch initializer and numpy generators.
-
-    num_workers_loader: int=os.cpu_count(), workers to be used by TimeSeriesDataLoader.
-
-    drop_last_loader: bool=False, if True TimeSeriesDataLoader drops last non-full batch.
-
-    alias: str, optional, Custom name of the model.
-
-    **trainer_kwargs: int, keyword trainer arguments inherited from PyTorch Lighning’s trainer.
+    * ``h``: ``int``, Forecast horizon.
+    * ``input_size``: ``int``, autorregresive inputs size,
+      ``y=[1,2,3,4] input_size=2 -> y_[t-2:t]=[1,2]``.
+
+    .. rubric:: Hyperparams:
+
+    * ``n_harmonics``: ``int``, Number of harmonic terms for seasonality stack type. Note that
+      ``len(n_harmonics) = len(stack_types)``. Note that it will only be used if a seasonality
+      stack is used.
+    * ``n_polynomials``: ``int``, polynomial degree for trend stack. Note that
+      ``len(n_polynomials) = len(stack_types)``. Note that it will only be used if a trend
+      stack is used.
+    * ``stack_types``: ``List[str]``, List of stack types. Subset from ``['seasonality',
+      'trend', 'identity']``.
+    * ``n_blocks``: ``List[int]``, Number of blocks for each stack. Note that ``len(n_blocks) =
+      len(stack_types)``.
+    * ``mlp_units``: ``List[List[int]]``, Structure of hidden layers for each stack type. Each
+      internal list should contain the number of units of each hidden layer. Note that
+      ``len(n_hidden) = len(stack_types).``
+    * ``dropout_prob_theta``: ``float``, Float between ``(0, 1)``. Dropout for N-BEATS basis.
+    * ``shared_weights``: ``bool``, If ``True``, all blocks within each stack will share parameters.
+    * ``activation``: ``str``, activation from ``['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU',
+      'PReLU', 'Sigmoid']``.
+    * ``loss``: PyTorch module, instantiated train loss class from losses collection.
+    * ``valid_loss``: PyTorch module=``loss``, instantiated valid loss class from losses collection.
+    * ``max_steps``: ``int=1000``, maximum number of training steps.
+    * ``learning_rate``: ``float=1e-3``, Learning rate between ``(0, 1)``.
+    * ``num_lr_decays``: ``int=3``, Number of learning rate decays, evenly distributed across
+      max_steps.
+    * ``early_stop_patience_steps``: ``int=-1``, Number of validation iterations before early
+      stopping.
+    * ``val_check_steps``: ``int=100``, Number of training steps between every validation loss
+      check.
+    * ``batch_size``: ``int=32``, number of different series in each batch.
+    * ``valid_batch_size``: ``int=None``, number of different series in each validation and test
+      batch, if None uses batch_size.
+    * ``windows_batch_size``: ``int=1024``, number of windows to sample in each training batch,
+      default uses all.
+    * ``inference_windows_batch_size``: ``int=-1``, number of windows to sample in each inference
+      batch, -1 uses all.
+    * ``step_size``: ``int=1``, step size between each window of temporal data.
+    * ``scaler_type``: ``str=identity``, type of scaler for temporal inputs normalization see
+      temporal scalers.
+    * ``random_seed``: ``int``, random_seed for pytorch initializer and numpy generators.
+    * ``num_workers_loader``: ``int=os.cpu_count()``, workers to be used by TimeSeriesDataLoader.
+    * ``drop_last_loader``: ``bool=False``, if True TimeSeriesDataLoader drops last non-full batch.
+    * ``alias``: ``str``, optional, Custom name of the model.
+    * ``**trainer_kwargs``: ``int``, keyword trainer arguments inherited from
+      PyTorch Lightning's trainer.
     '''
     _name = 'neuralforecast.models.NBEATS'
     _basename = 'NBEATS'
     _tags = {
         'task': [TaskType.FORECASTING.name],
         'data_type': [DataType.TIMESERIES.name],
         'for_tests': ['true'],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATS_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATS_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from neuralforecast.utils import AirPassengersDF  # type: ignore[import]
 
 import pandas as pd
 from pytorch_lightning.utilities.warnings import PossibleUserWarning
 import pytest
 
+from ngautonml.problem_def.problem_def import ProblemDefinition
 from ngautonml.wrangler.dataset import Column, Dataset, DatasetKeys, Metadata, RoleName
 from .NBEATS import NBEATSModel
 
 
 def test_sunny_day() -> None:
     warnings.filterwarnings("ignore", category=UserWarning)
     warnings.filterwarnings("ignore", category=PossibleUserWarning)
@@ -22,21 +23,38 @@
 
     model = NBEATSModel()
     dut = model.instantiate()
 
     AirPassengersCovariates = AirPassengersDF[['unique_id', 'ds']]
     AirPassengersTarget = AirPassengersDF[['y']]
 
+    problem_def = ProblemDefinition({
+        'dataset': {
+            'config': 'ignore',
+            'column_roles': {
+                'time': {'name': 'ds'}
+            }
+        },
+        'problem_type': {
+            'task': 'forecasting'
+        },
+        'forecasting': {
+            'horizon': 12,
+            'input_size': 24,
+            'frequency': 'ME'
+        }
+    })
+
     metadata = Metadata(
+        problem_def=problem_def,
         roles={
             RoleName.TIMESERIES_ID: [Column('unique_id')],
             RoleName.TIME: [Column('ds')],
             RoleName.TARGET: [Column('y')]
-        },
-        forecasting={'horizon': 12, 'input_size': 24, 'frequency': 'M'})
+        })
     dataset = Dataset(metadata=metadata, **{
         DatasetKeys.COVARIATES.value: AirPassengersCovariates,
         DatasetKeys.TARGET.value: AirPassengersTarget,
     })
 
     dut.fit(dataset)
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/NBEATSx_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/NBEATSx_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from neuralforecast.utils import AirPassengersDF  # type: ignore[import]
 
 import pandas as pd
 from pytorch_lightning.utilities.warnings import PossibleUserWarning
 import pytest
 
+from ngautonml.problem_def.problem_def import ProblemDefinition
 from ngautonml.wrangler.dataset import Column, Dataset, DatasetKeys, Metadata, RoleName
 from .NBEATSx import NBEATSxModel
 
 
 def test_sunny_day() -> None:
     warnings.filterwarnings("ignore", category=UserWarning)
     warnings.filterwarnings("ignore", category=PossibleUserWarning)
@@ -22,21 +23,38 @@
 
     model = NBEATSxModel()
     dut = model.instantiate()
 
     AirPassengersCovariates = AirPassengersDF[['unique_id', 'ds']]
     AirPassengersTarget = AirPassengersDF[['y']]
 
+    problem_def = ProblemDefinition({
+        'dataset': {
+            'config': 'ignore',
+            'column_roles': {
+                'time': {'name': 'ds'},
+            }
+        },
+        'problem_type': {
+            'task': 'forecasting'
+        },
+        'forecasting': {
+            'horizon': 12,
+            'input_size': 24,
+            'frequency': 'ME'
+        }
+    })
+
     metadata = Metadata(
+        problem_def=problem_def,
         roles={
             RoleName.TIMESERIES_ID: [Column('unique_id')],
             RoleName.TIME: [Column('ds')],
             RoleName.TARGET: [Column('y')]
-        },
-        forecasting={'horizon': 12, 'input_size': 24, 'frequency': 'M'})
+        })
     dataset = Dataset(metadata=metadata, **{
         DatasetKeys.COVARIATES.value: AirPassengersCovariates,
         DatasetKeys.TARGET.value: AirPassengersTarget,
     })
 
     dut.fit(dataset)
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_auto_model.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_auto_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 '''An AutonML implementation of neuralforecast.models.NHITS'''
 # pylint: disable=invalid-name, duplicate-code
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import abc
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 import neuralforecast as nf  # type: ignore[import]
 from neuralforecast.common._base_windows import BaseWindows  # type: ignore[import]
 from pytorch_lightning import seed_everything
 from ray import tune
 
 from ngautonml.algorithms.impl.algorithm import Algorithm, AlgorithmCatalog
 from ngautonml.algorithms.impl.algorithm_instance import DatasetError
 from ngautonml.wrangler.dataset import Dataset
 
+from ...config_components.forecasting_config import ForecastingConfig
 from .neuralforecast_model import NeuralForecastModel, NeuralForecastModelInstance
 
 
 class NeuralForecastAutoModel(NeuralForecastModel, metaclass=abc.ABCMeta):
     '''Base class for neuralforecast.auto.*'''
     _name: str = 'unnamed_neuralforecast_auto_model'
 
@@ -56,47 +57,53 @@
             # Compute validation every 50 steps
             "val_check_steps": 50,
             # Random seed
             # TODO(Merritt/Piggy/Kin/Cristian): why is this picked randomly?
             "random_seed": tune.randint(1, 10),
         }
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit a model based on train data.
 
         Fit for neuralforecast auto models instantiates the model.
         '''
+        if dataset is None:
+            return
         # The next 4 lines are to work around a bug in
         # pytorch_lightning/utilities/parsing.py:_get_init_args.
         # TODO(piggy): Put a link to the pytorch_lightning bug here.
         parent = None
         parent = parent  # pylint: disable=self-assigning-variable
         overrides: Dict[str, Any] = {}
         overrides = overrides  # pylint: disable=self-assigning-variable
 
         ds = self._combine_and_rename(dataset=dataset)
 
-        hyperparams = self.hyperparams(h=dataset.metadata.horizon)
+        forecasting_metadata = dataset.metadata.get_conf('forecasting')
+        assert isinstance(forecasting_metadata, ForecastingConfig), (
+            f'BUG: "forecasting" config is of type {type(forecasting_metadata)}',
+            'expected ForecastingConfig')
+
+        hyperparams = self.hyperparams(h=forecasting_metadata.horizon)
         if hyperparams['config'] is None:
             hyperparams['config'] = self._default_config
 
         assert isinstance(hyperparams['config'], Dict)
 
         # set input size from metadata
-        if dataset.metadata.input_size is None:
+        if forecasting_metadata.input_size is None:
             raise DatasetError(
                 f'Attempt to fit {self._algorithm.name} on a dataset with no input_size metadata.')
-        hyperparams['config']['input_size'] = dataset.metadata.input_size
+        hyperparams['config']['input_size'] = forecasting_metadata.input_size
 
         models = [
             self._constructor(**hyperparams)
         ]
-        assert dataset.metadata.frequency is not None, (
-            'BUG: Neuralforecast model was given a dataset without frequency metadata.')
-        self._impl = nf.NeuralForecast(models=models, freq=dataset.metadata.frequency)
+        self._impl = nf.NeuralForecast(models=models,
+                                       freq=forecasting_metadata.frequency)
         try:
             self._impl.fit(df=ds.get_dataframe())
         except KeyError as err:
             raise DatasetError(f'fit dataset malformed {ds!r}') from err
 
         self._trained = True
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 '''An AutonML implementation of neuralforecast.models.NHITS'''
 # pylint: disable=invalid-name, duplicate-code
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import abc
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 
 import neuralforecast as nf  # type: ignore[import]
 from neuralforecast.common._base_windows import BaseWindows  # type: ignore[import]
 
 from ngautonml.algorithms.impl.algorithm import Algorithm, AlgorithmCatalog, InputValueError
 from ngautonml.algorithms.impl.algorithm_instance import DatasetError
 from ngautonml.algorithms.impl.fittable_algorithm_instance import FittableAlgorithmInstance
 from ngautonml.wrangler.constants import Defaults
 from ngautonml.wrangler.dataset import Column, Dataset, DatasetKeys, RoleName
 
+from ...config_components.forecasting_config import ForecastingConfig
+
 
 class NeuralForecastModel(Algorithm, metaclass=abc.ABCMeta):
     '''Base class for neuralforecast.models.*'''
     _name: str = 'unnamed_neuralforecast_model'
     _default_hyperparams: Dict[str, Any] = {
         'futr_exog_list': None,
         'hist_exog_list': None,
@@ -36,15 +38,15 @@
     _default_hyperparams: Dict[str, Any]
 
     def __init__(self, parent: Algorithm, **overrides: Any):
         super().__init__(parent=parent)
         if ('true' in parent.tags.get('supports_random_seed', ['false'])
                 and 'random_seed' not in overrides):
             overrides['random_seed'] = Defaults.SEED
-        self._default_hyperparams = self._algorithm.hyperparams(**overrides)
+        self._default_hyperparams = self.algorithm.hyperparams(**overrides)
         # check if default hyp has a seed and if not add it
 
     def _combine_and_rename(self, dataset: Dataset) -> Dataset:
         time_cols = dataset.metadata.roles.get(RoleName.TIME, [])
         assert len(time_cols) == 1, (
             f'BUG: validation should catch missing or non-unique time column: {time_cols}')
         time_col = time_cols[0]
@@ -96,19 +98,21 @@
 
     def hyperparams(self, **overrides: Any) -> Dict[str, Any]:
         '''Apply overrides to the default hyperparams.'''
         default_hyperparams = self._default_hyperparams.copy()
         default_hyperparams.update(**overrides)
         return default_hyperparams
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit a model based on train data.
 
         Fit for neuralforecast models instantiates the model.
         '''
+        if dataset is None:
+            return
         self._trained = True
 
         # The next 4 lines are to work around a bug in
         # pytorch_lightning/utilities/parsing.py:_get_init_args.
         # TODO(piggy): Put a link to the pytorch_lightning bug here.
         parent = None
         parent = parent  # pylint: disable=self-assigning-variable
@@ -127,37 +131,41 @@
         stat_exog_df = None
         if DatasetKeys.STATIC_EXOGENOUS.value in dataset and (
             dataset[
                 DatasetKeys.STATIC_EXOGENOUS.value] is not None):
             stat_exog = dataset[DatasetKeys.STATIC_EXOGENOUS.value].columns
             stat_exog_df = dataset[DatasetKeys.STATIC_EXOGENOUS.value]
 
+        forecast_conf = dataset.metadata.get_conf('forecasting')
+        assert isinstance(forecast_conf, ForecastingConfig)
         models = [
             self._constructor(
                 **self.hyperparams(
-                    h=dataset.metadata.horizon, input_size=dataset.metadata.input_size,
+                    h=forecast_conf.horizon, input_size=forecast_conf.input_size,
                     futr_exog_list=futr_exog,
                     hist_exog_list=hist_exog,
                     stat_exog_list=stat_exog))
         ]
-        assert dataset.metadata.frequency is not None, (
+        assert forecast_conf.frequency is not None, (
             'BUG: Neuralforecast model was given a dataset without frequency metadata.')
-        self._impl = nf.NeuralForecast(models=models, freq=dataset.metadata.frequency)
+        self._impl = nf.NeuralForecast(models=models, freq=forecast_conf.frequency)
         try:
             self._impl.fit(df=ds.get_dataframe(), static_df=stat_exog_df)
         except KeyError as err:
             raise DatasetError(f'fit dataset malformed: \n{ds!r}') from err
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         ds = self._combine_and_rename(dataset=dataset)
         try:
             result = self._impl.predict(df=ds.dataframe)
         except KeyError as err:
             raise DatasetError(f'predict dataset malformed {ds!r}') from err
-        result.rename(columns={self._algorithm.basename: 'y'}, inplace=True)
+        result.rename(columns={self.algorithm.basename: 'y'}, inplace=True)
         # this is a workaround to a neuralforecast bug:
         # unique_id is incorrectly returned as an index rather than a column
         result.reset_index(inplace=True)
         retval = ds.output()
         retval.predictions = result
         return retval
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/examples_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/examples_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 '''Tests replicating example notebooks.'''
 # pylint: disable=missing-function-docstring,missing-class-docstring
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from glob import glob
-import subprocess
 from pathlib import Path
+import subprocess
 import warnings
 
+import pytest
 from pytorch_lightning.utilities.warnings import PossibleUserWarning
 
 from ngautonml.wrangler.wrangler import Wrangler
 from ngautonml.problem_def.problem_def import ProblemDefinition
 from ngautonml.algorithms.impl.algorithm_auto import FakeAlgorithmCatalogAuto
-# pylint: disable=duplicate-code
+# pylint: disable=duplicate-code, redefined-outer-name
 
 
 def module_path() -> Path:
     return Path(__file__).parents[3]
 
 
+@pytest.fixture(scope="session")
+def resource() -> str:
+    plugin_root = Path(__file__).parents[1]
+
+    subprocess.run(['python', '-m', 'build'], cwd=plugin_root, check=False)
+
+    pluginpaths = glob(str(plugin_root / 'dist' / 'ngautonml_forecasting-*py3-none-any.whl'))
+    assert len(pluginpaths) == 1, f'BUG: unexpected extra whl files: {pluginpaths}'
+    pluginpath = Path(pluginpaths[0])
+    subprocess.run(['pip', 'install', pluginpath], check=True)
+
+    yield "plugin"
+
+    subprocess.run(['pip', 'uninstall', '-y', pluginpath], check=False)
+
+
 AIR_PASSENGERS_CONFIG = """
 {{
     "dataset" : {{
         "config" : "local",
         "train_path" : "{train_path}",
         "test_path" : "{test_path}",
         "column_roles": {{
@@ -33,21 +50,21 @@
             }},
             "time" : {{
                 "name" : "ds"
             }},
             "target" : {{
                 "name" : "y"
             }}
-        }},
-        "forecasting" : {{
-            "horizon" : 5,
-            "input_size" : 15,
-            "frequency": "M"
         }}
     }},
+    "forecasting" : {{
+        "horizon" : 5,
+        "input_size" : 15,
+        "frequency": "ME"
+    }},
     "problem_type" : {{
         "data_type": "TIMESERIES",
         "task": "FORECASTING"
     }},
     "metrics" :  {{
         "root_mean_squared_error": {{}}
     }},
@@ -62,38 +79,49 @@
 def air_passengers_config():
     train_path = module_path() / 'examples' / 'forecasting' / 'air-passengers-train.csv'
     test_path = module_path() / 'examples' / 'forecasting' / 'air-passengers-test.csv'
     pdef = AIR_PASSENGERS_CONFIG.format(train_path=train_path, test_path=test_path)
     return ProblemDefinition(pdef)
 
 
-def test_wrangle_forecasting() -> None:
-    plugin_root = Path(__file__).parents[1]
-
-    subprocess.run(['python', '-m', 'build'], cwd=plugin_root, check=True)
-
-    pluginpaths = glob(str(plugin_root / 'dist' / 'ngautonml_forecasting-*py3-none-any.whl'))
-    assert len(pluginpaths) == 1, f'BUG: unexpected extra whl files: {pluginpaths}'
-    pluginpath = Path(pluginpaths[0])
-    subprocess.run(['pip', 'install', pluginpath], check=True)
-
+def test_wrangle_forecasting(resource: str) -> None:
+    _ = resource
     warnings.filterwarnings("ignore", category=UserWarning)
     warnings.filterwarnings("ignore", category=PossibleUserWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
     problem_definition = air_passengers_config()
     dut = Wrangler(
         problem_definition=problem_definition,
         algorithm_catalog=FakeAlgorithmCatalogAuto
     )
 
-    try:
-        got = dut.fit_predict_rank()
+    got = dut.fit_predict_rank()
 
-        assert got.test_results is not None
-        train_predictions = list(got.train_results.values())[0].prediction.predictions
-        test_predictions = list(got.test_results.values())[0].prediction.predictions
-
-        assert train_predictions.shape == (5, 4)
-        assert test_predictions.shape == (5, 3)
-    finally:
-        subprocess.run(['pip', 'uninstall', '-y', pluginpath], check=False)
+    assert got.test_results is not None
+    train_predictions = list(got.train_results.values())[0].prediction.predictions
+    test_predictions = list(got.test_results.values())[0].prediction.predictions
+
+    assert train_predictions.shape == (5, 4)
+    assert test_predictions.shape == (5, 3)
+
+
+def test_example_forecasting(tmp_path: Path, resource: str) -> None:
+    _ = resource
+    path = module_path() / 'examples' / 'forecasting' / 'air-passengers.json'
+    csv_path = module_path() / 'examples' / 'forecasting' / 'air-passengers-train.csv'
+    test_csv_path = module_path() / 'examples' / 'forecasting' / 'air-passengers-test.csv'
+    with path.open() as file:
+        pd_str = file.read()
+    pd_paths_fixed = pd_str.replace(
+        'ngautonml/examples/forecasting/air-passengers-train.csv',
+        str(csv_path)
+    )
+    pd_paths_fixed = pd_paths_fixed.replace(
+        'ngautonml/examples/forecasting/air-passengers-test.csv',
+        str(test_csv_path)
+    )
+    pd_paths_fixed = pd_paths_fixed.replace(
+        'ngautonml/examples/forecasting/air-passengers-output',
+        str(tmp_path / 'output_dir')
+    )
+    ProblemDefinition(pd_paths_fixed)  # fails if example json is not valid
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/splitters/forecasting_splitter.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/splitters/forecasting_splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ngautonml.problem_def.cross_validation_config import CrossValidationConfig
 from ngautonml.problem_def.task import DataType, TaskType
 from ngautonml.splitters.impl.splitter import (Fold, SplitDataset, Splitter,
                                                SplitterCatalog)
 from ngautonml.wrangler.dataset import Dataset, DatasetKeys, RoleName
 
+from ..config_components.forecasting_config import ForecastingConfig
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 # We favor standalone clarity over code unification for splitters.
 # pylint: disable=duplicate-code
 
@@ -24,27 +25,35 @@
              'data_type': [DataType.TABULAR.name,
                            DataType.TIMESERIES.name]}
 
     def split(self,
               dataset: Dataset,
               **unused_overrides) -> SplitDataset:
         '''Split dataset into ground_truth, train, and validation sets
-          for time series forecasting problems.
+        for time series forecasting problems.
+
+        Generated fields are:
+
+        * ``ground_truth`` is the last ``dataset_config.horizon`` entries of the dataset.
+        * ``train`` is all entries that are not in ``ground_truth``.
+        * ``validate`` is the last ``input_size`` entries of train (what is needed to predict
+          values for ``ground_truth``)
 
-        ground_truth is the last dataset_config.horizon entries of the dataset
-        train is all entries that are not in ground_truth
-        validate is the last input_size entries of train (what is needed to predict
-          values for ground_truth)
         '''
         train = dataset.output()
         validate = dataset.output()
         ground_truth = dataset.output()
 
-        horizon = dataset.metadata.horizon
-        input_size = dataset.metadata.input_size
+        forecasting_metadata = dataset.metadata.get_conf('forecasting')
+        assert isinstance(forecasting_metadata, ForecastingConfig), (
+            f'BUG: "forecasting" component is a {type(forecasting_metadata)},'
+            ', exepcted a ForecastingConfig.')
+
+        horizon = forecasting_metadata.horizon
+        input_size = forecasting_metadata.input_size
         assert horizon is not None, (
             'BUG: forecasting splitter used without horizon metadata.')
         assert input_size is not None, (
             'BUG: forecasting splitter used without input size metadata.')
 
         data_df = dataset.get_dataframe()
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/splitters/forecasting_splitter_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/splitters/forecasting_splitter_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,89 @@
 '''Tests for sampled_splitter.py'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import pandas as pd
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
-import pytest
 
-from ngautonml.dataset_formats.impl.dataset_format_catalog import DatasetFormatCatalogAuto
+from ngautonml.config_components.dataset_config import DatasetConfig
 from ngautonml.problem_def.cross_validation_config import CrossValidationConfig
+from ngautonml.problem_def.problem_def import ProblemDefinition
 from ngautonml.wrangler.dataset import Dataset, DatasetKeys
 from .forecasting_splitter import ForecastingSplitter
 
 # pylint: disable=missing-function-docstring, duplicate-code
 
-TEST_DATASET_CONFIG = {
-    "config": "ignore",
-    "forecasting": {
-        "horizon": 30,
-        "input_size": 90
+
+TEST_PROBLEM_DEF = {
+    'dataset': {
+        'config': 'ignore',
+        'column_roles': {
+            'time': {'name': 'a'},
+            'target': {'name': 'c'}
+        }
     },
-    "column_roles": {
-        "target": {
-            "name": "c",
-        },
-        "time": {
-            "name": "a",
-        },
+    'problem_type': {
+        'task': 'forecasting'
     },
+    'forecasting': {
+        'horizon': 30,
+        'input_size': 90,
+        'frequency': 'ME'
+    }
 }
 
 
 def test_split_sunny_day() -> None:
-    dataset_config = DatasetFormatCatalogAuto().build(TEST_DATASET_CONFIG)
-    metadata = dataset_config.metadata
+    problem_def = ProblemDefinition(TEST_PROBLEM_DEF)
+    dataset_config = problem_def.get_conf(problem_def.Keys.DATASET)
+    assert isinstance(dataset_config, DatasetConfig)
     dataframe = pd.DataFrame({
         'a': range(1, 1001),
         'b': range(1001, 2001),
         'c': range(2001, 3001)})
-    data = Dataset(metadata=metadata, **{
+    data = Dataset(metadata=dataset_config.metadata, **{
         'dataframe': dataframe,
         'static_exogenous': None})
 
     dut = ForecastingSplitter(cv_config=CrossValidationConfig({}))
 
+    dataset_config = problem_def.get_conf(problem_def.Keys.DATASET)
+    assert isinstance(dataset_config, DatasetConfig)
+
     got = dut.split(dataset=data, dataset_config=dataset_config)
     assert len(got.folds) == 1
 
     assert got.folds[0].train.dataframe.shape == (970, 3)
     assert got.folds[0].validate.dataframe.shape == (90, 3)
     assert got.ground_truth is not None
     assert got.ground_truth.ground_truth.shape == (30, 3)
 
     # Confirm that order is preserved.
     assert got.folds[0].train[DatasetKeys.DATAFRAME.value].index[599] == 599
 
 
-TEST_DATASET_CONFIG_NO_TIME = {
-    "config": "ignore",
-    "forecasting": {
-        "horizon": 30,
-        "input_size": 90
-    },
-    "column_roles": {
-        "target": {
-            "name": "class",
-        },
-    },
-}
-
-
-def test_split_no_time() -> None:
-    dataset_config = DatasetFormatCatalogAuto().build(TEST_DATASET_CONFIG_NO_TIME)
-    metadata = dataset_config.metadata
-    dataframe = pd.DataFrame({
-        'a': range(1, 1001),
-        'b': range(1001, 2001),
-        'c': range(2001, 3001)})
-    data = Dataset(metadata=metadata, **{DatasetKeys.DATAFRAME.value: dataframe})
-
-    dut = ForecastingSplitter(cv_config=CrossValidationConfig({}))
-
-    with pytest.raises(AssertionError, match='TIME'):
-        dut.split(dataset=data, dataset_config=dataset_config)
-
-
 def test_datetime_parse() -> None:
-    dataset_config = DatasetFormatCatalogAuto().build(TEST_DATASET_CONFIG)
-    metadata = dataset_config.metadata
+    problem_def = ProblemDefinition(TEST_PROBLEM_DEF)
+    dataset_config = problem_def.get_conf(problem_def.Keys.DATASET)
+    assert isinstance(dataset_config, DatasetConfig)
+
     dataframe = pd.DataFrame({
         'a': ['2013-12-22', '2013-12-23', '2013-12-24'],
         'b': range(1000, 1003),
         'c': range(2000, 2003)})
-    data = Dataset(metadata=metadata, **{
+    data = Dataset(metadata=dataset_config.metadata, **{
         'dataframe': dataframe,
         'static_exogenous': None})
 
     dut = ForecastingSplitter(cv_config=CrossValidationConfig({}))
 
+    dataset_config = problem_def.get_conf(problem_def.Keys.DATASET)
+    assert isinstance(dataset_config, DatasetConfig)
+
     got = dut.split(dataset=data, dataset_config=dataset_config)
     assert len(got.folds) == 1
     assert is_datetime(got.folds[0].train.get_dataframe()['a'])
     assert is_datetime(got.folds[0].validate.get_dataframe()['a'])
     assert got.ground_truth is not None
     assert is_datetime(got.ground_truth.ground_truth['a'])
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/templates/forecasting.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/templates/forecasting.py`

 * *Files identical despite different names*

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting/templates/forecasting_test.py` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting/templates/forecasting_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     "output": {},
     "dataset": {
         "config": "ignore",
         "column_roles": {
             "time": {
                 "name": "some_col"
             }
-        },
-        "forecasting": {
-            "horizon": 5,
-            "input_size": 10,
-            "frequency": "M"
         }
     },
     "problem_type": {
         "task": "forecasting"
+    },
+    "forecasting": {
+        "horizon": 5,
+        "input_size": 10,
+        "frequency": "ME"
     }
 }
 '''
 
 
 def test_forecasting_template_generate() -> None:
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/PKG-INFO` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngautonml_forecasting
-Version: 0.4.1b1
+Version: 0.4.1b2
 Summary: a plugin that installs forecasting tools for ngAutonML
 Author-email: "L.H. Piggy Yarroll" <piggy@cmu.edu>, Merritt Kowaleski <merrittk@cmu.edu>, Andrew Williams <awillia2@andrew.cmu.edu>, Jieshi Chen <jieshic@andrew.cmu.edu>
 Keywords: machine learning,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
```

### Comparing `ngautonml_forecasting-0.4.1b1/ngautonml_forecasting.egg-info/SOURCES.txt` & `ngautonml_forecasting-0.4.1b2/ngautonml_forecasting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,16 @@
 ngautonml_forecasting/algorithms/neuralforecast/NBEATSx_test.py
 ngautonml_forecasting/algorithms/neuralforecast/NHITS.py
 ngautonml_forecasting/algorithms/neuralforecast/NHITS_test.py
 ngautonml_forecasting/algorithms/neuralforecast/__init__.py
 ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_auto_model.py
 ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model.py
 ngautonml_forecasting/algorithms/neuralforecast/neuralforecast_model_test.py
+ngautonml_forecasting/config_components/__init__.py
+ngautonml_forecasting/config_components/forecasting_config.py
+ngautonml_forecasting/config_components/forecasting_config_test.py
 ngautonml_forecasting/splitters/__init__.py
 ngautonml_forecasting/splitters/forecasting_splitter.py
 ngautonml_forecasting/splitters/forecasting_splitter_test.py
 ngautonml_forecasting/templates/__init__.py
 ngautonml_forecasting/templates/forecasting.py
 ngautonml_forecasting/templates/forecasting_test.py
```

### Comparing `ngautonml_forecasting-0.4.1b1/pyproject.toml` & `ngautonml_forecasting-0.4.1b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngautonml_forecasting"
-version = "0.4.1b01"
+version = "0.4.1b02"
 description = "a plugin that installs forecasting tools for ngAutonML"
 authors = [
     {name = "L.H. Piggy Yarroll", email = "piggy@cmu.edu"},
     {name = "Merritt Kowaleski", email = "merrittk@cmu.edu"},
     {name = "Andrew Williams", email = "awillia2@andrew.cmu.edu"},
     {name = "Jieshi Chen", email = "jieshic@andrew.cmu.edu"},
 ]
@@ -17,7 +17,8 @@
     "Typing :: Typed"
 ]
 
 [project.entry-points."ngautonml.make_catalog"]
 templates = "ngautonml_forecasting:templates_make_catalog"
 algorithms = "ngautonml_forecasting:algorithms_make_catalog"
 splitters = "ngautonml_forecasting:splitters_make_catalog"
+config_components = "ngautonml_forecasting:config_components_make_catalog"
```

