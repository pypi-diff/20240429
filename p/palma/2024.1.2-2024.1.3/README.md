# Comparing `tmp/palma-2024.1.2.tar.gz` & `tmp/palma-2024.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palma-2024.1.2.tar", last modified: Thu Apr 18 10:00:51 2024, max compression
+gzip compressed data, was "palma-2024.1.3.tar", last modified: Mon Apr 29 15:41:20 2024, max compression
```

## Comparing `palma-2024.1.2.tar` & `palma-2024.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 10:00:47.000000 palma-2024.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 10:00:47.000000 palma-2024.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 10:00:51.789838 palma-2024.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-18 10:00:47.000000 palma-2024.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.781838 palma-2024.1.2/palma/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/base/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/base/splitting_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/data_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/data_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/components/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.785838 palma-2024.1.2/palma/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/preprocessing/na_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11376 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/preprocessing/pca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/palma/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    51350 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-18 10:00:47.000000 palma-2024.1.2/palma/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/palma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 10:00:51.000000 palma-2024.1.2/palma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 10:00:47.000000 palma-2024.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 10:00:47.000000 palma-2024.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:00:51.789838 palma-2024.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:00:51.789838 palma-2024.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-18 10:00:47.000000 palma-2024.1.2/tests/test_utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.714908 palma-2024.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 15:41:14.000000 palma-2024.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 15:41:14.000000 palma-2024.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-29 15:41:20.714908 palma-2024.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-29 15:41:14.000000 palma-2024.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.706908 palma-2024.1.3/palma/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.706908 palma-2024.1.3/palma/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/base/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/base/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/base/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/base/splitting_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.706908 palma-2024.1.3/palma/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/data_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/data_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24319 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/components/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.710908 palma-2024.1.3/palma/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.710908 palma-2024.1.3/palma/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/preprocessing/na_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11376 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/preprocessing/pca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.710908 palma-2024.1.3/palma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/utils/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51350 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/utils/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-29 15:41:14.000000 palma-2024.1.3/palma/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.710908 palma-2024.1.3/palma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-29 15:41:20.000000 palma-2024.1.3/palma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-29 15:41:20.000000 palma-2024.1.3/palma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:41:20.000000 palma-2024.1.3/palma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-29 15:41:20.000000 palma-2024.1.3/palma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 15:41:20.000000 palma-2024.1.3/palma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-29 15:41:14.000000 palma-2024.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 15:41:14.000000 palma-2024.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:41:20.714908 palma-2024.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:20.710908 palma-2024.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-29 15:41:14.000000 palma-2024.1.3/tests/test_utils_.py
```

### Comparing `palma-2024.1.2/LICENSE` & `palma-2024.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/PKG-INFO` & `palma-2024.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palma
-Version: 2024.1.2
+Version: 2024.1.3
 Author-email: Vincent Laurent <vlaurent@mews-labs.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: seaborn>0.12.0
 Requires-Dist: tabulate>0.8.10
 Requires-Dist: frozendict>2.3.4
@@ -66,19 +66,23 @@
 of performances etc. In short, any element that can be replicated and that must,
 in most cases, be included in the analysis results of the models.
 Also, thanks to the use of components, this
 library is designed to be modular and allows the user to add his own
 analyses.    
 It therefore contains the following elements
 
-1. A vanilla approach described below (in basic usage section) and in the notebooks
-[classification](examples/classification.ipynb) and [regression](examples/regression.ipynb)
+1. A vanilla approach described below (in basic usage section) and in the
+   notebooks [classification](examples/classification.ipynb) and
+   [regression](examples/regression.ipynb). In this approach, the users define
+   a `Project`, which can then be passed to either a `ModelSelector` to find
+   the best model for this project, or to a `ModelEvaluation` to study more in
+   depth the behavior of a given model on this project.
 
 2. A collection of [components](doc/components.md) that can be added to enrich
-   analysis
+   analysis.
 
 Install it with 
 ``` powershell
 python -m pip install palma
 ```
 
 ## Documentation 
