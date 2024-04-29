# Comparing `tmp/kubeflow-katib-0.16.0rc1.tar.gz` & `tmp/kubeflow-katib-0.17.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeflow-katib-0.16.0rc1.tar", last modified: Wed Aug 16 12:18:26 2023, max compression
+gzip compressed data, was "kubeflow-katib-0.17.0rc0.tar", last modified: Mon Apr 29 12:20:32 2024, max compression
```

## Comparing `kubeflow-katib-0.16.0rc1.tar` & `kubeflow-katib-0.17.0rc0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.440154 kubeflow-katib-0.16.0rc1/
--rw-r--r--   0 avelichk   (501) staff       (20)     1193 2023-08-16 12:18:26.440045 kubeflow-katib-0.16.0rc1/PKG-INFO
--rw-r--r--   0 avelichk   (501) staff       (20)     5474 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/README.md
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.432807 kubeflow-katib-0.16.0rc1/kubeflow/
--rw-r--r--   0 avelichk   (501) staff       (20)       65 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/__init__.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.433583 kubeflow-katib-0.16.0rc1/kubeflow/katib/
--rw-r--r--   0 avelichk   (501) staff       (20)     4402 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/__init__.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.433935 kubeflow-katib-0.16.0rc1/kubeflow/katib/api/
--rw-r--r--   0 avelichk   (501) staff       (20)       87 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/api/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)    47097 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/api/katib_client.py
--rw-r--r--   0 avelichk   (501) staff       (20)     1998 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/api/search.py
--rw-r--r--   0 avelichk   (501) staff       (20)    26164 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/api_client.py
--rw-r--r--   0 avelichk   (501) staff       (20)    12364 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/configuration.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.434150 kubeflow-katib-0.16.0rc1/kubeflow/katib/constants/
--rw-r--r--   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/constants/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)     2094 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/constants/constants.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3711 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/exceptions.py
--rw-r--r--   0 avelichk   (501) staff       (20)   113357 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/katib_api_pb2.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.439016 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/
--rw-r--r--   0 avelichk   (501) staff       (20)     3565 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4099 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_algorithm_setting.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4681 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_algorithm_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4118 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_collector_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5659 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_config_map_source.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6208 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_early_stopping_rule.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4155 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_early_stopping_setting.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4757 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_early_stopping_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7260 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment.py
--rw-r--r--   0 avelichk   (501) staff       (20)     8063 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_condition.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6818 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_list.py
--rw-r--r--   0 avelichk   (501) staff       (20)    12877 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)    22676 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_status.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5051 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_feasible_space.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4520 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_file_system_path.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3821 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_filter_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4885 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_graph_config.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4933 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_metric.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3887 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_metric_strategy.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4172 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_metrics_collector_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4188 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_nas_config.py
--rw-r--r--   0 avelichk   (501) staff       (20)     8263 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_objective_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3470 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_observation.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4195 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_operation.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5573 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_optimal_trial.py
--rw-r--r--   0 avelichk   (501) staff       (20)     3947 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_parameter_assignment.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4913 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_parameter_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4905 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_source_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7260 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion.py
--rw-r--r--   0 avelichk   (501) staff       (20)     8063 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_condition.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6818 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_list.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6155 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     9515 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_status.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7110 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6577 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_assignment.py
--rw-r--r--   0 avelichk   (501) staff       (20)     7913 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_condition.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6703 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_list.py
--rw-r--r--   0 avelichk   (501) staff       (20)     5184 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_parameter_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4135 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_source.py
--rw-r--r--   0 avelichk   (501) staff       (20)    13953 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_spec.py
--rw-r--r--   0 avelichk   (501) staff       (20)     6840 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_status.py
--rw-r--r--   0 avelichk   (501) staff       (20)    11124 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_template.py
--rw-r--r--   0 avelichk   (501) staff       (20)    12243 2023-08-16 12:18:10.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/rest.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.439222 kubeflow-katib-0.16.0rc1/kubeflow/katib/utils/
--rw-r--r--   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/utils/__init__.py
--rw-r--r--   0 avelichk   (501) staff       (20)     4090 2023-08-16 12:18:00.000000 kubeflow-katib-0.16.0rc1/kubeflow/katib/utils/utils.py
-drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2023-08-16 12:18:26.439880 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/
--rw-r--r--   0 avelichk   (501) staff       (20)     1193 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/PKG-INFO
--rw-r--r--   0 avelichk   (501) staff       (20)     2686 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/SOURCES.txt
--rw-r--r--   0 avelichk   (501) staff       (20)        1 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/dependency_links.txt
--rw-r--r--   0 avelichk   (501) staff       (20)        1 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/not-zip-safe
--rw-r--r--   0 avelichk   (501) staff       (20)      123 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/requires.txt
--rw-r--r--   0 avelichk   (501) staff       (20)        9 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/top_level.txt
--rw-r--r--   0 avelichk   (501) staff       (20)       38 2023-08-16 12:18:26.440195 kubeflow-katib-0.16.0rc1/setup.cfg
--rw-r--r--   0 avelichk   (501) staff       (20)     2584 2023-08-16 12:18:26.000000 kubeflow-katib-0.16.0rc1/setup.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.756443 kubeflow-katib-0.17.0rc0/
+-rw-r--r--   0 avelichk   (501) staff       (20)     1193 2024-04-29 12:20:32.756335 kubeflow-katib-0.17.0rc0/PKG-INFO
+-rw-r--r--   0 avelichk   (501) staff       (20)     5474 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/README.md
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.746160 kubeflow-katib-0.17.0rc0/kubeflow/
+-rw-r--r--   0 avelichk   (501) staff       (20)       65 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/__init__.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.747224 kubeflow-katib-0.17.0rc0/kubeflow/katib/
+-rw-r--r--   0 avelichk   (501) staff       (20)     4402 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/__init__.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.748119 kubeflow-katib-0.17.0rc0/kubeflow/katib/api/
+-rw-r--r--   0 avelichk   (501) staff       (20)       87 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/api/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    50234 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/api/katib_client.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     1998 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/api/search.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    26164 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/api_client.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    12364 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/configuration.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.748335 kubeflow-katib-0.17.0rc0/kubeflow/katib/constants/
+-rw-r--r--   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/constants/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     2093 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/constants/constants.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3711 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/exceptions.py
+-rw-r--r--   0 avelichk   (501) staff       (20)   113357 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/katib_api_pb2.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.755218 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/
+-rw-r--r--   0 avelichk   (501) staff       (20)     3565 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4099 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_algorithm_setting.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4681 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_algorithm_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4118 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_collector_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5659 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_config_map_source.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6208 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_early_stopping_rule.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4155 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_early_stopping_setting.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4757 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_early_stopping_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7260 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     8063 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_condition.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6818 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_list.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    12877 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    22676 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_status.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5051 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_feasible_space.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4520 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_file_system_path.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3821 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_filter_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4885 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_graph_config.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4933 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_metric.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3887 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_metric_strategy.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4172 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_metrics_collector_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4188 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_nas_config.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     8263 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_objective_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3470 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_observation.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4195 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_operation.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5573 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_optimal_trial.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     3947 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_parameter_assignment.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4913 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_parameter_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4905 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_source_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7260 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     8063 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_condition.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6818 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_list.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6155 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     9515 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_status.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7110 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6577 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_assignment.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     7913 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_condition.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6703 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_list.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     5184 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_parameter_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4135 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_source.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    13953 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_spec.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     6840 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_status.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    11124 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_template.py
+-rw-r--r--   0 avelichk   (501) staff       (20)    12243 2024-04-29 12:20:16.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/rest.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.755565 kubeflow-katib-0.17.0rc0/kubeflow/katib/utils/
+-rw-r--r--   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/utils/__init__.py
+-rw-r--r--   0 avelichk   (501) staff       (20)     4090 2024-04-29 12:20:07.000000 kubeflow-katib-0.17.0rc0/kubeflow/katib/utils/utils.py
+drwxr-xr-x   0 avelichk   (501) staff       (20)        0 2024-04-29 12:20:32.756185 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/
+-rw-r--r--   0 avelichk   (501) staff       (20)     1193 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/PKG-INFO
+-rw-r--r--   0 avelichk   (501) staff       (20)     2686 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/SOURCES.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)        1 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/dependency_links.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)        1 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/not-zip-safe
+-rw-r--r--   0 avelichk   (501) staff       (20)      123 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/requires.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)        9 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/top_level.txt
+-rw-r--r--   0 avelichk   (501) staff       (20)       38 2024-04-29 12:20:32.756483 kubeflow-katib-0.17.0rc0/setup.cfg
+-rw-r--r--   0 avelichk   (501) staff       (20)     2592 2024-04-29 12:20:32.000000 kubeflow-katib-0.17.0rc0/setup.py
```

### Comparing `kubeflow-katib-0.16.0rc1/PKG-INFO` & `kubeflow-katib-0.17.0rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kubeflow-katib
-Version: 0.16.0rc1
+Version: 0.17.0rc0
 Summary: Katib Python SDK for APIVersion v1beta1
 Home-page: https://github.com/kubeflow/katib/tree/master/sdk/python/v1beta1
 Author: Kubeflow Authors
 Author-email: premnath.vel@gmail.com
 License: Apache License Version 2.0
 Description: Katib Python SDK for APIVersion v1beta1
 Platform: UNKNOWN
