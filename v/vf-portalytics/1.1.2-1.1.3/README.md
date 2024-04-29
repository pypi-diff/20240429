# Comparing `tmp/vf_portalytics-1.1.2.tar.gz` & `tmp/vf_portalytics-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vf_portalytics-1.1.2.tar", last modified: Wed Apr 10 07:56:50 2024, max compression
+gzip compressed data, was "dist/vf_portalytics-1.1.3.tar", last modified: Mon Apr 29 07:58:54 2024, max compression
```

## Comparing `vf_portalytics-1.1.2.tar` & `vf_portalytics-1.1.3.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/.circleci/
--rw-r--r--   0 root         (0) root         (0)     2045 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/.codacy.yml
--rw-r--r--   0 root         (0) root         (0)      884 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     8383 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    35141 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      192 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3581 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/example_notebooks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39193 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/example.ipynb
--rw-r--r--   0 root         (0) root         (0)    35263 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/feature_subset_example.ipynb
--rw-r--r--   0 root         (0) root         (0)    20806 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/example_notebooks/multimodel_example.ipynb
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1719 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1437 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_account_cluster_transformer.py
--rw-r--r--   0 root         (0) root         (0)     5926 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     1436 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_custom_cluster_transformer.py
--rw-r--r--   0 root         (0) root         (0)     5596 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_feature_subset.py
--rw-r--r--   0 root         (0) root         (0)     6262 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_lw_cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     1471 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_ml_helpers.py
--rw-r--r--   0 root         (0) root         (0)     5577 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_multi_model.py
--rw-r--r--   0 root         (0) root         (0)     3483 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_multi_transformer.py
--rw-r--r--   0 root         (0) root         (0)      877 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_phasing_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2244 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_prediction_model.py
--rw-r--r--   0 root         (0) root         (0)     4637 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_preprocessing.py
--rw-r--r--   0 root         (0) root         (0)      707 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/tests/test_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics/
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13085 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     1258 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4864 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/feature_subset.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/lw_cluster_model.py
--rw-r--r--   0 root         (0) root         (0)     7390 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/ml_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6939 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/model.py
--rw-r--r--   0 root         (0) root         (0)    12096 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/multi_model.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/tool.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-04-10 07:56:45.000000 vf_portalytics-1.1.2/vf_portalytics/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3581 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-10 07:56:50.000000 vf_portalytics-1.1.2/vf_portalytics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/.codacy.yml
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     8841 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    35141 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3581 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/example_notebooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/example_notebooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39193 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/example_notebooks/example.ipynb
+-rw-r--r--   0 root         (0) root         (0)    35263 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/example_notebooks/feature_subset_example.ipynb
+-rw-r--r--   0 root         (0) root         (0)    20806 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/example_notebooks/multimodel_example.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_account_cluster_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_custom_cluster_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_feature_subset.py
+-rw-r--r--   0 root         (0) root         (0)     6262 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_lw_cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_ml_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5577 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_multi_model.py
+-rw-r--r--   0 root         (0) root         (0)     3483 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_multi_transformer.py
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_phasing_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_prediction_model.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_terrain_model.py
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/tests/test_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics/
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13085 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/feature_subset.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/lw_cluster_model.py
+-rw-r--r--   0 root         (0) root         (0)     7390 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/ml_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/model.py
+-rw-r--r--   0 root         (0) root         (0)    12096 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/multi_model.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/terrain_config.py
+-rw-r--r--   0 root         (0) root         (0)     5728 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/terrain_model.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-29 07:58:48.000000 vf_portalytics-1.1.3/vf_portalytics/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3581 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-29 07:58:54.000000 vf_portalytics-1.1.3/vf_portalytics.egg-info/top_level.txt
```

### Comparing `vf_portalytics-1.1.2/.circleci/config.yml` & `vf_portalytics-1.1.3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/AUTHORS` & `vf_portalytics-1.1.3/AUTHORS`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/ChangeLog` & `vf_portalytics-1.1.3/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 CHANGES
 =======
 
+1.1.3
+-----
+
+* Formatting improvements
+* Update requirements
+* Added tests
+* Remove redundant columns in test DataFrame
+* Add pyarrow to requirements
+* Update tests (WIP)
+* Clean up imports
+* Updated ordered column list creation
+* Updated ordered column list creation
+* Updated ordered column list creation
+* String formatting
+* String formatting
+* Updated string formatting for 2.7
+* Created tests, updated terrain model config
+* Added terrain model files
+
 1.1.2
 -----
 
 * Depreciate xgboost
 * Speedup tests
 
 1.1.1
```