@@ -89,24 +93,26 @@
 
 1. Start your project
 
 To start using the library, use the project class
 
 ```python
 import pandas as pd
-from sklearn import model_selection
 from sklearn.datasets import make_classification
+from sklearn.model_selection import ShuffleSplit
 from palma import Project
 
 X, y = make_classification(n_informative=2, n_features=100)
 X, y = pd.DataFrame(X), pd.Series(y).astype(bool)
+
 project = Project(problem="classification", project_name="default")
+
 project.start(
     X, y,
-    splitter=model_selection.ShuffleSplit(n_splits=10, random_state=42),
+    splitter=ShuffleSplit(n_splits=10, random_state=42),
 )
 ```
 
 The instantiation defines the type of problem and the `start` method will set
 what is needed to carry out ML project :
 
 - A testing strategy (argument `splitter`). That will define train and test
@@ -119,20 +125,23 @@
 
 ```python
 splitter = model_selection.ShuffleSplit(n_splits=5, random_state=42)
 ```
 
 - Training data `X` and target `y`
 
+This initialization is done in two steps to allow user to add optional
+``Component``s to the project before its start.
+
 2.  Run hyper-optimisation
 
 The hyper-optimisation process will look for the best model in pool of models
-that tend to perform well on various problem.
-For this specific task we make use of FLAML module. After hyper parametrisation,
-the metric to track can be computed
+that tend to perform well on various problem. For this specific task we make
+use of [FLAML module](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
+After hyper parametrisation, the metric to track can be computed
 
 ```python
 from palma import ModelSelector
 
 ms = ModelSelector(engine="FlamlOptimizer",
                    engine_parameters=dict(time_budget=30))
 ms.start(project)
@@ -150,14 +159,15 @@
 model = ModelEvaluation(estimator=RandomForestClassifier())
 model.fit(project)
 
 # Get the optimized estimator
 model = ModelEvaluation(estimator=ms.best_model_)
 model.fit(project)
 ```
+
 ## Contributing
 
 You are very welcome to contribute to the project, by requesting features,
 pointing out new tools that can be added as component, by identifying issues and creating new features. 
 Development guidelines will be detailed in near future.
 
 * Fork the repository
```

### Comparing `palma-2024.1.2/README.md` & `palma-2024.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,23 @@
 of performances etc. In short, any element that can be replicated and that must,
 in most cases, be included in the analysis results of the models.
 Also, thanks to the use of components, this
 library is designed to be modular and allows the user to add his own
 analyses.    
 It therefore contains the following elements
 
-1. A vanilla approach described below (in basic usage section) and in the notebooks
-[classification](examples/classification.ipynb) and [regression](examples/regression.ipynb)
+1. A vanilla approach described below (in basic usage section) and in the
+   notebooks [classification](examples/classification.ipynb) and
+   [regression](examples/regression.ipynb). In this approach, the users define
+   a `Project`, which can then be passed to either a `ModelSelector` to find
+   the best model for this project, or to a `ModelEvaluation` to study more in
+   depth the behavior of a given model on this project.
 
 2. A collection of [components](doc/components.md) that can be added to enrich
-   analysis
+   analysis.
 
 Install it with 
 ``` powershell
 python -m pip install palma
 ```
 
 ## Documentation 
@@ -40,24 +44,26 @@
 
 1. Start your project
 
 To start using the library, use the project class
 
 ```python
 import pandas as pd
-from sklearn import model_selection
 from sklearn.datasets import make_classification
+from sklearn.model_selection import ShuffleSplit
 from palma import Project
 
 X, y = make_classification(n_informative=2, n_features=100)
 X, y = pd.DataFrame(X), pd.Series(y).astype(bool)
+
 project = Project(problem="classification", project_name="default")
+
 project.start(
     X, y,
-    splitter=model_selection.ShuffleSplit(n_splits=10, random_state=42),
+    splitter=ShuffleSplit(n_splits=10, random_state=42),
 )
 ```
 
 The instantiation defines the type of problem and the `start` method will set
 what is needed to carry out ML project :
 
 - A testing strategy (argument `splitter`). That will define train and test
@@ -70,20 +76,23 @@
 
 ```python
 splitter = model_selection.ShuffleSplit(n_splits=5, random_state=42)
 ```
 
 - Training data `X` and target `y`
 
+This initialization is done in two steps to allow user to add optional
+``Component``s to the project before its start.
+
 2.  Run hyper-optimisation
 
 The hyper-optimisation process will look for the best model in pool of models
-that tend to perform well on various problem.
-For this specific task we make use of FLAML module. After hyper parametrisation,
-the metric to track can be computed
+that tend to perform well on various problem. For this specific task we make
+use of [FLAML module](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
+After hyper parametrisation, the metric to track can be computed
 
 ```python
 from palma import ModelSelector
 
 ms = ModelSelector(engine="FlamlOptimizer",
                    engine_parameters=dict(time_budget=30))
 ms.start(project)
@@ -101,14 +110,15 @@
 model = ModelEvaluation(estimator=RandomForestClassifier())
 model.fit(project)
 
 # Get the optimized estimator
 model = ModelEvaluation(estimator=ms.best_model_)
 model.fit(project)
 ```
+
 ## Contributing
 
 You are very welcome to contribute to the project, by requesting features,
 pointing out new tools that can be added as component, by identifying issues and creating new features. 
 Development guidelines will be detailed in near future.
 
 * Fork the repository
```

### Comparing `palma-2024.1.2/palma/__init__.py` & `palma-2024.1.3/palma/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/base/__init__.py` & `palma-2024.1.3/palma/base/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/base/engine.py` & `palma-2024.1.3/palma/base/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 try:
     from autosklearn.classification import AutoSklearnClassifier
     from autosklearn.regression import AutoSklearnRegressor
 except ImportError:
     pass
 
 
-class BaseOptimizer(object, metaclass=ABCMeta):
+class BaseOptimizer(metaclass=ABCMeta):
 
     def __init__(self, engine_parameters: dict) -> None:
         self.__engine_parameters = engine_parameters
 
     @abstractmethod
     def optimize(self, X: pd.DataFrame, y: pd.Series,
                  splitter: "ValidationStrategy" = None
```

### Comparing `palma-2024.1.2/palma/base/model.py` & `palma-2024.1.3/palma/base/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,17 +46,17 @@
                 project.X, project.y,
                 indexes))
 
         self.all_estimators_val_, self.avg_estimator_val_ = ret[0]
         self.all_estimators_, self.avg_estimator_ = ret[1]
 
         self.predictions_ = self.__compute_predictions(
-            project, project.validation_strategy.indexes_train_test)
+            project, project.validation_strategy.indexes_train_test, self.all_estimators_)
         self.predictions_val_ = self.__compute_predictions(
-            project, project.validation_strategy.indexes_val)
+            project, project.validation_strategy.indexes_val, self.all_estimators_val_)
 
         for name, comp in self.__components.items():
             comp(project, self)
 
     def __get_fit_estimators(self, X, y, indexes):
         est = []
         for i, (train, _) in enumerate(indexes):