```

### Comparing `kubeflow-katib-0.16.0rc1/README.md` & `kubeflow-katib-0.17.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/__init__.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/api/katib_client.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/api/katib_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,58 +89,85 @@
         Raises:
             TimeoutError: Timeout to create Katib Experiment.
             RuntimeError: Failed to create Katib Experiment.
         """
 
         namespace = namespace or self.namespace
 
+        experiment_name = None
+        if type(experiment) == models.V1beta1Experiment:
+            if experiment.metadata.name is not None:
+                experiment_name = experiment.metadata.name
+            elif experiment.metadata.generate_name is not None:
+                experiment_name = experiment.metadata.generate_name
+        elif "name" in experiment["metadata"]:
+            experiment_name = experiment["metadata"]["name"]
+        elif "generate_name" in experiment["metadata"]:
+            experiment_name = experiment["metadata"]["generate_name"]
+
+        if experiment_name is None:
+            raise ValueError("Experiment must have a name or generateName")
+
         try:
-            self.custom_api.create_namespaced_custom_object(
+            outputs = self.custom_api.create_namespaced_custom_object(
                 constants.KUBEFLOW_GROUP,
                 constants.KATIB_VERSION,
                 namespace,
                 constants.EXPERIMENT_PLURAL,
                 experiment,
             )
+            experiment_name = outputs["metadata"][
+                "name"
+            ]  # if "generate_name" is used, "name" gets a prefix from server
         except multiprocessing.TimeoutError:
             raise TimeoutError(
-                f"Timeout to create Katib Experiment: {namespace}/{experiment.metadata.name}"
+                f"Timeout to create Katib Experiment: {namespace}/{experiment_name}"
             )
-        except Exception:
+        except Exception as e:
+            if hasattr(e, "status") and e.status == 409:
+                raise Exception(
+                    f"A Katib Experiment with the name {namespace}/{experiment_name} already exists."
+                )
             raise RuntimeError(
-                f"Failed to create Katib Experiment: {namespace}/{experiment.metadata.name}"
+                f"Failed to create Katib Experiment: {namespace}/{experiment_name}"
             )
 
         # TODO (andreyvelich): Use proper logger.
-        print(f"Experiment {namespace}/{experiment.metadata.name} has been created")
+        print(f"Experiment {namespace}/{experiment_name} has been created")
 
         if self._is_ipython():
             if self.in_cluster:
                 import IPython
 
                 IPython.display.display(
                     IPython.display.HTML(
                         "Katib Experiment {} "
                         'link <a href="/_/katib/#/katib/hp_monitor/{}/{}" target="_blank">here</a>'.format(
-                            experiment.metadata.name,
+                            experiment_name,
                             namespace,
-                            experiment.metadata.name,
+                            experiment_name,
                         )
                     )
                 )
 
     def tune(
         self,
         # TODO (andreyvelich): How to be consistent with other APIs (name) ?
         name: str,
         objective: Callable,
         parameters: Dict[str, Any],
         base_image: str = constants.BASE_IMAGE_TENSORFLOW,
         namespace: Optional[str] = None,
+        env_per_trial: Optional[
+            Union[Dict[str, str], List[Union[client.V1EnvVar, client.V1EnvFromSource]]]
+        ] = None,
         algorithm_name: str = "random",
+        algorithm_settings: Union[
+            dict, List[models.V1beta1AlgorithmSetting], None
+        ] = None,
         objective_metric_name: str = None,
         additional_metric_names: List[str] = [],
         objective_type: str = "maximize",
         objective_goal: float = None,
         max_trial_count: int = None,
         parallel_trial_count: int = None,
         max_failed_trial_count: int = None,
@@ -163,15 +190,24 @@
 
                 For example: `parameters = {"lr": katib.search.double(min=0.1, max=0.2)}`
 
                 Also, you can use these parameters to define input for your
                 objective function.
             base_image: Image to use when executing the objective function.
             namespace: Namespace for the Experiment.
+            env_per_trial: Environment variable(s) to be attached to each trial container.
+                You can specify a dictionary as a mapping object representing the environment
+                variables. Otherwise, you can specify a list, in which the element can either
+                be a kubernetes.client.models.V1EnvVar (documented here:
+                https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1EnvVar.md)
+                or a kubernetes.client.models.V1EnvFromSource (documented here:
+                https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1EnvFromSource.md)
             algorithm_name: Search algorithm for the HyperParameter tuning.
+            algorithm_settings: Settings for the search algorithm given.
+                For available fields, check this doc: https://www.kubeflow.org/docs/components/katib/experiment/#search-algorithms-in-detail.
             objective_metric_name: Objective metric that Katib optimizes.
             additional_metric_names: List of metrics that Katib collects from the
                 objective function in addition to objective metric.
             objective_type: Type for the Experiment optimization for the objective metric.
                 Must be one of `minimize` or `maximize`.
             objective_goal: Objective goal that Experiment should reach to be Succeeded.
             max_trial_count: Maximum number of Trials to run. For the default
@@ -199,15 +235,15 @@
             retain_trials: Whether Trials' resources (e.g. pods) are deleted after Succeeded state.
             packages_to_install: List of Python packages to install in addition
                 to the base image packages. These packages are installed before
                 executing the objective function.
             pip_index_url: The PyPI url from which to install Python packages.
 
         Raises:
-            ValueError: Objective function has invalid arguments.
+            ValueError: Function arguments have incorrect type or value.
             TimeoutError: Timeout to create Katib Experiment.
             RuntimeError: Failed to create Katib Experiment.
         """
 
         namespace = namespace or self.namespace
 
         # Create Katib Experiment template.