### Comparing `vf_portalytics-1.1.2/LICENSE` & `vf_portalytics-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/PKG-INFO` & `vf_portalytics-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf_portalytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: A consistent interface for creating Machine Learning Models compatible with VisualFabriq environment
 Home-page: https://github.com/visualfabriq/portalytics
 Author: Carst Vaartjes
 Author-email: cvaartjes@visualfabriq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vf_portalytics-1.1.2/README.md` & `vf_portalytics-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/example_notebooks/example.ipynb` & `vf_portalytics-1.1.3/example_notebooks/example.ipynb`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/example_notebooks/feature_subset_example.ipynb` & `vf_portalytics-1.1.3/example_notebooks/feature_subset_example.ipynb`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/example_notebooks/multimodel_example.ipynb` & `vf_portalytics-1.1.3/example_notebooks/multimodel_example.ipynb`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/requirements.txt` & `vf_portalytics-1.1.3/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 xgboost==0.82; python_version <= "2.7"
 xgboost==0.82; python_version > "3.3"
 statsmodels==0.10.2; python_version <= "2.7"
 statsmodels>=0.12.0; python_version > "3.3"
 pytest>=5.3.5; python_version > '3.3'
 pytest==4.6.9; python_version <= '2.7'
 pytest-cov==2.8.1
+# for tests only
+pyarrow
```

### Comparing `vf_portalytics-1.1.2/setup.cfg` & `vf_portalytics-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/helpers.py` & `vf_portalytics-1.1.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_account_cluster_transformer.py` & `vf_portalytics-1.1.3/tests/test_account_cluster_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_cluster_model.py` & `vf_portalytics-1.1.3/tests/test_cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_custom_cluster_transformer.py` & `vf_portalytics-1.1.3/tests/test_custom_cluster_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_feature_subset.py` & `vf_portalytics-1.1.3/tests/test_feature_subset.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_lw_cluster_model.py` & `vf_portalytics-1.1.3/tests/test_lw_cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_ml_helpers.py` & `vf_portalytics-1.1.3/tests/test_ml_helpers.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_multi_model.py` & `vf_portalytics-1.1.3/tests/test_multi_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_multi_transformer.py` & `vf_portalytics-1.1.3/tests/test_multi_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_phasing_transformer.py` & `vf_portalytics-1.1.3/tests/test_phasing_transformer.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_prediction_model.py` & `vf_portalytics-1.1.3/tests/test_prediction_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_preprocessing.py` & `vf_portalytics-1.1.3/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/tests/test_tool.py` & `vf_portalytics-1.1.3/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/cluster_model.py` & `vf_portalytics-1.1.3/vf_portalytics/cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/dataset.py` & `vf_portalytics-1.1.3/vf_portalytics/dataset.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/feature_subset.py` & `vf_portalytics-1.1.3/vf_portalytics/feature_subset.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/lw_cluster_model.py` & `vf_portalytics-1.1.3/vf_portalytics/lw_cluster_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/ml_helpers.py` & `vf_portalytics-1.1.3/vf_portalytics/ml_helpers.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/model.py` & `vf_portalytics-1.1.3/vf_portalytics/model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/multi_model.py` & `vf_portalytics-1.1.3/vf_portalytics/multi_model.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/tool.py` & `vf_portalytics-1.1.3/vf_portalytics/tool.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics/viz.py` & `vf_portalytics-1.1.3/vf_portalytics/viz.py`

 * *Files identical despite different names*

### Comparing `vf_portalytics-1.1.2/vf_portalytics.egg-info/PKG-INFO` & `vf_portalytics-1.1.3/vf_portalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf-portalytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: A consistent interface for creating Machine Learning Models compatible with VisualFabriq environment
 Home-page: https://github.com/visualfabriq/portalytics
 Author: Carst Vaartjes
 Author-email: cvaartjes@visualfabriq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vf_portalytics-1.1.2/vf_portalytics.egg-info/SOURCES.txt` & `vf_portalytics-1.1.3/vf_portalytics.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,23 +21,26 @@
 tests/test_lw_cluster_model.py
 tests/test_ml_helpers.py
 tests/test_multi_model.py
 tests/test_multi_transformer.py
 tests/test_phasing_transformer.py
 tests/test_prediction_model.py
 tests/test_preprocessing.py
+tests/test_terrain_model.py
 tests/test_tool.py
 vf_portalytics/__init__.py
 vf_portalytics/cluster_model.py
 vf_portalytics/dataset.py
 vf_portalytics/feature_subset.py
 vf_portalytics/lw_cluster_model.py
 vf_portalytics/ml_helpers.py
 vf_portalytics/model.py
 vf_portalytics/multi_model.py
+vf_portalytics/terrain_config.py
+vf_portalytics/terrain_model.py
 vf_portalytics/tool.py
 vf_portalytics/viz.py
 vf_portalytics.egg-info/PKG-INFO
 vf_portalytics.egg-info/SOURCES.txt
 vf_portalytics.egg-info/dependency_links.txt
 vf_portalytics.egg-info/not-zip-safe
 vf_portalytics.egg-info/pbr.json
```

### Comparing `vf_portalytics-1.1.2/vf_portalytics.egg-info/requires.txt` & `vf_portalytics-1.1.3/vf_portalytics.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 category-encoders==2.2.2
 pytest-cov==2.8.1
+pyarrow
 
 [:(python_version < "3.10")]
 scikit-learn==0.20.4
 
 [:(python_version <= "2.7")]
 joblib==0.14.1
 numpy>=1.16.6
```