@@ -64,18 +64,18 @@
             y_train = y.iloc[train]
             self.__estimator = _clone(self.__estimator)
             self.__estimator.fit(x_train, y_train)
             est.append(self.__estimator)
         avg_estimator = AverageEstimator(est)
         return est, avg_estimator
 
-    def __compute_predictions(self, project, indexes):
+    def __compute_predictions(self, project, indexes, estimators):
         predictions = {}
         for i, (train, test) in enumerate(indexes):
-            est = self.all_estimators_val_[i]
+            est = estimators[i]
             if hasattr(est, "predict_proba"):
                 predict_train = est.predict_proba(project.X.iloc[train])[:, 1]
                 predict_test = est.predict_proba(project.X.iloc[test])[:, 1]
             else:
                 predict_train = est.predict(project.X.iloc[train])
                 predict_test = est.predict(project.X.iloc[test])
 
@@ -86,7 +86,11 @@
     def id(self) -> str:
         return self.__model_id
 
     @property
     def components(self):
         return self.__components
 
+    @property
+    def unfit_estimator(self):
+        return self.__estimator
+
```

### Comparing `palma-2024.1.2/palma/base/model_selection.py` & `palma-2024.1.3/palma/base/model_selection.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,32 @@
 
 from palma.base import engine as eng
 from palma.utils.utils import get_hash
 import logging
 
 
 class ModelSelector:
+    """
+    Wrapper to optimizers selecting the best model for a Project.
+
+    The optimization can be launched with the ``start`` method.
+    Once the optimization is done, the best model can be accessed as the ``best_model_`` attribute.
+
+    Parameters
+    ----------
+    - engine (str): Currently accepted values are "FlamlOptimizer" or
+      "AutoSklearnOptimizer" (the latter is deprecatted).
+    - engine_parameters (dict): parameters passed to the engine.
+
+    Methods
+    -------
+    - start(project: Project): look for best model
+
+
+    """
 
     def __init__(
             self,
             engine: Union[str, eng.BaseOptimizer],
             engine_parameters: Dict
     ) -> None:
```

### Comparing `palma-2024.1.2/palma/base/project.py` & `palma-2024.1.3/palma/base/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from hashlib import blake2b
-from typing import List
 
 import pandas as pd
 
 from palma.base.splitting_strategy import ValidationStrategy
-from palma.utils.names import get_random_name
 from palma.utils.utils import check_started
 
 
-class Project(object):
+class Project:
     """
     Represents a machine learning project with various components
     and logging capabilities.
 
     Parameters
     ----------
     project_name (str): The name of the project.
     problem (str): The description of the machine learning problem.
+                   Accepted values: "classification" or "regression".
 
     Attributes
     ----------
     base_index (List[int]): List of base indices for the project.
     components (dict): Dictionary containing project components.
     date (datetime): The date and time when the project was created.
     project_id (str): Unique identifier for the project.
```

### Comparing `palma-2024.1.2/palma/base/splitting_strategy.py` & `palma-2024.1.3/palma/base/splitting_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     return ret.astype(bool)
 
 
 def _bool_to_index(array):
     return np.where(array)[0]
 
 
-class ValidationStrategy(object):
+class ValidationStrategy:
     """
     Validation strategy for a machine learning project.
 
     Parameters
     ----------
     - splitter (Union[BaseShuffleSplit, BaseCrossValidator, List[tuple], List[str]]): The data splitting strategy.
```

### Comparing `palma-2024.1.2/palma/components/__init__.py` & `palma-2024.1.3/palma/components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 from palma.components.logger import FileSystemLogger
 from palma.components.logger import MLFlowLogger
 from palma.components.data_profiler import ProfilerYData
 from palma.components.dashboard import ExplainerDashboard
 from palma.components.performance import RegressionAnalysis
 from palma.components.performance import ScoringAnalysis
 from palma.components.performance import ShapAnalysis
+from palma.components.performance import PermutationFeatureImportance
 from palma.components.data_checker import DeepCheck, Leakage
 
 __all__ = [
     "Component",
     "FileSystemLogger",
     "MLFlowLogger",
     "ProfilerYData",
     "ExplainerDashboard",
     "RegressionAnalysis",
     "ScoringAnalysis",
     "ShapAnalysis",
+    "PermutationFeatureImportance",
     "DeepCheck",
     "Leakage"
 ]
```

### Comparing `palma-2024.1.2/palma/components/base.py` & `palma-2024.1.3/palma/components/base.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/components/checker.py` & `palma-2024.1.3/palma/components/checker.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/components/dashboard.py` & `palma-2024.1.3/palma/components/dashboard.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/components/data_checker.py` & `palma-2024.1.3/palma/components/data_checker.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/components/data_profiler.py` & `palma-2024.1.3/palma/components/data_profiler.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/components/logger.py` & `palma-2024.1.3/palma/components/logger.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/components/performance.py` & `palma-2024.1.3/palma/components/performance.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import matplotlib.pyplot as plot
 import numpy as np
 import pandas as pd
 import shap
 from sklearn import metrics
 from sklearn.metrics import _regression, _ranking