@@ -224,16 +260,23 @@
             objective_metric_name=objective_metric_name,
             additional_metric_names=additional_metric_names,
         )
         if objective_goal is not None:
             experiment.spec.objective.goal = objective_goal
 
         # Add Algorithm to the Katib Experiment.
+        if isinstance(algorithm_settings, dict):
+            algorithm_settings = [
+                models.V1beta1AlgorithmSetting(name=str(k), value=str(v))
+                for k, v in algorithm_settings.items()
+            ]
+
         experiment.spec.algorithm = models.V1beta1AlgorithmSpec(
-            algorithm_name=algorithm_name
+            algorithm_name=algorithm_name,
+            algorithm_settings=algorithm_settings,
         )
 
         # Add Trial budget to the Katib Experiment.
         if max_trial_count is not None:
             experiment.spec.max_trial_count = max_trial_count
         if parallel_trial_count is not None:
             experiment.spec.parallel_trial_count = parallel_trial_count
@@ -304,14 +347,32 @@
                 resources_per_trial["nvidia.com/gpu"] = resources_per_trial.pop("gpu")
 
             resources_per_trial = client.V1ResourceRequirements(
                 requests=resources_per_trial,
                 limits=resources_per_trial,
             )
 
+        env = []
+        env_from = []
+        if isinstance(env_per_trial, dict):
+            env = [
+                client.V1EnvVar(name=str(k), value=str(v))
+                for k, v in env_per_trial.items()
+            ]
+        elif env_per_trial:
+            for x in env_per_trial:
+                if isinstance(x, client.V1EnvVar):
+                    env.append(x)
+                elif isinstance(x, client.V1EnvFromSource):
+                    env_from.append(x)
+                else:
+                    raise ValueError(
+                        f"Incorrect value for env_per_trial: {env_per_trial}"
+                    )
+
         # Create Trial specification.
         trial_spec = client.V1Job(
             api_version="batch/v1",
             kind="Job",
             spec=client.V1JobSpec(
                 template=client.V1PodTemplateSpec(
                     metadata=models.V1ObjectMeta(
@@ -321,14 +382,16 @@
                         restart_policy="Never",
                         containers=[
                             client.V1Container(
                                 name=constants.DEFAULT_PRIMARY_CONTAINER_NAME,
                                 image=base_image,
                                 command=["bash", "-c"],
                                 args=[exec_script],
+                                env=env,
+                                env_from=env_from,
                                 resources=resources_per_trial,
                             )
                         ],
                     ),
                 )
             ),
         )