+from sklearn.inspection import permutation_importance
 
 from palma.components.base import ModelComponent
 from palma.components.logger import logger
 from palma.utils import plotting, utils
 
 __fpr_sampling__ = np.linspace(0, 1, 200)
 
@@ -596,7 +597,66 @@
         g = sns.PairGrid(df_plot, hue="error quartile", palette=palette,
                          x_vars=features, y_vars=features,
                          )
         g.map_diag(sns.histplot, multiple="stack")
         g.map_offdiag(sns.scatterplot, size=df_plot["error"])
         g.add_legend(title="", adjust_subtitles=True)
         logger.logger.log_artifact(plot.gcf(), "pair_grid")
+
+
+class PermutationFeatureImportance(ModelComponent):
+    """
+    Class for doing permutation feature importance
+
+    Parameters
+    ----------
+    n_repeat: int
+        The number of times to permute a feature.
+    random_state: int
+        The pseudo-random number generator to control the permutations of each feature.
+    n_job: int
+        The number of jobs to run in parallel. If n_job = -1, it takes all processors.
+    max_samples: int or float
+        The number of samples to draw from X to compute feature importance in each repeat (without replacement).
+        If int, then draw max_samples samples.
+        If float, then draw max_samples * X.shape[0] samples.
+    color: str
+        The color for bar plot.
+
+    Methods
+    -------
+    plot_permutation_feature_importance()
+        Plotting the result of feature permutation ONLY on the TRAINING SET
+    """
+
+    def __init__(self, n_repeat: int = 5, random_state: int = 42, n_job: int = 2,
+                 scoring: str = None, max_samples: typing.Union[int, float] = 0.7, color: str = 'darkblue'):
+        self.n_repeat = n_repeat
+        self.random_state = random_state
+        self.n_job = n_job
+        self.scoring = scoring
+        self.max_samples = max_samples
+        self.color = color
+
+    def __call__(self, project: "Project", model: "ModelEvaluation"):
+        self.indexes = project.validation_strategy.indexes_train_test
+        self.estimator = model.unfit_estimator
+        train_id = self.indexes[0][0]  # get only training indices
+        self.X_train = project.X.iloc[train_id]
+        self.y_train = project.y.iloc[train_id]
+        self.plot_permutation_feature_importance()
+
+    def plot_permutation_feature_importance(self):
+
+        args = dict(edgecolor='white', color=self.color)
+        ax = plot.gca()
+        train_res = permutation_importance(self.estimator, self.X_train, self.y_train, n_repeats=self.n_repeat,
+                                           random_state=self.random_state, n_jobs=self.n_job, scoring=self.scoring,
+                                           max_samples=self.max_samples)
+
+        sorted_importances_idx = train_res.importances_mean.argsort()
+        ax.barh(range(len(sorted_importances_idx)), train_res.importances_mean[sorted_importances_idx],
+                align='center', **args)
+        ax.set_yticks(range(len(sorted_importances_idx)), np.array(self.X_train.columns)[sorted_importances_idx])
+        ax.set_title('Train set')
+        plot.tight_layout()
+        logger.logger.log_artifact(plot.gcf(), "permutation_feature_importance")
```

### Comparing `palma-2024.1.2/palma/datasets/__init__.py` & `palma-2024.1.3/palma/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/preprocessing/__init__.py` & `palma-2024.1.3/palma/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/preprocessing/na_encoder.py` & `palma-2024.1.3/palma/preprocessing/na_encoder.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/preprocessing/pca.py` & `palma-2024.1.3/palma/preprocessing/pca.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/utils/__init__.py` & `palma-2024.1.3/palma/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/utils/checker.py` & `palma-2024.1.3/palma/utils/checker.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/utils/names.py` & `palma-2024.1.3/palma/utils/names.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/utils/plotting.py` & `palma-2024.1.3/palma/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma/utils/utils.py` & `palma-2024.1.3/palma/utils/utils.py`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/palma.egg-info/PKG-INFO` & `palma-2024.1.3/palma.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palma
-Version: 2024.1.2
+Version: 2024.1.3
 Author-email: Vincent Laurent <vlaurent@mews-labs.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: seaborn>0.12.0
 Requires-Dist: tabulate>0.8.10
 Requires-Dist: frozendict>2.3.4
@@ -66,19 +66,23 @@
 of performances etc. In short, any element that can be replicated and that must,
 in most cases, be included in the analysis results of the models.
 Also, thanks to the use of components, this
 library is designed to be modular and allows the user to add his own
 analyses.    
 It therefore contains the following elements
 
-1. A vanilla approach described below (in basic usage section) and in the notebooks
-[classification](examples/classification.ipynb) and [regression](examples/regression.ipynb)
+1. A vanilla approach described below (in basic usage section) and in the
+   notebooks [classification](examples/classification.ipynb) and
+   [regression](examples/regression.ipynb). In this approach, the users define
+   a `Project`, which can then be passed to either a `ModelSelector` to find
+   the best model for this project, or to a `ModelEvaluation` to study more in
+   depth the behavior of a given model on this project.
 
 2. A collection of [components](doc/components.md) that can be added to enrich
-   analysis
+   analysis.
 
 Install it with 
 ``` powershell
 python -m pip install palma
 ```
 
 ## Documentation 
@@ -89,24 +93,26 @@
 
 1. Start your project
 
 To start using the library, use the project class
 
 ```python
 import pandas as pd