@@ -1108,17 +1171,17 @@
                     and len(trial.status.conditions) > 0
                 ):
                     if utils.has_condition(
                         trial.status.conditions, constants.TRIAL_CONDITION_SUCCEEDED
                     ):
                         output = {}
                         output["name"] = trial.metadata.name
-                        output[
-                            "parameter_assignments"
-                        ] = trial.spec.parameter_assignments
+                        output["parameter_assignments"] = (
+                            trial.spec.parameter_assignments
+                        )
                         output["metrics"] = trial.status.observation.metrics
                         result.append(output)
         except multiprocessing.TimeoutError:
             raise TimeoutError(
                 f"Timeout to list Katib Trials in namespace: {namespace}"
             )
         except Exception:
```

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/api/search.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/api/search.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/api_client.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/api_client.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/configuration.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/configuration.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/constants/constants.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,11 +48,11 @@
 # Trial conditions.
 TRIAL_CONDITION_SUCCEEDED = "Succeeded"
 
 # Supported base images for the Katib Trials.
 # TODO (andreyvelich): Implement list_base_images function to get each image description.
 BASE_IMAGE_TENSORFLOW = "docker.io/tensorflow/tensorflow:2.13.0"
 BASE_IMAGE_TENSORFLOW_GPU = "docker.io/tensorflow/tensorflow:2.13.0-gpu"
-BASE_IMAGE_PYTORCH = "docker.io/pytorch/pytorch:1.12.1-cuda11.3-cudnn8-runtime"
+BASE_IMAGE_PYTORCH = "docker.io/pytorch/pytorch:2.2.1-cuda12.1-cudnn8-runtime"
 BASE_IMAGE_MXNET = "docker.io/mxnet/python:1.9.1_native_py3"
 
 DEFAULT_DB_MANAGER_ADDRESS = "katib-db-manager.kubeflow:6789"
```

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/exceptions.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/exceptions.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/katib_api_pb2.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/katib_api_pb2.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/__init__.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_algorithm_setting.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_algorithm_setting.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_algorithm_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_algorithm_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_collector_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_collector_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_config_map_source.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_config_map_source.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_early_stopping_rule.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_early_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_early_stopping_setting.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_early_stopping_setting.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_early_stopping_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_early_stopping_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_condition.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_condition.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_list.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_list.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_experiment_status.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_experiment_status.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_feasible_space.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_feasible_space.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_file_system_path.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_file_system_path.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_filter_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_filter_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_graph_config.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_graph_config.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_metric.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_metric.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_metric_strategy.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_metric_strategy.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_metrics_collector_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_metrics_collector_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_nas_config.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_nas_config.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_objective_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_objective_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_observation.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_observation.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_operation.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_operation.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_optimal_trial.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_optimal_trial.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_parameter_assignment.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_parameter_assignment.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_parameter_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_parameter_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_source_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_source_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_condition.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_condition.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_list.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_list.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_suggestion_status.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_suggestion_status.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_assignment.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_assignment.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_condition.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_condition.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_list.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_list.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_parameter_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_parameter_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_source.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_source.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_spec.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_spec.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_status.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_status.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/models/v1beta1_trial_template.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/models/v1beta1_trial_template.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/rest.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/rest.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow/katib/utils/utils.py` & `kubeflow-katib-0.17.0rc0/kubeflow/katib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/PKG-INFO` & `kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kubeflow-katib
-Version: 0.16.0rc1
+Version: 0.17.0rc0
 Summary: Katib Python SDK for APIVersion v1beta1
 Home-page: https://github.com/kubeflow/katib/tree/master/sdk/python/v1beta1
 Author: Kubeflow Authors
 Author-email: premnath.vel@gmail.com
 License: Apache License Version 2.0
 Description: Katib Python SDK for APIVersion v1beta1
 Platform: UNKNOWN