-from sklearn import model_selection
 from sklearn.datasets import make_classification
+from sklearn.model_selection import ShuffleSplit
 from palma import Project
 
 X, y = make_classification(n_informative=2, n_features=100)
 X, y = pd.DataFrame(X), pd.Series(y).astype(bool)
+
 project = Project(problem="classification", project_name="default")
+
 project.start(
     X, y,
-    splitter=model_selection.ShuffleSplit(n_splits=10, random_state=42),
+    splitter=ShuffleSplit(n_splits=10, random_state=42),
 )
 ```
 
 The instantiation defines the type of problem and the `start` method will set
 what is needed to carry out ML project :
 
 - A testing strategy (argument `splitter`). That will define train and test
@@ -119,20 +125,23 @@
 
 ```python
 splitter = model_selection.ShuffleSplit(n_splits=5, random_state=42)
 ```
 
 - Training data `X` and target `y`
 
+This initialization is done in two steps to allow user to add optional
+``Component``s to the project before its start.
+
 2.  Run hyper-optimisation
 
 The hyper-optimisation process will look for the best model in pool of models
-that tend to perform well on various problem.
-For this specific task we make use of FLAML module. After hyper parametrisation,
-the metric to track can be computed
+that tend to perform well on various problem. For this specific task we make
+use of [FLAML module](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
+After hyper parametrisation, the metric to track can be computed
 
 ```python
 from palma import ModelSelector
 
 ms = ModelSelector(engine="FlamlOptimizer",
                    engine_parameters=dict(time_budget=30))
 ms.start(project)
@@ -150,14 +159,15 @@
 model = ModelEvaluation(estimator=RandomForestClassifier())
 model.fit(project)
 
 # Get the optimized estimator
 model = ModelEvaluation(estimator=ms.best_model_)
 model.fit(project)
 ```
+
 ## Contributing
 
 You are very welcome to contribute to the project, by requesting features,
 pointing out new tools that can be added as component, by identifying issues and creating new features. 
 Development guidelines will be detailed in near future.
 
 * Fork the repository
```

### Comparing `palma-2024.1.2/palma.egg-info/SOURCES.txt` & `palma-2024.1.3/palma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palma-2024.1.2/pyproject.toml` & `palma-2024.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "palma"
-version = "2024.1.2"
+version = "2024.1.3"
 description = ""
 authors = [{ name = 'Vincent Laurent', email = 'vlaurent@mews-labs.com' }]
 readme = "README.md"
 
 requires-python = '>=3.9'
```

### Comparing `palma-2024.1.2/tests/test_utils_.py` & `palma-2024.1.3/tests/test_utils_.py`

 * *Files identical despite different names*