```

### Comparing `kubeflow-katib-0.16.0rc1/kubeflow_katib.egg-info/SOURCES.txt` & `kubeflow-katib-0.17.0rc0/kubeflow_katib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubeflow-katib-0.16.0rc1/setup.py` & `kubeflow-katib-0.17.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,32 @@
 import setuptools
 
 REQUIRES = [
     "certifi>=14.05.14",
     "six>=1.10",
     "setuptools>=21.0.0",
     "urllib3>=1.15.1",
-    "kubernetes>=23.6.0",
+    "kubernetes>=27.2.0",
     "grpcio>=1.41.1",
     "protobuf>=3.19.5, <=3.20.3",
 ]
 
 katib_grpc_api_file = "../../../pkg/apis/manager/v1beta1/python/api_pb2.py"
 
 # Copy Katib gRPC Python APIs to use it in the Katib SDK Client.
 # We need to always copy this file only on the SDK building stage, not on SDK installation stage.
 if os.path.exists(katib_grpc_api_file):
     shutil.copy(
-        katib_grpc_api_file, "kubeflow/katib/katib_api_pb2.py",
+        katib_grpc_api_file,
+        "kubeflow/katib/katib_api_pb2.py",
     )
 
 setuptools.setup(
     name="kubeflow-katib",
-    version="0.16.0rc1",
+    version="0.17.0rc0",
     author="Kubeflow Authors",
     author_email="premnath.vel@gmail.com",
     license="Apache License Version 2.0",
     url="https://github.com/kubeflow/katib/tree/master/sdk/python/v1beta1",
     description="Katib Python SDK for APIVersion v1beta1",
     long_description="Katib Python SDK for APIVersion v1beta1",
     packages=setuptools.find_packages(include=("kubeflow*")),
```

