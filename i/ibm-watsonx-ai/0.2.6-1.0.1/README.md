# Comparing `tmp/ibm_watsonx_ai-0.2.6.tar.gz` & `tmp/ibm_watsonx_ai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm_watsonx_ai-0.2.6.tar", last modified: Thu Apr 11 15:28:11 2024, max compression
+gzip compressed data, was "ibm_watsonx_ai-1.0.1.tar", last modified: Fri Apr 26 14:36:06 2024, max compression
```

## Comparing `ibm_watsonx_ai-0.2.6.tar` & `ibm_watsonx_ai-1.0.1.tar`

### file list

```diff
@@ -1,747 +1,744 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.455202 ibm_watsonx_ai-0.2.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    26463 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     7938 2024-04-11 15:28:11.455202 ibm_watsonx_ai-0.2.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/VERSION
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.835202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/Set.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      765 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/_wrappers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/_wrappers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9609 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/_wrappers/requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      633 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/assets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2077 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      658 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/connections.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/datasets/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/datasets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13929 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/datasets/experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2199 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/experiment.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25284 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/base_deployment.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    26283 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/batch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11915 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/web_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      550 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployments.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40208 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/autoai.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.839202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/
--rw-rw-r--   0 travis    (2000) travis    (2000)      429 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1802 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/base_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    66019 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/service_engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67201 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/wml_engine.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.843202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/base_auto_pipelines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27294 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/local_auto_pipelines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41424 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/remote_auto_pipelines.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.843202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      460 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21268 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/auto_pipelines_runs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1409 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/base_auto_pipelines_runs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8097 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/local_auto_pipelines_runs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.843202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/base_experiment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/base_experiment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/base_experiment/base_experiment.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.843202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/fm_tune/
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/fm_tune/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11200 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/fm_tune/tune_experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6555 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/fm_tune/tune_runs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      651 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/export_assets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      507 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/factsheets.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.843202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/federated_learning/
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/federated_learning/FLExceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/federated_learning/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      555 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/federated_learning/data_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/federated_learning/data_util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.843202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/embeddings/
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/embeddings/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1940 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/embeddings/base_embeddings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12018 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/embeddings/embeddings.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/extensions/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/extensions/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/extensions/langchain/
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/extensions/langchain/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3698 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/extensions/langchain/llm.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14983 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/base_model_inference.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12055 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/deployment_model_inference.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11335 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/fm_model_inference.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18932 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/model_inference.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12469 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27302 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/prompt_tuner.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/prompts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/prompts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32591 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/prompts/prompt_template.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      754 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18780 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      504 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.847202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      555 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      549 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/base_connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52369 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/base_data_connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      599 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/base_location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76205 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/connections.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65632 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/flight_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/local.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2340 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/hpo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27789 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/href_definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      637 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/hw_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/import_assets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/instance_new_plan.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cloud/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cloud/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cloud/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cloud/ibmfl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cloud/ibmfl/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.851202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2449 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/route_declarations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17919 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/websockets_connection.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.855202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7961 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14762 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.855202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25835 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/pytorch_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23131 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/tensorflow_fl_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.855202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17962 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/xgb_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17444 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/xgb_fl_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.855202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5937 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/metrics_recorder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14847 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12607 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party_protocol_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1324 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/fedavg_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10608 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1940 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/pfnm_local_training_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18932 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/xgboost_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18034 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/xgboost_local_training_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19474 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9831 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12423 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/matching.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3009 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4092 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/hyperparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      758 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.871202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.875202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17965 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/websockets_connection.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.875202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.875202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8529 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/metrics_recorder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15121 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12218 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party_protocol_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.899202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20561 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.903202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/party/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2442 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/party_env_validator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.903202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.903202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.903202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2982 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/route_declarations.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.903202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      872 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_enumeration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      705 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9731 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_library.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.907202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17261 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/fhe.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.931202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6533 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      740 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      878 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_int.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.931202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      823 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14383 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.931202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1009 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/message_type.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.935202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30886 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/pytorch_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29774 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/tensorflow_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17862 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/xgb_fl_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.935202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16342 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13787 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party_protocol_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.935202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10617 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/crypto_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13384 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2168 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/pfnm_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29004 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/xgboost_local_training_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.935202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.959202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8063 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/hyperparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.959202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.959202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.959202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2982 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/route_declarations.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.963202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      872 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_enumeration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      705 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9731 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_library.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.963202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17261 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/fhe.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.987202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6533 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      740 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      878 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_int.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.987202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      823 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14383 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.987202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1009 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/message_type.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.987202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30886 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/pytorch_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29774 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/tensorflow_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17862 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/xgb_fl_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.987202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16342 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13787 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party_protocol_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.991202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10617 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/crypto_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13384 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2168 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/pfnm_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29004 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/xgboost_local_training_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.015202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.015202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8063 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/hyperparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.015202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.015202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.019202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2927 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/route_declarations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/router_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20803 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/websockets_connection.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.023202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8190 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15000 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      954 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_data_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1980 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/pandas_data_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/envs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.055202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/json_serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3731 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      901 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1552 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/pickle_serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      948 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1341 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer_factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      412 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer_types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.059202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9276 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2451 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/model_update.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7701 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/naive_bayes_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27487 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/pytorch_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16560 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_SGD_linear_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6960 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9187 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_kmeans_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25212 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/tensorflow_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17962 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/xgb_fl_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.059202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.059202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8530 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/metrics_recorder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15612 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12198 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party_protocol_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      515 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/status_type.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.063202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/fedavg_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12661 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2048 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/pfnm_local_training_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20446 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/xgboost_local_training_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.099202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20640 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7885 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/fl_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5484 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/log_config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.099202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9831 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12423 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/matching.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3009 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.099202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7757 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/hyperparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      758 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.099202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.099202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.103202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28686 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/pytorch_fl_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17964 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/xgb_fl_model.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.103202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.103202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21427 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/xgboost_local_training_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.103202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.103202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4221 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/hyperparams.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.139202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1642 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/edge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5521 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/javaproxy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10420 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/mlpipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/serialization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      648 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/mlpipelinepy/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.139202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11831 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/DAG.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13967 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/IBMSparkPipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6010 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/IBMSparkPipelineModel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/Result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2186 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/Sink.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2220 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/Source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10916 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/Wrapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/pipeline/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.143202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5768 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/TestRepoSaveLoad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/base_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3155 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/ml_api_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6936 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/ml_authorization.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.147202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      623 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/artifact_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      829 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      859 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_pipeline_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      797 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/hybrid_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11171 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/meta_names.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/meta_props.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      736 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/pipeline_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/scikit_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      814 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/tensorflow_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      759 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_experiment_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_function_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      754 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_libraries_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      753 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_runtimes_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      800 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/xgboost_model_artifact.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.219202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2456 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6340 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/content_loaders.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/experiment_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1625 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      838 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      836 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6123 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4485 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      892 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3331 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1655 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      830 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      637 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19342 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/ml_repository_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/python_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2548 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1698 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      835 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2236 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15122 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1157 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2841 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2561 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10874 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2196 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      851 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9805 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1995 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6113 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/version_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2693 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/xgboost_model_reader.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.223202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2485 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/content_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6393 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17498 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5963 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14711 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9550 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10656 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4736 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14715 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44340 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2600 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9728 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_adapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22031 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_collection.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.223202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11676 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22137 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/api_client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.243202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/apis/
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/apis/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   258565 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/apis/repository_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11443 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/apis/token_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8770 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/configuration.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.395202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11010 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_data_input_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4520 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_metrics_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4538 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4502 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_version_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3119 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_training_output_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2939 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_author.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4140 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4079 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3500 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_short_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/author_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2851 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/author_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3540 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5834 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3430 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_meta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4981 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3492 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/cols_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3548 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/compute_configuration_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_source_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_target_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4622 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_with_name_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4260 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/content_location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3936 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/content_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2337 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/custom_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3854 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/deploy_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3509 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_bad_request_libraries_target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4655 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3440 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments_target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4615 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4557 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3397 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository_target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3551 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3688 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3730 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4060 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4753 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6669 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5829 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input_settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2903 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array_first.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2367 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8209 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_status_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5724 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3593 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_libraries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3581 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_runtimes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4764 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6739 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5018 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5018 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4946 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4262 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4946 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3808 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4050 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4206 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5398 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2367 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/input_data_schema.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3688 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_input_batch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_output_batch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4113 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5457 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3611 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input_platform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2942 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4898 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4781 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_functions_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7380 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3022 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7694 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/metric_object_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/metrics_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6527 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3701 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3154 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8107 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_function_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3654 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5173 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2971 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5173 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2971 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19747 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3088 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3741 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3713 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5227 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2983 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2167 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_model_size_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3574 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_function.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2387 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3695 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3102 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4925 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5411 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_content_location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2835 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_definition_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9767 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3642 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3534 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics_values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3525 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11672 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3754 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3850 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_training_data_ref.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3968 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3656 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_metrics_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8696 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3606 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3562 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/online_deploy_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3502 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3040 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2345 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/output_data_schema.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4916 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4857 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4857 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_libraries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4893 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_runtime_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5723 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3335 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3564 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6715 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3303 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3655 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3694 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2373 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_environment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3493 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_output_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6179 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4498 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2953 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/sample_scoring_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5174 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2988 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/score_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2888 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/score_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3797 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/size_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2834 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/software_spec_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3313 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/space_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3715 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/spark_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3830 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_input_internal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5067 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_internal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3502 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3002 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3900 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_internal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3494 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/tag_repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2911 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/token_response.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2366 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_data_schema.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3665 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_output_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7857 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_reference_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13762 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3131 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8967 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/rest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.395202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/base_singleton.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/compression_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      486 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/file_system_ops.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      936 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/generic_archive_file_check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/json_2_object_mapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3942 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/library_imports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2459 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/spark_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/unique_id_gen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/lifecycle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.399202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      389 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/globalization_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1959 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9581 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/messages_en.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12009 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/metanames.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      750 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/migration_v4ga_cloud.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/model_definition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12431 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/parameter_sets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      749 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/party_wrapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      644 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/pipelines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      668 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/pkg_extn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      805 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/platform_spaces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/remote_training_system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1060 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/repository.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      637 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      629 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/shiny.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      648 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/sw_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2024-04-11 15:26:20.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/task_credentials.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/training.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.415202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/API_VERSION_PARAM
--rw-rw-r--   0 travis    (2000) travis    (2000)      361 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8477 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12958 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19181 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5633 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/fairness.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3242 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/incremental.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3151 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/local_training_message_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2089 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/progress_bar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1677 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/training.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102291 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1155 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/watson_studio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2602 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/change_methods_docstring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2895 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/cpd_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/deployment/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3381 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/deployment/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      533 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24661 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      498 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/volumes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2589 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/wml_client_error.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      475 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/wml_resource.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/workspace/
--rw-rw-r--   0 travis    (2000) travis    (2000)      330 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/workspace/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7493 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/workspace/workspace.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     7938 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    41469 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibmfl/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibmfl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibmfl/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibmfl/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      882 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibmfl/data/data_handler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:11.419202 ibm_watsonx_ai-0.2.6/ibmfl/party/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-11 15:28:10.000000 ibm_watsonx_ai-0.2.6/ibmfl/party/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      519 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibmfl/party/party.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/ibmfl/party_env_validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2024-04-11 15:28:11.459202 ibm_watsonx_ai-0.2.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     5851 2024-04-11 15:26:22.000000 ibm_watsonx_ai-0.2.6/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.039183 ibm_watsonx_ai-1.0.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28253 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     5543 2024-04-26 14:36:06.039183 ibm_watsonx_ai-1.0.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/VERSION
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.575183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7171 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/Set.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      638 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.575183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/_wrappers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/_wrappers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10211 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/_wrappers/requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23127 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/assets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25063 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29362 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/connections.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7418 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/credentials.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/datasets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/datasets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15219 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/datasets/experiment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2384 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/experiment.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29438 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/base_deployment.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    27738 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/batch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12338 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/web_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70934 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployments.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      409 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40123 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/autoai.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      429 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1802 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/base_engine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66026 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/service_engine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67208 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/wml_engine.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/base_auto_pipelines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27294 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/local_auto_pipelines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41484 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/remote_auto_pipelines.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      460 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21264 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/auto_pipelines_runs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1409 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/base_auto_pipelines_runs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8097 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/local_auto_pipelines_runs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/base_experiment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      358 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/base_experiment/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/base_experiment/base_experiment.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.579183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/fm_tune/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/fm_tune/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11119 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/fm_tune/tune_experiment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6554 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/fm_tune/tune_runs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17177 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18791 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/export_assets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8099 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/factsheets.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/federated_learning/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/federated_learning/FLExceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/federated_learning/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8243 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/federated_learning/data_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15305 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/federated_learning/data_util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/base_embeddings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12001 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/embeddings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/sentence_transformer_embeddings.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/langchain/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      301 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/langchain/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3708 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/langchain/llm.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      380 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/pattern/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      326 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/pattern/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/pattern/default_deployable_function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22689 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/pattern/pattern.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      332 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2842 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/utils/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      602 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/base_vector_store.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6581 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/langchain_vector_store_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10819 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/vector_store.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9950 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/vector_store_connector.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.583183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14835 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/base_model_inference.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12767 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/deployment_model_inference.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11699 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/fm_model_inference.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19013 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/model_inference.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12095 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29212 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/prompt_tuner.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/prompts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/prompts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34441 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/prompts/prompt_template.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      665 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2463 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/utils/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23263 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/utils/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9928 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33462 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      555 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      549 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/base_connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52198 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/base_data_connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      599 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/base_location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76174 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/connections.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65669 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/flight_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/local.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2340 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5023 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/hpo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29553 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/href_definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11653 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/hw_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12335 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/import_assets.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cloud/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cloud/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cloud/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cloud/ibmfl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cloud/ibmfl/_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.587183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2449 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/route_declarations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17919 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/websockets_connection.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7961 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14762 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25835 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/pytorch_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23131 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/tensorflow_fl_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17962 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/xgb_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17444 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/xgb_fl_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.603183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5937 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/metrics_recorder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14847 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12607 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party_protocol_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.607183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1324 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/fedavg_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10608 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1940 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/pfnm_local_training_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.635183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18932 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/xgboost_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18034 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/xgboost_local_training_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.635183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19474 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.639183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9831 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12423 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/matching.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3009 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.639183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4092 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/hyperparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      758 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.639183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.639183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.643183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17965 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/websockets_connection.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.643183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.643183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8529 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/metrics_recorder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15121 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12218 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party_protocol_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.643183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20561 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.643183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      271 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/party/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      563 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2442 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/party_env_validator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.643183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.647184 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.647184 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2982 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/route_declarations.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.667183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      872 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_enumeration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      705 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9731 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_library.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.667183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17261 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/fhe.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.671183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6533 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      740 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      878 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_int.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.691183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      823 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14383 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.691183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1009 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/message_type.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.695183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30886 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/pytorch_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29774 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/tensorflow_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17862 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/xgb_fl_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.695183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16342 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13787 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party_protocol_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.695183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10617 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/crypto_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13384 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2168 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/pfnm_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29004 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/xgboost_local_training_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.695183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.699183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8063 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/hyperparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.699183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.715183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.715183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2982 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/route_declarations.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.715183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      872 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_enumeration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      705 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9731 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_library.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.715183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17261 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/fhe.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.719183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6533 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      740 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      878 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1235 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_int.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.735183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      823 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14383 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.739183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1009 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/message_type.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.739183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30886 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/pytorch_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29774 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/tensorflow_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17862 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/xgb_fl_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.739183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16342 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13787 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party_protocol_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.743183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10617 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/crypto_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13384 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2168 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/pfnm_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29004 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/xgboost_local_training_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.743183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.743183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8063 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/hyperparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.743183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.763183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.763183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2927 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/route_declarations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/router_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20803 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/websockets_connection.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.767183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8190 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15000 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      954 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_data_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1980 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/pandas_data_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/envs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.771183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/json_serializer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3731 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      901 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1552 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/pickle_serializer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      948 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1341 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer_factory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      412 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer_types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.795184 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9276 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2451 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/model_update.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7701 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/naive_bayes_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27487 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/pytorch_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16560 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_SGD_linear_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6960 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9187 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_kmeans_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25212 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/tensorflow_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17962 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/xgb_fl_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.799183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.799183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8530 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/metrics_recorder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15612 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12198 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party_protocol_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      515 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/status_type.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.799183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/fedavg_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12661 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2048 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/pfnm_local_training_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20446 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/xgboost_local_training_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.803183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20640 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7885 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/fl_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5484 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/log_config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.803183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9831 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12423 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/matching.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3009 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4090 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7757 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/hyperparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      758 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28686 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/pytorch_fl_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17964 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/xgb_fl_model.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21427 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/xgboost_local_training_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.815183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.819183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4221 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/hyperparams.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.819183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5756 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/TestRepoSaveLoad.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/base_constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3155 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/ml_api_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6936 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/ml_authorization.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.835183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      623 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/artifact_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      829 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      859 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_pipeline_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      797 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/hybrid_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11171 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/meta_names.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/meta_props.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      736 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/pipeline_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      962 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/scikit_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      814 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/tensorflow_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      759 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_experiment_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_function_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      754 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_libraries_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      753 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_runtimes_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      800 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/xgboost_model_artifact.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.855183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2456 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6340 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/content_loaders.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/experiment_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1625 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      838 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      836 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6123 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1329 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1123 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4485 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      892 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3331 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1655 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      830 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      637 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19342 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/ml_repository_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/python_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2548 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1698 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      835 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2236 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15122 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1157 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2841 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2561 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      579 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10874 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2196 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      851 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9805 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1995 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6113 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/version_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2693 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/xgboost_model_reader.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.871183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2485 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/content_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6393 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17498 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5963 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14711 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9550 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10656 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4736 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14715 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44340 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2600 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9728 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22031 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_collection.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.875183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11676 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22137 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/api_client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.875183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/apis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/apis/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   258565 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/apis/repository_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11443 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/apis/token_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8770 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/configuration.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:05.987183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11010 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_data_input_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4520 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_metrics_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4538 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4502 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_version_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3119 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_training_output_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2939 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_author.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4140 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4079 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3500 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_short_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/author_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2851 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/author_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3540 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5834 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3430 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_meta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4981 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3492 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2993 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/cols_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3548 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/compute_configuration_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_source_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_target_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4622 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_with_name_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4260 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/content_location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3936 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/content_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2337 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/custom_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3854 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/deploy_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3509 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_bad_request_libraries_target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4655 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3440 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments_target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4615 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4557 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3397 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository_target.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3551 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3688 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3730 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4060 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4753 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6669 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5829 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input_settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3624 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2903 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array_first.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2367 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8209 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_status_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5724 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3593 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_libraries.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3581 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_runtimes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4764 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6739 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5018 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5018 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4946 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4262 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4946 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3808 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4050 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4206 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5398 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2367 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/input_data_schema.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3688 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_input_batch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_output_batch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4113 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5457 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3611 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input_platform.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2942 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4898 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4781 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_functions_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7380 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3022 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7694 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/metric_object_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/metrics_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6527 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3701 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3154 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8107 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_function_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3654 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5173 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2971 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3691 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5173 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2971 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19747 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3088 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3741 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3713 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5227 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2983 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2167 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_model_size_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3574 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2387 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3695 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3102 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4925 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5411 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_content_location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2835 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_definition_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9767 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3642 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3534 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics_values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3525 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11672 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3754 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_schemas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3850 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_training_data_ref.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3968 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3656 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_metrics_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8696 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3606 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3562 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/online_deploy_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3502 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3040 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2345 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/output_data_schema.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4916 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4857 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4857 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_libraries.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4893 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_runtime_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5723 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3335 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3564 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6715 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3303 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3655 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3694 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2373 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_environment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3493 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_output_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6179 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3085 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4498 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2953 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/sample_scoring_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5174 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/schemas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2988 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/score_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2888 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/score_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3797 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/size_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2834 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/software_spec_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3313 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/space_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3715 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/spark_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3830 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_input_internal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5067 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_internal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3502 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3002 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3900 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_internal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3494 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/tag_repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2911 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/token_response.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2366 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_data_schema.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3665 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_output_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7857 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_reference_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13762 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3131 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8967 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/rest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.015183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/base_singleton.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/compression_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      486 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/file_system_ops.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      936 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/generic_archive_file_check.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/json_2_object_mapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3942 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/library_imports.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2459 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/spark_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      464 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/unique_id_gen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      569 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/lifecycle.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      390 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/globalization_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2096 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9555 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/messages_en.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88799 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/metanames.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37934 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/model_definition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   140580 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12707 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/parameter_sets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25727 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/party_wrapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23763 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/pipelines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18435 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/pkg_extn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19099 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/remote_training_system.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35116 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/repository.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40561 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16117 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/service_instance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32305 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/shiny.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30684 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/spaces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19653 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/sw_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8059 2024-04-26 14:34:07.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/task_credentials.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44682 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/training.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/API_VERSION_PARAM
+-rw-rw-r--   0 travis    (2000) travis    (2000)      361 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8509 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/connection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12958 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18531 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5633 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/fairness.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3242 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/incremental.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3151 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/local_training_message_handler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2089 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/progress_bar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1677 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/training.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102371 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3229 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/cpd_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/deployment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/deployment/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3975 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/deployment/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      533 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27199 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18441 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/volumes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11206 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/wml_client_error.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23905 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/wml_resource.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/workspace/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      330 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/workspace/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7964 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/workspace/workspace.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.023183 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     5543 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41613 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2024-04-26 14:36:05.000000 ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibmfl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibmfl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.019183 ibm_watsonx_ai-1.0.1/ibmfl/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibmfl/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      882 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibmfl/data/data_handler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:06.023183 ibm_watsonx_ai-1.0.1/ibmfl/party/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-26 14:36:04.000000 ibm_watsonx_ai-1.0.1/ibmfl/party/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      519 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibmfl/party/party.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/ibmfl/party_env_validator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2024-04-26 14:36:06.039183 ibm_watsonx_ai-1.0.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4629 2024-04-26 14:34:08.000000 ibm_watsonx_ai-1.0.1/setup.py
```

### Comparing `ibm_watsonx_ai-0.2.6/LICENSE.txt` & `ibm_watsonx_ai-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/MANIFEST.in` & `ibm_watsonx_ai-1.0.1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 include VERSION
 include ibm_watsonx_ai/messages/messages_en.json
 include ibm_watsonx_ai/utils/API_VERSION_PARAM
 exclude ibm_watsonx_ai/tests/__init__.py
 exclude ibm_watsonx_ai/tests/config.ini.enc
 exclude ibm_watsonx_ai/tests/conftest.py
 exclude ibm_watsonx_ai/tests/install_requirements.py
+exclude ibm_watsonx_ai/tests/pytest.ini
 exclude ibm_watsonx_ai/tests/requirements.txt
 exclude ibm_watsonx_ai/tests/run_base.py
 exclude ibm_watsonx_ai/tests/autoai/HOW_TO.md
 exclude ibm_watsonx_ai/tests/autoai/__init__.py
 exclude ibm_watsonx_ai/tests/autoai/requirements-RT22.2.txt
 exclude ibm_watsonx_ai/tests/autoai/requirements-RT23.1.txt
+exclude ibm_watsonx_ai/tests/autoai/requirements-RT24.1.txt
 exclude ibm_watsonx_ai/tests/autoai/requirements.linux-s390x.pypi.txt
 exclude ibm_watsonx_ai/tests/autoai/requirements.linux-s390x.txt
 exclude ibm_watsonx_ai/tests/autoai/abstract_tests_classes/__init__.py
 exclude ibm_watsonx_ai/tests/autoai/abstract_tests_classes/abstract_autoai_data_subsampling_iterator_batched.py
 exclude ibm_watsonx_ai/tests/autoai/abstract_tests_classes/abstract_autoai_test.py
 exclude ibm_watsonx_ai/tests/autoai/abstract_tests_classes/abstract_deployment_batch.py
 exclude ibm_watsonx_ai/tests/autoai/abstract_tests_classes/abstract_deployment_webservice.py
@@ -128,14 +130,15 @@
 exclude ibm_watsonx_ai/tests/autoai/data/xlsx/insurance.xlsx
 exclude ibm_watsonx_ai/tests/autoai/data/xlsx/insurance_credit_risk__two_sheets.xlsx
 exclude ibm_watsonx_ai/tests/autoai/data/xlsx/iris_dataset.xlsx
 exclude ibm_watsonx_ai/tests/autoai/db_driver_jars/db2jcc4-4.23.42.jar
 exclude ibm_watsonx_ai/tests/autoai/db_driver_jars/exajdbc-7.1.4.jar
 exclude ibm_watsonx_ai/tests/autoai/db_driver_jars/postgresql-42.2.26.jre7.jar
 exclude ibm_watsonx_ai/tests/autoai/fvt/__init__.py
+exclude ibm_watsonx_ai/tests/autoai/fvt/test_auth.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_binary_bank_xlsx_cda_ca_WebService.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_binary_breastcancer_batched_da_default_WebService.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_binary_breastcancer_uft16_da_default_WebService.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_binary_creditrisk_ca_ca_WebService_Batch.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_binary_makeclass_batched_da_default_WebService.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_forecasting_fooddemand_exogenous_cda_default_WebService.py
 exclude ibm_watsonx_ai/tests/autoai/fvt/test_autoai_forecasting_storeitemdemand_imputation_cda_default_WebService.py
@@ -311,26 +314,47 @@
 exclude ibm_watsonx_ai/tests/deployment/unit/test_web_service.py
 exclude ibm_watsonx_ai/tests/foundation_models/__init__.py
 exclude ibm_watsonx_ai/tests/foundation_models/requirements.txt
 exclude ibm_watsonx_ai/tests/foundation_models/abstract_tests_classes/__init__.py
 exclude ibm_watsonx_ai/tests/foundation_models/abstract_tests_classes/abstract_prompt_tuning_test.py
 exclude ibm_watsonx_ai/tests/foundation_models/artifacts/state_of_the_union.txt
 exclude ibm_watsonx_ai/tests/foundation_models/contract/api/test_embeddings_endpoint.py
+exclude ibm_watsonx_ai/tests/foundation_models/data/IBM_wikipedia.txt
 exclude ibm_watsonx_ai/tests/foundation_models/data/file_to_tune1.json
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/__init__.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/__init__.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/pattern/__init__.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/pattern/conftest.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/pattern/test_rag_pattern.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/test_classes/__init__.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/test_classes/debug_embeddings.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/vector_store/__init__.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/vector_store/conftest.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/vector_store/test_vectorstore.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/vector_store/test_vectorstore_connector.py
+exclude ibm_watsonx_ai/tests/foundation_models/extensions/rag/vector_store/test_vectorstore_elasticsearch.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/__init__.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/conftest.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_embeddings.py
+exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_foundation_models.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_langchain.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_model_hap_pii.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_model_hap_pii_deployment.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_model_init.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_prompt_template.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_prompt_template_deployment.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_prompt_template_e2e.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_prompt_tuning_c_default.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_prompt_tuning_ca_default.py
 exclude ibm_watsonx_ai/tests/foundation_models/fvt/test_prompt_tuning_da_default.py
+exclude ibm_watsonx_ai/tests/unit/__init__.py
+exclude ibm_watsonx_ai/tests/unit/conftest.py
+exclude ibm_watsonx_ai/tests/unit/test_connections.py
+exclude ibm_watsonx_ai/tests/unit/foundation_models/__init__.py
+exclude ibm_watsonx_ai/tests/unit/foundation_models/test_custom_model.py
+exclude ibm_watsonx_ai/tests/unit/foundation_models/test_embeddings.py
+exclude ibm_watsonx_ai/tests/unit/foundation_models/test_prompt_tuner.py
 exclude ibm_watsonx_ai/tests/utils/__init__.py
 exclude ibm_watsonx_ai/tests/utils/assertions.py
 exclude ibm_watsonx_ai/tests/utils/cleanup.py
 exclude ibm_watsonx_ai/tests/utils/profiling.py
 exclude ibm_watsonx_ai/tests/utils/utils.py
```

### Comparing `ibm_watsonx_ai-0.2.6/README.md` & `ibm_watsonx_ai-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/_wrappers/requests.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/_wrappers/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,65 +5,81 @@
 
 import os
 import requests
 import json as js
 from requests import packages, exceptions
 from functools import wraps
 
-verify = os.environ.get('WX_CLIENT_VERIFY_REQUESTS')
+verify = os.environ.get("WX_CLIENT_VERIFY_REQUESTS")
+additional_settings = {}
+
 
 def set_verify_for_requests(func):
     @wraps(func)
     def wrapper(*args, **kw):
         global verify
 
         if verify is not None:
-            if verify == 'True':
-                kw.update({'verify': True})
+            if verify == "True":
+                kw.update({"verify": True})
 
-            elif verify == 'False':
-                kw.update({'verify': False})
+            elif verify == "False":
+                kw.update({"verify": False})
 
             else:
-                kw.update({'verify': verify})
+                kw.update({"verify": verify})
 
         else:
-            kw.update({'verify': True})
+            kw.update({"verify": True})
 
         try:
             res = func(*args, **kw)
 
         except OSError as e:
 
             # User can pass verify the path to a CA_BUNDLE file or directory with certificates of trusted CAs
             if isinstance(verify, str):
-                raise OSError(f"Connection cannot be verified with default trusted CAs. "
-                              f"Please provide correct path to a CA_BUNDLE file or directory with "
-                              f"certificates of trusted CAs. Error: {e}")
+                raise OSError(
+                    f"Connection cannot be verified with default trusted CAs. "
+                    f"Please provide correct path to a CA_BUNDLE file or directory with "
+                    f"certificates of trusted CAs. Error: {e}"
+                )
 
             # forced verify to True
             elif verify:
                 raise e
 
             # default
             elif verify is None:
-                verify = 'False'
-                kw.update({'verify': False})
+                verify = "False"
+                kw.update({"verify": False})
                 res = func(*args, **kw)
 
             # disabled verify
             else:
                 raise e
 
         return res
 
     return wrapper
 
 
+def set_additional_settings_for_requests(func):
+    @wraps(func)
+    def wrapper(*args, **kw):
+        kwargs = {}
+        kwargs.update(additional_settings)
+        kwargs.update(kw)
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def get(url, params=None, **kwargs):
     r"""Sends a GET request.
 
     :param url: URL for the new :class:`Request` object.
     :param params: (optional) Dictionary, list of tuples or bytes to send
         in the query string for the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
@@ -71,27 +87,29 @@
     :rtype: requests.Response
     """
 
     return requests.get(url=url, params=params, **kwargs)
 
 
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def options(url, **kwargs):
     r"""Sends an OPTIONS request.
 
     :param url: URL for the new :class:`Request` object.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
 
     return requests.options(url=url, **kwargs)
 
 
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def head(url, **kwargs):
     r"""Sends a HEAD request.
 
     :param url: URL for the new :class:`Request` object.
     :param \*\*kwargs: Optional arguments that ``request`` takes. If
         `allow_redirects` is not provided, it will be set to `False` (as
         opposed to the default :meth:`request` behavior).
@@ -99,91 +117,99 @@
     :rtype: requests.Response
     """
 
     return requests.head(url=url, **kwargs)
 
 
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def post(url, data=None, json=None, **kwargs):
     r"""Sends a POST request.
 
     :param url: URL for the new :class:`Request` object.
     :param data: (optional) Dictionary, list of tuples, bytes, or file-like
         object to send in the body of the :class:`Request`.
     :param json: (optional) json data to send in the body of the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
     from ibm_watsonx_ai.utils.utils import NumpyTypeEncoder
+
     if json is not None and data is None:
         data = js.dumps(json, cls=NumpyTypeEncoder)
 
-        if kwargs.get('headers') and not kwargs.get('headers', {}).get('Content-Type'):
-            kwargs['headers']["Content-Type"] =  "application/json"
+        if kwargs.get("headers") and not kwargs.get("headers", {}).get("Content-Type"):
+            kwargs["headers"]["Content-Type"] = "application/json"
 
     return requests.post(url=url, data=data, **kwargs)
 
 
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def put(url, data=None, **kwargs):
     r"""Sends a PUT request.
 
     :param url: URL for the new :class:`Request` object.
     :param data: (optional) Dictionary, list of tuples, bytes, or file-like
         object to send in the body of the :class:`Request`.
     :param json: (optional) json data to send in the body of the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
     from ibm_watsonx_ai.utils.utils import NumpyTypeEncoder
-    if (json:=kwargs.get('json')) is not None and data is None:
+
+    if (json := kwargs.get("json")) is not None and data is None:
         data = js.dumps(json, cls=NumpyTypeEncoder)
 
-        if kwargs.get('headers') and not kwargs.get('headers', {}).get('Content-Type'):
-            kwargs['headers']["Content-Type"] =  "application/json"
+        if kwargs.get("headers") and not kwargs.get("headers", {}).get("Content-Type"):
+            kwargs["headers"]["Content-Type"] = "application/json"
 
     return requests.put(url=url, data=data, **kwargs)
 
 
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def patch(url, data=None, **kwargs):
     r"""Sends a PATCH request.
 
     :param url: URL for the new :class:`Request` object.
     :param data: (optional) Dictionary, list of tuples, bytes, or file-like
         object to send in the body of the :class:`Request`.
     :param json: (optional) json data to send in the body of the :class:`Request`.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
     from ibm_watsonx_ai.utils.utils import NumpyTypeEncoder
-    if (json:=kwargs.get('json')) is not None and data is None:
+
+    if (json := kwargs.get("json")) is not None and data is None:
         data = js.dumps(json, cls=NumpyTypeEncoder)
 
-        if kwargs.get('headers') and not kwargs.get('headers', {}).get('Content-Type'):
-            kwargs['headers']["Content-Type"] =  "application/json"
+        if kwargs.get("headers") and not kwargs.get("headers", {}).get("Content-Type"):
+            kwargs["headers"]["Content-Type"] = "application/json"
 
     return requests.patch(url=url, data=data, **kwargs)
 
 
 @set_verify_for_requests
+@set_additional_settings_for_requests
 def delete(url, **kwargs):
     r"""Sends a DELETE request.
 
     :param url: URL for the new :class:`Request` object.
     :param \*\*kwargs: Optional arguments that ``request`` takes.
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
 
     return requests.delete(url=url, **kwargs)
 
+
 class Session(requests.Session):
     """A Requests session.
 
     Provides cookie persistence, connection-pooling, and configuration.
 
     Basic Usage::
 
@@ -194,18 +220,20 @@
 
     Or as a context manager::
 
       >>> with requests.Session() as s:
       ...     s.get('https://httpbin.org/get')
       <Response [200]>
     """
+
     def __init__(self):
         requests.Session.__init__(self)
 
     @set_verify_for_requests
+    @set_additional_settings_for_requests
     def request(self, method, url, **kwargs):
         """Constructs a :class:`Request <Request>`, prepares it and sends it.
         Returns :class:`Response <Response>` object.
 
         :param method: method for the new :class:`Request` object.
         :param url: URL for the new :class:`Request` object.
         :param params: (optional) Dictionary or bytes to be sent in the query
@@ -240,16 +268,16 @@
             certificates, which will make your application vulnerable to
             man-in-the-middle (MitM) attacks. Setting verify to ``False``
             may be useful during local development or testing.
         :param cert: (optional) if String, path to ssl client cert file (.pem).
             If Tuple, ('cert', 'key') pair.
         :rtype: requests.Response
         """
-        kwargs['method'] = method
-        kwargs['url'] = url
+        kwargs["method"] = method
+        kwargs["url"] = url
         return super().request(**kwargs)
 
 
 def session():
     """
     Returns a :class:`Session` for context-management.
 
@@ -257,8 +285,8 @@
 
         This method has been deprecated since version 1.0.0 and is only kept for
         backwards compatibility. New code should use :class:`~requests.sessions.Session`
         to create a session. This may be removed at a future date.
 
     :rtype: Session
     """
-    return Session()
+    return Session()
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/datasets/experiment.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/datasets/experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,161 +1,200 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
 __all__ = ["ExperimentIterableDataset"]
 
 import os
 import pandas as pd
 
-from typing import Union, Optional
+from typing import TYPE_CHECKING, Iterator, Any, cast
 from warnings import warn
 from ibm_watsonx_ai.helpers.connections.local import LocalBatchReader
 from ibm_watsonx_ai.utils.autoai.enums import SamplingTypes
 from ibm_watsonx_ai.utils.autoai.errors import InvalidSizeLimit
 
+if TYPE_CHECKING:
+    from ibm_watsonx_ai.helpers.connections.flight_service import FlightConnection
+    from ibm_watsonx_ai.helpers.connections import DataConnection
+    from ibm_watsonx_ai import APIClient
+
 # Note: try to import torch lib if available, this fallback is done based on
 # torch dependency removal request
 try:
     from torch.utils.data import IterableDataset
 
 except ImportError:
-    IterableDataset = object
+    IterableDataset: type = object  # type: ignore[no-redef]
 # --- end note
 
-DEFAULT_SAMPLE_SIZE_LIMIT = 1073741824  # 1GB in Bytes is verified later by _set_sample_size_limit
+DEFAULT_SAMPLE_SIZE_LIMIT = (
+    1073741824  # 1GB in Bytes is verified later by _set_sample_size_limit
+)
 DEFAULT_REDUCED_SAMPLE_SIZE_LIMIT = 104857600  # 100MB in bytes
 DEFAULT_SAMPLING_TYPE = SamplingTypes.FIRST_VALUES
 
 
 class ExperimentIterableDataset(IterableDataset):
     """
-        This dataset is intended to be an Iterable stream from Flight Service.
-        It should iterate over flight logical batches and manages by Connection class
-        how batches are downloaded and created. It should take into consideration only 2 batches at a time.
-        If we have 2 batches already downloaded, it should block further download
-        and wait for first batch to be consumed.
-
-        Example
-        -------
-        >>> experiment_metadata = {
-        >>>     "prediction_column": 'species',
-        >>>     "prediction_type": "classification",
-        >>>     "project_id": os.environ.get('PROJECT_ID'),
-        >>>     'credentials': credentials
-        >>> }
-
-        >>> connection = DataConnection(data_asset_id='5d99c11a-2060-4ef6-83d5-dc593c6455e2')
-
-
-        >>># default sampling - read first 1GB of data
-        >>> iterable_dataset = ExperimentIterableDataset(connection=connection,
-        >>>                                              enable_sampling=True,
-        >>>                                              sampling_type='first_n_records',
-        >>>                                              sample_size_limit = 1GB,
-        >>>                                              experiment_metadata=experiment_metadata)
-
-        >>># read all data records in batches / no subsampling
-        >>> iterable_dataset = ExperimentIterableDataset(connection=connection,
-        >>>                                              enable_sampling=False,
-        >>>                                               experiment_metadata=experiment_metadata)
-
-        >>># stratified/random sampling
-        >>> iterable_dataset = ExperimentIterableDataset(connection=connection,
-        >>>                                              enable_sampling=True,
-        >>>                                              sampling_type='stratified',
-        >>>                                              sample_size_limit = 1GB,
-        >>>                                              experiment_metadata=experiment_metadata)
+    This dataset is intended to be an Iterable stream from Flight Service.
+    It should iterate over flight logical batches and manages by Connection class
+    how batches are downloaded and created. It should take into consideration only 2 batches at a time.
+    If we have 2 batches already downloaded, it should block further download
+    and wait for first batch to be consumed.
+
+    Example
+    -------
+    >>> experiment_metadata = {
+    >>>     "prediction_column": 'species',
+    >>>     "prediction_type": "classification",
+    >>>     "project_id": os.environ.get('PROJECT_ID'),
+    >>>     'credentials': credentials
+    >>> }
+
+    >>> connection = DataConnection(data_asset_id='5d99c11a-2060-4ef6-83d5-dc593c6455e2')
+
+
+    >>># default sampling - read first 1GB of data
+    >>> iterable_dataset = ExperimentIterableDataset(connection=connection,
+    >>>                                              enable_sampling=True,
+    >>>                                              sampling_type='first_n_records',
+    >>>                                              sample_size_limit = 1GB,
+    >>>                                              experiment_metadata=experiment_metadata)
+
+    >>># read all data records in batches / no subsampling
+    >>> iterable_dataset = ExperimentIterableDataset(connection=connection,
+    >>>                                              enable_sampling=False,
+    >>>                                               experiment_metadata=experiment_metadata)
+
+    >>># stratified/random sampling
+    >>> iterable_dataset = ExperimentIterableDataset(connection=connection,
+    >>>                                              enable_sampling=True,
+    >>>                                              sampling_type='stratified',
+    >>>                                              sample_size_limit = 1GB,
+    >>>                                              experiment_metadata=experiment_metadata)
 
     """
 
-    connection: Union["FlightConnection", LocalBatchReader] = None
+    connection: FlightConnection | LocalBatchReader | None = None
 
     def __init__(
         self,
-        connection: "DataConnection",
-        experiment_metadata: dict = None,
+        connection: DataConnection,
+        experiment_metadata: dict | None = None,
         enable_sampling: bool = True,
         sample_size_limit: int = DEFAULT_SAMPLE_SIZE_LIMIT,
         sampling_type: str = DEFAULT_SAMPLING_TYPE,
         binary_data: bool = False,
-        number_of_batch_rows: int = None,
+        number_of_batch_rows: int | None = None,
         stop_after_first_batch: bool = False,
-        total_size_limit=DEFAULT_SAMPLE_SIZE_LIMIT,
-        total_nrows_limit=None,
-        total_percentage_limit=1.0,
-        **kwargs,
+        total_size_limit: int = DEFAULT_SAMPLE_SIZE_LIMIT,
+        total_nrows_limit: int | None = None,
+        total_percentage_limit: float = 1.0,
+        **kwargs: Any,
     ):
         super().__init__()
         self.enable_sampling = enable_sampling
         self.sample_size_limit = sample_size_limit
         self.experiment_metadata = experiment_metadata
         self._api_client = getattr(connection, "_api_client", None)
         if self._api_client is None:
-            self._api_client = (kwargs.get("_api_client", None) or kwargs.get("_wml_client", None))
+            self._api_client = kwargs.get("_api_client", None) or kwargs.get(
+                "_wml_client", None
+            )
         self.binary_data = binary_data
         self.sampling_type = sampling_type
-        self.read_to_file = kwargs.get('read_to_file')
+        self.read_to_file = kwargs.get("read_to_file")
         self.authorized = self._check_authorization()
         self._set_size_limit(total_size_limit)
         self.total_nrows_limit = total_nrows_limit
         self.total_percentage_limit = total_percentage_limit
 
         # Note: convert to dictionary if we have object from API client
         if not isinstance(connection, dict):
             dict_connection = connection._to_dict()
 
         else:
             dict_connection = connection
         # --- end note
 
+        self.experiment_metadata = cast(dict[str, Any], self.experiment_metadata)
         # Note: backward compatibility after sampling refactoring #27255
-        if kwargs.get('with_sampling') or kwargs.get('normal_read'):
-            warn("The parameters with_sampling and normal_read in ExperimentIterableDataset are deprecated. "
-                 "Use enable_sampling and sampling_type instead.")
-            if kwargs.get('normal_read'):
+        if kwargs.get("with_sampling") or kwargs.get("normal_read"):
+            warn(
+                "The parameters with_sampling and normal_read in ExperimentIterableDataset are deprecated. "
+                "Use enable_sampling and sampling_type instead."
+            )
+            if kwargs.get("normal_read"):
                 self.enable_sampling = False
-            if kwargs.get('with_sampling'):
+            if kwargs.get("with_sampling"):
                 from ibm_watsonx_ai.utils.autoai.enums import PredictionType
+
                 self.enable_sampling = True
-                if self.experiment_metadata.get("prediction_type") in [PredictionType.REGRESSION]:
+
+                if self.experiment_metadata.get("prediction_type") in [
+                    PredictionType.REGRESSION
+                ]:
                     self.sampling_type = SamplingTypes.RANDOM
-                elif self.experiment_metadata.get("prediction_type") in [PredictionType.CLASSIFICATION,
-                                                                         PredictionType.BINARY,
-                                                                         PredictionType.MULTICLASS]:
+                elif self.experiment_metadata.get("prediction_type") in [
+                    PredictionType.CLASSIFICATION,
+                    PredictionType.BINARY,
+                    PredictionType.MULTICLASS,
+                ]:
                     self.sampling_type = SamplingTypes.STRATIFIED
         # --- end note
 
         # if number_of_batch_rows is provided, batch_size does not matter anymore
         if self.authorized:
-            is_cos_asset = bool(kwargs.get("flight_parameters", {}).get('datasource_type', {}).get('entity', {}).get('name', '') == 'bluemixcloudobjectstorage')
+            is_cos_asset = bool(
+                kwargs.get("flight_parameters", {})
+                .get("datasource_type", {})
+                .get("entity", {})
+                .get("name", "")
+                == "bluemixcloudobjectstorage"
+            )
             # first used headers from experiment metadata if they were set.
-            headers_ = None
+            headers_: dict | None = None
             if self.experiment_metadata.get("headers"):
                 headers_ = self.experiment_metadata.get("headers")
             elif self._api_client is not None:
                 headers_ = self._api_client._get_headers()
 
-            from ibm_watsonx_ai.helpers.connections.flight_service import FlightConnection
+            from ibm_watsonx_ai.helpers.connections.flight_service import (
+                FlightConnection,
+            )
 
+            headers_ = cast(dict, headers_)
+            number_of_batch_rows = cast(int, number_of_batch_rows)
             self.connection = FlightConnection(
                 headers=headers_,
                 sampling_type=self.sampling_type,
-                label=self.experiment_metadata.get("prediction_column"),
-                learning_type=self.experiment_metadata.get("prediction_type"),
+                label=self.experiment_metadata["prediction_column"],
+                learning_type=self.experiment_metadata["prediction_type"],
                 params=self.experiment_metadata,
-                project_id=self.experiment_metadata.get("project_id", getattr(self._api_client, 'default_project_id', None)),
-                space_id=self.experiment_metadata.get("space_id", getattr(self._api_client, 'default_space_id', None)),
-                asset_id=None if is_cos_asset else dict_connection.get("location", {}).get("id"), # do not pass asset id for data assets located on COS
+                project_id=self.experiment_metadata.get(
+                    "project_id", getattr(self._api_client, "default_project_id", None)
+                ),
+                space_id=self.experiment_metadata.get(
+                    "space_id", getattr(self._api_client, "default_space_id", None)
+                ),
+                asset_id=(
+                    None
+                    if is_cos_asset
+                    else dict_connection.get("location", {}).get("id")
+                ),  # do not pass asset id for data assets located on COS
                 connection_id=dict_connection.get("connection", {}).get("id"),
                 data_location=dict_connection,
                 data_batch_size_limit=self.sample_size_limit,
                 flight_parameters=kwargs.get("flight_parameters", {}),
-                extra_interaction_properties=kwargs.get("extra_interaction_properties",{}),
+                extra_interaction_properties=kwargs.get(
+                    "extra_interaction_properties", {}
+                ),
                 fallback_to_one_connection=kwargs.get(
                     "fallback_to_one_connection", True
                 ),
                 number_of_batch_rows=number_of_batch_rows,
                 stop_after_first_batch=stop_after_first_batch,
                 _api_client=self._api_client,
                 return_subsampling_stats=kwargs.get("_return_subsampling_stats", False),
@@ -168,94 +207,113 @@
 
             if (
                 dict_connection.get("type") == "fs"
                 and "location" in dict_connection
                 and "path" in dict_connection["location"]
             ):
                 self.connection = LocalBatchReader(
-                    file_path=dict_connection["location"]["path"], batch_size=sample_size_limit
+                    file_path=dict_connection["location"]["path"],
+                    batch_size=sample_size_limit,
                 )
 
             else:
                 raise NotImplementedError(
                     "For local data read please use 'fs' (file system) connection type."
                     "To use remote data read please provide 'experiment_metadata'."
                 )
 
     @property
-    def _wml_client(self):
+    def _wml_client(self) -> APIClient:
         # note: backward compatibility
-        warn(("`_wml_client` is deprecated and will be removed in future. "
-                "Instead, please use `_api_client`."), category=DeprecationWarning)
+        warn(
+            (
+                "`_wml_client` is deprecated and will be removed in future. "
+                "Instead, please use `_api_client`."
+            ),
+            category=DeprecationWarning,
+        )
         # --- end note
-        return self._api_client
-    
+        return self._api_client  # type: ignore[return-value]
+
     @_wml_client.setter
-    def _wml_client(self, var):
+    def _wml_client(self, var: APIClient) -> None:
         # note: backward compatibility
-        warn(("`_wml_client` is deprecated and will be removed in future. "
-                "Instead, please use `_api_client`."), category=DeprecationWarning)
+        warn(
+            (
+                "`_wml_client` is deprecated and will be removed in future. "
+                "Instead, please use `_api_client`."
+            ),
+            category=DeprecationWarning,
+        )
         # --- end note
         self._api_client = var
-        
+
     def _check_authorization(self) -> bool:
         """
         Check if we can authorize with Service.
         If the connection have api_client initialized use it as an attribute.
         Otherwise, credentials should be provided in the experiment_metadata dictionary.
         If the client is properly initialized True will be returned.
         """
         if self._api_client is not None:
             return True
 
         if self.experiment_metadata is None:
             return False
-        credentials = creds if (creds:=self.experiment_metadata.get("credentials")) is not None else self.experiment_metadata.get("wml_credentials")
+        credentials = (
+            creds
+            if (creds := self.experiment_metadata.get("credentials")) is not None
+            else self.experiment_metadata.get("wml_credentials")
+        )
         if credentials is not None:
             from ibm_watsonx_ai import APIClient
 
-            self._api_client = APIClient(
-                wml_credentials=credentials
-            )
+            self._api_client = APIClient(credentials=credentials)
             return True
 
         elif self.experiment_metadata.get("headers") is not None:
             return True
 
         else:
             return False
 
-    def _set_size_limit(self, size_limit):
+    def _set_size_limit(self, size_limit: int) -> None:
         """If non-default value of total_size_limit was not passed,
         set Sample Size Limit based on T-Shirt size if code is run on training pod:
         For memory < 16 (T-Shirts: XS,S) default is 10MB,
         For memory < 32 & >= 16 (T-Shirts: M) default is 100MB,
         For memory = 32 (T-Shirt L) default is 0.7GB,
         For memory > 32 (T-Shirt XL) or runs outside pod default is 1GB.
         """
+        self.total_size_limit: int | None
         from ibm_watsonx_ai.utils.autoai.connection import get_max_sample_size_limit
 
-        max_tshirt_size_limit = get_max_sample_size_limit() if os.getenv('MEM', False) else None  # limit manual setting of sample size limit on autoai clusters #31527
+        max_tshirt_size_limit = (
+            get_max_sample_size_limit() if os.getenv("MEM", False) else None
+        )  # limit manual setting of sample size limit on autoai clusters #31527
 
         if self.enable_sampling:
             if max_tshirt_size_limit:
-                if size_limit > max_tshirt_size_limit and size_limit != DEFAULT_SAMPLE_SIZE_LIMIT:
+                if (
+                    size_limit > max_tshirt_size_limit
+                    and size_limit != DEFAULT_SAMPLE_SIZE_LIMIT
+                ):
                     raise InvalidSizeLimit(size_limit, max_tshirt_size_limit)
                 else:
                     self.total_size_limit = min(size_limit, max_tshirt_size_limit)
             else:
                 self.total_size_limit = size_limit
         else:
             if size_limit == DEFAULT_SAMPLE_SIZE_LIMIT:
                 self.total_size_limit = None  # do not limit reading if sampling is disabled, we want read all data
             else:
                 self.total_size_limit = size_limit
 
     def write(
-        self, data: Optional[pd.DataFrame] = None, file_path: Optional[str] = None
+        self, data: pd.DataFrame | None = None, file_path: str | None = None
     ) -> None:
         """
         Writes data into data source connection.
 
         Parameters
         ----------
         data: pandas DataFrame, optional
@@ -280,27 +338,29 @@
                 f"'file_path' need to be a string, you provided: '{type(file_path)}'."
             )
 
         if data is not None:
             self.connection.write_data(data)
 
         else:
+            file_path = cast(str, file_path)
             self.connection.write_binary_data(file_path)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator:
         """Iterate over Flight Dataset."""
         if self.authorized:
             if self.enable_sampling:
                 if self.sampling_type == SamplingTypes.FIRST_VALUES:
                     return self.connection.iterable_read()
                 else:
                     self.connection.enable_subsampling = True
                     return self.connection.iterable_read()
             else:
                 if self.binary_data:
-                    return self.connection.read_binary_data(read_to_file=self.read_to_file)
+                    return self.connection.read_binary_data(read_to_file=self.read_to_file)  # type: ignore[return-value]
 
                 else:
                     self.total_size_limit = None
                     return self.connection.iterable_read()
         else:
+            self.connection = cast(LocalBatchReader, self.connection)
             return (batch for batch in self.connection)
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/data_loaders/experiment.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/data_loaders/experiment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
 __all__ = ["ExperimentDataLoader"]
 
+from typing import Iterator, Callable
+
 import pandas as pd
 
 # Note: Use torch DataLoader and Dataset if available, if not, use mocked ones.
 # SimpleDataLoader is the simplest wrapper ever for such thing, it is not compatible with torch anymore.
+
 try:
     from torch.utils.data import DataLoader, IterableDataset
 
 except ImportError:
+    IterableDataset: type = object  # type: ignore[no-redef]
 
     class SimpleDataLoader:
-        def __init__(self, dataset, collate_fn):
+        def __init__(self, dataset: IterableDataset, collate_fn: Callable):
             self.dataset = dataset
             self.collate_fn = collate_fn
 
-        def __iter__(self):
+        def __iter__(self) -> Iterator:
             return (data for data in self.dataset)
 
-    DataLoader = SimpleDataLoader
-    IterableDataset = object
+    DataLoader = SimpleDataLoader  # type: ignore[misc, assignment]
 # --- end note
 
 
 class ExperimentDataLoader(DataLoader):
     """Experiment Data Loader based on torch DataLoader.
     It interacts with the Flight Service to provide data batch stream
 
@@ -51,18 +55,18 @@
 
         data_loader = ExperimentDataLoader(dataset=iterable_dataset)
 
         for data in data_loader:
             print(data)
     """
 
-    def __init__(self, dataset: "IterableDataset"):
+    def __init__(self, dataset: IterableDataset):
         super().__init__(dataset=dataset, collate_fn=custom_collate)
 
 
-def custom_collate(batch: pd.DataFrame) -> pd.DataFrame:
+def custom_collate(batch: pd.DataFrame | list) -> pd.DataFrame:
     """Custom collate function for DataLoader, it simply get and return unchanged pandas DF"""
     if isinstance(batch, list):
         return batch[0]
 
     else:
         return batch
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/base_deployment.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/base_deployment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,195 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
 import os
 from abc import ABC, abstractmethod
 from copy import copy
 from functools import wraps
-from typing import TYPE_CHECKING, Union, Dict
+from typing import TYPE_CHECKING, Any, cast, Callable
 from warnings import warn
 from contextlib import redirect_stdout
 
 from pandas import DataFrame
-import ibm_watsonx_ai._wrappers.requests as requests
+from ..credentials import Credentials
 
 from ..experiment import AutoAI
 from ..utils import is_lale_pipeline
-from ..utils.autoai.utils import (prepare_auto_ai_model_to_publish, prepare_auto_ai_model_to_publish_normal_scenario,
-                                  remove_file, prepare_auto_ai_model_to_publish_notebook_normal_scenario, get_sw_spec_and_type_based_on_sklearn,
-                                  check_if_ts_pipeline_is_winner, convert_dataframe_to_fields_values_payload)
-from ..utils.deployment.errors import (WrongDeploymnetType, ModelTypeNotSupported, NotAutoAIExperiment,
-                                       DeploymentNotSupported, MissingSpace, ModelPromotionFailed,
-                                       ServingNameNotAvailable)
+from ..utils.autoai.utils import (
+    prepare_auto_ai_model_to_publish,
+    prepare_auto_ai_model_to_publish_normal_scenario,
+    remove_file,
+    prepare_auto_ai_model_to_publish_notebook_normal_scenario,
+    check_if_ts_pipeline_is_winner,
+    convert_dataframe_to_fields_values_payload,
+)
+from ..utils.deployment.errors import (
+    WrongDeploymnetType,
+    ModelTypeNotSupported,
+    NotAutoAIExperiment,
+    MissingSpace,
+    ServingNameNotAvailable,
+)
 from ..helpers import DataConnection
-from ..wml_client_error import ApiRequestFailure
 from ..workspace import WorkSpace
 
 if TYPE_CHECKING:
     from sklearn.pipeline import Pipeline
 
-__all__ = [
-    "BaseDeployment"
-]
+__all__ = ["BaseDeployment"]
 
 
 class BaseDeployment(ABC):
     """Base abstract class for Deployment."""
 
-    def __init__(self,
-                 deployment_type: str,
-                 source_instance_credentials: Union[dict, 'WorkSpace'] = None,
-                 source_project_id: str = None,
-                 source_space_id: str = None,
-                 target_instance_credentials: Union[dict, 'WorkSpace'] = None,
-                 target_project_id: str = None,
-                 target_space_id: str = None,
-                 project_id: str = None,
-                 space_id: str = None,
-                 **kwargs):
+    def __init__(
+        self,
+        deployment_type: str,
+        source_instance_credentials: Credentials | WorkSpace | None = None,
+        source_project_id: str | None = None,
+        source_space_id: str | None = None,
+        target_instance_credentials: Credentials | WorkSpace | None = None,
+        target_project_id: str | None = None,
+        target_space_id: str | None = None,
+        project_id: str | None = None,
+        space_id: str | None = None,
+        **kwargs: Any,
+    ):
 
         if space_id is None and source_space_id is None and target_space_id is None:
-            raise MissingSpace(reason="Any of the [space_id, source_space_id, target_space_id] is not specified.")
+            raise MissingSpace(
+                reason="Any of the [space_id, source_space_id, target_space_id] is not specified."
+            )
 
         # note: backward compatibility
-        if (source_wml_credentials:=kwargs.get('source_wml_credentials')) is not None:
+        if (source_wml_credentials := kwargs.get("source_wml_credentials")) is not None:
             if not source_instance_credentials:
                 source_instance_credentials = source_wml_credentials
-            warn(("`source_wml_credentials` is deprecated and will be removed in future. "
-                  "Instead, please use `source_instance_credentials`."), category=DeprecationWarning)
-            
-        if (target_wml_credentials:=kwargs.get('target_wml_credentials')) is not None:
+            warn(
+                (
+                    "`source_wml_credentials` is deprecated and will be removed in future. "
+                    "Instead, please use `source_instance_credentials`."
+                ),
+                category=DeprecationWarning,
+            )
+
+        if (target_wml_credentials := kwargs.get("target_wml_credentials")) is not None:
             if not target_instance_credentials:
                 target_instance_credentials = target_wml_credentials
-            warn(("`target_wml_credentials` is deprecated and will be removed in future. "
-                  "Instead, please use `target_instance_credentials`."), category=DeprecationWarning)
-            
+            warn(
+                (
+                    "`target_wml_credentials` is deprecated and will be removed in future. "
+                    "Instead, please use `target_instance_credentials`."
+                ),
+                category=DeprecationWarning,
+            )
+
         if project_id is not None:
             source_project_id = project_id
-            warn("\"project_id\" parameter is deprecated, please use \"source_project_id\"")
-            print("\"project_id\" parameter is deprecated, please use \"source_project_id\"")
+            warn('"project_id" parameter is deprecated, please use "source_project_id"')
+            print(
+                '"project_id" parameter is deprecated, please use "source_project_id"'
+            )
 
         if space_id is not None:
             source_space_id = space_id
-            warn("\"space_id\" parameter is deprecated, please use \"source_space_id\"")
-            print("\"space_id\" parameter is deprecated, please use \"source_space_id\"")
+            warn('"space_id" parameter is deprecated, please use "source_space_id"')
+            print('"space_id" parameter is deprecated, please use "source_space_id"')
         # --- end note
 
         # note: as workspace is not clear enough to understand, there is a possibility to use pure
         # credentials with project and space IDs, but in addition we
         # leave a possibility to use a previous WorkSpace implementation, it could be passed as a first argument
+        self._source_workspace: WorkSpace | None
+        target_project_id = cast(str, target_project_id)
+        target_space_id = cast(str, target_space_id)
+        source_project_id = cast(str, source_project_id)
+        source_space_id = cast(str, source_space_id)
         if isinstance(source_instance_credentials, WorkSpace):
             self._source_workspace = source_instance_credentials
 
-        elif isinstance(source_instance_credentials, dict):
-            self._source_workspace = WorkSpace(credentials=source_instance_credentials.copy(),
-                                               project_id=source_project_id,
-                                               space_id=source_space_id)
+        elif isinstance(source_instance_credentials, Credentials):
+            self._source_workspace = WorkSpace(
+                credentials=copy(source_instance_credentials),
+                project_id=source_project_id,
+                space_id=source_space_id,
+            )
         else:
             self._source_workspace = None
 
         if target_instance_credentials is None:
+            self._target_workspace: WorkSpace | None
             if isinstance(source_instance_credentials, WorkSpace):
-                self._target_workspace = WorkSpace(credentials=source_instance_credentials.credentials,
-                                                   space_id=target_space_id if target_space_id is not None else source_instance_credentials.space_id)
+                self._target_workspace = WorkSpace(
+                    credentials=source_instance_credentials.credentials,
+                    space_id=(
+                        target_space_id
+                        if target_space_id is not None
+                        else source_instance_credentials.space_id
+                    ),
+                )
 
-            elif isinstance(source_instance_credentials, dict):
-                self._target_workspace = WorkSpace(credentials=source_instance_credentials.copy(),
-                                                   space_id=target_space_id if target_space_id is not None else source_space_id)
+            elif isinstance(source_instance_credentials, Credentials):
+                self._target_workspace = WorkSpace(
+                    credentials=copy(source_instance_credentials),
+                    space_id=(
+                        target_space_id
+                        if target_space_id is not None
+                        else source_space_id
+                    ),
+                )
             else:
                 self._target_workspace = None
 
+            self._target_workspace = cast(WorkSpace, self._target_workspace)
             if target_space_id or target_project_id:
                 self._target_workspace.project_id = target_project_id
                 self._target_workspace.space_id = target_space_id
 
         else:
             if isinstance(target_instance_credentials, WorkSpace):
                 self._target_workspace = target_instance_credentials
 
-            elif isinstance(target_instance_credentials, dict):
-                self._target_workspace = WorkSpace(credentials=target_instance_credentials.copy(),
-                                                   project_id=target_project_id,
-                                                   space_id=target_space_id)
+            elif isinstance(target_instance_credentials, Credentials):
+                self._target_workspace = WorkSpace(
+                    credentials=copy(target_instance_credentials),
+                    project_id=target_project_id,
+                    space_id=target_space_id,
+                )
 
                 # note: only if user provides target instance information
                 if self._source_workspace is None:
                     self._source_workspace = copy(self._target_workspace)
 
             else:
                 self._target_workspace = None
         # --- end note
 
         if self._source_workspace is None and self._target_workspace is None:
-            raise TypeError(f"{self.__class__.__name__} is missing one of the parameters: "
-                            f"['source_instance_credentials', 'target_instance_credentials']")
+            raise TypeError(
+                f"{self.__class__.__name__} is missing one of the parameters: "
+                f"['source_instance_credentials', 'target_instance_credentials']"
+            )
 
-        self.name = None
-        self.id = None
-        if deployment_type == 'online':
-            self.scoring_url = None
+        self.name: str | None = None
+        self.id: str | None = None
+        if deployment_type == "online":
+            self.scoring_url: str | None = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"name: {self.name}, id: {self.id}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"name: {self.name}, id: {self.id}"
 
     @abstractmethod
-    def create(self, **kwargs):
+    def create(self, **kwargs: Any) -> None:
         """Create deployment from a model.
 
         :param model: AutoAI model name
         :type model: str
 
         :param deployment_name: name of the deployment
         :type deployment_name: str
@@ -154,383 +202,512 @@
 
         :param metadata: model meta properties
         :type metadata: dict, optional
 
         :param experiment_run_id: ID of a training/experiment (only applicable for AutoAI deployments)
         :type experiment_run_id: str, optional
         """
-
-        if kwargs.get('serving_name'):
-            status_code, response = self._target_workspace.api_client.deployments._get_serving_name_info(kwargs.get('serving_name'))
+        model_props: dict
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
+        self._source_workspace = cast(WorkSpace, self._source_workspace)
+
+        if kwargs.get("serving_name"):
+            status_code, response = (
+                self._target_workspace.api_client.deployments._get_serving_name_info(
+                    str(kwargs.get("serving_name"))
+                )
+            )
 
             if status_code == 409:
-                raise ServingNameNotAvailable(response['errors'][0])
+                raise ServingNameNotAvailable(response["errors"][0])
 
         # note: This section is only for deployments with specified experiment_id
-        if kwargs['experiment_run_id'] is not None:
+        if kwargs["experiment_run_id"] is not None:
             run_params = self._source_workspace.api_client.training.get_details(
-                training_uid=kwargs['experiment_run_id'], _internal=True)
+                training_id=kwargs["experiment_run_id"], _internal=True
+            )
             pipeline_details = self._source_workspace.api_client.pipelines.get_details(
-                run_params['entity']['pipeline']['id'])
+                run_params["entity"]["pipeline"]["id"]
+            )
 
-            if not ('autoai' in str(pipeline_details) or 'auto_ai' in str(pipeline_details)):
+            if not (
+                "autoai" in str(pipeline_details) or "auto_ai" in str(pipeline_details)
+            ):
                 raise NotAutoAIExperiment(
-                    kwargs['experiment_run_id'], reason="Currently WebService class supports only AutoAI models.")
+                    kwargs["experiment_run_id"],
+                    reason="Currently WebService class supports only AutoAI models.",
+                )
 
             print("Preparing an AutoAI Deployment...")
             # TODO: remove part with model object depployment
-            if not isinstance(kwargs['model'], str):
-                warning_msg = ("Depreciation Warning: Passing an object will no longer be supported. "
-                               "Please specify the AutoAI model name to deploy.")
+            if not isinstance(kwargs["model"], str):
+                warning_msg = (
+                    "Depreciation Warning: Passing an object will no longer be supported. "
+                    "Please specify the AutoAI model name to deploy."
+                )
                 print(warning_msg)
                 warn(warning_msg)
 
-            if is_lale_pipeline(kwargs['model']):
-                model = kwargs['model'].export_to_sklearn_pipeline()
+            if is_lale_pipeline(kwargs["model"]):
+                model = kwargs["model"].export_to_sklearn_pipeline()
             else:
-                model = kwargs['model']
+                model = kwargs["model"]
 
             # note: check if model is of lale type, if yes, convert it back to scikit
-            if not isinstance(kwargs['model'], str):
+            if not isinstance(kwargs["model"], str):
                 model_props = {
                     self._target_workspace.api_client.repository.ModelMetaNames.NAME: f"{kwargs['deployment_name']} Model",
                     self._target_workspace.api_client.repository.ModelMetaNames.TYPE: "wml-hybrid_0.1",
-                    self._target_workspace.api_client.repository.ModelMetaNames.SOFTWARE_SPEC_UID:
-                        self._target_workspace.api_client.software_specifications.get_uid_by_name("hybrid_0.1")
+                    self._target_workspace.api_client.repository.ModelMetaNames.SOFTWARE_SPEC_UID: self._target_workspace.api_client.software_specifications.get_uid_by_name(
+                        "hybrid_0.1"
+                    ),
                 }
 
                 schema, artifact_name = prepare_auto_ai_model_to_publish(
                     pipeline_model=model,
                     run_params=run_params,
-                    run_id=kwargs['experiment_run_id'],
-                    api_client=self._source_workspace.api_client)
+                    run_id=kwargs["experiment_run_id"],
+                    api_client=self._source_workspace.api_client,
+                )
 
-                model_props[self._target_workspace.api_client.repository.ModelMetaNames.INPUT_DATA_SCHEMA] = [schema]
+                model_props[
+                    self._target_workspace.api_client.repository.ModelMetaNames.INPUT_DATA_SCHEMA
+                ] = [schema]
 
             else:
                 # raise an error when TS pipeline is discarded one
                 check_if_ts_pipeline_is_winner(details=run_params, model_name=model)
 
                 # Note: We need to fetch credentials when 'container' is the type
-                if run_params['entity']['results_reference']['type'] == 'container':
-                    data_connection = DataConnection._from_dict(_dict=run_params['entity']['results_reference'])
+                if run_params["entity"]["results_reference"]["type"] == "container":
+                    data_connection = DataConnection._from_dict(
+                        _dict=run_params["entity"]["results_reference"]
+                    )
                     data_connection._api_client = self._source_workspace.api_client
                 else:
                     data_connection = None
                 # --- end note
 
                 try:
-                    auto_pipelines_parameters = pipeline_details.get('entity', {}).get('document', {}).get('pipelines', [])[0].get('nodes', [])[0].get('parameters')
+                    auto_pipelines_parameters = (
+                        pipeline_details.get("entity", {})
+                        .get("document", {})
+                        .get("pipelines", [])[0]
+                        .get("nodes", [])[0]
+                        .get("parameters")
+                    )
                 except:
                     auto_pipelines_parameters = None
 
-                artifact_name, model_props = prepare_auto_ai_model_to_publish_normal_scenario(
-                    pipeline_model=model,
-                    run_params=run_params,
-                    run_id=kwargs['experiment_run_id'],
-                    api_client=self._source_workspace.api_client,
-                    space_id=self._target_workspace.space_id,
-                    result_reference=data_connection,
-                    auto_pipelines_parameters=auto_pipelines_parameters
+                data_connection = cast(DataConnection, data_connection)
+
+                artifact_name, model_props = (
+                    prepare_auto_ai_model_to_publish_normal_scenario(
+                        pipeline_model=model,
+                        run_params=run_params,
+                        run_id=kwargs["experiment_run_id"],
+                        api_client=self._source_workspace.api_client,
+                        space_id=self._target_workspace.space_id,
+                        result_reference=data_connection,
+                        auto_pipelines_parameters=auto_pipelines_parameters,
+                    )
                 )
 
             deployment_details = self._deploy(
                 pipeline_model=artifact_name,
-                deployment_name=kwargs['deployment_name'],
-                serving_name=kwargs.get('serving_name'),
+                deployment_name=kwargs["deployment_name"],
+                serving_name=kwargs.get("serving_name"),
                 meta_props=model_props,
-                hardware_spec=kwargs.get('hardware_spec')
+                hardware_spec=kwargs.get("hardware_spec"),
             )
 
             remove_file(filename=artifact_name)
 
-            self.name = kwargs['deployment_name']
-            self.id = deployment_details.get('metadata').get('id')
-            if kwargs['deployment_type'] == 'online':
-                self.scoring_url = self._target_workspace.api_client.deployments.get_scoring_href(deployment_details)
+            self.name = kwargs["deployment_name"]
+            self.id = deployment_details["metadata"].get("id")
+            if kwargs["deployment_type"] == "online":
+                deployment_details = cast(dict, deployment_details)
+                self.scoring_url = (
+                    self._target_workspace.api_client.deployments.get_scoring_href(
+                        deployment_details
+                    )
+                )
         # --- end note
 
         # note: This section is for deployments from auto-gen notebook with COS connection
         else:
             # note: only if we have COS connections from the notebook
-            if kwargs.get('metadata') is not None:
+            if kwargs.get("metadata") is not None:
                 print("Preparing an AutoAI Deployment...")
                 # note: CP4D
-                if self._source_workspace is not None and self._source_workspace.api_client.ICP:
-                    optimizer = AutoAI(self._source_workspace).runs.get_optimizer(metadata=kwargs['metadata'])
+                if (
+                    self._source_workspace is not None
+                    and self._source_workspace.api_client.ICP_PLATFORM_SPACES
+                ):
+                    optimizer = AutoAI(self._source_workspace).runs.get_optimizer(metadata=kwargs["metadata"])  # type: ignore[attr-defined]
                 # note: CLOUD
                 else:
-                    optimizer = AutoAI().runs.get_optimizer(metadata=kwargs['metadata'],
-                                                            api_client=self._source_workspace.api_client)
+                    optimizer = AutoAI().runs.get_optimizer(  # type: ignore[attr-defined]
+                        metadata=kwargs["metadata"],
+                        api_client=self._source_workspace.api_client,
+                    )
 
                 # note: only when user did not pass WMLS credentials during Service initialization
                 if self._source_workspace is None:
                     self._source_workspace = copy(optimizer._workspace)
 
                 if self._target_workspace is None:
                     self._target_workspace = copy(optimizer._workspace)
                 # --- end note
 
                 # TODO: remove part with model object depployment
-                if not isinstance(kwargs['model'], str):
-                    warning_msg = ("Depreciation Warning: Passing an object will no longer be supported. "
-                                   "Please specify the AutoAI model name to deploy.")
+                if not isinstance(kwargs["model"], str):
+                    warning_msg = (
+                        "Depreciation Warning: Passing an object will no longer be supported. "
+                        "Please specify the AutoAI model name to deploy."
+                    )
                     print(warning_msg)
                     warn(warning_msg)
 
-                if is_lale_pipeline(kwargs['model']):
-                    model = kwargs['model'].export_to_sklearn_pipeline()
+                if is_lale_pipeline(kwargs["model"]):
+                    model = kwargs["model"].export_to_sklearn_pipeline()
                 else:
-                    model = kwargs['model']
+                    model = kwargs["model"]
 
-                if not self._target_workspace.api_client.ICP:
+                if not self._target_workspace.api_client.ICP_PLATFORM_SPACES:
 
-                    optimizer_2 = AutoAI(self._source_workspace).runs.get_optimizer(metadata=kwargs['metadata'])
-                    run_details = optimizer_2._workspace.api_client.training.get_details(
-                        optimizer_2.get_params()['run_id'], _internal=True
+                    optimizer_2 = AutoAI(self._source_workspace).runs.get_optimizer(metadata=kwargs["metadata"])  # type: ignore[attr-defined]
+                    run_details = (
+                        optimizer_2._workspace.api_client.training.get_details(
+                            optimizer_2.get_params()["run_id"], _internal=True
+                        )
                     )
-
-                    artifact_name, model_props = prepare_auto_ai_model_to_publish_notebook_normal_scenario(
-                        pipeline_model=model,
-                        result_connection=optimizer._result_client[0],
-                        cos_client=optimizer._result_client[1],
-                        run_params=run_details,
-                        space_id=self._target_workspace.space_id,
-                        auto_pipelines_parameters=optimizer.get_params()
+                    self._target_workspace.space_id = cast(
+                        str, self._target_workspace.space_id
+                    )
+                    artifact_name, model_props = (
+                        prepare_auto_ai_model_to_publish_notebook_normal_scenario(
+                            pipeline_model=model,
+                            result_connection=optimizer._result_client[0],
+                            cos_client=optimizer._result_client[1],
+                            run_params=run_details,
+                            space_id=self._target_workspace.space_id,
+                            auto_pipelines_parameters=optimizer.get_params(),
+                        )
                     )
 
                     deployment_details = self._deploy(
                         pipeline_model=artifact_name,
-                        deployment_name=kwargs['deployment_name'],
+                        deployment_name=kwargs["deployment_name"],
                         meta_props=model_props,
-                        serving_name=kwargs.get('serving_name'),
-                        result_client=optimizer._result_client
+                        serving_name=kwargs.get("serving_name"),
+                        result_client=optimizer._result_client,
                     )
 
                 # note: CP4D part
                 else:
-                     training_result_reference = kwargs['metadata'].get('training_result_reference')
-                     run_id = training_result_reference.location.path.split('/')[-3]
-                     run_params = self._source_workspace.api_client.training.get_details(training_uid=run_id, _internal=True)
-
-                     artifact_name, model_props = prepare_auto_ai_model_to_publish_normal_scenario(
-                         pipeline_model=model,
-                         run_params=run_params,
-                         run_id=run_id,
-                         api_client=self._source_workspace.api_client,
-                         space_id=self._target_workspace.space_id,
-                         auto_pipelines_parameters=optimizer.get_params()
-                     )
-
-                     deployment_details = self._deploy(
-                         pipeline_model=artifact_name,
-                         deployment_name=kwargs['deployment_name'],
-                         serving_name=kwargs.get('serving_name'),
-                         meta_props=model_props
-                     )
-                 # --- end note
+                    training_result_reference = kwargs["metadata"].get(
+                        "training_result_reference"
+                    )
+                    run_id = training_result_reference.location.path.split("/")[-3]
+                    run_params = self._source_workspace.api_client.training.get_details(
+                        training_id=run_id, _internal=True
+                    )
+
+                    artifact_name, model_props = (
+                        prepare_auto_ai_model_to_publish_normal_scenario(
+                            pipeline_model=model,
+                            run_params=run_params,
+                            run_id=run_id,
+                            api_client=self._source_workspace.api_client,
+                            space_id=self._target_workspace.space_id,
+                            auto_pipelines_parameters=optimizer.get_params(),
+                        )
+                    )
+
+                    deployment_details = self._deploy(
+                        pipeline_model=artifact_name,
+                        deployment_name=kwargs["deployment_name"],
+                        serving_name=kwargs.get("serving_name"),
+                        meta_props=model_props,
+                    )
+                # --- end note
                 remove_file(filename=artifact_name)
 
-                self.name = kwargs['deployment_name']
-                self.id = deployment_details.get('metadata').get('id')
-                if kwargs['deployment_type'] == 'online':
-                    self.scoring_url = self._target_workspace.api_client.deployments.get_scoring_href(
-                        deployment_details
+                self.name = kwargs["deployment_name"]
+                self.id = deployment_details["metadata"].get("id")
+                if kwargs["deployment_type"] == "online":
+                    self.scoring_url = (
+                        self._target_workspace.api_client.deployments.get_scoring_href(
+                            deployment_details
+                        )
                     )
             # --- end note
 
             else:
-                raise ModelTypeNotSupported(type(kwargs['model']),
-                                            reason="Currently WebService class supports only AutoAI models.")
+                raise ModelTypeNotSupported(
+                    str(type(kwargs["model"])),
+                    reason="Currently WebService class supports only AutoAI models.",
+                )
 
     @abstractmethod
-    def get_params(self):
+    def get_params(self) -> dict:
         """Get deployment parameters."""
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
         return self._target_workspace.api_client.deployments.get_details(self.id)
 
     @abstractmethod
-    def score(self, **kwargs):
+    def score(self, **kwargs: Any) -> dict:
         """Scoring on Service. Payload is passed to the scoring endpoint where model have been deployed.
 
         :param payload: data to test the model
         :type payload: pandas.DataFrame
         """
-
-        if isinstance(kwargs['payload'], DataFrame):
-            payload = convert_dataframe_to_fields_values_payload(kwargs['payload'])
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
+        if isinstance(kwargs["payload"], DataFrame):
+            payload = convert_dataframe_to_fields_values_payload(kwargs["payload"])
             input_data = [payload]
 
-        elif isinstance(kwargs['payload'], dict):
-            observations_df = kwargs['payload'].get('observations', DataFrame())
-            supporting_features_df = kwargs['payload'].get('supporting_features')
-
-            if isinstance(observations_df, DataFrame) and \
-                    (isinstance(supporting_features_df, DataFrame) or supporting_features_df is None):
-                observations_payload = convert_dataframe_to_fields_values_payload(observations_df)
-                observations_payload['id'] = 'observations'
+        elif isinstance(kwargs["payload"], dict):
+            observations_df = kwargs["payload"].get("observations", DataFrame())
+            supporting_features_df = kwargs["payload"].get("supporting_features")
+
+            if isinstance(observations_df, DataFrame) and (
+                isinstance(supporting_features_df, DataFrame)
+                or supporting_features_df is None
+            ):
+                observations_payload = convert_dataframe_to_fields_values_payload(
+                    observations_df
+                )
+                observations_payload["id"] = "observations"
                 input_data = [observations_payload]
 
                 if supporting_features_df is not None:
-                    supporting_features_payload = convert_dataframe_to_fields_values_payload(supporting_features_df)
-                    supporting_features_payload['id'] = 'supporting_features'
+                    supporting_features_payload = (
+                        convert_dataframe_to_fields_values_payload(
+                            supporting_features_df
+                        )
+                    )
+                    supporting_features_payload["id"] = "supporting_features"
                     input_data.append(supporting_features_payload)
             else:
-                raise TypeError('Missing data observations in payload or observations'
-                                 'or supporting_features are not pandas DataFrames.')
+                raise TypeError(
+                    "Missing data observations in payload or observations"
+                    "or supporting_features are not pandas DataFrames."
+                )
 
         else:
-            raise TypeError(f"Scoring payload has invalid type: {type(kwargs['payload'])}. "
-                            f"Supported types are: pandas.DataFrame and dictionary.")
-
-        transaction_id = kwargs.get('transaction_id')
+            raise TypeError(
+                f"Scoring payload has invalid type: {type(kwargs['payload'])}. "
+                f"Supported types are: pandas.DataFrame and dictionary."
+            )
 
-        scoring_payload = {self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA: input_data}
+        transaction_id = kwargs.get("transaction_id")
 
-        score = self._target_workspace.api_client.deployments.score(self.id, scoring_payload, transaction_id=transaction_id)
+        scoring_payload = {
+            self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA: input_data
+        }
+
+        self.id = cast(str, self.id)
+        score = self._target_workspace.api_client.deployments.score(
+            self.id, scoring_payload, transaction_id=transaction_id
+        )
 
         return score
 
     @abstractmethod
-    def delete(self, **kwargs):
+    def delete(self, **kwargs: Any) -> None:
         """Delete deployment.
 
         :param deployment_id: ID of the deployment to delete, if empty, current deployment will be deleted
         :type deployment_id: str, optional
 
         :param deployment_type: type of the deployment: [online, batch]
         :type deployment_type: str
         """
-        if kwargs['deployment_id'] is None:
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
+        if kwargs["deployment_id"] is None:
             self._target_workspace.api_client.deployments.delete(self.id)
             self.name = None
             self.scoring_url = None
             self.id = None
 
         else:
-            deployment_details = self._target_workspace.api_client.deployments.get_details(
-                deployment_uid=kwargs['deployment_id'])
-            if deployment_details.get('entity', {}).get(kwargs['deployment_type']) is not None:
-                self._target_workspace.api_client.deployments.delete(kwargs['deployment_id'])
+            deployment_details = (
+                self._target_workspace.api_client.deployments.get_details(
+                    deployment_uid=kwargs["deployment_id"]
+                )
+            )
+            if (
+                deployment_details.get("entity", {}).get(kwargs["deployment_type"])
+                is not None
+            ):
+                self._target_workspace.api_client.deployments.delete(
+                    kwargs["deployment_id"]
+                )
 
             else:
                 raise WrongDeploymnetType(
                     f"{kwargs['deployment_type']}",
-                    reason=f"Deployment with ID: {kwargs['deployment_id']} is not of \"{kwargs['deployment_type']}\" type!")
+                    reason=f"Deployment with ID: {kwargs['deployment_id']} is not of \"{kwargs['deployment_type']}\" type!",
+                )
 
     @abstractmethod
-    def list(self, **kwargs):
+    def list(self, **kwargs: Any) -> DataFrame:
         """List deployments.
 
         :param limit: set the limit of how many deployments to list,
             default is `None` (all deployments should be fetched)
         :type limit: int, optional
 
         :param deployment_type: type of the deployment: [online, batch]
         :type deployment_type: str
         """
-        deployments = self._target_workspace.api_client.deployments.get_details(limit=kwargs['limit'])
-        columns = [
-            'created_at',
-            'modified_at',
-            'id',
-            'name',
-            'status'
-        ]
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
+        deployments = self._target_workspace.api_client.deployments.get_details(
+            limit=kwargs["limit"]
+        )
+        columns = ["created_at", "modified_at", "id", "name", "status"]
 
         data = [
-            [deployment.get('metadata')['created_at'],
-             deployment.get('metadata')['modified_at'],
-             deployment.get('metadata')['id'],
-             deployment.get('metadata')['name'],
-             deployment.get('entity')['status']['state'],
-             ] for deployment in deployments.get('resources', []) if
-            isinstance(deployment.get('entity', {}).get(kwargs['deployment_type']), dict)
+            [
+                deployment.get("metadata")["created_at"],
+                deployment.get("metadata")["modified_at"],
+                deployment.get("metadata")["id"],
+                deployment.get("metadata")["name"],
+                deployment.get("entity")["status"]["state"],
+            ]
+            for deployment in deployments.get("resources", [])
+            if isinstance(
+                deployment.get("entity", {}).get(kwargs["deployment_type"]), dict
+            )
         ]
 
-        deployments = DataFrame(data=data, columns=columns).sort_values(by=['created_at'], ascending=False)
-        return deployments.head(n=kwargs['limit'])
+        deployments_df = DataFrame(data=data, columns=columns).sort_values(
+            by=["created_at"], ascending=False
+        )
+        return deployments_df.head(n=kwargs["limit"])
 
     @abstractmethod
-    def get(self, **kwargs):
+    def get(self, **kwargs: Any) -> None:
         """Get deployment.
 
         :param deployment_id: ID of the deployment to work with
         :type deployment_id: str
 
         :param deployment_type: type of the deployment: [online, batch]
         :type deployment_type: str
         """
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
         deployment_details = self._target_workspace.api_client.deployments.get_details(
-            deployment_uid=kwargs['deployment_id'])
-        if deployment_details.get('entity', {}).get(kwargs['deployment_type']) is not None:
-            self.name = deployment_details.get('metadata').get('name')
-            self.id = deployment_details.get('metadata').get('id')
-            if kwargs['deployment_type'] == 'online':
-                self.scoring_url = self._target_workspace.api_client.deployments.get_scoring_href(deployment_details)
+            deployment_uid=kwargs["deployment_id"]
+        )
+        if (
+            deployment_details.get("entity", {}).get(kwargs["deployment_type"])
+            is not None
+        ):
+            self.name = deployment_details["metadata"].get("name")
+            self.id = deployment_details["metadata"].get("id")
+            if kwargs["deployment_type"] == "online":
+                self.scoring_url = (
+                    self._target_workspace.api_client.deployments.get_scoring_href(
+                        deployment_details
+                    )
+                )
 
         else:
             raise WrongDeploymnetType(
                 f"{kwargs['deployment_type']}",
-                reason=f"Deployment with ID: {kwargs['deployment_id']} is not of \"{kwargs['deployment_type']}\" type!")
+                reason=f"Deployment with ID: {kwargs['deployment_id']} is not of \"{kwargs['deployment_type']}\" type!",
+            )
 
     @abstractmethod
-    def _deploy(self, **kwargs):
+    def _deploy(self, **kwargs: Any) -> dict:
         """Protected method to create a deployment."""
         pass
 
-    def _publish_model(self,
-                       pipeline_model: Union['Pipeline', str],
-                       meta_props: Dict) -> str:
+    def _publish_model(self, pipeline_model: Pipeline | str, meta_props: dict) -> str:
         """Publish model into Service.
 
         :param pipeline_model: model of the pipeline to publish
         :type pipeline_model: Pipeline or str
 
         :param meta_props: model meta properties
         :type meta_props: dict
 
         :return: asset id
         :rtype: str
         """
 
         # Note: publish model to project and then promote to space
-        if self._source_workspace.project_id and self._source_workspace.project_id in str(meta_props):
-            published_model_details = self._source_workspace.api_client.repository.store_model(
-                model=pipeline_model,
-                meta_props=meta_props)
-
-            project_asset_id = self._source_workspace.api_client.repository.get_model_id(published_model_details)
-
-            asset_id = self._source_workspace.api_client.spaces.promote(asset_id=project_asset_id,
-                                                                        source_project_id=self._source_workspace.project_id,
-                                                                        target_space_id=self._target_workspace.space_id)
+        self._source_workspace = cast(WorkSpace, self._source_workspace)
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
+        if (
+            self._source_workspace.project_id
+            and self._source_workspace.project_id in str(meta_props)
+        ):
+            published_model_details = (
+                self._source_workspace.api_client.repository.store_model(
+                    model=pipeline_model, meta_props=meta_props
+                )
+            )
+
+            project_asset_id = (
+                self._source_workspace.api_client.repository.get_model_id(
+                    published_model_details
+                )
+            )
+
+            self._target_workspace.space_id = cast(str, self._target_workspace.space_id)
+            asset_id = self._source_workspace.api_client.spaces.promote(
+                asset_id=project_asset_id,
+                source_project_id=self._source_workspace.project_id,
+                target_space_id=self._target_workspace.space_id,
+            )
 
         else:
-            published_model_details = self._target_workspace.api_client.repository.store_model(
-                model=pipeline_model,
-                meta_props=meta_props)
+            published_model_details = (
+                self._target_workspace.api_client.repository.store_model(
+                    model=pipeline_model, meta_props=meta_props
+                )
+            )
 
-            asset_id = self._target_workspace.api_client.repository.get_model_id(published_model_details)
+            asset_id = self._target_workspace.api_client.repository.get_model_id(
+                published_model_details
+            )
 
         print(f"Published model uid: {asset_id}")
         return asset_id
 
     @staticmethod
-    def _project_to_space_to_project(method):
+    def _project_to_space_to_project(method: Callable) -> Callable:
         @wraps(method)
-        def _method(self, *method_args, **method_kwargs):
+        def _method(
+            self: BaseDeployment, *method_args: Any, **method_kwargs: Any
+        ) -> Callable:
+            self._target_workspace = cast(WorkSpace, self._target_workspace)
             with redirect_stdout(open(os.devnull, "w")):
                 if self._target_workspace.space_id is not None:
-                    self._target_workspace.api_client.set.default_space(
-                        self._target_workspace.space_id) if self._target_workspace.api_client.ICP else None
+                    (
+                        self._target_workspace.api_client.set.default_space(
+                            self._target_workspace.space_id
+                        )
+                        if self._target_workspace.api_client.ICP_PLATFORM_SPACES
+                        else None
+                    )
 
             try:
                 return method(self, *method_args, **method_kwargs)
 
             finally:
-                if  self._target_workspace.project_id:
+                if self._target_workspace.project_id:
                     with redirect_stdout(open(os.devnull, "w")):
                         if self._target_workspace.project_id is not None:
-                            self._target_workspace.api_client.set.default_project(
-                                self._target_workspace.project_id) if self._target_workspace.api_client.ICP else None
+                            (
+                                self._target_workspace.api_client.set.default_project(
+                                    self._target_workspace.project_id
+                                )
+                                if self._target_workspace.api_client.ICP_PLATFORM_SPACES
+                                else None
+                            )
 
         return _method
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/batch.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/batch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
+from __future__ import annotations
+
 import io
 import os
 import time
-from typing import TYPE_CHECKING, Any, Dict, Union, List, Optional
+from typing import TYPE_CHECKING, Any, cast
 
 import pandas as pd
-from pandas import DataFrame, concat
+from pandas import DataFrame
 
 from .base_deployment import BaseDeployment
 from ..helpers import DataConnection, AssetLocation
 from ..utils import StatusLogger, print_text_header_h1
-from ..utils.autoai.connection import validate_source_data_connections, validate_deployment_output_connection
-from ..utils.autoai.utils import init_cos_client, try_load_dataset, convert_dataframe_to_fields_values_payload
+from ..utils.autoai.connection import (
+    validate_source_data_connections,
+    validate_deployment_output_connection,
+)
+from ..utils.autoai.utils import convert_dataframe_to_fields_values_payload
 from ..utils.autoai.errors import NoneDataConnection
 from ..utils.deployment.errors import BatchJobFailed, MissingScoringResults
 from ..wml_client_error import WMLClientError
-from ibm_watsonx_ai.utils.autoai.enums import DataConnectionTypes
 
 if TYPE_CHECKING:
     from sklearn.pipeline import Pipeline
     from pandas import DataFrame
     from numpy import ndarray
     from ..workspace import WorkSpace
+    from ..credentials import Credentials
 
-__all__ = [
-    "Batch"
-]
+__all__ = ["Batch"]
 
 
 class Batch(BaseDeployment):
     """The Batch Deployment class.
     With this class object you can manage any batch deployment.
 
     :param source_instance_credentials: credentials to the instance where training was performed
@@ -52,59 +55,63 @@
     :type target_project_id: str, optional
 
     :param target_space_id: ID of the Watson Studio Space where you want to deploy
     :type target_space_id: str, optional
 
     """
 
-    def __init__(self,
-                 source_instance_credentials: Union[dict, 'WorkSpace'] = None,
-                 source_project_id: str = None,
-                 source_space_id: str = None,
-                 target_instance_credentials: Union[dict, 'WorkSpace'] = None,
-                 target_project_id: str = None,
-                 target_space_id: str = None,
-                 project_id: str = None,
-                 space_id: str = None,
-                 **kwargs):
+    def __init__(
+        self,
+        source_instance_credentials: Credentials | WorkSpace | None = None,
+        source_project_id: str | None = None,
+        source_space_id: str | None = None,
+        target_instance_credentials: Credentials | WorkSpace | None = None,
+        target_project_id: str | None = None,
+        target_space_id: str | None = None,
+        project_id: str | None = None,
+        space_id: str | None = None,
+        **kwargs: Any,
+    ):
 
         super().__init__(
-            deployment_type='batch',
-            source_wml_credentials=kwargs.get('source_wml_credentials'),
+            deployment_type="batch",
+            source_wml_credentials=kwargs.get("source_wml_credentials"),
             source_project_id=source_project_id,
             source_space_id=source_space_id,
-            target_wml_credentials=kwargs.get('target_wml_credentials'),
+            target_wml_credentials=kwargs.get("target_wml_credentials"),
             target_project_id=target_project_id,
             target_space_id=target_space_id,
             project_id=project_id,
             space_id=space_id,
             source_instance_credentials=source_instance_credentials,
-            target_instance_credentials=target_instance_credentials
+            target_instance_credentials=target_instance_credentials,
         )
 
         self.name = None
         self.id = None
-        self.asset_id = None
+        self.asset_id: str | None = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"name: {self.name}, id: {self.id}, asset_id: {self.asset_id}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"name: {self.name}, id: {self.id}, asset_id: {self.asset_id}"
 
-    def score(self, **kwargs):
+    def score(self, **kwargs: Any) -> dict:
         raise NotImplementedError("Batch deployment supports only job runs.")
 
-    def create(self,
-               model: str,
-               deployment_name: str,
-               metadata: Optional[Dict] = None,
-               training_data: Optional[Union['DataFrame', 'ndarray']] = None,
-               training_target: Optional[Union['DataFrame', 'ndarray']] = None,
-               experiment_run_id: Optional[str] = None) -> None:
+    def create(  # type: ignore[override]
+        self,
+        model: str,
+        deployment_name: str,
+        metadata: dict | None = None,
+        training_data: DataFrame | ndarray | None = None,
+        training_target: DataFrame | ndarray | None = None,
+        experiment_run_id: str | None = None,
+    ) -> None:
         """Create deployment from a model.
 
         :param model: AutoAI model name
         :type model: str
 
         :param deployment_name: name of the deployment
         :type deployment_name: str
@@ -142,33 +149,42 @@
 
             deployment.create(
                    experiment_run_id="...",
                    model=model,
                    deployment_name='My new deployment'
                )
         """
-        return super().create(model=model,
-                              deployment_name=deployment_name,
-                              metadata=metadata,
-                              training_data=training_data,
-                              training_target=training_target,
-                              experiment_run_id=experiment_run_id,
-                              deployment_type='batch')
+        return super().create(
+            model=model,
+            deployment_name=deployment_name,
+            metadata=metadata,
+            training_data=training_data,
+            training_target=training_target,
+            experiment_run_id=experiment_run_id,
+            deployment_type="batch",
+        )
 
     @BaseDeployment._project_to_space_to_project
-    def get_params(self) -> Dict:
+    def get_params(self) -> dict:
         """Get deployment parameters."""
         return super().get_params()
 
     @BaseDeployment._project_to_space_to_project
-    def run_job(self,
-                payload: Union[DataFrame, List[DataConnection], Dict[str, DataFrame], Dict[str, DataConnection]] = pd.DataFrame(),
-                output_data_reference: 'DataConnection' = None,
-                transaction_id: str = None,
-                background_mode: 'bool' = True) -> Union[Dict, Dict[str, List], DataConnection]:
+    def run_job(
+        self,
+        payload: (
+            DataFrame
+            | list[DataConnection]
+            | dict[str, DataFrame]
+            | dict[str, DataConnection]
+        ) = pd.DataFrame(),
+        output_data_reference: DataConnection | None = None,
+        transaction_id: str | None = None,
+        background_mode: bool = True,
+    ) -> dict | DataConnection:
         """Batch scoring job. Payload or Payload data reference is required.
         It is passed to the Service where model have been deployed.
 
         :param payload: DataFrame that contains data to test the model or data storage connection details
             that inform the model where payload data is stored
         :type payload: pandas.DataFrame or List[DataConnection] or Dict
 
@@ -207,166 +223,219 @@
 
             payload_reference = DataConnection(location=DSLocation(asset_id=asset_id))
             score_details = batch_service.run_job(payload=payload_reference, output_data_filename = "scoring_output.csv")
             score_details = batch_service.run_job(payload={'observations': payload_reference})
             score_details = batch_service.run_job(payload=[payload_reference])
             score_details = batch_service.run_job(payload={'observations': payload_reference, 'supporting_features': supporting_features_reference})  # supporting features time series forecasting sceanrio
         """
-
+        self._target_workspace: WorkSpace
+        input_data: list[DataConnection] | list[dict]
+        scoring_payload: dict
         if isinstance(payload, dict):
-            observations = payload.get('observations', pd.DataFrame())
-            supporting_features = payload.get('supporting_features')
+            observations = payload.get("observations", pd.DataFrame())
+            supporting_features = payload.get("supporting_features")
 
-            if isinstance(observations, DataFrame) and \
-                    (isinstance(supporting_features, DataFrame) or supporting_features is None):
-                observations_payload = convert_dataframe_to_fields_values_payload(observations, return_values_only=True)
-                observations_payload['id'] = 'observations'
+            if isinstance(observations, DataFrame) and (
+                isinstance(supporting_features, DataFrame)
+                or supporting_features is None
+            ):
+                observations_payload = convert_dataframe_to_fields_values_payload(
+                    observations, return_values_only=True
+                )
+                observations_payload["id"] = "observations"
                 input_data = [observations_payload]
 
                 if supporting_features is not None:
-                    supporting_features_payload = convert_dataframe_to_fields_values_payload(supporting_features, return_values_only=True)
-                    supporting_features_payload['id'] = 'supporting_features'
+                    supporting_features_payload = (
+                        convert_dataframe_to_fields_values_payload(
+                            supporting_features, return_values_only=True
+                        )
+                    )
+                    supporting_features_payload["id"] = "supporting_features"
                     input_data.append(supporting_features_payload)
 
                 scoring_payload = {
                     self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA: input_data
                 }
 
-            elif isinstance(observations, DataConnection) and \
-                    (isinstance(supporting_features, DataConnection) or supporting_features is None):
+            elif isinstance(observations, DataConnection) and (
+                isinstance(supporting_features, DataConnection)
+                or supporting_features is None
+            ):
 
-                observations.id = 'observations'
+                observations.id = "observations"
                 input_data = [observations]
                 if supporting_features is not None:
-                    supporting_features.id = 'supporting_features'
+                    supporting_features.id = "supporting_features"
                     input_data.append(supporting_features)
 
                 for data_conn in input_data:
-                    if hasattr(data_conn, 'location') and isinstance(data_conn.location, AssetLocation):
-                        data_conn.location.api_client = self._target_workspace.api_client
+                    if hasattr(data_conn, "location") and isinstance(
+                        data_conn.location, AssetLocation
+                    ):
+                        data_conn.location.api_client = (
+                            self._target_workspace.api_client
+                        )
 
-                input_data = validate_source_data_connections(source_data_connections=input_data,
-                                                              workspace=self._target_workspace,
-                                                              deployment=True)
-                input_data = [data_connection._to_dict() for data_connection in input_data]
+                input_data = validate_source_data_connections(
+                    source_data_connections=input_data,
+                    workspace=self._target_workspace,
+                    deployment=True,
+                )
+                input_data = [
+                    data_connection._to_dict() for data_connection in input_data
+                ]
 
                 if output_data_reference is None:
-                    raise ValueError("\"output_data_reference\" should be provided.")
+                    raise ValueError('"output_data_reference" should be provided.')
 
                 if isinstance(output_data_reference, DataConnection):
 
                     # api_client sets correct href for Data Assets
-                    if hasattr(output_data_reference, 'location') and isinstance(output_data_reference.location,
-                                                                                 AssetLocation):
-                        output_data_reference.location.api_client = self._target_workspace.api_client
+                    if hasattr(output_data_reference, "location") and isinstance(
+                        output_data_reference.location, AssetLocation
+                    ):
+                        output_data_reference.location.api_client = (
+                            self._target_workspace.api_client
+                        )
 
+                    input_data = cast(list[DataConnection], input_data)
                     output_data_reference = validate_deployment_output_connection(
                         results_data_connection=output_data_reference,
                         workspace=self._target_workspace,
-                        source_data_connections=input_data)
-                    output_data_reference = output_data_reference._to_dict()
+                        source_data_connections=input_data,
+                    )
+                    output_data_reference = output_data_reference._to_dict()  # type: ignore[assignment]
 
+                input_data = cast(list[dict], input_data)
                 scoring_payload = {
                     self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA_REFERENCES: input_data,
-                    self._target_workspace.api_client.deployments.ScoringMetaNames.OUTPUT_DATA_REFERENCE:
-                        output_data_reference}
+                    self._target_workspace.api_client.deployments.ScoringMetaNames.OUTPUT_DATA_REFERENCE: output_data_reference,
+                }
 
             else:
-                raise TypeError('Missing data observations in payload or observations '
-                                 'or supporting_features are not pandas.DataFrames.')
+                raise TypeError(
+                    "Missing data observations in payload or observations "
+                    "or supporting_features are not pandas.DataFrames."
+                )
         # note: support for DataFrame payload
         elif isinstance(payload, DataFrame):
             scoring_payload = {
-                self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA: [{'values': payload}]
+                self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA: [
+                    {"values": payload}
+                ]
             }
         # note: support for DataConnections and dictionaries payload
         elif isinstance(payload, list):
             if isinstance(payload[0], DataConnection):
                 if None in payload:
-                    raise NoneDataConnection('payload')
+                    raise NoneDataConnection("payload")
 
                 # api_client sets correct href for Data Assets
                 for data_conn in payload:
-                    if hasattr(data_conn, 'location') and isinstance(data_conn.location, AssetLocation):
-                        data_conn.location.api_client = self._target_workspace.api_client
-
-                payload = [new_conn for conn in payload for new_conn in conn._subdivide_connection()]
-                payload = validate_source_data_connections(source_data_connections=payload,
-                                                           workspace=self._target_workspace,
-                                                           deployment=True)
-                payload = [data_connection._to_dict() for data_connection in payload]
+                    if hasattr(data_conn, "location") and isinstance(
+                        data_conn.location, AssetLocation
+                    ):
+                        data_conn.location.api_client = (
+                            self._target_workspace.api_client
+                        )
+
+                payload = [
+                    new_conn
+                    for conn in payload
+                    for new_conn in conn._subdivide_connection()
+                ]
+                payload = validate_source_data_connections(
+                    source_data_connections=payload,
+                    workspace=self._target_workspace,
+                    deployment=True,
+                )
+                payload = [data_connection._to_dict() for data_connection in payload]  # type: ignore[assignment]
             elif isinstance(payload[0], dict):
                 pass
             else:
-                raise ValueError(f"Current payload type: list of {type(payload[0])} is not supported.")
+                raise ValueError(
+                    f"Current payload type: list of {type(payload[0])} is not supported."
+                )
 
             if output_data_reference is None:
-                raise ValueError("\"output_data_reference\" should be provided.")
+                raise ValueError('"output_data_reference" should be provided.')
 
             if isinstance(output_data_reference, DataConnection):
 
                 # api_client sets correct href for Data Assets
-                if hasattr(output_data_reference, 'location') and isinstance(output_data_reference.location, AssetLocation):
-                    output_data_reference.location.api_client = self._target_workspace.api_client
+                if hasattr(output_data_reference, "location") and isinstance(
+                    output_data_reference.location, AssetLocation
+                ):
+                    output_data_reference.location.api_client = (
+                        self._target_workspace.api_client
+                    )
 
                 output_data_reference = validate_deployment_output_connection(
                     results_data_connection=output_data_reference,
                     workspace=self._target_workspace,
-                    source_data_connections=payload)
-                output_data_reference = output_data_reference._to_dict()
+                    source_data_connections=payload,
+                )
+                output_data_reference = output_data_reference._to_dict()  # type: ignore[assignment]
 
             scoring_payload = {
                 self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA_REFERENCES: payload,
-                self._target_workspace.api_client.deployments.ScoringMetaNames.OUTPUT_DATA_REFERENCE:
-                    output_data_reference}
+                self._target_workspace.api_client.deployments.ScoringMetaNames.OUTPUT_DATA_REFERENCE: output_data_reference,
+            }
 
         else:
             raise ValueError(
-                f"Incorrect payload type. Required: DataFrame or List[DataConnection], Passed: {type(payload)}")
+                f"Incorrect payload type. Required: DataFrame or List[DataConnection], Passed: {type(payload)}"
+            )
 
-        scoring_payload['hybrid_pipeline_hardware_specs'] = [
-            {
-                'node_runtime_id': 'auto_ai.kb',
-                'hardware_spec': {
-                    'name': 'M'
-                }
-            }
+        scoring_payload["hybrid_pipeline_hardware_specs"] = [
+            {"node_runtime_id": "auto_ai.kb", "hardware_spec": {"name": "M"}}
         ]
 
-        job_details = self._target_workspace.api_client.deployments.create_job(self.id,
-                                                                               scoring_payload, _asset_id=self.asset_id)
-
+        self.id = cast(str, self.id)
+        job_details = self._target_workspace.api_client.deployments.create_job(
+            self.id, scoring_payload, _asset_id=self.asset_id
+        )
+        job_details = cast(dict, job_details)
         if background_mode:
             return job_details
 
         else:
             # note: monitor scoring job
-            job_id = self._target_workspace.api_client.deployments.get_job_uid(job_details)
-            print_text_header_h1(u'Synchronous scoring for id: \'{}\' started'.format(job_id))
 
-            status = self.get_job_status(job_id)['state']
+            job_id = self._target_workspace.api_client.deployments.get_job_id(
+                job_details
+            )
+            print_text_header_h1(
+                "Synchronous scoring for id: '{}' started".format(job_id)
+            )
+
+            status = self.get_job_status(job_id)["state"]
 
             with StatusLogger(status) as status_logger:
-                while status not in ['failed', 'error', 'completed', 'canceled']:
+                while status not in ["failed", "error", "completed", "canceled"]:
                     time.sleep(10)
-                    status = self.get_job_status(job_id)['state']
+                    status = self.get_job_status(job_id)["state"]
                     status_logger.log_state(status)
             # --- end note
 
-            if u'completed' in status:
-                print(u'\nScoring job  \'{}\' finished successfully.'.format(job_id))
+            if "completed" in status:
+                print("\nScoring job  '{}' finished successfully.".format(job_id))
             else:
-                raise BatchJobFailed(job_id, f"Scoring job failed with status: {self.get_job_status(job_id)}")
+                raise BatchJobFailed(
+                    job_id,
+                    f"Scoring job failed with status: {self.get_job_status(job_id)}",
+                )
 
             return self.get_job_params(job_id)
 
     @BaseDeployment._project_to_space_to_project
-    def rerun_job(self,
-                  scoring_job_id: str,
-                  background_mode: bool = True) -> Union[dict, 'DataFrame', 'DataConnection']:
+    def rerun_job(
+        self, scoring_job_id: str, background_mode: bool = True
+    ) -> dict | DataFrame | DataConnection:
         """Rerun scoring job with the same parameters as job described by `scoring_job_id`.
 
         :param scoring_job_id: Id described scoring job
         :type scoring_job_id: str
 
         :param background_mode: indicator if score_rerun() method will run in background (async) or (sync)
         :type background_mode: bool, optional
@@ -376,33 +445,44 @@
 
         **Example**
 
         .. code-block:: python
 
             scoring_details = deployment.score_rerun(scoring_job_id)
         """
-        scoring_params = self.get_job_params(scoring_job_id)['entity']['scoring']
-        input_data_references = self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA_REFERENCES
-        output_data_reference = self._target_workspace.api_client.deployments.ScoringMetaNames.OUTPUT_DATA_REFERENCE
+        scoring_params = self.get_job_params(scoring_job_id)["entity"]["scoring"]
+        input_data_references = (
+            self._target_workspace.api_client.deployments.ScoringMetaNames.INPUT_DATA_REFERENCES
+        )
+        output_data_reference = (
+            self._target_workspace.api_client.deployments.ScoringMetaNames.OUTPUT_DATA_REFERENCE
+        )
 
         if input_data_references in scoring_params:
-            payload_ref = [input_ref for input_ref in scoring_params[input_data_references]]
-
-            if 'href' in scoring_params[output_data_reference]['location']:
-                del scoring_params[output_data_reference]['location']['href']
-
-            return self.run_job(payload=payload_ref, output_data_reference=scoring_params['output_data_reference'],
-                                background_mode=background_mode)
+            payload_ref = [
+                input_ref for input_ref in scoring_params[input_data_references]
+            ]
+
+            if "href" in scoring_params[output_data_reference]["location"]:
+                del scoring_params[output_data_reference]["location"]["href"]
+
+            return self.run_job(
+                payload=payload_ref,
+                output_data_reference=scoring_params["output_data_reference"],
+                background_mode=background_mode,
+            )
         else:
-            raise NotImplementedError("'rerun_job' method supports only jobs with "
-                                      "payload passed as a list of DataConnections. If you want to rerun job "
-                                      "with payload passed directly, please use 'run_job' one more time.")
+            raise NotImplementedError(
+                "'rerun_job' method supports only jobs with "
+                "payload passed as a list of DataConnections. If you want to rerun job "
+                "with payload passed directly, please use 'run_job' one more time."
+            )
 
     @BaseDeployment._project_to_space_to_project
-    def delete(self, deployment_id: str = None) -> None:
+    def delete(self, deployment_id: str | None = None) -> None:
         """Delete deployment.
 
         :param deployment_id: ID of the deployment to delete, if empty, current deployment will be deleted
         :type deployment_id: str, optional
 
         **Example**
 
@@ -410,18 +490,18 @@
 
             deployment = Batch(workspace=...)
             # Delete current deployment
             deployment.delete()
             # Or delete a specific deployment
             deployment.delete(deployment_id='...')
         """
-        super().delete(deployment_id=deployment_id, deployment_type='batch')
+        super().delete(deployment_id=deployment_id, deployment_type="batch")
 
     @BaseDeployment._project_to_space_to_project
-    def list(self, limit=None) -> 'DataFrame':
+    def list(self, limit: int | None = None) -> DataFrame:
         """List deployments.
 
         :param limit: set the limit of how many deployments to list,
             default is `None` (all deployments should be fetched)
         :type limit: int, optional
 
         :return: Pandas DataFrame with information about deployments
@@ -439,15 +519,15 @@
             #                  created_at  ...  status
             # 0  2020-03-06T10:50:49.401Z  ...   ready
             # 1  2020-03-06T13:16:09.789Z  ...   ready
             # 4  2020-03-11T14:46:36.035Z  ...  failed
             # 3  2020-03-11T14:49:55.052Z  ...  failed
             # 2  2020-03-11T15:13:53.708Z  ...   ready
         """
-        return super().list(limit=limit, deployment_type='batch')
+        return super().list(limit=limit, deployment_type="batch")
 
     @BaseDeployment._project_to_space_to_project
     def get(self, deployment_id: str) -> None:
         """Get deployment.
 
         :param deployment_id: ID of the deployment to work with
         :type deployment_id: str
@@ -455,145 +535,169 @@
         **Example**
 
         .. code-block:: python
 
             deployment = Batch(workspace=...)
             deployment.get(deployment_id="...")
         """
-        super().get(deployment_id=deployment_id, deployment_type='batch')
+        super().get(deployment_id=deployment_id, deployment_type="batch")
 
     @BaseDeployment._project_to_space_to_project
-    def get_job_params(self, scoring_job_id: str = None) -> Dict:
+    def get_job_params(self, scoring_job_id: str | None = None) -> dict:
         """Get batch deployment job parameters.
 
         :param scoring_job_id: Id of scoring job
         :type scoring_job_id: str
 
         :return: parameters of the scoring job
         :rtype: dict
         """
-        return self._target_workspace.api_client.deployments.get_job_details(scoring_job_id)
+        return self._target_workspace.api_client.deployments.get_job_details(
+            scoring_job_id
+        )
 
     @BaseDeployment._project_to_space_to_project
-    def get_job_status(self, scoring_job_id: str) -> Dict:
+    def get_job_status(self, scoring_job_id: str) -> dict:
         """Get status of scoring job.
 
         :param scoring_job_id: Id of scoring job
         :type scoring_job_id: str
 
         :return: dictionary with state of scoring job (one of: [completed, failed, starting, queued])
             and additional details if they exist
         :rtype: dict
         """
-        return self._target_workspace.api_client.deployments.get_job_status(scoring_job_id)
+        return self._target_workspace.api_client.deployments.get_job_status(
+            scoring_job_id
+        )
 
     @BaseDeployment._project_to_space_to_project
-    def get_job_result(self, scoring_job_id: str) -> 'DataFrame':
+    def get_job_result(self, scoring_job_id: str) -> DataFrame:
         """Get batch deployment results of job with id `scoring_job_id`.
 
         :param scoring_job_id: Id of scoring job which results will be returned
         :type scoring_job_id: str
 
         :return: result
         :rtype: pandas.DataFrame
 
         :raises MissingScoringResults: in case of incompleted or failed job
             `MissingScoringResults` scoring exception is raised
         """
-        scoring_params = self.get_job_params(scoring_job_id)['entity']['scoring']
-        if scoring_params['status']['state'] == 'completed':
-            if 'predictions' in scoring_params:
-                data = DataFrame(scoring_params['predictions'][0]['values'], columns=scoring_params['predictions'][0]['fields'])
+        scoring_params = self.get_job_params(scoring_job_id)["entity"]["scoring"]
+        if scoring_params["status"]["state"] == "completed":
+            if "predictions" in scoring_params:
+                data = DataFrame(
+                    scoring_params["predictions"][0]["values"],
+                    columns=scoring_params["predictions"][0]["fields"],
+                )
                 return data
             else:
-                conn = DataConnection._from_dict(scoring_params['output_data_reference'])
+                conn = DataConnection._from_dict(
+                    scoring_params["output_data_reference"]
+                )
                 conn._api_client = self._target_workspace.api_client
 
-                return conn.read(raw=True) # if in future output may be excel file or with custom separator, here it should be recognized
+                return conn.read(
+                    raw=True
+                )  # if in future output may be excel file or with custom separator, here it should be recognized
         else:
-            raise MissingScoringResults(scoring_job_id, reason="Scoring is not completed.")
+            raise MissingScoringResults(
+                scoring_job_id, reason="Scoring is not completed."
+            )
 
     @BaseDeployment._project_to_space_to_project
-    def get_job_id(self, batch_scoring_details):
+    def get_job_id(self, batch_scoring_details: dict) -> str:
         """Get id from batch scoring details."""
-        return self._target_workspace.api_client.deployments.get_job_uid(batch_scoring_details)
+        return self._target_workspace.api_client.deployments.get_job_id(
+            batch_scoring_details
+        )
 
     @BaseDeployment._project_to_space_to_project
-    def list_jobs(self):
+    def list_jobs(self) -> DataFrame:
         """Returns pandas DataFrame with list of deployment jobs"""
 
-        resources = self._target_workspace.api_client.deployments.get_job_details()['resources']
-        columns = [u'job id', u'state', u'creted', u'deployment id']
+        resources = self._target_workspace.api_client.deployments.get_job_details()[
+            "resources"
+        ]
+        columns = ["job id", "state", "creted", "deployment id"]
         values = []
         for scoring_details in resources:
-            if 'scoring' in scoring_details['entity']:
-                state = scoring_details['entity']['scoring']['status']['state']
-                score_values = (scoring_details[u'metadata'][u'id'], state,
-                                scoring_details[u'metadata'][u'created_at'],
-                                scoring_details['entity']['deployment']['id'])
+            if "scoring" in scoring_details["entity"]:
+                state = scoring_details["entity"]["scoring"]["status"]["state"]
+                score_values = (
+                    scoring_details["metadata"]["id"],
+                    state,
+                    scoring_details["metadata"]["created_at"],
+                    scoring_details["entity"]["deployment"]["id"],
+                )
                 if self.id:
-                    if self.id == scoring_details['entity']['deployment']['id']:
+                    if self.id == scoring_details["entity"]["deployment"]["id"]:
                         values.append(score_values)
                 else:
                     values.append(score_values)
 
         return DataFrame(values, columns=columns)
 
     @BaseDeployment._project_to_space_to_project
-    def _deploy(self,
-                pipeline_model: 'Pipeline',
-                deployment_name: str,
-                meta_props: Dict,
-                serving_name=None, # Not used, but added to match unified parameters for _deploy
-                result_client=None,
-                hardware_spec=None) -> Dict: # Not used, but added to match unified parameters for _deploy
+    def _deploy(
+        self,
+        pipeline_model: Pipeline,
+        deployment_name: str,
+        meta_props: dict,
+        serving_name: (
+            str | None
+        ) = None,  # Not used, but added to match unified parameters for _deploy
+        result_client: str | None = None,
+        hardware_spec: str | None = None,
+    ) -> dict:  # Not used, but added to match unified parameters for _deploy
         """Deploy model into Service.
 
         :param pipeline_model: model of the pipeline to deploy
         :type pipeline_model: Pipeline or str
 
         :param deployment_name: name of the deployment
         :type deployment_name: str
 
         :param meta_props: model meta properties
         :type meta_props: dict
 
         :param result_client: tuple with Result DataConnection object and initialized COS client
         :type result_client: tuple[DataConnection, resource]
         """
-        deployment_details = {}
-        asset_uid = self._publish_model(pipeline_model=pipeline_model,
-                                        meta_props=meta_props)
+        deployment_details: dict | None = {}
+        deployment_props: dict[str, Any]
+        asset_uid = self._publish_model(
+            pipeline_model=pipeline_model, meta_props=meta_props
+        )
 
         self.asset_id = asset_uid
 
         deployment_props = {
             self._target_workspace.api_client.deployments.ConfigurationMetaNames.NAME: deployment_name,
-            self._target_workspace.api_client.deployments.ConfigurationMetaNames.BATCH: {}
+            self._target_workspace.api_client.deployments.ConfigurationMetaNames.BATCH: {},
         }
 
-        deployment_props[self._target_workspace.api_client.deployments.ConfigurationMetaNames.ASSET] = {
-            "id": asset_uid
-        }
+        deployment_props[
+            self._target_workspace.api_client.deployments.ConfigurationMetaNames.ASSET
+        ] = {"id": asset_uid}
 
         deployment_props[
-            self._target_workspace.api_client.deployments.ConfigurationMetaNames.HYBRID_PIPELINE_HARDWARE_SPECS] = [
-            {
-                'node_runtime_id': 'auto_ai.kb',
-                'hardware_spec': {
-                    'name': 'M'
-                }
-            }
-        ]
+            self._target_workspace.api_client.deployments.ConfigurationMetaNames.HYBRID_PIPELINE_HARDWARE_SPECS
+        ] = [{"node_runtime_id": "auto_ai.kb", "hardware_spec": {"name": "M"}}]
 
         print("Deploying model {} using V4 client.".format(asset_uid))
         try:
             deployment_details = self._target_workspace.api_client.deployments.create(
-                artifact_uid=asset_uid,
-                meta_props=deployment_props)
-
-            self.deployment_id = self._target_workspace.api_client.deployments.get_uid(deployment_details)
+                artifact_uid=asset_uid,  # type: ignore[arg-type]
+                meta_props=deployment_props,
+            )
+
+            deployment_details = cast(dict, deployment_details)
+            self.deployment_id = self._target_workspace.api_client.deployments.get_id(
+                deployment_details
+            )
 
         except WMLClientError as e:
             raise e
 
         return deployment_details
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/deployment/web_service.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/deployment/web_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, Union, List, Optional
+from typing import TYPE_CHECKING, Any, cast
 
 import pandas as pd
 from pandas import DataFrame
 
 from .base_deployment import BaseDeployment
 from ..wml_client_error import WMLClientError
 
 if TYPE_CHECKING:
     from sklearn.pipeline import Pipeline
-    from pandas import DataFrame
     from numpy import ndarray
     from ..workspace import WorkSpace
+    from ..credentials import Credentials
+    from ibm_watsonx_ai.helpers.connections import DataConnection
+    from ibm_boto3 import resource
 
-__all__ = [
-    "WebService"
-]
+__all__ = ["WebService"]
 
 
 class WebService(BaseDeployment):
     """An Online Deployment class aka. WebService.
     With this class object you can manage any online (WebService) deployment.
 
     :param source_instance_credentials: credentials to the instance where training was performed
@@ -42,59 +43,63 @@
     :type target_project_id: str, optional
 
     :param target_space_id: ID of the Watson Studio Space where you want to deploy
     :type target_space_id: str, optional
 
     """
 
-    def __init__(self,
-                 source_instance_credentials: Union[dict, 'WorkSpace'] = None,
-                 source_project_id: str = None,
-                 source_space_id: str = None,
-                 target_instance_credentials: Union[dict, 'WorkSpace'] = None,
-                 target_project_id: str = None,
-                 target_space_id: str = None,
-                 project_id: str = None,
-                 space_id: str = None,
-                 **kwargs):
+    def __init__(
+        self,
+        source_instance_credentials: Credentials | WorkSpace | None = None,
+        source_project_id: str | None = None,
+        source_space_id: str | None = None,
+        target_instance_credentials: Credentials | WorkSpace | None = None,
+        target_project_id: str | None = None,
+        target_space_id: str | None = None,
+        project_id: str | None = None,
+        space_id: str | None = None,
+        **kwargs: Any,
+    ):
 
         super().__init__(
-            deployment_type='online',
-            source_wml_credentials=kwargs.get('source_wml_credentials'),
+            deployment_type="online",
+            source_wml_credentials=kwargs.get("source_wml_credentials"),
             source_project_id=source_project_id,
             source_space_id=source_space_id,
-            target_wml_credentials=kwargs.get('target_wml_credentials'),
+            target_wml_credentials=kwargs.get("target_wml_credentials"),
             target_project_id=target_project_id,
             target_space_id=target_space_id,
             project_id=project_id,
             space_id=space_id,
             source_instance_credentials=source_instance_credentials,
-            target_instance_credentials=target_instance_credentials
+            target_instance_credentials=target_instance_credentials,
         )
 
-        self.name = None
-        self.scoring_url = None
-        self.id = None
-        self.asset_id = None
+        self.name: str | None = None
+        self.scoring_url: str | None = None
+        self.id: str | None = None
+        self.asset_id: str | None = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"name: {self.name}, id: {self.id}, scoring_url: {self.scoring_url}, asset_id: {self.asset_id}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"name: {self.name}, id: {self.id}, scoring_url: {self.scoring_url}, asset_id: {self.asset_id}"
 
-    def create(self,
-               model: str,
-               deployment_name: str,
-               serving_name: str = None,
-               metadata: Optional[Dict] = None,
-               training_data: Optional[Union['DataFrame', 'ndarray']] = None,
-               training_target: Optional[Union['DataFrame', 'ndarray']] = None,
-               experiment_run_id: Optional[str] = None,
-               hardware_spec: Optional[dict] = None) -> None:
+    def create(  # type: ignore[override]
+        self,
+        model: str,
+        deployment_name: str,
+        serving_name: str | None = None,
+        metadata: dict | None = None,
+        training_data: DataFrame | ndarray | None = None,
+        training_target: DataFrame | ndarray | None = None,
+        experiment_run_id: str | None = None,
+        hardware_spec: dict | None = None,
+    ) -> None:
         """Create deployment from a model.
 
         :param model: AutoAI model name
         :type model: str
 
         :param deployment_name: name of the deployment
         :type deployment_name: str
@@ -139,31 +144,37 @@
             deployment.create(
                    experiment_run_id="...",
                    model=model,
                    deployment_name='My new deployment',
                    serving_name='my_new_deployment'
                )
         """
-        return super().create(model=model,
-                              deployment_name=deployment_name,
-                              metadata=metadata,
-                              serving_name=serving_name,
-                              training_data=training_data,
-                              training_target=training_target,
-                              experiment_run_id=experiment_run_id,
-                              deployment_type='online',
-                              hardware_spec=hardware_spec)
+        return super().create(
+            model=model,
+            deployment_name=deployment_name,
+            metadata=metadata,
+            serving_name=serving_name,
+            training_data=training_data,
+            training_target=training_target,
+            experiment_run_id=experiment_run_id,
+            deployment_type="online",
+            hardware_spec=hardware_spec,
+        )
 
     @BaseDeployment._project_to_space_to_project
-    def get_params(self) -> Dict:
+    def get_params(self) -> dict:
         """Get deployment parameters."""
         return super().get_params()
 
     @BaseDeployment._project_to_space_to_project
-    def score(self, payload: Union[dict, 'DataFrame'] = pd.DataFrame(), transaction_id: str = None) -> Dict[str, List]:
+    def score(
+        self,
+        payload: dict | DataFrame = pd.DataFrame(),
+        transaction_id: str | None = None,
+    ) -> dict:
         """Online scoring. Payload is passed to the Service scoring endpoint where model have been deployed.
 
         :param payload: DataFrame with data to test the model or dictionary with keys `observations`
             and `supporting_features` and DataFrames with data for `observations` and `supporting_features`
             to score forecasting models
         :type payload: pandas.DataFrame or dict
 
@@ -191,15 +202,15 @@
 
             predictions = web_service.score(payload={'observations': new_observations_df})
             predictions = web_service.score(payload={'observations': new_observations_df, 'supporting_features': supporting_features_df}) # supporting features time series forecasting sceanrio
         """
         return super().score(payload=payload, transaction_id=transaction_id)
 
     @BaseDeployment._project_to_space_to_project
-    def delete(self, deployment_id: str = None) -> None:
+    def delete(self, deployment_id: str | None = None) -> None:
         """Delete deployment.
 
         :param deployment_id: ID of the deployment to delete, if empty, current deployment will be deleted
         :type deployment_id: str, optional
 
         **Example**
 
@@ -207,18 +218,18 @@
 
             deployment = WebService(workspace=...)
             # Delete current deployment
             deployment.delete()
             # Or delete a specific deployment
             deployment.delete(deployment_id='...')
         """
-        super().delete(deployment_id=deployment_id, deployment_type='online')
+        super().delete(deployment_id=deployment_id, deployment_type="online")
 
     @BaseDeployment._project_to_space_to_project
-    def list(self, limit=None) -> 'DataFrame':
+    def list(self, limit: int | None = None) -> DataFrame:
         """List deployments.
 
         :param limit: set the limit of how many deployments to list,
             default is `None` (all deployments should be fetched)
         :type limit: int, optional
 
         :return: Pandas DataFrame with information about deployments
@@ -236,15 +247,15 @@
             #                  created_at  ...  status
             # 0  2020-03-06T10:50:49.401Z  ...   ready
             # 1  2020-03-06T13:16:09.789Z  ...   ready
             # 4  2020-03-11T14:46:36.035Z  ...  failed
             # 3  2020-03-11T14:49:55.052Z  ...  failed
             # 2  2020-03-11T15:13:53.708Z  ...   ready
         """
-        return super().list(limit=limit, deployment_type='online')
+        return super().list(limit=limit, deployment_type="online")
 
     @BaseDeployment._project_to_space_to_project
     def get(self, deployment_id: str) -> None:
         """Get deployment.
 
         :param deployment_id: ID of the deployment to work with
         :type deployment_id: str
@@ -252,67 +263,80 @@
         **Example**
 
         .. code-block:: python
 
             deployment = WebService(workspace=...)
             deployment.get(deployment_id="...")
         """
-        super().get(deployment_id=deployment_id, deployment_type='online')
+        super().get(deployment_id=deployment_id, deployment_type="online")
 
     @BaseDeployment._project_to_space_to_project
-    def _deploy(self,
-                pipeline_model: 'Pipeline',
-                deployment_name: str,
-                meta_props: Dict,
-                serving_name=None,
-                result_client=None,
-                hardware_spec=None) -> Dict:
+    def _deploy(
+        self,
+        pipeline_model: Pipeline,
+        deployment_name: str,
+        meta_props: dict,
+        serving_name: str | None = None,
+        result_client: tuple[DataConnection, resource] | None = None,
+        hardware_spec: str | None = None,
+    ) -> dict:
         """Deploy model into Service.
 
         :param pipeline_model: model of the pipeline to deploy
         :type pipeline_model: Pipeline or str
 
         :param deployment_name: name of the deployment
         :type deployment_name: str
 
         :param meta_props: model meta properties
         :type meta_props: dict
 
         :param serving_name: serving name of the deployment
-        :type serving_name: str
+        :type serving_name: str, optional
 
         :param result_client: tuple with Result DataConnection object and initialized COS client
         :rtype: tuple[DataConnection, resource]
 
         :return: deployment details
         :rtype: dict
         """
-        asset_uid = self._publish_model(pipeline_model=pipeline_model,
-                                        meta_props=meta_props)
+        from ..workspace import WorkSpace
+
+        self._target_workspace = cast(WorkSpace, self._target_workspace)
+        deployment_details: dict | None
+        deployment_props: dict[str, Any]
+        asset_uid = self._publish_model(
+            pipeline_model=pipeline_model, meta_props=meta_props
+        )
 
         self.asset_id = asset_uid
 
-        conf_names = self._target_workspace.api_client.deployments.ConfigurationMetaNames
+        conf_names = (
+            self._target_workspace.api_client.deployments.ConfigurationMetaNames
+        )
 
-        deployment_props = {
-            conf_names.NAME: deployment_name,
-            conf_names.ONLINE: {}
-        }
+        deployment_props = {conf_names.NAME: deployment_name, conf_names.ONLINE: {}}
 
         if hardware_spec:
             deployment_props[conf_names.HARDWARE_SPEC] = hardware_spec
 
         if serving_name:
-            deployment_props[conf_names.ONLINE]["parameters"] = {conf_names.SERVING_NAME: serving_name}
+            deployment_props[conf_names.ONLINE]["parameters"] = {
+                conf_names.SERVING_NAME: serving_name
+            }
 
         print("Deploying model {} using V4 client.".format(asset_uid))
         try:
 
             deployment_details = self._target_workspace.api_client.deployments.create(
-                artifact_uid=asset_uid,
-                meta_props=deployment_props)
-            self.deployment_id = self._target_workspace.api_client.deployments.get_uid(deployment_details)
+                artifact_uid=asset_uid,  # type: ignore[arg-type]
+                meta_props=deployment_props,
+            )
+            deployment_details = cast(dict, deployment_details)
+            self.deployment_id = self._target_workspace.api_client.deployments.get_id(
+                deployment_details
+            )
 
         except WMLClientError as e:
             raise e
 
         return deployment_details
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/autoai.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/autoai.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 from .runs import AutoPipelinesRuns, LocalAutoPipelinesRuns
 from ..base_experiment.base_experiment import BaseExperiment
 
 __all__ = [
     "AutoAI"
 ]
 
+from ...credentials import Credentials
+
 
 class AutoAI(BaseExperiment):
     """AutoAI class for pipeline models optimization automation.
 
     :param credentials: credentials to instance
     :type credentials: dict
 
@@ -85,38 +87,45 @@
     Metrics = Metrics
     Transformers = Transformers
     DataConnectionTypes = DataConnectionTypes
     PipelineTypes = PipelineTypes
     SamplingTypes = SamplingTypes
 
     def __init__(self,
-                 credentials: Union[dict, 'WorkSpace'] = None,
+                 credentials: Union[Credentials, dict, 'WorkSpace'] = None,
                  project_id: str = None,
                  space_id: str = None,
                  verify=None,
                  **kwargs) -> None:
         # note: as workspace is not clear enough to understand, there is a possibility to use pure
         # credentials with project and space IDs, but in addition we
         # leave a possibility to use a previous WorkSpace implementation, it could be passed as a first argument
          # note: backward compatibility
         if (wml_credentials:=kwargs.get('wml_credentials')) is not None:
             if credentials is None:
                 credentials = wml_credentials
             warn(("`wml_credentials` is deprecated and will be removed in future. "
                     "Instead, please use `credentials`."), category=DeprecationWarning)
+
+        if isinstance(credentials, dict):
+            credentials = Credentials.from_dict(credentials, _verify=verify)
+
+        if isinstance(credentials, Credentials):
+            credentials._set_env_vars_from_credentials()
+
         # --- end note
         if credentials is None:
             self._workspace = None
             self.runs = LocalAutoPipelinesRuns()
 
         else:
             if isinstance(credentials, WorkSpace):
                 self._workspace = credentials
             else:
-                self._workspace = WorkSpace(credentials=credentials.copy(),
+                self._workspace = WorkSpace(credentials=copy.copy(credentials),
                                             project_id=project_id,
                                             space_id=space_id,
                                             verify=verify)
 
             self.project_id = self._workspace.project_id
             self.space_id = self._workspace.space_id
             self.runs = AutoPipelinesRuns(engine=ServiceEngine(self._workspace))
@@ -506,22 +515,16 @@
             retrain_on_holdout = True
 
         # Deprecation of excel_sheet as number:
         if isinstance(excel_sheet, int):
             warn(
                 message="Support for excel sheet as number of the sheet (int) is deprecated! Please set excel sheet with name of the sheet.")
 
-        if prediction_type == PredictionType.FORECASTING and self._workspace.api_client.ICP and \
-                (self._workspace.api_client.wml_credentials['version'].startswith('2.5') or \
-                        self._workspace.api_client.wml_credentials['version'].startswith('3.0') or \
-                        self._workspace.api_client.wml_credentials['version'].startswith('3.5')):
-            raise TSNotSupported()
-
-        if prediction_type == PredictionType.TIMESERIES_ANOMALY_PREDICTION and self._workspace.api_client.ICP and \
-                self._workspace.api_client.wml_credentials['version'].startswith(('2.5', '3.0', '3.5', '4.0', '4.5', '4.6')):
+        if prediction_type == PredictionType.TIMESERIES_ANOMALY_PREDICTION and self._workspace.api_client.ICP_PLATFORM_SPACES and \
+                self._workspace.api_client.credentials.version.startswith(('2.5', '3.0', '3.5', '4.0', '4.5', '4.6')):
             raise TSADNotSupported()
 
         if prediction_type in (PredictionType.FORECASTING, 'timeseries'):
             if not numerical_imputation_strategy and type(numerical_imputation_strategy) is not list:
                 numerical_imputation_strategy = ImputationStrategy.BEST_OF_DEFAULT_IMPUTERS
             elif not numerical_imputation_strategy and type(numerical_imputation_strategy) is list:
                 numerical_imputation_strategy = ImputationStrategy.NO_IMPUTATION
@@ -607,15 +610,15 @@
             daub_include_only_estimators=daub_include_only_estimators,
             include_only_estimators=include_only_estimators,
             include_batched_ensemble_estimators=include_batched_ensemble_estimators,
             cognito_transform_names=cognito_transform_names,
             imputation_strategies=[x for y in list(filter(None, [categorical_imputation_strategy, numerical_imputation_strategy])) for x in (y if type(y) is list else [y])],
             scoring=scoring,
             t_shirt_size=kwargs.get("t_shirt_size", TShirtSize.M),
-            is_cpd=self._workspace.api_client.ICP
+            is_cpd=self._workspace.api_client.ICP_PLATFORM_SPACES
         )
 
         if daub_give_priority_to_runtime is not None:
             if daub_give_priority_to_runtime < 0.0 or daub_give_priority_to_runtime > 5.0:
                 raise ParamOutOfRange('daub_give_priority_to_runtime', daub_give_priority_to_runtime, 0.0, 5.0)
 
         if (prediction_type == PredictionType.BINARY and scoring in vars(PositiveLabelClass).values()
@@ -684,15 +687,15 @@
                 prediction_columns=prediction_columns,
                 timestamp_column_name=timestamp_column_name,
                 scoring=scoring,
                 desc=desc,
                 holdout_size=holdout_size,
                 max_num_daub_ensembles=max_number_of_estimators,
                 t_shirt_size=self._workspace.restrict_pod_size(t_shirt_size=kwargs.get(
-                    't_shirt_size', TShirtSize.M if self._workspace.api_client.ICP else TShirtSize.L)
+                    't_shirt_size', TShirtSize.M if self._workspace.api_client.ICP_PLATFORM_SPACES else TShirtSize.L)
                 ),
                 train_sample_rows_test_size=train_sample_rows_test_size,
                 include_only_estimators=include_only_estimators,
                 include_batched_ensemble_estimators=include_batched_ensemble_estimators,
                 backtest_num=backtest_num,
                 lookback_window=lookback_window,
                 forecast_window=forecast_window,
@@ -738,15 +741,15 @@
                 feature_selector_mode=feature_selector_mode,
                 **reduced_kwargs
             )
             optimizer._workspace = self._workspace
             return optimizer
 
     def _init_estimator_enums(self):
-        if self._workspace and self._workspace.api_client.ICP:
+        if self._workspace and self._workspace.api_client.ICP_PLATFORM_SPACES:
             self.ClassificationAlgorithms = ClassificationAlgorithmsCP4D
             self.RegressionAlgorithms = RegressionAlgorithmsCP4D
             self.ForecastingAlgorithms = ForecastingAlgorithmsCP4D
         else:
             self.ClassificationAlgorithms = ClassificationAlgorithms
             self.RegressionAlgorithms = RegressionAlgorithms
             self.ForecastingAlgorithms = ForecastingAlgorithms
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/base_engine.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/service_engine.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/service_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,15 @@
                 self._pipeline_metadata[self._api_client.pipelines.ConfigurationMetaNames.DOCUMENT][
                     'pipelines'][0]['nodes'][0]['parameters']['optimization']['preprocessor_num_imp_strategy'] = \
                     get_values_for_imputation_strategy(
                         self._auto_pipelines_parameters.get('numerical_imputation_strategy'),
                         self._auto_pipelines_parameters.get('prediction_type'))
 
         # note: KB part: send version autoai_pod_version if set in pipeline details details (See supported formats)
-        if not self._api_client.ICP and self._auto_pipelines_parameters['autoai_pod_version'] is not None:
+        if not self._api_client.ICP_PLATFORM_SPACES and self._auto_pipelines_parameters['autoai_pod_version'] is not None:
             self._pipeline_metadata[
                 self._api_client.pipelines.ConfigurationMetaNames.DOCUMENT]['runtimes'][0]['version'] = (
                 self._auto_pipelines_parameters['autoai_pod_version'])
         # --- end note
 
 
     def _initialize_training_metadata(self,
@@ -631,15 +631,15 @@
 
         run_params = self._api_client.training.run(meta_props=self._training_metadata,
                                                    asynchronous=True)
 
         self._current_run_id = run_params['metadata'].get('id', run_params['metadata'].get('guid'))
 
         if background_mode:
-            return self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+            return self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         else:
             pipeline_details = self.get_params()
             number_of_estimators = pipeline_details.get('max_num_daub_ensembles', 2)
 
             base_url = self._api_client.service_instance._href_definitions.get_trainings_href()
             url = f"{base_url.replace('https', 'wss')}/{self._current_run_id}"
@@ -727,42 +727,42 @@
                 except:
                     websocket.close()
                     break
 
                 if disconnection_no >= attempts_no:
                     raise CannotConnectToWebsocket(attempts_no)
 
-            return self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+            return self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
     def get_run_status(self) -> str:
         """Check status/state of initialized AutoPipelineOptimizer run if ran in background mode.
 
         :return: run status
         :rtype: str
         """
 
         if self._current_run_id is None:
             raise FitNeeded(reason="Firstly schedule a fit job by using the fit() method.")
 
-        return self._api_client.training.get_status(training_uid=self._current_run_id).get('state')
+        return self._api_client.training.get_status(training_id=self._current_run_id).get('state')
 
     def get_run_details(self, include_metrics: bool = False) -> dict:
         """Get fit/run details.
 
         :param include_metrics: indicates to include metrics in the training details output
         :type include_metrics: bool, optional
 
         :return: AutoPipelineOptimizer fit/run details
         :rtype: dict
         """
 
         if self._current_run_id is None:
             raise FitNeeded(reason="Firstly schedule a fit job by using the fit() method.")
 
-        details = self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        details = self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         if include_metrics:
             return details
 
         if details['entity']['status'].get('metrics', False):
             del details['entity']['status']['metrics']
             return details
@@ -770,15 +770,15 @@
             return details
 
     def cancel_run(self) -> None:
         """Cancels an AutoAI run."""
         if self._current_run_id is None:
             raise FitNeeded(reason="To cancel an AutoAI run, first schedule a fit job by using the fit() method.")
 
-        self._api_client.training.cancel(training_uid=self._current_run_id)
+        self._api_client.training.cancel(training_id=self._current_run_id)
 
     #################################################################################
     #   Auto_AI Trained Pipelines Part / AutoPipelineOptimizer Pipelines Part   #
     #################################################################################
     def summary(self, scoring: str = None, sort_by_holdout_score: bool = True) -> 'DataFrame':
         """Prints AutoPipelineOptimizer Pipelines details (autoai trained pipelines).
 
@@ -792,15 +792,15 @@
 
         :return: DataFrame with computed pipelines and ML metrics
         :rtype: pandas.DataFrame
         """
         if self._current_run_id is None:
             raise FitNeeded(reason="To list computed pipelines, first schedule a fit job by using the fit() method.")
 
-        details = self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        details = self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
         optimized_scoring = self._auto_pipelines_parameters.get('scoring', None)
 
         if scoring is None:
             scoring = optimized_scoring
 
         summary = create_summary(details=details, scoring=scoring, sort_by_holdout_score=sort_by_holdout_score)
 
@@ -822,15 +822,15 @@
 
         if self._current_run_id is None:
             raise FitNeeded(reason="To list computed pipelines parameters, "
                                    "first schedule a fit job by using a fit() method.")
 
         if pipeline_name is None:
             pipeline_name = self.summary().index[0]
-        run_params = self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        run_params = self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         pipeline_parameters = {
             "composition_steps": [],
             "pipeline_nodes": [],
         }
 
         # note: retrieve all additional pipeline evaluation information
@@ -1064,15 +1064,15 @@
         :param persist: indicates if selected pipeline should be stored locally
         :type persist: bool, optional
 
         :return: Scikit-Learn pipeline and lale check result
         :rtype: tuple[Pipeline, bool]
         """
 
-        run_params = self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        run_params = self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         # note: recreation of s3 creds from connection asset
         results_reference = DataConnection._from_dict(run_params['entity']['results_reference'])
         results_reference._api_client = self._api_client
         results_reference._check_if_connection_asset_is_s3()
         run_params['entity']['results_reference'] = results_reference._to_dict()
         # --- end note
@@ -1115,15 +1115,15 @@
         :param filename: filename under which the pipeline notebook will be saved
         :type filename: str, optional
 
         :return: path to saved pipeline notebook
         :rtype: str
         """
 
-        run_params = self._api_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        run_params = self._api_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         # note: recreation of s3 creds from connection asset
         results_reference = DataConnection._from_dict(run_params['entity']['results_reference'])
         results_reference._api_client = self._api_client
         results_reference._check_if_connection_asset_is_s3()
         run_params['entity']['results_reference'] = results_reference._to_dict()
         # --- end note
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/engines/wml_engine.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/engines/wml_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
                 self._wml_pipeline_metadata[self._wml_client.pipelines.ConfigurationMetaNames.DOCUMENT][
                     'pipelines'][0]['nodes'][0]['parameters']['optimization']['preprocessor_num_imp_strategy'] = \
                     get_values_for_imputation_strategy(
                         self._auto_pipelines_parameters.get('numerical_imputation_strategy'),
                         self._auto_pipelines_parameters.get('prediction_type'))
 
         # note: KB part: send version autoai_pod_version if set in pipeline details details (See supported formats)
-        if not self._wml_client.ICP and self._auto_pipelines_parameters['autoai_pod_version'] is not None:
+        if not self._wml_client.ICP_PLATFORM_SPACES and self._auto_pipelines_parameters['autoai_pod_version'] is not None:
             self._wml_pipeline_metadata[
                 self._wml_client.pipelines.ConfigurationMetaNames.DOCUMENT]['runtimes'][0]['version'] = (
                 self._auto_pipelines_parameters['autoai_pod_version'])
         # --- end note
 
 
     def _initialize_wml_training_metadata(self,
@@ -635,15 +635,15 @@
 
         run_params = self._wml_client.training.run(meta_props=self._wml_training_metadata,
                                                    asynchronous=True)
 
         self._current_run_id = run_params['metadata'].get('id', run_params['metadata'].get('guid'))
 
         if background_mode:
-            return self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+            return self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         else:
             wml_pipeline_details = self.get_params()
             number_of_estimators = wml_pipeline_details.get('max_num_daub_ensembles', 2)
 
             base_url = self._wml_client.service_instance._href_definitions.get_trainings_href()
             url = f"{base_url.replace('https', 'wss')}/{self._current_run_id}"
@@ -739,42 +739,42 @@
                 except:
                     websocket.close()
                     break
 
                 if disconnection_no >= attempts_no:
                     raise CannotConnectToWebsocket(attempts_no)
 
-            return self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+            return self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
     def get_run_status(self) -> str:
         """Check status/state of initialized AutoPipelineOptimizer run if ran in background mode.
 
         :return: run status
         :rtype: str
         """
 
         if self._current_run_id is None:
             raise FitNeeded(reason="Firstly schedule a fit job by using the fit() method.")
 
-        return self._wml_client.training.get_status(training_uid=self._current_run_id).get('state')
+        return self._wml_client.training.get_status(training_id=self._current_run_id).get('state')
 
     def get_run_details(self, include_metrics: bool = False) -> dict:
         """Get fit/run details.
 
         :param include_metrics: indicates to include metrics in the training details output
         :type include_metrics: bool, optional
 
         :return: AutoPipelineOptimizer fit/run details
         :rtype: dict
         """
 
         if self._current_run_id is None:
             raise FitNeeded(reason="Firstly schedule a fit job by using the fit() method.")
 
-        details = self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        details = self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         if include_metrics:
             return details
 
         if details['entity']['status'].get('metrics', False):
             del details['entity']['status']['metrics']
             return details
@@ -782,15 +782,15 @@
             return details
 
     def cancel_run(self) -> None:
         """Cancels an AutoAI run."""
         if self._current_run_id is None:
             raise FitNeeded(reason="To cancel an AutoAI run, first schedule a fit job by using the fit() method.")
 
-        self._wml_client.training.cancel(training_uid=self._current_run_id)
+        self._wml_client.training.cancel(training_id=self._current_run_id)
 
     #################################################################################
     #   WML Auto_AI Trained Pipelines Part / AutoPipelineOptimizer Pipelines Part   #
     #################################################################################
     def summary(self, scoring: str = None, sort_by_holdout_score: bool = True) -> 'DataFrame':
         """Prints AutoPipelineOptimizer Pipelines details (autoai trained pipelines).
 
@@ -804,15 +804,15 @@
 
         :return: DataFrame with computed pipelines and ML metrics
         :rtype: pandas.DataFrame
         """
         if self._current_run_id is None:
             raise FitNeeded(reason="To list computed pipelines, first schedule a fit job by using the fit() method.")
 
-        details = self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        details = self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
         optimized_scoring = self._auto_pipelines_parameters.get('scoring', None)
 
         if scoring is None:
             scoring = optimized_scoring
 
         summary = create_summary(details=details, scoring=scoring, sort_by_holdout_score=sort_by_holdout_score)
 
@@ -834,15 +834,15 @@
 
         if self._current_run_id is None:
             raise FitNeeded(reason="To list computed pipelines parameters, "
                                    "first schedule a fit job by using a fit() method.")
 
         if pipeline_name is None:
             pipeline_name = self.summary().index[0]
-        run_params = self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        run_params = self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         pipeline_parameters = {
             "composition_steps": [],
             "pipeline_nodes": [],
         }
 
         # note: retrieve all additional pipeline evaluation information
@@ -1076,15 +1076,15 @@
         :param persist: indicates if selected pipeline should be stored locally
         :type persist: bool, optional
 
         :return: Scikit-Learn pipeline and lale check result
         :rtype: tuple[Pipeline, bool]
         """
 
-        run_params = self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        run_params = self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         # note: recreation of s3 creds from connection asset
         results_reference = DataConnection._from_dict(run_params['entity']['results_reference'])
         results_reference._api_client = self._wml_client
         results_reference._check_if_connection_asset_is_s3()
         run_params['entity']['results_reference'] = results_reference._to_dict()
         # --- end note
@@ -1127,15 +1127,15 @@
         :param filename: filename under which the pipeline notebook will be saved
         :type filename: str, optional
 
         :return: path to saved pipeline notebook
         :rtype: str
         """
 
-        run_params = self._wml_client.training.get_details(training_uid=self._current_run_id, _internal=True)
+        run_params = self._wml_client.training.get_details(training_id=self._current_run_id, _internal=True)
 
         # note: recreation of s3 creds from connection asset
         results_reference = DataConnection._from_dict(run_params['entity']['results_reference'])
         results_reference._api_client = self._wml_client
         results_reference._check_if_connection_asset_is_s3()
         run_params['entity']['results_reference'] = results_reference._to_dict()
         # --- end note
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/base_auto_pipelines.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/base_auto_pipelines.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/local_auto_pipelines.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/local_auto_pipelines.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/optimizers/remote_auto_pipelines.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/optimizers/remote_auto_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,22 +434,22 @@
                 conn.auto_pipeline_params['fairness_info'] = metrics[-1]['context']['fairness'].get('info')
 
         return run_params
 
     def determine_result_reference(self, results_reference, data_references, result_path):
         # note: if user did not provide results storage information, use default ones
         if results_reference is None:
-            if isinstance(data_references[0].location, S3Location) and not self._workspace.api_client.ICP:
+            if isinstance(data_references[0].location, S3Location) and not self._workspace.api_client.ICP_PLATFORM_SPACES:
                 results_reference = DataConnection(
                     connection=data_references[0].connection,
                     location=S3Location(bucket=data_references[0].location.bucket,
                                         path=".")
                 )
 
-            elif isinstance(data_references[0].location, AssetLocation) and not self._workspace.api_client.ICP:
+            elif isinstance(data_references[0].location, AssetLocation) and not self._workspace.api_client.ICP_PLATFORM_SPACES:
                 connection_id = data_references[0].location._get_connection_id(self._workspace.api_client)
 
                 if connection_id is not None:
                     results_reference = DataConnection(
                         connection_asset_id=connection_id,
                         location=S3Location(
                             bucket=data_references[0].location._get_bucket(self._workspace.api_client),
@@ -457,19 +457,19 @@
                     )
 
                 else:  # set container output location when default DAta Asset is as a train ref
                     results_reference = DataConnection(
                         location=ContainerLocation(path=result_path))
 
             elif isinstance(data_references[0].location,
-                            ContainerLocation) and not self._workspace.api_client.ICP:
+                            ContainerLocation) and not self._workspace.api_client.ICP_PLATFORM_SPACES:
                 results_reference = DataConnection(location=ContainerLocation(path=result_path))
 
             elif isinstance(data_references[0].location,
-                            DatabaseLocation) and not self._workspace.api_client.ICP:
+                            DatabaseLocation) and not self._workspace.api_client.ICP_PLATFORM_SPACES:
                 results_reference = DataConnection(location=ContainerLocation(path=result_path))
 
             else:
                 location = FSLocation()
                 client = self._engine._api_client if isinstance(self._engine, ServiceEngine) else self._engine._wml_client
                 if self._workspace.api_client.default_project_id is None:
                     
@@ -745,15 +745,15 @@
                     for varname, obj in module.__dict__.items():
                         if obj is self:
                             return varname
 
             if '\'PUT_YOUR_APIKEY_HERE\'' in result:
                 try:
                     optimizer_var_name = get_optimizer_var_name()
-                    result = result.replace('\'PUT_YOUR_APIKEY_HERE\'', f'{optimizer_var_name}._workspace.credentials[\'apikey\']')
+                    result = result.replace('\'PUT_YOUR_APIKEY_HERE\'', f'{optimizer_var_name}._workspace.credentials.api_key')
 
                 except:
                     pass
 
             import IPython.core
             ipython = IPython.core.getipython.get_ipython()
             comment = "# generated by get_pipeline_notebook(insert_to_cell=True) from previous cell\n\n"
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/auto_pipelines_runs.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/auto_pipelines_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         data = [run for run in data if run['entity'].get('pipeline', {}).get('id')]
         # --- end note
 
 
         def get_value(pipeline_id, timestamp, run):
             try:
                 client = self._engine._api_client if isinstance(self._engine, ServiceEngine) else self._engine._wml_client
-                pipeline_details = client.pipelines.get_details(pipeline_uid=pipeline_id)
+                pipeline_details = client.pipelines.get_details(pipeline_id=pipeline_id)
             except ApiRequestFailure:
                 pipeline_details = {'metadata': {'name': 'Experiment data is missing...'}}
 
             if self.auto_pipeline_optimizer_name and pipeline_details['metadata']['name'] != self.auto_pipeline_optimizer_name:
                 return None
 
             if not ('automl' in str(pipeline_details) or 'autoai-ts' in str(pipeline_details)) or not 'hybrid' in str(pipeline_details):
@@ -143,18 +143,18 @@
             
             optimizer_id = client.training.get_details(
                 limit=1, training_type='pipeline', _internal=True
                 ).get('resources')[0]['entity']['pipeline']['id']
 
         else:
             optimizer_id = client.training.get_details(
-                training_uid=run_id, _internal=True
+                training_id=run_id, _internal=True
                 ).get('entity')['pipeline']['id']
 
-        optimizer_config = client.pipelines.get_details(pipeline_uid=optimizer_id)
+        optimizer_config = client.pipelines.get_details(pipeline_id=optimizer_id)
 
         # note: if experiment has more than 1 node (e.g. KB + sth), we need to find which one is KB
         kb_node_number, kb_runtime_number = get_node_and_runtime_index(node_name='kb',
                                                                        optimizer_config=optimizer_config)
         # --- end note
 
         # note: try to find ts node
@@ -341,15 +341,15 @@
         client = self._engine._api_client if isinstance(self._engine, ServiceEngine) else self._engine._wml_client
         if run_id is None:
             details = client.training.get_details(limit=1, 
                                                   training_type='pipeline', 
                                                   _internal=True).get('resources')[0]
 
         else:
-            details = client.training.get_details(training_uid=run_id, _internal=True)
+            details = client.training.get_details(training_id=run_id, _internal=True)
 
         if details['entity']['status'].get('metrics', False):
             del details['entity']['status']['metrics']
             return details
         else:
             return details
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/base_auto_pipelines_runs.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/base_auto_pipelines_runs.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/autoai/runs/local_auto_pipelines_runs.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/autoai/runs/local_auto_pipelines_runs.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/base_experiment/base_experiment.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/base_experiment/base_experiment.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/fm_tune/tune_experiment.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/fm_tune/tune_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,21 +209,20 @@
         """
 
         task_id, base_model = [
             enum_possible_field.value if isinstance(enum_possible_field, Enum) else enum_possible_field for
             enum_possible_field in (task_id, base_model)]
 
         prompt_tuning_supported_models = [model_spec['model_id'] for model_spec in
-                                          get_model_specs_with_prompt_tuning_support(
-                                              url=self.client.wml_credentials.get('url')).get('resources', [])]
+                                          self.client.foundation_models.get_model_specs_with_prompt_tuning_support().get('resources', [])]
         if base_model not in prompt_tuning_supported_models:
             raise WMLClientError(f"Base model '{base_model}' is not supported. Supported models: {prompt_tuning_supported_models}")
 
         # check if model is in constricted mode
-        _check_model_state(self.client.wml_credentials.get('url'), base_model)
+        _check_model_state(self.client.credentials.url, base_model)
 
         prompt_tuner = PromptTuner(name=name,
                                    task_id=task_id,
                                    description=description,
                                    base_model=base_model,
                                    accumulate_steps=accumulate_steps,
                                    batch_size=batch_size,
@@ -242,10 +241,10 @@
 
         return prompt_tuner
 
     def _get_tasks_enum(self):
         try:
             from ibm_watsonx_ai.foundation_models.utils.utils import get_all_supported_tasks_dict
             return Enum(value='TuneExperimentTasks',
-                        names=get_all_supported_tasks_dict(url=self.client.wml_credentials.get('url')))
+                        names=get_all_supported_tasks_dict(url=self.client.credentials.url))
         except Exception:
             return TuneExperimentTasks
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/experiment/fm_tune/tune_runs.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/experiment/fm_tune/tune_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
             experiment.runs.get_run_details(run_id='02bab973-ae83-4283-9d73-87b9fd462d35')
             experiment.runs.get_run_details()
         """
         if run_id is None:
             details = self.client.training.get_details(limit=1, training_type='prompt_tuning', _internal=True).get('resources')[0]
         else:
-            details = self.client.training.get_details(training_uid=run_id, _internal=True)
+            details = self.client.training.get_details(training_id=run_id, _internal=True)
 
         if include_metrics:
             return details
 
         if details['entity']['status'].get('metrics', False):
             del details['entity']['status']['metrics']
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/federated_learning/FLExceptions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/federated_learning/FLExceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/embeddings/base_embeddings.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/base_embeddings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
 from __future__ import annotations
+import copy
 import importlib
 from abc import ABC, abstractmethod
 
 
 class BaseEmbeddings(ABC):
     """Langchain-like embedding function interface."""
 
@@ -19,27 +20,28 @@
     @abstractmethod
     def embed_query(self, text: str) -> list[float]:
         """Embed query text."""
         raise NotImplementedError()
 
     def to_dict(self) -> dict:
         """Serialize Embeddings.
-        
-        :return: serializes this Embeddings so that it can be reconstructed by from_dict class method.
+
+        :return: serializes this Embeddings so that it can be reconstructed by ``from_dict`` class method.
         :rtype: dict
         """
         return {"__class__": self.__class__.__name__, "__module__": self.__module__}
 
     @classmethod
     def from_dict(cls, data: dict) -> BaseEmbeddings | None:
-        """Deserialize BaseEmbeddings into concrete one using arguments
+        """Deserialize ``BaseEmbeddings`` into concrete one using arguments
 
         :return: concrete Embeddings or None if data is incorrect
         :rtype: BaseEmbeddings | None
         """
+        data = copy.deepcopy(data)
         if isinstance(data, dict):
             class_type = data.pop("__class__", None)
             module_name = data.pop("__module__", None)
 
             if module_name:
                 module = importlib.import_module(module_name)
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/embeddings/embeddings.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/embeddings/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
 
 from __future__ import annotations
 import time
 import os
-from typing import TypeAlias
+from typing import TypeAlias, TYPE_CHECKING
 from concurrent.futures import ThreadPoolExecutor
 from functools import reduce
 
 from ibm_watsonx_ai.wml_client_error import WMLClientError, InvalidMultipleArguments
 from .base_embeddings import BaseEmbeddings
 from ibm_watsonx_ai.foundation_models.utils.enums import EmbeddingTypes
 from ibm_watsonx_ai.wml_resource import WMLResource
 import ibm_watsonx_ai._wrappers.requests as requests
 
-from ibm_watsonx_ai import APIClient
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
+    from ibm_watsonx_ai import Credentials
 
 # Type Aliasses
 ParamsType: TypeAlias = dict[str, str | dict[str, str]]
 PayloadType: TypeAlias = dict[str, str | list[str] | ParamsType]
 
 
 __all__ = ["Embeddings"]
@@ -93,33 +95,31 @@
     """
 
     def __init__(
         self,
         *,
         model_id: str,
         params: ParamsType | None = None,
-        credentials: dict[str, str] | None = None,
+        credentials: Credentials | dict[str, str] | None = None,
         project_id: str | None = None,
         space_id: str | None = None,
         api_client: APIClient | None = None,
         verify: bool | str | None = None,
     ) -> None:
-
         if isinstance(model_id, EmbeddingTypes):
             self.model_id = model_id.value
         else:
             self.model_id = model_id
 
         self.params = params
 
-        # remove when initializing APIClient with client._wml_credentials will be available
-        self._credentials = credentials
         Embeddings._validate_type(params, "params", dict, False)
 
         if credentials:
+            from ibm_watsonx_ai import APIClient
             self._client = APIClient(credentials, verify=verify)
         elif api_client:
             self._client = api_client
         else:
             raise InvalidMultipleArguments(
                 params_names_list=["credentials", "api_client"],
                 reason="None of the arguments were provided.",
@@ -133,26 +133,26 @@
             raise InvalidMultipleArguments(
                 params_names_list=["space_id", "project_id"],
                 reason="None of the arguments were provided.",
             )
         if not self._client.CLOUD_PLATFORM_SPACES and self._client.CPD_version < 5.0:
             raise WMLClientError(error_msg="Operation is unsupported for this release.")
 
-        super(WMLResource, self).__init__(__name__, self._client)
+        WMLResource.__init__(self, __name__, self._client)
 
     def generate(
         self,
         inputs: list[str],
         params: ParamsType | None = None,
         concurrency_limit: int = 10,
     ) -> dict:
         """Generates embeddings vectors for the given input with the given
         parameters and returns a REST API response.
 
-        :param inputs: List of texts for which embedding vevtors will be generated.
+        :param inputs: List of texts for which embedding vectors will be generated.
         :type inputs: list[str]
         :param params: meta props for embedding generation, use ``ibm_watsonx_ai.metanames.EmbedTextParamsMetaNames().show()`` to view the list of MetaNames, defaults to None
         :type params: ParamsType | None, optional
         :param concurrency_limit: number of requests that will be sent in parallel, max is 10, defaults to 10
         :type concurrency_limit: int, optional
         :return: scoring results containing generated embeddings vectors
         :rtype: dict
@@ -184,37 +184,40 @@
                                 [params] * len(inputs_batch),
                             )
                         )
                     generated_responses.extend(response_batch)
 
             def reduce_response(left: dict, right: dict) -> dict:
                 import copy
+
                 left_copy = copy.deepcopy(left)
-                left_copy['results'].extend(right['results'])
-                left_copy['input_token_count'] += right['input_token_count']
+                left_copy["results"].extend(right["results"])
+                left_copy["input_token_count"] += right["input_token_count"]
                 return left_copy
-            
-            return reduce(reduce_response, generated_responses[1:], generated_responses[0])
+
+            return reduce(
+                reduce_response, generated_responses[1:], generated_responses[0]
+            )
 
         else:
             # Refactor when APIClient will be ported
             from ibm_watsonx_ai.href_definitions import HrefDefinitions
 
             generate_url = HrefDefinitions(client=self._client).get_fm_embeddings_href()
             return self._generate(generate_url, inputs, params)
 
     def embed_documents(
         self,
         texts: list[str],
         params: ParamsType | None = None,
         concurrency_limit: int = 10,
     ) -> list[list[float]]:
-        """Return list of embeding vectors for provided texts.
+        """Return list of embedding vectors for provided texts.
 
-        :param texts: List of texts for which embedding vevtors will be generated.
+        :param texts: List of texts for which embedding vectors will be generated.
         :type texts: list[str]
         :param params: meta props for embedding generation, use ``ibm_watsonx_ai.metanames.EmbedTextParamsMetaNames().show()`` to view the list of MetaNames, defaults to None
         :type params: ParamsType | None, optional
         :param concurrency_limit: number of requests that will be sent in parallel, max is 10, defaults to 10
         :type concurrency_limit: int, optional
 
         :return: List of embedding vectors
@@ -236,17 +239,17 @@
             vector.get("embedding")
             for vector in self.generate(
                 inputs=texts, params=params, concurrency_limit=concurrency_limit
             ).get("results", [{}])
         ]
 
     def embed_query(self, text: str, params: ParamsType | None = None) -> list[float]:
-        """Return embeding vector for provided text.
+        """Return embedding vector for provided text.
 
-        :param text: Text for which embedding vevtor will be generated.
+        :param text: Text for which embedding vector will be generated.
         :type text: str
         :param params: meta props for embedding generation, use ``ibm_watsonx_ai.metanames.EmbedTextParamsMetaNames().show()`` to view the list of MetaNames, defaults to None
         :type params: ParamsType | None, optional
         :return: Embedding vector
         :rtype: list[float]
 
         **Example**
@@ -302,20 +305,20 @@
             else:
                 break
 
         return self._handle_response(200, "generate", response_scoring)
 
     def to_dict(self) -> dict:
         data = super().to_dict()
-        # No yet available when only APIClient is provided
+
         data.update(
             {
                 "model_id": self.model_id,
                 "params": self.params,
-                "credentials": self._credentials,
+                "credentials": self._client.credentials.to_dict(),
                 "project_id": self._client.default_project_id,
                 "space_id": self._client.default_space_id,
                 "verify": os.environ.get("WML_CLIENT_VERIFY_REQUESTS"),
             }
         )
 
         return data
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/extensions/langchain/llm.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/extensions/langchain/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 try:
     from langchain.llms.base import LLM
     from langchain.llms.utils import enforce_stop_tokens
 except ImportError:
     raise ImportError("Could not import langchain: Please install langchain extension.")
 from ibm_watsonx_ai.foundation_models import Model, ModelInference
-from ibm_watsonx_ai.foundation_models.utils.utils import _raise_watsonxllm_deprecation_warning
+from ibm_watsonx_ai.foundation_models.utils.utils import (
+    _raise_watsonxllm_deprecation_warning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class WatsonxLLM(LLM):
     """
     `LangChain CustomLLM <https://python.langchain.com/docs/modules/model_io/models/llms/custom_llm>`_ wrapper for watsonx foundation models.
@@ -52,14 +54,15 @@
             params=generate_params,
             project_id="*****"
         )
 
         custom_llm = WatsonxLLM(model=model)
 
     """
+
     _raise_watsonxllm_deprecation_warning()
 
     model: Model | ModelInference = None
     llm_type: str = "IBM watsonx.ai"
 
     def __init__(self, model: Model | ModelInference) -> None:
         super(WatsonxLLM, self).__init__()
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/base_model_inference.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/base_model_inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,312 +1,402 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
 import time
 import json
 import warnings
 
 from abc import ABC, abstractmethod
-from typing import Union, List, Optional
+from typing import TYPE_CHECKING, Generator
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
-from ibm_watsonx_ai.foundation_models.utils.utils import HAPDetectionWarning, PIIDetectionWarning
+from ibm_watsonx_ai.foundation_models.utils.utils import (
+    HAPDetectionWarning,
+    PIIDetectionWarning,
+)
 import ibm_watsonx_ai._wrappers.requests as requests
 from ibm_watsonx_ai.wml_resource import WMLResource
 from ibm_watsonx_ai.wml_client_error import WMLClientError
 
-__all__ = [
-    "BaseModelInference"
-]
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
+
+__all__ = ["BaseModelInference"]
 
 
 class BaseModelInference(WMLResource, ABC):
     """Base interface class for the model interface."""
 
-    def __init__(self, name, client):
+    def __init__(self, name: str, client: APIClient):
         WMLResource.__init__(self, name, client)
 
     @abstractmethod
-    def get_details(self):
+    def get_details(self) -> dict:
         """Get model interface's details
 
-                :return: details of model or deployment
-                :rtype: dict
+        :return: details of model or deployment
+        :rtype: dict
         """
         pass
 
     @abstractmethod
-    def generate(self, prompt, params: dict, concurrency_limit: int, async_mode: bool) -> Union[dict, List[dict]]:
+    def generate(
+        self,
+        prompt: str | list | None = None,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+        async_mode: bool = False,
+    ) -> dict | list[dict] | Generator:
         """
         Given a text prompt as input, and parameters the selected inference
         will generate a completion text as generated_text response.
         """
         pass
 
     @abstractmethod
-    def generate_text_stream(self, prompt, params=None):
+    def generate_text_stream(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> Generator:
         """
         Given a text prompt as input, and parameters the selected inference
         will generate a completion text as generator.
         """
         pass
 
     @abstractmethod
+    def tokenize(self, prompt: str, return_tokens: bool = False) -> dict:
+        pass
+
+    @abstractmethod
     def get_identifying_params(self) -> dict:
         """Represent Model Inference's setup in dictionary"""
         pass
 
-    def _prepare_inference_payload(self,
-                                   prompt: str,
-                                   params: Optional[dict] = None,
-                                   guardrails: bool = False,
-                                   guardrails_hap_params: Optional[dict] = None,
-                                   guardrails_pii_params: Optional[dict] = None) -> dict:
+    def _prepare_inference_payload(
+        self,
+        prompt: str,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
         raise NotImplementedError
 
-    def _prepare_beta_inference_payload(self,
-                                        prompt: str,
-                                        params: Optional[dict] = None,
-                                        guardrails: bool = False,
-                                        guardrails_hap_params: Optional[dict] = None,
-                                        guardrails_pii_params: Optional[dict] = None) -> dict:
+    def _prepare_beta_inference_payload(
+        self,
+        prompt: str,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
         raise NotImplementedError
 
-    def _send_inference_payload(self,
-                                prompt: str,
-                                params: dict,
-                                generate_url: str,
-                                guardrails: bool = False,
-                                guardrails_hap_params: Optional[dict] = None,
-                                guardrails_pii_params: Optional[dict] = None
-                                ):
+    def _send_inference_payload(
+        self,
+        prompt: str,
+        params: dict,
+        generate_url: str,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
         if self._client._use_fm_ga_api:
-            payload = self._prepare_inference_payload(prompt,
-                                                      params=params,
-                                                      guardrails=guardrails,
-                                                      guardrails_hap_params=guardrails_hap_params,
-                                                      guardrails_pii_params=guardrails_pii_params)
+            payload = self._prepare_inference_payload(
+                prompt,
+                params=params,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+            )
         else:  # Remove on CPD 5.0 release
-            payload = self._prepare_beta_inference_payload(prompt,
-                                                           params=params,
-                                                           guardrails=guardrails,
-                                                           guardrails_hap_params=guardrails_hap_params,
-                                                           guardrails_pii_params=guardrails_pii_params)
+            payload = self._prepare_beta_inference_payload(
+                prompt,
+                params=params,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+            )
         retries = 0
         while retries < 3:
             response_scoring = requests.post(
                 url=generate_url,
                 json=payload,
                 params=self._client._params(skip_for_create=True),
-                headers=self._client._get_headers()
+                headers=self._client._get_headers(),
             )
             if response_scoring.status_code in [429, 503, 504, 520]:
-                time.sleep(2 ** retries)
+                time.sleep(2**retries)
                 retries += 1
             else:
                 break
 
-        return self._handle_response(200, u'generate', response_scoring)
+        return self._handle_response(200, "generate", response_scoring)
 
-    def _generate_with_url(self,
-                           prompt: list | str,
-                           params: dict,
-                           generate_url: str,
-                           guardrails: bool = False,
-                           guardrails_hap_params: Optional[dict] = None,
-                           guardrails_pii_params: Optional[dict] = None,
-                           concurrency_limit: int = 10):
+    def _generate_with_url(
+        self,
+        prompt: list | str,
+        params: dict,
+        generate_url: str,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+    ) -> list | dict:
         """
         Helper method which implements multi-threading for with passed generate_url.
         """
 
         if isinstance(prompt, list):
             generated_responses = []
             if len(prompt) <= concurrency_limit:
                 with ThreadPoolExecutor() as executor:
                     response_batch = list(
-                        executor.map(self._generate_with_url, prompt, [params] * len(prompt),
-                                     [generate_url] * len(prompt), [guardrails] * len(prompt),
-                                     [guardrails_hap_params] * len(prompt), [guardrails_pii_params] * len(prompt))
+                        executor.map(
+                            self._generate_with_url,
+                            prompt,
+                            [params] * len(prompt),
+                            [generate_url] * len(prompt),
+                            [guardrails] * len(prompt),
+                            [guardrails_hap_params] * len(prompt),
+                            [guardrails_pii_params] * len(prompt),
+                        )
                     )
                 generated_responses.extend(response_batch)
             else:
                 for i in range(0, len(prompt), concurrency_limit):
-                    prompt_batch = prompt[i:i + concurrency_limit]
+                    prompt_batch = prompt[i : i + concurrency_limit]
                     with ThreadPoolExecutor() as executor:
                         response_batch = list(
-                            executor.map(self._generate_with_url, prompt_batch,
-                                         [params] * len(prompt_batch),
-                                         [generate_url] * len(prompt_batch), [guardrails] * len(prompt),
-                                         [guardrails_hap_params] * len(prompt), [guardrails_pii_params] * len(prompt))
+                            executor.map(
+                                self._generate_with_url,
+                                prompt_batch,
+                                [params] * len(prompt_batch),
+                                [generate_url] * len(prompt_batch),
+                                [guardrails] * len(prompt),
+                                [guardrails_hap_params] * len(prompt),
+                                [guardrails_pii_params] * len(prompt),
+                            )
                         )
                     generated_responses.extend(response_batch)
             return generated_responses
 
         else:
-            return self._send_inference_payload(prompt,
-                                                params,
-                                                generate_url,
-                                                guardrails,
-                                                guardrails_hap_params,
-                                                guardrails_pii_params)
-
-    def _generate_with_url_async(self,
-                                 prompt: list | str,
-                                 params: dict,
-                                 generate_url: str,
-                                 guardrails: bool = False,
-                                 guardrails_hap_params: Optional[dict] = None,
-                                 guardrails_pii_params: Optional[dict] = None,
-                                 concurrency_limit: int = 10):
+            return self._send_inference_payload(
+                prompt,
+                params,
+                generate_url,
+                guardrails,
+                guardrails_hap_params,
+                guardrails_pii_params,
+            )
+
+    def _generate_with_url_async(
+        self,
+        prompt: list | str,
+        params: dict,
+        generate_url: str,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+    ) -> Generator:
         async_params = params or {}
-        async_params['return_options'] = {"input_text": True}
+        async_params["return_options"] = {"input_text": True}
 
         if isinstance(prompt, list):
             for i in range(0, len(prompt), concurrency_limit):
-                prompt_batch = prompt[i:i + concurrency_limit]
+                prompt_batch = prompt[i : i + concurrency_limit]
                 with ThreadPoolExecutor() as executor:
-                    futures = [executor.submit(self._send_inference_payload,
-                                               single_prompt,
-                                               async_params,
-                                               generate_url,
-                                               guardrails,
-                                               guardrails_hap_params,
-                                               guardrails_pii_params) for single_prompt in prompt_batch]
+                    futures = [
+                        executor.submit(
+                            self._send_inference_payload,
+                            single_prompt,
+                            async_params,
+                            generate_url,
+                            guardrails,
+                            guardrails_hap_params,
+                            guardrails_pii_params,
+                        )
+                        for single_prompt in prompt_batch
+                    ]
                     for future in as_completed(futures):
                         yield future.result()
         else:
-            yield self._send_inference_payload(prompt,
-                                               async_params,
-                                               generate_url,
-                                               guardrails,
-                                               guardrails_hap_params,
-                                               guardrails_pii_params)
-
-    def _generate_stream_with_url(self,
-                                  prompt: str,
-                                  params: dict,
-                                  generate_stream_url: str,
-                                  raw_response: bool = False,
-                                  guardrails: bool = False,
-                                  guardrails_hap_params: Optional[dict] = None,
-                                  guardrails_pii_params: Optional[dict] = None):
+            yield self._send_inference_payload(
+                prompt,
+                async_params,
+                generate_url,
+                guardrails,
+                guardrails_hap_params,
+                guardrails_pii_params,
+            )
 
+    def _generate_stream_with_url(
+        self,
+        prompt: str,
+        params: dict,
+        generate_stream_url: str,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> Generator:
         if self._client._use_fm_ga_api:
-            payload = self._prepare_inference_payload(prompt,
-                                                      params=params,
-                                                      guardrails=guardrails,
-                                                      guardrails_hap_params=guardrails_hap_params,
-                                                      guardrails_pii_params=guardrails_pii_params)
+            payload = self._prepare_inference_payload(
+                prompt,
+                params=params,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+            )
         else:  # Remove on CPD 5.0 release
-            payload = self._prepare_beta_inference_payload(prompt,
-                                                           params=params,
-                                                           guardrails=guardrails,
-                                                           guardrails_hap_params=guardrails_hap_params,
-                                                           guardrails_pii_params=guardrails_pii_params)
+            payload = self._prepare_beta_inference_payload(
+                prompt,
+                params=params,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+            )
 
         s = requests.Session()
         retries = 0
         while retries < 3:
-            with s.post(url=generate_stream_url,
-                        json=payload,
-                        headers=self._client._get_headers(),
-                        params=self._client._params(skip_for_create=True),
-                        stream=True) as resp:
+            with s.post(
+                url=generate_stream_url,
+                json=payload,
+                headers=self._client._get_headers(),
+                params=self._client._params(skip_for_create=True),
+                stream=True,
+            ) as resp:
                 if resp.status_code in [429, 503, 504, 520]:
-                    time.sleep(2 ** retries)
+                    time.sleep(2**retries)
                     retries += 1
                 elif resp.status_code == 200:
                     for chunk in resp.iter_lines(decode_unicode=False):
-                        chunk = chunk.decode('utf-8')
-                        if 'generated_text' in chunk:
-                            response = chunk.replace('data: ', '')
+                        chunk = chunk.decode("utf-8")
+                        if "generated_text" in chunk:
+                            response = chunk.replace("data: ", "")
                             try:
                                 parsed_response = json.loads(response)
                             except json.JSONDecodeError:
                                 raise Exception(f"Could not parse {response} as json")
                             if raw_response:
                                 yield parsed_response
                                 continue
-                            yield self._return_guardrails_stats(parsed_response)['generated_text']
+                            yield self._return_guardrails_stats(parsed_response)[
+                                "generated_text"
+                            ]
                     break
 
         if resp.status_code != 200:
-            raise WMLClientError(f'Request failed with: {resp.text} ({resp.status_code})')
-
-    def _tokenize_with_url(self,
-                           prompt: str,
-                           tokenize_url: str,
-                           return_tokens: bool,
-                           ):
+            raise WMLClientError(
+                f"Request failed with: {resp.text} ({resp.status_code})"
+            )
 
+    def _tokenize_with_url(
+        self,
+        prompt: str,
+        tokenize_url: str,
+        return_tokens: bool,
+    ) -> dict:
         payload = self._prepare_inference_payload(prompt)
 
-        parameters = payload.get('parameters', {})
+        parameters = payload.get("parameters", {})
         parameters.update({"return_tokens": return_tokens})
-        payload['parameters'] = parameters
+        payload["parameters"] = parameters
 
         retries = 0
         while retries < 3:
             response_scoring = requests.post(
                 url=tokenize_url,
                 json=payload,
                 params=self._client._params(skip_for_create=True),
-                headers=self._client._get_headers()
+                headers=self._client._get_headers(),
             )
             if response_scoring.status_code in [429, 503, 504, 520]:
-                time.sleep(2 ** retries)
+                time.sleep(2**retries)
                 retries += 1
             elif response_scoring.status_code == 404:
                 raise WMLClientError("Tokenize is not supported for this release")
             else:
                 break
 
-        return self._handle_response(200, u'generate', response_scoring)
+        return self._handle_response(200, "generate", response_scoring)
 
-    def _return_guardrails_stats(self, single_response):
-        results = single_response['results'][0]
-        hap_details = results.get("moderations", {}).get("hap") if self._client._use_fm_ga_api else results.get(
-            "moderation", {}).get("hap")  # Remove 'else' on CPD 5.0 release
+    def _return_guardrails_stats(self, single_response: dict) -> dict:
+        results = single_response["results"][0]
+        hap_details = (
+            results.get("moderations", {}).get("hap")
+            if self._client._use_fm_ga_api
+            else results.get("moderation", {}).get("hap")
+        )  # Remove 'else' on CPD 5.0 release
         if hap_details:
             if hap_details[0].get("input"):
-                warnings.warn(next(warning.get('message') for warning in single_response.get('system', {}).get('warnings')
-                                if warning.get('id') == 'UNSUITABLE_INPUT'), category=HAPDetectionWarning)
+                warnings.warn(
+                    next(
+                        warning.get("message")
+                        for warning in single_response.get("system", {}).get("warnings")
+                        if warning.get("id") == "UNSUITABLE_INPUT"
+                    ),
+                    category=HAPDetectionWarning,
+                )
             else:
-                warnings.warn(f'Potentially harmful text detected: {hap_details}', category=HAPDetectionWarning)
-        pii_details = results.get("moderations", {}).get("pii") if self._client._use_fm_ga_api else results.get(
-            "moderation", {}).get("pii")  # Remove 'else' on CPD 5.0 release
+                warnings.warn(
+                    f"Potentially harmful text detected: {hap_details}",
+                    category=HAPDetectionWarning,
+                )
+        pii_details = (
+            results.get("moderations", {}).get("pii")
+            if self._client._use_fm_ga_api
+            else results.get("moderation", {}).get("pii")
+        )  # Remove 'else' on CPD 5.0 release
         if pii_details:
             if pii_details[0].get("input"):
-                warnings.warn(next(warning.get('message') for warning in single_response.get('system', {}).get('warnings')
-                                if warning.get('id') == 'UNSUITABLE_INPUT'), category=PIIDetectionWarning)
+                warnings.warn(
+                    next(
+                        warning.get("message")
+                        for warning in single_response.get("system", {}).get("warnings")
+                        if warning.get("id") == "UNSUITABLE_INPUT"
+                    ),
+                    category=PIIDetectionWarning,
+                )
             else:
-                warnings.warn(f'Personally identifiable information detected: {pii_details}', category=PIIDetectionWarning)
+                warnings.warn(
+                    f"Personally identifiable information detected: {pii_details}",
+                    category=PIIDetectionWarning,
+                )
         return results
 
     @staticmethod
     def _update_moderations_params(additional_params: dict) -> dict:
-
-        default_params = {
-            'input': {
-                'enabled': True
-            },
-            'output': {
-                'enabled': True
-            }
-        }
+        default_params = {"input": {"enabled": True}, "output": {"enabled": True}}
         if additional_params:
             for key, value in default_params.items():
                 if key in additional_params:
                     if additional_params[key]:
                         if "threshold" in additional_params:
-                            default_params[key]["threshold"] = additional_params["threshold"]
+                            default_params[key]["threshold"] = additional_params[
+                                "threshold"
+                            ]
                     else:
                         default_params[key]["enabled"] = False
                 else:
                     if "threshold" in additional_params:
-                        default_params[key]["threshold"] = additional_params["threshold"]
+                        default_params[key]["threshold"] = additional_params[
+                            "threshold"
+                        ]
             if "mask" in additional_params:
                 default_params.update({"mask": additional_params["mask"]})
         return default_params
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/deployment_model_inference.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/deployment_model_inference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,235 +1,331 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from typing import Union, List, Optional, Generator
+from __future__ import annotations
+from typing import TYPE_CHECKING, Generator, cast
 
-from ibm_watsonx_ai import APIClient
-from ibm_watsonx_ai.wml_client_error import (WMLClientError, MissingValue, PromptVariablesError,
-                                             UnsupportedOperation)
+from ibm_watsonx_ai.wml_client_error import (
+    WMLClientError,
+    MissingValue,
+    PromptVariablesError,
+    UnsupportedOperation,
+)
 from ibm_watsonx_ai.foundation_models.utils.enums import DecodingMethods
 from ibm_watsonx_ai.metanames import GenTextParamsMetaNames
 from ibm_watsonx_ai.messages.messages import Messages
 from ibm_watsonx_ai.foundation_models.utils.utils import _check_model_state
 
 from .base_model_inference import BaseModelInference
 
-__all__ = [
-    "DeploymentModelInference"
-]
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
+
+__all__ = ["DeploymentModelInference"]
 
 
 class DeploymentModelInference(BaseModelInference):
     """Base abstract class for the model interface."""
 
-    def __init__(self,
-                 *,
-                 deployment_id: str = None,
-                 params: dict = None,
-                 api_client: APIClient = None) -> None:
+    def __init__(
+        self, *, deployment_id: str, api_client: APIClient, params: dict | None = None
+    ) -> None:
         self.deployment_id = deployment_id
 
         self.params = params
-        DeploymentModelInference._validate_type(params, u'params', dict, False)
+        DeploymentModelInference._validate_type(params, "params", dict, False)
 
         self._client = api_client
 
         # check if model is in constricted mode
-        _check_model_state(self._client.wml_credentials.get('url'),
-                           self._client.deployments.get_details(deployment_id).get('entity', {}).get('base_model_id'))
-        
+        self._client.credentials.url = cast(str, self._client.credentials.url)
+        _check_model_state(
+            self._client.credentials.url,
+            self._client.deployments.get_details(deployment_id)
+            .get("entity", {})
+            .get("base_model_id"),
+        )
+
         if not self._client.CLOUD_PLATFORM_SPACES and self._client.CPD_version < 4.8:
             raise WMLClientError(error_msg="Operation is unsupported for this release.")
 
         BaseModelInference.__init__(self, __name__, self._client)
 
-    def get_details(self):
+    def get_details(self) -> dict:
         """Get deployment's details
 
         :return: details of model or deployment
         :rtype: dict
         """
-        return self._client.deployments.get_details(deployment_uid=self.deployment_id, _silent=True)
-
-    def generate(self,
-                 prompt: Optional[str] = None,
-                 params: Optional[dict] = None,
-                 guardrails: bool = False,
-                 guardrails_hap_params: Optional[dict] = None,
-                 guardrails_pii_params: Optional[dict] = None,
-                 concurrency_limit: int = 10,
-                 async_mode: bool = False) -> Union[dict, List[dict], Generator[dict, str, None]]:
+        return self._client.deployments.get_details(
+            deployment_id=self.deployment_id, _silent=True
+        )
+
+    def generate(
+        self,
+        prompt: str | list | None = None,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+        async_mode: bool = False,
+    ) -> dict | list[dict] | Generator:
         """
         Given a text prompt as input, and parameters the selected inference
         will generate a completion text as generated_text response.
         """
+        params = cast(dict, params)
+        prompt = cast(str | list, prompt)
+        self.params = cast(dict, self.params)
         prompt_required = self._deployment_type_validation(params)
-        self._validate_type(prompt, u'prompt', [str, list], prompt_required, raise_error_for_list=True)
-        self._validate_type(guardrails_hap_params, u'guardrails_hap_params', dict, False)
-        self._validate_type(guardrails_pii_params, u'guardrails_pii_params', dict, False)
+        self._validate_type(
+            prompt, "prompt", [str, list], prompt_required, raise_error_for_list=True
+        )
+        self._validate_type(guardrails_hap_params, "guardrails_hap_params", dict, False)
+        self._validate_type(guardrails_pii_params, "guardrails_pii_params", dict, False)
         generate_text_url = self._client.service_instance._href_definitions.get_fm_deployment_generation_href(
-            deployment_id=self.deployment_id, item="text")
+            deployment_id=self.deployment_id, item="text"
+        )
 
         if async_mode:
-            return self._generate_with_url_async(prompt=prompt,
-                                                 params=params or self.params,
-                                                 generate_url=generate_text_url,
-                                                 guardrails=guardrails,
-                                                 guardrails_hap_params=guardrails_hap_params,
-                                                 guardrails_pii_params=guardrails_pii_params,
-                                                 concurrency_limit=concurrency_limit)
+            return self._generate_with_url_async(
+                prompt=prompt,
+                params=params or self.params,
+                generate_url=generate_text_url,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+                concurrency_limit=concurrency_limit,
+            )
         else:
-            return self._generate_with_url(prompt=prompt,
-                                           params=params,
-                                           generate_url=generate_text_url,
-                                           guardrails=guardrails,
-                                           guardrails_hap_params=guardrails_hap_params,
-                                           guardrails_pii_params=guardrails_pii_params,
-                                           concurrency_limit=concurrency_limit)
-
-    def generate_text_stream(self,
-                             prompt: Optional[str] = None,
-                             params: Optional[dict] = None,
-                             raw_response: bool = False,
-                             guardrails: bool = False,
-                             guardrails_hap_params: Optional[dict] = None,
-                             guardrails_pii_params: Optional[dict] = None):
+            return self._generate_with_url(
+                prompt=prompt,
+                params=params,
+                generate_url=generate_text_url,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+                concurrency_limit=concurrency_limit,
+            )
+
+    def generate_text_stream(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> Generator:
         """
         Given a text prompt as input, and parameters the selected inference
         will generate a completion text as generator.
         """
+        params = cast(dict, params)
+        prompt = cast(str, prompt)
+        self.params = cast(dict, self.params)
         prompt_required = self._deployment_type_validation(params)
-        self._validate_type(prompt, u'prompt', str, prompt_required)
-        self._validate_type(guardrails_hap_params, u'guardrails_hap_params', dict, False)
-        self._validate_type(guardrails_pii_params, u'guardrails_pii_params', dict, False)
+        self._validate_type(prompt, "prompt", str, prompt_required)
+        self._validate_type(guardrails_hap_params, "guardrails_hap_params", dict, False)
+        self._validate_type(guardrails_pii_params, "guardrails_pii_params", dict, False)
         if self._client._use_fm_ga_api:
             generate_text_stream_url = self._client.service_instance._href_definitions.get_fm_deployment_generation_stream_href(
-                deployment_id=self.deployment_id)
+                deployment_id=self.deployment_id
+            )
         else:  # Remove on CPD 5.0 release
             generate_text_stream_url = self._client.service_instance._href_definitions.get_fm_deployment_generation_href(
-                deployment_id=self.deployment_id, item="text_stream")
+                deployment_id=self.deployment_id, item="text_stream"
+            )
 
-        return self._generate_stream_with_url(prompt=prompt,
-                                              params=params,
-                                              raw_response=raw_response,
-                                              generate_stream_url=generate_text_stream_url,
-                                              guardrails=guardrails,
-                                              guardrails_hap_params=guardrails_hap_params,
-                                              guardrails_pii_params=guardrails_pii_params)
-
-    def tokenize(self,
-                 prompt=None,
-                 return_tokens: bool = False):
+        return self._generate_stream_with_url(
+            prompt=prompt,
+            params=params,
+            raw_response=raw_response,
+            generate_stream_url=generate_text_stream_url,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+        )
+
+    def tokenize(self, prompt: str, return_tokens: bool = False) -> dict:
         """
         Given a text prompt as input, and return_tokens parameter will return tokenized input text.
         """
-        raise UnsupportedOperation(Messages.get_message(message_id="fm_tokenize_no_supported_deployment"))
+        raise UnsupportedOperation(
+            Messages.get_message(message_id="fm_tokenize_no_supported_deployment")
+        )
 
     def get_identifying_params(self) -> dict:
         """Represent Model Inference's setup in dictionary"""
         return {
             "deployment_id": self.deployment_id,
             "params": self.params,
             "project_id": self._client.default_project_id,
-            "space_id": self._client.default_space_id
+            "space_id": self._client.default_space_id,
         }
 
-    def _prepare_inference_payload(self,
-                                   prompt: str,
-                                   params: dict = None,
-                                   guardrails: bool = False,
-                                   guardrails_hap_params: Optional[dict] = None,
-                                   guardrails_pii_params: Optional[dict] = None) -> dict:
-        payload = {
+    def _prepare_inference_payload(
+        self,
+        prompt: str,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
+        payload: dict = {
             "input": prompt,
         }
 
         if guardrails:
             if guardrails_hap_params is None:
-                guardrails_hap_params = dict(input=True, output=True)  # HAP enabled if guardrails = True
-
-            for guardrail_type,  guardrails_params in zip(('hap', 'pii'), (guardrails_hap_params, guardrails_pii_params)):
+                guardrails_hap_params = dict(
+                    input=True, output=True
+                )  # HAP enabled if guardrails = True
+
+            for guardrail_type, guardrails_params in zip(
+                ("hap", "pii"), (guardrails_hap_params, guardrails_pii_params)
+            ):
                 if guardrails_params is not None:
                     if "moderations" not in payload:
                         payload["moderations"] = {}
-                    payload["moderations"].update({guardrail_type: self._update_moderations_params(guardrails_params)})
+                    payload["moderations"].update(
+                        {
+                            guardrail_type: self._update_moderations_params(
+                                guardrails_params
+                            )
+                        }
+                    )
 
         if params:
-            payload['parameters'] = params
+            payload["parameters"] = params
         elif self.params:
-            payload['parameters'] = self.params
+            payload["parameters"] = self.params
 
-        if 'parameters' in payload and GenTextParamsMetaNames.DECODING_METHOD in payload['parameters']:
-            if isinstance(payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD], DecodingMethods):
-                payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD] = \
-                    payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD].value
-
-        if 'parameters' in payload and 'return_options' in payload['parameters']:
-            if not (payload['parameters']['return_options'].get("input_text", False) or
-                    payload['parameters']['return_options'].get("input_tokens", False)):
-                raise WMLClientError(Messages.get_message(message_id="fm_required_parameters_not_provided"))
+        if (
+            "parameters" in payload
+            and GenTextParamsMetaNames.DECODING_METHOD in payload["parameters"]
+        ):
+            if isinstance(
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD],
+                DecodingMethods,
+            ):
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD] = payload[
+                    "parameters"
+                ][GenTextParamsMetaNames.DECODING_METHOD].value
+
+        if "parameters" in payload and "return_options" in payload["parameters"]:
+            if not (
+                payload["parameters"]["return_options"].get("input_text", False)
+                or payload["parameters"]["return_options"].get("input_tokens", False)
+            ):
+                raise WMLClientError(
+                    Messages.get_message(
+                        message_id="fm_required_parameters_not_provided"
+                    )
+                )
 
         return payload
 
-    def _prepare_beta_inference_payload(self,  # Remove on CPD 5.0 release
-                                        prompt: str,
-                                        params: dict = None,
-                                        guardrails: bool = False,
-                                        guardrails_hap_params: Optional[dict] = None,
-                                        guardrails_pii_params: Optional[dict] = None) -> dict:
-        payload = {
+    def _prepare_beta_inference_payload(
+        self,  # Remove on CPD 5.0 release
+        prompt: str,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
+        payload: dict = {
             "input": prompt,
         }
 
         if guardrails:
-            default_moderations_params = {
-                'input': True,
-                'output': True
-            }
-            payload.update({
-                "moderations": {
-                    "hap": (default_moderations_params | (guardrails_hap_params or {}))
+            default_moderations_params = {"input": True, "output": True}
+            payload.update(
+                {
+                    "moderations": {
+                        "hap": (
+                            default_moderations_params | (guardrails_hap_params or {})
+                        )
+                    }
                 }
-            })
+            )
 
             if guardrails_pii_params is not None:
-                payload['moderations'].update({"pii": guardrails_pii_params})
+                payload["moderations"].update({"pii": guardrails_pii_params})
 
         if params:
-            payload['parameters'] = params
+            payload["parameters"] = params
         elif self.params:
-            payload['parameters'] = self.params
+            payload["parameters"] = self.params
 
-        if 'parameters' in payload and GenTextParamsMetaNames.DECODING_METHOD in payload['parameters']:
-            if isinstance(payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD], DecodingMethods):
-                payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD] = \
-                    payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD].value
-
-        if 'parameters' in payload and 'return_options' in payload['parameters']:
-            if not (payload['parameters']['return_options'].get("input_text", False) or
-                    payload['parameters']['return_options'].get("input_tokens", False)):
-                raise WMLClientError(Messages.get_message(message_id="fm_required_parameters_not_provided"))
+        if (
+            "parameters" in payload
+            and GenTextParamsMetaNames.DECODING_METHOD in payload["parameters"]
+        ):
+            if isinstance(
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD],
+                DecodingMethods,
+            ):
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD] = payload[
+                    "parameters"
+                ][GenTextParamsMetaNames.DECODING_METHOD].value
+
+        if "parameters" in payload and "return_options" in payload["parameters"]:
+            if not (
+                payload["parameters"]["return_options"].get("input_text", False)
+                or payload["parameters"]["return_options"].get("input_tokens", False)
+            ):
+                raise WMLClientError(
+                    Messages.get_message(
+                        message_id="fm_required_parameters_not_provided"
+                    )
+                )
 
         return payload
 
-    def _deployment_type_validation(self, params: dict):
-        deployment_details = self._client.deployments.get_details(deployment_uid=self.deployment_id, _silent=True)
+    def _deployment_type_validation(self, params: dict) -> bool:
+        deployment_details = self._client.deployments.get_details(
+            deployment_uid=self.deployment_id, _silent=True
+        )
         prompt_required = True
-        prompt_id = deployment_details.get('entity', {}).get('prompt_template', {}).get('id')
+        prompt_id = (
+            deployment_details.get("entity", {}).get("prompt_template", {}).get("id")
+        )
         if prompt_id is not None:
             prompt_required = False
-            from ibm_watsonx_ai.foundation_models.prompts import PromptTemplateManager
-
-            prompt_template = PromptTemplateManager(api_client=self._client).load_prompt(prompt_id)
+            from ibm_watsonx_ai.foundation_models.prompts import (
+                PromptTemplateManager,
+                PromptTemplate,
+            )
+
+            prompt_template = PromptTemplateManager(
+                api_client=self._client
+            ).load_prompt(prompt_id)
+            prompt_template = cast(PromptTemplate, prompt_template)
+            prompt_template.input_variables = cast(
+                dict, prompt_template.input_variables
+            )
             # params may be not specified but instead self.params is specified
             parameters = params if params is not None else self.params
-            template_inputs = parameters.get("prompt_variables") if parameters is not None else None
+            template_inputs = (
+                parameters.get("prompt_variables") if parameters is not None else None
+            )
             if template_inputs is None and prompt_template.input_variables is not None:
-                raise MissingValue('prompt_variables', reason=("Prompt template contains input variables but " 
-                                                               "`prompt_variables` parameter not provided in `params`."))
-                
-            if (input_variables:=set(prompt_template.input_variables.keys())) != set(template_inputs.keys()):
-                raise PromptVariablesError(input_variables-set(template_inputs.keys()))
+                raise MissingValue(
+                    "prompt_variables",
+                    reason=(
+                        "Prompt template contains input variables but "
+                        "`prompt_variables` parameter not provided in `params`."
+                    ),
+                )
+            template_inputs = cast(dict, template_inputs)
+            if (input_variables := set(prompt_template.input_variables.keys())) != set(
+                template_inputs.keys()
+            ):
+                raise PromptVariablesError(
+                    str(input_variables - set(template_inputs.keys()))
+                )
 
         return prompt_required
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/fm_model_inference.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/fm_model_inference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,232 +1,318 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from typing import Union, List, Optional, Generator
+from __future__ import annotations
+from typing import Generator, cast, TYPE_CHECKING
 
-__all__ = [
-    "FMModelInference"
-]
+__all__ = ["FMModelInference"]
 
-from ibm_watsonx_ai import APIClient
 from ibm_watsonx_ai.wml_client_error import WMLClientError
 from ibm_watsonx_ai.foundation_models.utils.enums import ModelTypes, DecodingMethods
-from ibm_watsonx_ai.foundation_models.utils.utils import get_model_specs, _check_model_state
+from ibm_watsonx_ai.foundation_models.utils.utils import (
+    get_model_specs,
+    _check_model_state,
+)
 from ibm_watsonx_ai.metanames import GenTextParamsMetaNames
 from ibm_watsonx_ai.messages.messages import Messages
 from .base_model_inference import BaseModelInference
 
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
+
 
 class FMModelInference(BaseModelInference):
     """Base abstract class for the model interface."""
 
-    def __init__(self,
-                 *,
-                 model_id: str = None,
-                 params: dict = None,
-                 api_client: APIClient = None,
-                 validate: bool = True) -> None:
-
+    def __init__(
+        self,
+        *,
+        model_id: str,
+        api_client: APIClient,
+        params: dict | None = None,
+        validate: bool = True,
+    ):
         self.model_id = model_id
         if isinstance(self.model_id, ModelTypes):
             self.model_id = self.model_id.value
 
         self.params = params
-        FMModelInference._validate_type(params, u'params', dict, False)
+        FMModelInference._validate_type(params, "params", dict, False)
 
         self._client = api_client
         if validate:
-            supported_models = [model_spec['model_id'] for model_spec in get_model_specs(self._client.wml_credentials.get('url')).get('resources', [])]
+            supported_models = [
+                model_spec["model_id"]
+                for model_spec in self._client.foundation_models.get_model_specs().get(  # type: ignore[union-attr]
+                    "resources", []
+                )
+            ]
             if self.model_id not in supported_models:
-                raise WMLClientError(error_msg=f"Model '{self.model_id}' is not supported for this environment. "
-                                            f"Supported models: {supported_models}")
+                raise WMLClientError(
+                    error_msg=f"Model '{self.model_id}' is not supported for this environment. "
+                    f"Supported models: {supported_models}"
+                )
 
         # check if model is in constricted mode
-        _check_model_state(self._client.wml_credentials.get('url'), self.model_id)
+        self.model_id = cast(str, self.model_id)
+        self._client.credentials.url = cast(str, self._client.credentials.url)
+        _check_model_state(self._client.credentials.url, self.model_id)
 
         if not self._client.CLOUD_PLATFORM_SPACES and self._client.CPD_version < 4.8:
             raise WMLClientError(error_msg="Operation is unsupported for this release.")
 
         BaseModelInference.__init__(self, __name__, self._client)
 
-    def get_details(self):
+    def get_details(self) -> dict:
         """Get model's details
 
         :return: details of model or deployment
         :rtype: dict
         """
-        models = get_model_specs(self._client.wml_credentials['url']).get('resources', [])
-        return next((item for item in models if item['model_id'] == self.model_id), None)
+        return self._client.foundation_models.get_model_specs(self.model_id)  # type: ignore[return-value]
 
-    def generate(self,
-                 prompt,
-                 params: dict = None,
-                 guardrails: bool = False,
-                 guardrails_hap_params: Optional[dict] = None,
-                 guardrails_pii_params: Optional[dict] = None,
-                 concurrency_limit: int = 10,
-                 async_mode: bool = False) -> Union[dict, List[dict], Generator[dict, str, None]]:
+    def generate(
+        self,
+        prompt: str | list | None = None,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+        async_mode: bool = False,
+    ) -> dict | list[dict] | Generator:
         """
         Given a text prompt as input, and parameters the selected inference
         will generate a completion text as generated_text response.
         """
-        self._validate_type(prompt, u'prompt', [str, list], True, raise_error_for_list=True)
-        self._validate_type(guardrails_hap_params, u'guardrails_hap_params', dict, mandatory=False)
-        self._validate_type(guardrails_pii_params, u'guardrails_pii_params', dict, mandatory=False)
-
-        generate_text_url = self._client.service_instance._href_definitions.get_fm_generation_href('text')
+        self._validate_type(
+            prompt, "prompt", [str, list], True, raise_error_for_list=True
+        )
+        self._validate_type(
+            guardrails_hap_params, "guardrails_hap_params", dict, mandatory=False
+        )
+        self._validate_type(
+            guardrails_pii_params, "guardrails_pii_params", dict, mandatory=False
+        )
+
+        generate_text_url = (
+            self._client.service_instance._href_definitions.get_fm_generation_href(
+                "text"
+            )
+        )
+
+        prompt = cast(str | list, prompt)
+        params = cast(dict, params)
+        self.params = cast(dict, self.params)
 
         if async_mode:
-            return self._generate_with_url_async(prompt=prompt,
-                                                 params=params or self.params,
-                                                 generate_url=generate_text_url,
-                                                 guardrails=guardrails,
-                                                 guardrails_hap_params=guardrails_hap_params,
-                                                 guardrails_pii_params=guardrails_pii_params,
-                                                 concurrency_limit=concurrency_limit)
+            return self._generate_with_url_async(
+                prompt=prompt,
+                params=params or self.params,
+                generate_url=generate_text_url,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+                concurrency_limit=concurrency_limit,
+            )
         else:
-            return self._generate_with_url(prompt=prompt,
-                                           params=params,
-                                           generate_url=generate_text_url,
-                                           guardrails=guardrails,
-                                           guardrails_hap_params=guardrails_hap_params,
-                                           guardrails_pii_params=guardrails_pii_params,
-                                           concurrency_limit=concurrency_limit)
-
-    def generate_text_stream(self,
-                             prompt,
-                             params=None,
-                             raw_response=False,
-                             guardrails: bool = False,
-                             guardrails_hap_params: Optional[dict] = None,
-                             guardrails_pii_params: Optional[dict] = None):
+            return self._generate_with_url(
+                prompt=prompt,
+                params=params,
+                generate_url=generate_text_url,
+                guardrails=guardrails,
+                guardrails_hap_params=guardrails_hap_params,
+                guardrails_pii_params=guardrails_pii_params,
+                concurrency_limit=concurrency_limit,
+            )
+
+    def generate_text_stream(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> Generator:
         """
         Given a text prompt as input, and parameters the selected inference
         will generate a completion text as generator.
         """
-        self._validate_type(prompt, u'prompt', str, True)
+        self._validate_type(prompt, "prompt", str, True)
         if self._client._use_fm_ga_api:
-            generate_text_stream_url = self._client.service_instance._href_definitions.get_fm_generation_stream_href()
+            generate_text_stream_url = (
+                self._client.service_instance._href_definitions.get_fm_generation_stream_href()
+            )
         else:
-            generate_text_stream_url = self._client.service_instance._href_definitions.get_fm_generation_href(f'text_stream')  # Remove on CPD 5.0 release
+            generate_text_stream_url = (
+                self._client.service_instance._href_definitions.get_fm_generation_href(
+                    f"text_stream"
+                )
+            )  # Remove on CPD 5.0 release
+
+        prompt = cast(str, prompt)
+        params = cast(dict, params)
+        return self._generate_stream_with_url(
+            prompt=prompt,
+            params=params,
+            raw_response=raw_response,
+            generate_stream_url=generate_text_stream_url,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+        )
 
-        return self._generate_stream_with_url(prompt=prompt,
-                                              params=params,
-                                              raw_response=raw_response,
-                                              generate_stream_url=generate_text_stream_url,
-                                              guardrails=guardrails,
-                                              guardrails_hap_params=guardrails_hap_params,
-                                              guardrails_pii_params=guardrails_pii_params)
-
-    def tokenize(self,
-                 prompt,
-                 return_tokens: bool = False):
+    def tokenize(self, prompt: str, return_tokens: bool = False) -> dict:
         """
         Given a text prompt as input, and return_tokens parameter will return tokenized input text.
         """
-        self._validate_type(prompt, u'prompt', str, True)
-        generate_tokenize_url = self._client.service_instance._href_definitions.get_fm_tokenize_href()
-
-        return self._tokenize_with_url(prompt=prompt,
-                                       tokenize_url=generate_tokenize_url,
-                                       return_tokens=return_tokens)
+        self._validate_type(prompt, "prompt", str, True)
+        generate_tokenize_url = (
+            self._client.service_instance._href_definitions.get_fm_tokenize_href()
+        )
+
+        return self._tokenize_with_url(
+            prompt=prompt,
+            tokenize_url=generate_tokenize_url,
+            return_tokens=return_tokens,
+        )
 
     def get_identifying_params(self) -> dict:
         """Represent Model Inference's setup in dictionary"""
         return {
             "model_id": self.model_id,
             "params": self.params,
             "project_id": self._client.default_project_id,
-            "space_id": self._client.default_space_id
+            "space_id": self._client.default_space_id,
         }
 
-    def _prepare_inference_payload(self,
-                                   prompt: str,
-                                   params: dict = None,
-                                   guardrails: bool = False,
-                                   guardrails_hap_params: Optional[dict] = None,
-                                   guardrails_pii_params: Optional[dict] = None) -> dict:
-        payload = {
+    def _prepare_inference_payload(
+        self,
+        prompt: str,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
+        payload: dict = {
             "model_id": self.model_id,
             "input": prompt,
         }
         if guardrails:
             if guardrails_hap_params is None:
-                    guardrails_hap_params = dict(input=True, output=True)  # HAP enabled if guardrails = True
-
-            for guardrail_type, guardrails_params in zip(('hap', 'pii'),
-                                                         (guardrails_hap_params, guardrails_pii_params)):
+                guardrails_hap_params = dict(
+                    input=True, output=True
+                )  # HAP enabled if guardrails = True
+
+            for guardrail_type, guardrails_params in zip(
+                ("hap", "pii"), (guardrails_hap_params, guardrails_pii_params)
+            ):
                 if guardrails_params is not None:
                     if "moderations" not in payload:
                         payload["moderations"] = {}
-                    payload["moderations"].update({guardrail_type: self._update_moderations_params(guardrails_params)})
+                    payload["moderations"].update(
+                        {
+                            guardrail_type: self._update_moderations_params(
+                                guardrails_params
+                            )
+                        }
+                    )
 
         if params:
-            payload['parameters'] = params
+            payload["parameters"] = params
         elif self.params:
-            payload['parameters'] = self.params
+            payload["parameters"] = self.params
 
-        if 'parameters' in payload and GenTextParamsMetaNames.DECODING_METHOD in payload[
-            'parameters']:
-            if isinstance(payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD], DecodingMethods):
-                payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD] = \
-                    payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD].value
+        if (
+            "parameters" in payload
+            and GenTextParamsMetaNames.DECODING_METHOD in payload["parameters"]
+        ):
+            if isinstance(
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD],
+                DecodingMethods,
+            ):
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD] = payload[
+                    "parameters"
+                ][GenTextParamsMetaNames.DECODING_METHOD].value
 
         if self._client.default_project_id:
-            payload['project_id'] = self._client.default_project_id
+            payload["project_id"] = self._client.default_project_id
         elif self._client.default_space_id:
-            payload['space_id'] = self._client.default_space_id
+            payload["space_id"] = self._client.default_space_id
 
-        if 'parameters' in payload and 'return_options' in payload['parameters']:
-            if not (payload['parameters']['return_options'].get("input_text", False) or
-                    payload['parameters']['return_options'].get("input_tokens", False)):
-                raise WMLClientError(Messages.get_message(message_id="fm_required_parameters_not_provided"))
+        if "parameters" in payload and "return_options" in payload["parameters"]:
+            if not (
+                payload["parameters"]["return_options"].get("input_text", False)
+                or payload["parameters"]["return_options"].get("input_tokens", False)
+            ):
+                raise WMLClientError(
+                    Messages.get_message(
+                        message_id="fm_required_parameters_not_provided"
+                    )
+                )
 
         return payload
 
-    def _prepare_beta_inference_payload(self,  # Remove on CPD 5.0 release
-                                        prompt: str,
-                                        params: dict = None,
-                                        guardrails: bool = False,
-                                        guardrails_hap_params: Optional[dict] = None,
-                                        guardrails_pii_params: Optional[dict] = None) -> dict:
-        payload = {
+    def _prepare_beta_inference_payload(
+        self,  # Remove on CPD 5.0 release
+        prompt: str,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> dict:
+        payload: dict = {
             "model_id": self.model_id,
             "input": prompt,
         }
         if guardrails:
-            default_moderations_params = {
-                'input': True,
-                'output': True
-            }
-            payload.update({
-                "moderations": {
-                    "hap": (default_moderations_params | (guardrails_hap_params or {}))
+            default_moderations_params = {"input": True, "output": True}
+            payload.update(
+                {
+                    "moderations": {
+                        "hap": (
+                            default_moderations_params | (guardrails_hap_params or {})
+                        )
+                    }
                 }
-            })
+            )
 
             if guardrails_pii_params is not None:
-                payload['moderations'].update({"pii": guardrails_pii_params})
+                payload["moderations"].update({"pii": guardrails_pii_params})
 
         if params:
-            payload['parameters'] = params
+            payload["parameters"] = params
         elif self.params:
-            payload['parameters'] = self.params
+            payload["parameters"] = self.params
 
-        if 'parameters' in payload and GenTextParamsMetaNames.DECODING_METHOD in payload['parameters']:
-            if isinstance(payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD], DecodingMethods):
-                payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD] = \
-                    payload['parameters'][GenTextParamsMetaNames.DECODING_METHOD].value
+        if (
+            "parameters" in payload
+            and GenTextParamsMetaNames.DECODING_METHOD in payload["parameters"]
+        ):
+            if isinstance(
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD],
+                DecodingMethods,
+            ):
+                payload["parameters"][GenTextParamsMetaNames.DECODING_METHOD] = payload[
+                    "parameters"
+                ][GenTextParamsMetaNames.DECODING_METHOD].value
 
         if self._client.default_project_id:
-            payload['project_id'] = self._client.default_project_id
+            payload["project_id"] = self._client.default_project_id
         elif self._client.default_space_id:
-            payload['space_id'] = self._client.default_space_id
+            payload["space_id"] = self._client.default_space_id
 
-        if 'parameters' in payload and 'return_options' in payload['parameters']:
-            if not (payload['parameters']['return_options'].get("input_text", False) or
-                    payload['parameters']['return_options'].get("input_tokens", False)):
-                raise WMLClientError(Messages.get_message(message_id="fm_required_parameters_not_provided"))
+        if "parameters" in payload and "return_options" in payload["parameters"]:
+            if not (
+                payload["parameters"]["return_options"].get("input_text", False)
+                or payload["parameters"]["return_options"].get("input_tokens", False)
+            ):
+                raise WMLClientError(
+                    Messages.get_message(
+                        message_id="fm_required_parameters_not_provided"
+                    )
+                )
 
         return payload
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/inference/model_inference.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/inference/model_inference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
-from ibm_watsonx_ai import APIClient
-from ibm_watsonx_ai.wml_client_error import WMLClientError, ParamOutOfRange, InvalidMultipleArguments
+from typing import TYPE_CHECKING, Generator, cast
+
+from ibm_watsonx_ai.wml_client_error import (
+    WMLClientError,
+    ParamOutOfRange,
+    InvalidMultipleArguments,
+)
 from ibm_watsonx_ai.foundation_models.utils.enums import ModelTypes
 from .base_model_inference import BaseModelInference
 from .fm_model_inference import FMModelInference
 from .deployment_model_inference import DeploymentModelInference
 
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient, Credentials
+    from langchain_ibm import WatsonxLLM
+
 
 class ModelInference(BaseModelInference):
     """Instantiate the model interface.
 
     .. hint::
         To use the ModelInference class with LangChain, use the :func:`WatsonxLLM <ibm_watsonx_ai.foundation_models.extensions.langchain.WatsonxLLM>` wrapper.
 
@@ -94,107 +104,126 @@
                 "url": "https://us-south.ml.cloud.ibm.com"
             },
             project_id="*****"
             )
 
     """
 
-    def __init__(self,
-                 *,
-                 model_id: str = None,
-                 deployment_id: str = None,
-                 params: dict = None,
-                 credentials: dict = None,
-                 project_id: str = None,
-                 space_id: str = None,
-                 verify=None,
-                 api_client: APIClient = None,
-                 validate: bool = True) -> None:
-
+    def __init__(
+        self,
+        *,
+        model_id: str | None = None,
+        deployment_id: str | None = None,
+        params: dict | None = None,
+        credentials: dict | Credentials | None = None,
+        project_id: str | None = None,
+        space_id: str | None = None,
+        verify: bool | str | None = None,
+        api_client: APIClient | None = None,
+        validate: bool = True,
+    ) -> None:
         self.model_id = model_id
         if isinstance(self.model_id, ModelTypes):
             self.model_id = self.model_id.value
 
         self.deployment_id = deployment_id
 
         if self.model_id and self.deployment_id:
-            raise InvalidMultipleArguments(params_names_list=["model_id", "deployment_id"],
-                                           reason="Both arguments were provided.")
+            raise InvalidMultipleArguments(
+                params_names_list=["model_id", "deployment_id"],
+                reason="Both arguments were provided.",
+            )
         elif not self.model_id and not self.deployment_id:
-            raise InvalidMultipleArguments(params_names_list=["model_id", "deployment_id"],
-                                           reason="None of the arguments were provided.")
+            raise InvalidMultipleArguments(
+                params_names_list=["model_id", "deployment_id"],
+                reason="None of the arguments were provided.",
+            )
 
         self.params = params
-        ModelInference._validate_type(params, u'params', dict, False)
+        ModelInference._validate_type(params, "params", dict, False)
 
         if credentials:
-            self._client = APIClient(credentials, verify=verify) 
+            from ibm_watsonx_ai import APIClient
+
+            self._client = APIClient(credentials, verify=verify)
         elif api_client:
             self._client = api_client
         else:
-            raise InvalidMultipleArguments(params_names_list=["credentials", "api_client"],
-                                           reason="None of the arguments were provided.")
+            raise InvalidMultipleArguments(
+                params_names_list=["credentials", "api_client"],
+                reason="None of the arguments were provided.",
+            )
 
         if space_id:
             self._client.set.default_space(space_id)
         elif project_id:
             self._client.set.default_project(project_id)
         elif not api_client:
-            raise InvalidMultipleArguments(params_names_list=["space_id", "project_id"],
-                                           reason="None of the arguments were provided.")
+            raise InvalidMultipleArguments(
+                params_names_list=["space_id", "project_id"],
+                reason="None of the arguments were provided.",
+            )
         if not self._client.CLOUD_PLATFORM_SPACES and self._client.CPD_version < 4.8:
             raise WMLClientError(error_msg="Operation is unsupported for this release.")
 
+        self._inference: BaseModelInference
         if self.model_id:
-            self._inference = FMModelInference(model_id=self.model_id,
-                                               params=self.params,
-                                               api_client=self._client,
-                                               validate=validate)
+            self._inference = FMModelInference(
+                model_id=self.model_id,
+                api_client=self._client,
+                params=self.params,
+                validate=validate,
+            )
         else:
-            self._inference = DeploymentModelInference(deployment_id=self.deployment_id,
-                                                       params=self.params,
-                                                       api_client=self._client)
+            self.deployment_id = cast(str, self.deployment_id)
+            self._inference = DeploymentModelInference(
+                deployment_id=self.deployment_id,
+                api_client=self._client,
+                params=self.params,
+            )
         BaseModelInference.__init__(self, __name__, self._client)
 
-    def get_details(self):
+    def get_details(self) -> dict:
         """Get model interface's details
 
         :return: details of model or deployment
         :rtype: dict
 
         **Example**
 
         .. code-block:: python
 
             model_inference.get_details()
 
         """
         return self._inference.get_details()
 
-    def generate(self,
-                 prompt=None,
-                 params=None,
-                 guardrails=False,
-                 guardrails_hap_params=None,
-                 guardrails_pii_params=None,
-                 concurrency_limit=10,
-                 async_mode=False):
+    def generate(
+        self,
+        prompt: str | list | None = None,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+        async_mode: bool = False,
+    ) -> dict | list[dict] | Generator:
         """Given a text prompt as input, and parameters the selected model (model_id) or deployment (deployment_id)
         will generate a completion text as generated_text. For prompt template deployment `prompt` should be None.
 
         :param params: meta props for text generation, use ``ibm_watsonx_ai.metanames.GenTextParamsMetaNames().show()`` to view the list of MetaNames
         :type params: dict
 
         :param concurrency_limit: number of requests that will be sent in parallel, max is 10
         :type concurrency_limit: int
 
         :param prompt: the prompt string or list of strings. If list of strings is passed requests will be managed in parallel with the rate of concurency_limit, defaults to None
         :type prompt: (str | list | None), optional
 
-        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection 
+        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection
                            filter is toggle on for both prompt and generated text, defaults to False
         :type guardrails: bool
 
         :param guardrails_hap_params: meta props for HAP moderations, use ``ibm_watsonx_ai.metanames.GenTextModerationsMetaNames().show()``
                                       to view the list of MetaNames
         :type guardrails_hap_params: dict
 
@@ -211,40 +240,51 @@
         .. code-block:: python
 
             q = "What is 1 + 1?"
             generated_response = model_inference.generate(prompt=q)
             print(generated_response['results'][0]['generated_text'])
 
         """
-        self._validate_type(params, u'params', dict, False)
-        self._validate_type(concurrency_limit, 'concurrency_limit', [int, float], False,
-                            raise_error_for_list=True)
+        self._validate_type(params, "params", dict, False)
+        self._validate_type(
+            concurrency_limit,
+            "concurrency_limit",
+            [int, float],
+            False,
+            raise_error_for_list=True,
+        )
 
         if isinstance(concurrency_limit, float):  # convert float (ex. 10.0) to int
             concurrency_limit = int(concurrency_limit)
 
         if concurrency_limit > 10 or concurrency_limit < 1:
-            raise ParamOutOfRange(param_name='concurrency_limit', value=concurrency_limit, min=1, max=10)
+            raise ParamOutOfRange(
+                param_name="concurrency_limit", value=concurrency_limit, min=1, max=10
+            )
 
-        return self._inference.generate(prompt=prompt,
-                                        params=params,
-                                        guardrails=guardrails,
-                                        guardrails_hap_params=guardrails_hap_params,
-                                        guardrails_pii_params=guardrails_pii_params,
-                                        concurrency_limit=concurrency_limit,
-                                        async_mode=async_mode)
-
-    def generate_text(self,
-                      prompt=None,
-                      params=None,
-                      guardrails=False,
-                      guardrails_hap_params=None,
-                      guardrails_pii_params=None,
-                      raw_response=False,
-                      concurrency_limit=10):
+        return self._inference.generate(
+            prompt=prompt,
+            params=params,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+            concurrency_limit=concurrency_limit,
+            async_mode=async_mode,
+        )
+
+    def generate_text(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+    ) -> str | dict:
         """Given a text prompt as input, and parameters the selected model (model_id)
         will generate a completion text as generated_text. For prompt template deployment `prompt` should be None.
 
         :param params: meta props for text generation, use ``ibm_watsonx_ai.metanames.GenTextParamsMetaNames().show()`` to view the list of MetaNames
         :type params: dict
 
         :param concurrency_limit: number of requests that will be sent in parallel, max is 10
@@ -261,56 +301,65 @@
                                       to view the list of MetaNames
         :type guardrails_hap_params: dict
 
         :param raw_response: return the whole response object
         :type raw_response: bool, optional
 
         :return: generated content
-        :rtype: str
+        :rtype: str or dict
 
         .. note::
             By default only the first occurance of `HAPDetectionWarning` is displayed. To enable printing all warnings of this category, use:
 
             .. code-block:: python
 
                 import warnings
                 from ibm_watsonx_ai.foundation_models.utils import HAPDetectionWarning
 
                 warnings.filterwarnings("always", category=HAPDetectionWarning)
-            
+
 
         **Example**
 
         .. code-block:: python
 
             q = "What is 1 + 1?"
             generated_text = model_inference.generate_text(prompt=q)
             print(generated_text)
 
         """
-        metadata = self.generate(prompt=prompt, params=params,
-                                 guardrails=guardrails,
-                                 guardrails_hap_params=guardrails_hap_params,
-                                 guardrails_pii_params=guardrails_pii_params,
-                                 concurrency_limit=concurrency_limit)
+        metadata = self.generate(
+            prompt=prompt,
+            params=params,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+            concurrency_limit=concurrency_limit,
+        )
+        metadata = cast(dict, metadata)
         if raw_response:
             return metadata
         else:
             if isinstance(prompt, list):
-                return [self._return_guardrails_stats(single_response)['generated_text'] for single_response in metadata]
+                return [
+                    self._return_guardrails_stats(single_response)["generated_text"]
+                    for single_response in metadata
+                ]
             else:
-                return self._return_guardrails_stats(metadata)['generated_text']
+                return self._return_guardrails_stats(metadata)["generated_text"]
 
-    def generate_text_stream(self,
-                             prompt=None,
-                             params=None,
-                             raw_response=False,
-                             guardrails=False,
-                             guardrails_hap_params=None,
-                             guardrails_pii_params=None):
+    def generate_text_stream(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> Generator:
         """Given a text prompt as input, and parameters the selected model (model_id)
         will generate a streamed text as generate_text_stream. For prompt template deployment `prompt` should be None.
 
         :param params: meta props for text generation, use ``ibm_watsonx_ai.metanames.GenTextParamsMetaNames().show()`` to view the list of MetaNames
         :type params: dict
 
         :param prompt: the prompt string, defaults to None
@@ -330,15 +379,15 @@
         :return: scoring result containing generated content
         :rtype: generator
 
         .. note::
             By default only the first occurance of `HAPDetectionWarning` is displayed. To enable printing all warnings of this category, use:
 
             .. code-block:: python
-            
+
                 import warnings
                 from ibm_watsonx_ai.foundation_models.utils import HAPDetectionWarning
 
                 warnings.filterwarnings("always", category=HAPDetectionWarning)
 
         **Example**
 
@@ -347,26 +396,26 @@
             q = "Write an epigram about the sun"
             generated_response = model_inference.generate_text_stream(prompt=q)
 
             for chunk in generated_response:
                 print(chunk, end='')
 
         """
-        self._validate_type(params, u'params', dict, False)
+        self._validate_type(params, "params", dict, False)
+
+        return self._inference.generate_text_stream(
+            prompt=prompt,
+            params=params,
+            raw_response=raw_response,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+        )
 
-        return self._inference.generate_text_stream(prompt=prompt,
-                                                    params=params,
-                                                    raw_response=raw_response,
-                                                    guardrails=guardrails,
-                                                    guardrails_hap_params=guardrails_hap_params,
-                                                    guardrails_pii_params=guardrails_pii_params)
-
-    def tokenize(self,
-                 prompt=None,
-                 return_tokens: bool = False):
+    def tokenize(self, prompt: str, return_tokens: bool = False) -> dict:
         """
         The text tokenize operation allows you to check the conversion of provided input to tokens for a given model.
         It splits text into words or sub-words, which then are converted to ids through a look-up table (vocabulary).
         Tokenization allows the model to have a reasonable vocabulary size.
 
         .. note::
             Method is not supported for deployments, available only for base models.
@@ -385,18 +434,17 @@
         .. code-block:: python
 
             q = "Write an epigram about the moon"
             tokenized_response = model_inference.tokenize(prompt=q, return_tokens=True)
             print(tokenized_response["result"])
 
         """
-        return self._inference.tokenize(prompt=prompt,
-                                        return_tokens=return_tokens)
+        return self._inference.tokenize(prompt=prompt, return_tokens=return_tokens)
 
-    def to_langchain(self):
+    def to_langchain(self) -> WatsonxLLM:
         """
 
         :return: WatsonxLLM wrapper for watsonx foundation models
         :rtype: WatsonxLLM
 
         **Example**
 
@@ -442,13 +490,15 @@
             llm_chain = LLMChain(llm=deployed_model.to_langchain(), prompt=PromptTemplate.from_template(prompt_template))
             llm_chain('sunflower')
 
         """
         try:
             from langchain_ibm import WatsonxLLM
         except ImportError:
-            raise ImportError("Could not import langchain_ibm: Please install `langchain_ibm` extension.")
+            raise ImportError(
+                "Could not import langchain_ibm: Please install `langchain_ibm` extension."
+            )
         return WatsonxLLM(watsonx_model=self)
 
     def get_identifying_params(self) -> dict:
         """Represent Model Inference's setup in dictionary"""
         return self._inference.get_identifying_params()
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING, Generator
 
 from ibm_watsonx_ai.foundation_models.inference import ModelInference
 
+if TYPE_CHECKING:
+    from langchain_ibm import WatsonxLLM
+
+
 class Model(ModelInference):
     """Instantiate the model interface.
 
     .. hint::
         To use the Model class with LangChain, use the :func:`to_langchain() <ibm_watsonx_ai.foundation_models.Model.to_langchain>` function.
 
     :param model_id: the type of model to use
@@ -67,48 +72,51 @@
                 "apikey": "***",
                 "url": "https://us-south.ml.cloud.ibm.com"
             },
             project_id="*****"
             )
     """
 
-    def __init__(self,
-                 model_id: str,
-                 credentials: dict,
-                 params: dict = None,
-                 project_id: str = None,
-                 space_id: str = None,
-                 verify=None,
-                 validate: bool = True) -> None:
-        ModelInference.__init__(self,
-                                model_id=model_id,
-                                credentials=credentials,
-                                params=params,
-                                project_id=project_id,
-                                space_id=space_id,
-                                verify=verify,
-                                validate=validate
-                                )
+    def __init__(
+        self,
+        model_id: str,
+        credentials: dict,
+        params: dict | None = None,
+        project_id: str | None = None,
+        space_id: str | None = None,
+        verify: str | bool | None = None,
+        validate: bool = True,
+    ) -> None:
+        ModelInference.__init__(
+            self,
+            model_id=model_id,
+            credentials=credentials,
+            params=params,
+            project_id=project_id,
+            space_id=space_id,
+            verify=verify,
+            validate=validate,
+        )
 
-    def get_details(self):
+    def get_details(self) -> dict:
         """Get model's details
 
         :return: model's details
         :rtype: dict
 
         **Example**
 
         .. code-block:: python
 
             model.get_details()
 
         """
         return super().get_details()
 
-    def to_langchain(self):
+    def to_langchain(self) -> WatsonxLLM:
         """
 
         :return: WatsonxLLM wrapper for watsonx foundation models
         :rtype: WatsonxLLM
 
         **Example**
 
@@ -133,38 +141,42 @@
             llm_chain = LLMChain(llm=flan_ul2_model.to_langchain(), prompt=PromptTemplate.from_template(prompt_template))
             llm_chain('sunflower')
 
         """
         try:
             from langchain_ibm import WatsonxLLM
         except ImportError:
-            raise ImportError("Could not import langchain_ibm: Please install `langchain_ibm` extension.")
+            raise ImportError(
+                "Could not import langchain_ibm: Please install `langchain_ibm` extension."
+            )
         return WatsonxLLM(watsonx_model=self)
 
-    def generate(self,
-                 prompt,
-                 params=None,
-                 guardrails: bool = False,
-                 guardrails_hap_params: Optional[dict] = None,
-                 guardrails_pii_params: Optional[dict] = None,
-                 concurrency_limit=10,
-                 async_mode: bool = False):
+    def generate(
+        self,
+        prompt: str | list | None = None,
+        params: dict | None = None,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+        async_mode: bool = False,
+    ) -> dict | list[dict] | Generator:
         """Given a text prompt as input, and parameters the selected model (model_id)
         will generate a completion text as generated_text.
 
         :param params: meta props for text generation, use ``ibm_watsonx_ai.metanames.GenTextParamsMetaNames().show()`` to view the list of MetaNames
         :type params: dict
 
         :param concurrency_limit: number of requests that will be sent in parallel, max is 10
         :type concurrency_limit: int
 
         :param prompt: the prompt string or list of strings. If list of strings is passed requests will be managed in parallel with the rate of concurency_limit
         :type prompt: str, list
 
-        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection 
+        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection
                            filter is toggle on for both prompt and generated text, defaults to False
         :type guardrails: bool
 
         :param guardrails_hap_params: meta props for HAP moderations, use ``ibm_watsonx_ai.metanames.GenTextModerationsMetaNames().show()``
                                       to view the list of MetaNames
         :type params: dict
 
@@ -181,30 +193,34 @@
         .. code-block:: python
 
             q = "What is 1 + 1?"
             generated_response = model.generate(prompt=q)
             print(generated_response['results'][0]['generated_text'])
 
         """
-        return super().generate(prompt=prompt,
-                                params=params,
-                                guardrails=guardrails,
-                                guardrails_hap_params=guardrails_hap_params,
-                                guardrails_pii_params=guardrails_pii_params,
-                                concurrency_limit=concurrency_limit,
-                                async_mode=async_mode)
-
-    def generate_text(self,
-                      prompt,
-                      params=None,
-                      raw_response=False,
-                      guardrails=False,
-                      guardrails_hap_params=None,
-                      guardrails_pii_params=None,
-                      concurrency_limit=10):
+        return super().generate(
+            prompt=prompt,
+            params=params,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+            concurrency_limit=concurrency_limit,
+            async_mode=async_mode,
+        )
+
+    def generate_text(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+        concurrency_limit: int = 10,
+    ) -> str | dict:
         """Given a text prompt as input, and parameters the selected model (model_id)
         will generate a completion text as generated_text.
 
         :param params: meta props for text generation, use ``ibm_watsonx_ai.metanames.GenTextParamsMetaNames().show()`` to view the list of MetaNames
         :type params: dict
 
         :param concurrency_limit: number of requests that will be sent in parallel, max is 10
@@ -212,62 +228,66 @@
 
         :param prompt: the prompt string or list of strings. If list of strings is passed requests will be managed in parallel with the rate of concurency_limit
         :type prompt: str, list
 
         :param raw_response: return the whole response object
         :type raw_response: bool, optional
 
-        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection 
+        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection
                            filter is toggle on for both prompt and generated text, defaults to False
         :type guardrails: bool
 
         :param guardrails_hap_params: meta props for HAP moderations, use ``ibm_watsonx_ai.metanames.GenTextModerationsMetaNames().show()``
                                       to view the list of MetaNames
         :type params: dict
 
         :return: generated content
-        :rtype: str
+        :rtype: str or dict
 
         **Example**
 
         .. code-block:: python
 
             q = "What is 1 + 1?"
             generated_text = model.generate_text(prompt=q)
             print(generated_text)
 
         """
-        return super().generate_text(prompt=prompt,
-                                     params=params,
-                                     raw_response=raw_response,
-                                     guardrails=guardrails,
-                                     guardrails_hap_params=guardrails_hap_params,
-                                     guardrails_pii_params=guardrails_pii_params,
-                                     concurrency_limit=concurrency_limit)
-
-    def generate_text_stream(self,
-                             prompt,
-                             params=None,
-                             raw_response=False,
-                             guardrails=False,
-                             guardrails_hap_params=None,
-                             guardrails_pii_params=None):
+        return super().generate_text(
+            prompt=prompt,
+            params=params,
+            raw_response=raw_response,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+            concurrency_limit=concurrency_limit,
+        )
+
+    def generate_text_stream(
+        self,
+        prompt: str | None = None,
+        params: dict | None = None,
+        raw_response: bool = False,
+        guardrails: bool = False,
+        guardrails_hap_params: dict | None = None,
+        guardrails_pii_params: dict | None = None,
+    ) -> Generator:
         """Given a text prompt as input, and parameters the selected model (model_id)
         will generate a streamed text as generate_text_stream.
 
         :param params: meta props for text generation, use ``ibm_watsonx_ai.metanames.GenTextParamsMetaNames().show()`` to view the list of MetaNames
         :type params: dict
 
         :param prompt: the prompt string
         :type prompt: str,
 
         :param raw_response: yields the whole response object
         :type raw_response: bool, optional
 
-        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection 
+        :param guardrails: If True then potentially hateful, abusive, and/or profane language (HAP) detection
                            filter is toggle on for both prompt and generated text, defaults to False
         :type guardrails: bool
 
         :param guardrails_hap_params: meta props for HAP moderations, use ``ibm_watsonx_ai.metanames.GenTextModerationsMetaNames().show()``
                                       to view the list of MetaNames
         :type params: dict
 
@@ -281,24 +301,24 @@
             q = "Write an epigram about the sun"
             generated_response = model.generate_text_stream(prompt=q)
 
             for chunk in generated_response:
                 print(chunk, end='')
 
         """
-        return super().generate_text_stream(prompt=prompt,
-                                            params=params,
-                                            raw_response=raw_response,
-                                            guardrails=guardrails,
-                                            guardrails_hap_params=guardrails_hap_params,
-                                            guardrails_pii_params=guardrails_pii_params)
-
-    def tokenize(self,
-                 prompt,
-                 return_tokens: bool = False):
+        return super().generate_text_stream(
+            prompt=prompt,
+            params=params,
+            raw_response=raw_response,
+            guardrails=guardrails,
+            guardrails_hap_params=guardrails_hap_params,
+            guardrails_pii_params=guardrails_pii_params,
+        )
+
+    def tokenize(self, prompt: str, return_tokens: bool = False) -> dict:
         """
         The text tokenize operation allows you to check the conversion of provided input to tokens for a given model.
         It splits text into words or sub-words, which then are converted to ids through a look-up table (vocabulary).
         Tokenization allows the model to have a reasonable vocabulary size.
 
         :param prompt: the prompt string
         :type prompt: str
@@ -314,9 +334,8 @@
         .. code-block:: python
 
             q = "Write an epigram about the moon"
             tokenized_response = model.tokenize(prompt=q, return_tokens=True)
             print(tokenized_response["result"])
 
         """
-        return super().tokenize(prompt=prompt,
-                                return_tokens=return_tokens)
+        return super().tokenize(prompt=prompt, return_tokens=return_tokens)
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/prompt_tuner.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/prompt_tuner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,115 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from typing import List, Dict
+from __future__ import annotations
+from typing import TYPE_CHECKING, cast
 
-from ibm_watsonx_ai import APIClient
 from ibm_watsonx_ai.messages.messages import Messages
 from ibm_watsonx_ai.wml_resource import WMLResource
 from ibm_watsonx_ai.wml_client_error import WMLClientError
 from ibm_watsonx_ai.utils.autoai.errors import ContainerTypeNotSupported
-from ibm_watsonx_ai.helpers.connections import (DataConnection, ContainerLocation, S3Connection,
-                                                             S3Location, FSLocation, AssetLocation)
+from ibm_watsonx_ai.helpers.connections import (
+    DataConnection,
+    ContainerLocation,
+    S3Connection,
+    S3Location,
+    FSLocation,
+    AssetLocation,
+)
 from ibm_watsonx_ai.utils.autoai.utils import is_ipython
 from ibm_watsonx_ai.foundation_models.utils import PromptTuningParams
 
 import datetime
 import numpy as np
 
 
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
+    from pandas import DataFrame
+
+
 class PromptTuner:
-    id: str = None
+    id: str | None = None
     _client: APIClient = None
-    _training_metadata: dict = None
-
-    def __init__(self,
-                 name: str,
-                 task_id: str,
-                 *,
-                 description: str = None,
-                 base_model: str = None,
-                 accumulate_steps: int = None,
-                 batch_size: int = None,
-                 init_method: str = None,
-                 init_text: str = None,
-                 learning_rate: float = None,
-                 max_input_tokens: int = None,
-                 max_output_tokens: int = None,
-                 num_epochs: int = None,
-                 verbalizer: str = None,
-                 tuning_type: str = None,
-                 auto_update_model: bool = True,
-                 group_by_name: bool = None):
+    _training_metadata: dict | None = None
 
+    def __init__(
+        self,
+        name: str,
+        task_id: str,
+        *,
+        description: str | None = None,
+        base_model: str | None = None,
+        accumulate_steps: int | None = None,
+        batch_size: int | None = None,
+        init_method: str | None = None,
+        init_text: str | None = None,
+        learning_rate: float | None = None,
+        max_input_tokens: int | None = None,
+        max_output_tokens: int | None = None,
+        num_epochs: int | None = None,
+        verbalizer: str | None = None,
+        tuning_type: str | None = None,
+        auto_update_model: bool = True,
+        group_by_name: bool | None = None,
+    ):
         self.name = name
         self.description = description if description else "Prompt tuning with SDK"
         self.auto_update_model = auto_update_model
         self.group_by_name = group_by_name
 
-        base_model = {'model_id': base_model}
+        base_model_red: dict = {"model_id": base_model}
 
-        self.prompt_tuning_params = PromptTuningParams(base_model=base_model,
-                                                       accumulate_steps=accumulate_steps,
-                                                       batch_size=batch_size,
-                                                       init_method=init_method,
-                                                       init_text=init_text,
-                                                       learning_rate=learning_rate,
-                                                       max_input_tokens=max_input_tokens,
-                                                       max_output_tokens=max_output_tokens,
-                                                       num_epochs=num_epochs,
-                                                       task_id=task_id,
-                                                       tuning_type=tuning_type,
-                                                       verbalizer=verbalizer)
+        self.prompt_tuning_params = PromptTuningParams(
+            base_model=base_model_red,
+            accumulate_steps=accumulate_steps,
+            batch_size=batch_size,
+            init_method=init_method,
+            init_text=init_text,
+            learning_rate=learning_rate,
+            max_input_tokens=max_input_tokens,
+            max_output_tokens=max_output_tokens,
+            num_epochs=num_epochs,
+            task_id=task_id,
+            tuning_type=tuning_type,
+            verbalizer=verbalizer,
+        )
 
         if not isinstance(self.name, str):
-            raise WMLClientError(f"'name' param expected string, but got {type(self.name)}: {self.name}")
+            raise WMLClientError(
+                f"'name' param expected string, but got {type(self.name)}: {self.name}"
+            )
 
         if self.description and (not isinstance(self.description, str)):
-            raise WMLClientError(f"'description' param expected string, but got {type(self.description)}: "
-                                 f"{self.description}")
+            raise WMLClientError(
+                f"'description' param expected string, but got {type(self.description)}: "
+                f"{self.description}"
+            )
 
         if self.auto_update_model and (not isinstance(self.auto_update_model, bool)):
-            raise WMLClientError(f"'auto_update_model' param expected bool, but got {type(self.auto_update_model)}: "
-                                 f"{self.auto_update_model}")
+            raise WMLClientError(
+                f"'auto_update_model' param expected bool, but got {type(self.auto_update_model)}: "
+                f"{self.auto_update_model}"
+            )
 
         if self.group_by_name and (not isinstance(self.group_by_name, bool)):
-            raise WMLClientError(f"'group_by_name' param expected bool, but got {type(self.group_by_name)}: "
-                                 f"{self.group_by_name}")
-
-    def run(self,
-            training_data_references: List['DataConnection'],
-            training_results_reference: DataConnection = None,
-            background_mode=False
-            ) -> dict:
+            raise WMLClientError(
+                f"'group_by_name' param expected bool, but got {type(self.group_by_name)}: "
+                f"{self.group_by_name}"
+            )
+
+    def run(
+        self,
+        training_data_references: list[DataConnection],
+        training_results_reference: DataConnection | None = None,
+        background_mode: bool = False,
+    ) -> dict:
         """Run a prompt tuning process of foundation model on top of the training data referenced by DataConnection.
 
         :param training_data_references: data storage connection details to inform where training data is stored
         :type training_data_references: list[DataConnection]
 
         :param training_results_reference: data storage connection details to store pipeline training results
         :type training_results_reference: DataConnection, optional
@@ -112,223 +135,290 @@
                     connection_asset_id=connection_id,
                     location=S3Location(
                         bucket='prompt_tuning_data',
                         path='pt_train_data.json')
                     )
                 )]
                 background_mode=False)
-            """
-        WMLResource._validate_type(training_data_references, "training_data_references", list, mandatory=True)
-        WMLResource._validate_type(training_results_reference, "training_results_reference", object, mandatory=False)
+        """
+        WMLResource._validate_type(
+            training_data_references, "training_data_references", list, mandatory=True
+        )
+        WMLResource._validate_type(
+            training_results_reference,
+            "training_results_reference",
+            object,
+            mandatory=False,
+        )
 
         for source_data_connection in [training_data_references]:
             if source_data_connection:
                 self._validate_source_data_connections(source_data_connection)
-
-        training_results_reference = self._determine_result_reference(results_reference=training_results_reference,
-                                                                      data_references=training_data_references)
-
-        self._initialize_training_metadata(training_data_references, test_data_references=None,
-                                               training_results_reference=training_results_reference)
-
-        tuning_details = self._client.training.run(meta_props=self._training_metadata, asynchronous=background_mode)
+        training_results_reference = cast(DataConnection, training_results_reference)
+        training_results_reference = self._determine_result_reference(
+            results_reference=training_results_reference,
+            data_references=training_data_references,
+        )
+
+        self._initialize_training_metadata(
+            training_data_references,
+            test_data_references=None,
+            training_results_reference=training_results_reference,
+        )
+
+        self._training_metadata = cast(dict, self._training_metadata)
+        tuning_details = self._client.training.run(
+            meta_props=self._training_metadata, asynchronous=background_mode
+        )
         self.id = self._client.training.get_id(tuning_details)
 
-        return self._client.training.get_details(self.id)  # TODO improve the background_mode = False option
-
-    def _initialize_training_metadata(self,
-                                          training_data_references: List['DataConnection'],
-                                          test_data_references: List['DataConnection'] = None,
-                                          training_results_reference: DataConnection = None,
-                                          ):
-
+        return self._client.training.get_details(
+            self.id
+        )  # TODO improve the background_mode = False option
+
+    def _initialize_training_metadata(
+        self,
+        training_data_references: list[DataConnection],
+        test_data_references: list[DataConnection] | None = None,
+        training_results_reference: DataConnection | None = None,
+    ) -> None:
         self._training_metadata = {
             self._client.training.ConfigurationMetaNames.TAGS: self._get_tags(),
-
-            self._client.training.ConfigurationMetaNames.TRAINING_DATA_REFERENCES:
-                [connection._to_dict() for connection in training_data_references],
-
+            self._client.training.ConfigurationMetaNames.TRAINING_DATA_REFERENCES: [
+                connection._to_dict() for connection in training_data_references
+            ],
             self._client.training.ConfigurationMetaNames.NAME: f"{self.name[:100]}",
-            self._client.training.ConfigurationMetaNames.PROMPT_TUNING: self.prompt_tuning_params.to_dict()
+            self._client.training.ConfigurationMetaNames.PROMPT_TUNING: self.prompt_tuning_params.to_dict(),
         }
         if test_data_references:
-            self._training_metadata[self._client.training.ConfigurationMetaNames.TEST_DATA_REFERENCES] = [
-                connection._to_dict() for connection in test_data_references]
+            self._training_metadata[
+                self._client.training.ConfigurationMetaNames.TEST_DATA_REFERENCES
+            ] = [connection._to_dict() for connection in test_data_references]
         if training_results_reference:
             self._training_metadata[
-                self._client.training.ConfigurationMetaNames.TRAINING_RESULTS_REFERENCE] = \
-                training_results_reference._to_dict()
+                self._client.training.ConfigurationMetaNames.TRAINING_RESULTS_REFERENCE
+            ] = training_results_reference._to_dict()
 
         if self.description:
             self._training_metadata[
-                self._client.training.ConfigurationMetaNames.DESCRIPTION] = f"{self.description}"
+                self._client.training.ConfigurationMetaNames.DESCRIPTION
+            ] = f"{self.description}"
 
         if self.auto_update_model is not None:
             self._training_metadata[
-                self._client.training.ConfigurationMetaNames.AUTO_UPDATE_MODEL] = self.auto_update_model
+                self._client.training.ConfigurationMetaNames.AUTO_UPDATE_MODEL
+            ] = self.auto_update_model
 
-    def _validate_source_data_connections(self, source_data_connections):
+    def _validate_source_data_connections(
+        self, source_data_connections: list[DataConnection]
+    ) -> list[DataConnection]:
         for data_connection in source_data_connections:
             if isinstance(data_connection.location, ContainerLocation):
-                if self._client.ICP:
+                if self._client.ICP_PLATFORM_SPACES:
                     raise ContainerTypeNotSupported()  # block Container type on CPD
                 elif isinstance(data_connection.connection, S3Connection):
                     # note: remove S3 inline credential from data asset before training
                     data_connection.connection = None
-                    if hasattr(data_connection.location, 'bucket'):
-                        delattr(data_connection.location, 'bucket')
+                    if hasattr(data_connection.location, "bucket"):
+                        delattr(data_connection.location, "bucket")
                     # --- end note
-            if isinstance(data_connection.connection, S3Connection) and isinstance(data_connection.location,
-                                                                                   AssetLocation):
+            if isinstance(data_connection.connection, S3Connection) and isinstance(
+                data_connection.location, AssetLocation
+            ):
                 # note: remove S3 inline credential from data asset before training
                 data_connection.connection = None
 
-                for s3_attr in ['bucket', 'path']:
+                for s3_attr in ["bucket", "path"]:
                     if hasattr(data_connection.location, s3_attr):
                         delattr(data_connection.location, s3_attr)
                 # --- end note
 
         return source_data_connections
 
-    def _determine_result_reference(self, results_reference, data_references, result_path="default_tuning_output"):
+    def _determine_result_reference(
+        self,
+        results_reference: DataConnection,
+        data_references: list[DataConnection],
+        result_path: str = "default_tuning_output",
+    ) -> DataConnection:
         # note: if user did not provide results storage information, use default ones
         if results_reference is None:
-            if self._client.ICP:
+            if self._client.ICP_PLATFORM_SPACES:
                 location = FSLocation(path="/{option}/{id}/assets/wx_prompt_tune")
                 if self._client.default_project_id is None:
-                    location.path = location.path.format(option='spaces',
-                                                         id=self._client.default_space_id)
+                    location.path = location.path.format(
+                        option="spaces", id=self._client.default_space_id
+                    )
 
                 else:
-                    location.path = location.path.format(option='projects',
-                                                         id=self._client.default_project_id)
-                results_reference = DataConnection(
-                    connection=None,
-                    location=location
-                )
+                    location.path = location.path.format(
+                        option="projects", id=self._client.default_project_id
+                    )
+                results_reference = DataConnection(connection=None, location=location)
 
             else:
                 if isinstance(data_references[0].location, S3Location):
                     results_reference = DataConnection(
                         connection=data_references[0].connection,
-                        location=S3Location(bucket=data_references[0].location.bucket,
-                                            path=".")
+                        location=S3Location(
+                            bucket=data_references[0].location.bucket, path="."
+                        ),
                     )
 
                 elif isinstance(data_references[0].location, AssetLocation):
-                    connection_id = data_references[0].location._get_connection_id(self._client)
+                    connection_id = data_references[0].location._get_connection_id(
+                        self._client
+                    )
 
                     if connection_id is not None:
                         results_reference = DataConnection(
                             connection_asset_id=connection_id,
                             location=S3Location(
-                                bucket=data_references[0].location._get_bucket(self._client),
-                                path=result_path)
+                                bucket=data_references[0].location._get_bucket(
+                                    self._client
+                                ),
+                                path=result_path,
+                            ),
                         )
 
                     else:  # set container output location when default DAta Asset is as a train ref
                         results_reference = DataConnection(
-                            location=ContainerLocation(path=result_path))
+                            location=ContainerLocation(path=result_path)
+                        )
 
                 else:
-                    results_reference = DataConnection(location=ContainerLocation(path=result_path))
+                    results_reference = DataConnection(
+                        location=ContainerLocation(path=result_path)
+                    )
         # -- end note
 
         # note: validate location types:
-        if self._client.ICP:
-            if not isinstance(results_reference.location,
-                              FSLocation):
-                raise TypeError('Unsupported results location type. Results reference can be stored on FSLocation.')
+        if self._client.ICP_PLATFORM_SPACES:
+            if not isinstance(results_reference.location, FSLocation):
+                raise TypeError(
+                    "Unsupported results location type. Results reference can be stored on FSLocation."
+                )
         else:
-            if not isinstance(results_reference.location,
-                              (S3Location, ContainerLocation)):
-                raise TypeError('Unsupported results location type. Results reference can be stored'
-                                ' only on S3Location or ContainerLocation.')
+            if not isinstance(
+                results_reference.location, (S3Location, ContainerLocation)
+            ):
+                raise TypeError(
+                    "Unsupported results location type. Results reference can be stored"
+                    " only on S3Location or ContainerLocation."
+                )
         # -- end note
         return results_reference
 
-    def _get_tags(self):
-
-        tags = ['prompt_tuning']
+    def _get_tags(self) -> list:
+        tags = ["prompt_tuning"]
         if self.group_by_name is not None and self.group_by_name:
-
-            for training in self._client.training.get_details(tag_value='prompt_tuning')['resources']:
-                if training['metadata'].get('name') == self.name:
+            for training in self._client.training.get_details(
+                tag_value="prompt_tuning"
+            )["resources"]:
+                if training["metadata"].get("name") == self.name:
                     # Find recent tags related to 'name'
-                    tags = list(set(tags) | set(training['metadata'].get('tags')))
+                    tags = list(set(tags) | set(training["metadata"].get("tags")))
                     break
 
-            if tags != ['prompt_tuning']:
+            if tags != ["prompt_tuning"]:
                 self._client.generate_ux_tag = False
 
         return tags
 
     @staticmethod
-    def _get_last_iteration_metrics_for_each_epoch(tuning_details):
-
+    def _get_last_iteration_metrics_for_each_epoch(tuning_details: dict) -> list:
         last_iteration_metrics_for_each_epoch = []
-        for ind in range(len(tuning_details['entity']['status']['metrics'])):
+        for ind in range(len(tuning_details["entity"]["status"]["metrics"])):
             if ind == 0:
-                last_iteration_metrics_for_each_epoch.append(tuning_details['entity']['status']['metrics'][0])
+                last_iteration_metrics_for_each_epoch.append(
+                    tuning_details["entity"]["status"]["metrics"][0]
+                )
             else:
-                if tuning_details['entity']['status']['metrics'][ind]['ml_metrics']['epoch'] == \
-                        tuning_details['entity']['status']['metrics'][ind - 1]['ml_metrics']['epoch']:
+                if (
+                    tuning_details["entity"]["status"]["metrics"][ind]["ml_metrics"][
+                        "epoch"
+                    ]
+                    == tuning_details["entity"]["status"]["metrics"][ind - 1][
+                        "ml_metrics"
+                    ]["epoch"]
+                ):
                     last_iteration_metrics_for_each_epoch.pop()
-                    last_iteration_metrics_for_each_epoch.append(tuning_details['entity']['status']['metrics'][ind])
+                    last_iteration_metrics_for_each_epoch.append(
+                        tuning_details["entity"]["status"]["metrics"][ind]
+                    )
                 else:
-                    last_iteration_metrics_for_each_epoch.append(tuning_details['entity']['status']['metrics'][ind])
+                    last_iteration_metrics_for_each_epoch.append(
+                        tuning_details["entity"]["status"]["metrics"][ind]
+                    )
         return last_iteration_metrics_for_each_epoch
 
     @staticmethod
-    def _get_average_loss_score_for_each_epoch(tuning_details):
-
+    def _get_average_loss_score_for_each_epoch(tuning_details: dict) -> list:
         scores = []
         temp_score = []
         epoch = 0
-        if "data" in tuning_details['entity']['status']['metrics'][0]:
-            for ind, metric in enumerate(tuning_details['entity']['status']['metrics']):
-                if int(metric['data']['epoch']) == epoch:
-                    temp_score.append(metric['data']['value'])
+        if "data" in tuning_details["entity"]["status"]["metrics"][0]:
+            for ind, metric in enumerate(tuning_details["entity"]["status"]["metrics"]):
+                if int(metric["data"]["epoch"]) == epoch:
+                    temp_score.append(metric["data"]["value"])
                 else:
                     epoch += 1
                     scores.append(np.average(temp_score))
-                    temp_score = [metric['data']['value']]
+                    temp_score = [metric["data"]["value"]]
             scores.append(np.average(temp_score))
         else:
-            for ind, metric in enumerate(tuning_details['entity']['status']['metrics']):
-                if int(metric['ml_metrics']['epoch']) == epoch:
-                    temp_score.append(metric['ml_metrics']['loss'])
+            for ind, metric in enumerate(tuning_details["entity"]["status"]["metrics"]):
+                if int(metric["ml_metrics"]["epoch"]) == epoch:
+                    temp_score.append(metric["ml_metrics"]["loss"])
                 else:
                     epoch += 1
                     scores.append(np.average(temp_score))
-                    temp_score = [metric['ml_metrics']['loss']]
+                    temp_score = [metric["ml_metrics"]["loss"]]
             scores.append(np.average(temp_score))
         return scores
 
     @staticmethod
-    def _get_first_and_last_iteration_metrics_for_each_epoch(tuning_details):
-
+    def _get_first_and_last_iteration_metrics_for_each_epoch(
+        tuning_details: dict,
+    ) -> list:
         first_and_last_iteration_metrics_for_each_epoch = []
         first_iteration = True
 
-        tuning_metrics = tuning_details['entity']['status']['metrics']
+        tuning_metrics = tuning_details["entity"]["status"]["metrics"]
         for ind in range(len(tuning_metrics)):
             if ind == 0:
-                first_and_last_iteration_metrics_for_each_epoch.append(tuning_metrics[ind])
-                first_and_last_iteration_metrics_for_each_epoch.append(tuning_metrics[ind])
+                first_and_last_iteration_metrics_for_each_epoch.append(
+                    tuning_metrics[ind]
+                )
+                first_and_last_iteration_metrics_for_each_epoch.append(
+                    tuning_metrics[ind]
+                )
                 first_iteration = False
             elif first_iteration:
-                first_and_last_iteration_metrics_for_each_epoch.append(tuning_metrics[ind])
+                first_and_last_iteration_metrics_for_each_epoch.append(
+                    tuning_metrics[ind]
+                )
                 first_iteration = False
             else:
-                if tuning_metrics[ind].get("data", tuning_metrics[ind].get("ml_metrics"))['epoch'] == tuning_metrics[ind - 1].get("data", tuning_metrics[ind-1].get("ml_metrics"))['epoch']:
+                if (
+                    tuning_metrics[ind].get(
+                        "data", tuning_metrics[ind].get("ml_metrics")
+                    )["epoch"]
+                    == tuning_metrics[ind - 1].get(
+                        "data", tuning_metrics[ind - 1].get("ml_metrics")
+                    )["epoch"]
+                ):
                     first_and_last_iteration_metrics_for_each_epoch.pop()
-                    first_and_last_iteration_metrics_for_each_epoch.append(tuning_metrics[ind])
+                    first_and_last_iteration_metrics_for_each_epoch.append(
+                        tuning_metrics[ind]
+                    )
                 else:
-                    first_and_last_iteration_metrics_for_each_epoch.append(tuning_metrics[ind])
+                    first_and_last_iteration_metrics_for_each_epoch.append(
+                        tuning_metrics[ind]
+                    )
                     first_iteration = True
         return first_and_last_iteration_metrics_for_each_epoch
 
     def get_params(self) -> dict:
         """Get configuration parameters of PromptTuner.
 
         :return: PromptTuner parameters
@@ -351,25 +441,25 @@
             #  'task_id': 'summarization',
             #  'name': 'Prompt Tuning of Flan T5 model',
             #  'auto_update_model': False,
             #  'group_by_name': False}
         """
 
         params = self.prompt_tuning_params.to_dict()
-        params['name'] = self.name
-        params['description'] = self.description
-        params['auto_update_model'] = self.auto_update_model
-        params['group_by_name'] = self.group_by_name
+        params["name"] = self.name
+        params["description"] = self.description
+        params["auto_update_model"] = self.auto_update_model
+        params["group_by_name"] = self.group_by_name
         return params
 
     #####################
     #   Run operations  #
     #####################
 
-    def get_run_status(self):
+    def get_run_status(self) -> str:
         """Check status/state of initialized Prompt Tuning run if ran in background mode.
 
         :return: Prompt tuning run status
         :rtype: str
 
         **Example**
 
@@ -383,17 +473,19 @@
 
             prompt_tuner.get_run_details()
 
             # Result:
             # 'completed'
         """
         if self.id is None:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_not_scheduled"))
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_not_scheduled")
+            )
 
-        return self._client.training.get_status(training_uid=self.id).get('state')
+        return self._client.training.get_status(training_uid=self.id).get("state")  # type: ignore[return-value]
 
     def get_run_details(self, include_metrics: bool = False) -> dict:
         """Get prompt tuning run details.
 
         :param include_metrics: indicates to include metrics in the training details output
         :type include_metrics: bool, optional
 
@@ -409,41 +501,47 @@
             experiment = TuneExperiment(credentials, ...)
             prompt_tuner = experiment.prompt_tuner(...)
             prompt_tuner.run(...)
 
             prompt_tuner.get_run_details()
         """
         if self.id is None:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_not_scheduled"))
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_not_scheduled")
+            )
 
-        details = self._client.training.get_details(training_uid=self.id)
+        details = self._client.training.get_details(training_id=self.id)
 
         if include_metrics:
             try:
-                details["entity"]["status"]["metrics"] = self._get_metrics_data_from_property_or_file(details)
+                details["entity"]["status"]["metrics"] = (
+                    self._get_metrics_data_from_property_or_file(details)
+                )
             except KeyError:
                 pass
             finally:
                 return details
 
-        if details['entity']['status'].get('metrics', False):
-            del details['entity']['status']['metrics']
+        if details["entity"]["status"].get("metrics", False):
+            del details["entity"]["status"]["metrics"]
 
         return details
 
-    def _get_metrics_data_from_property_or_file(self, details: Dict) -> Dict:
-        path = details["entity"]["status"]["metrics"][0]["context"]["prompt_tuning"]["metrics_location"]
-        results_reference = details["entity"]['results_reference']
+    def _get_metrics_data_from_property_or_file(self, details: dict) -> dict:
+        path = details["entity"]["status"]["metrics"][0]["context"]["prompt_tuning"][
+            "metrics_location"
+        ]
+        results_reference = details["entity"]["results_reference"]
         conn = DataConnection._from_dict(results_reference)
         conn._wml_client = self._client
         metrics_data = conn._download_json_file(path)
 
         return metrics_data
 
-    def plot_learning_curve(self):
+    def plot_learning_curve(self) -> None:
         """Plot learning curves.
 
         .. note ::
             Available only for Jupyter notebooks.
 
         **Example**
 
@@ -454,47 +552,68 @@
             experiment = TuneExperiment(credentials, ...)
             prompt_tuner = experiment.prompt_tuner(...)
             prompt_tuner.run(...)
 
             prompt_tuner.plot_learning_curve()
         """
         if not is_ipython():
-            raise WMLClientError("Function `plot_learning_curve` is available only for Jupyter notebooks.")
+            raise WMLClientError(
+                "Function `plot_learning_curve` is available only for Jupyter notebooks."
+            )
         from ibm_watsonx_ai.utils.autoai.incremental import plot_learning_curve
         import matplotlib.pyplot as plt
-        
-        tuning_details = self.get_run_details(include_metrics=True)
 
-        if 'metrics' in tuning_details['entity']['status']:
+        tuning_details = self.get_run_details(include_metrics=True)
 
+        if "metrics" in tuning_details["entity"]["status"]:
             # average loss score for each epoch
-            scores = self._get_average_loss_score_for_each_epoch(tuning_details=tuning_details)
+            scores = self._get_average_loss_score_for_each_epoch(
+                tuning_details=tuning_details
+            )
 
             # date_time from the first and last iteration on each epoch
-            if "data" in tuning_details['entity']['status']['metrics'][0]:
-                date_times = [datetime.datetime.strptime(m_obj["data"]['timestamp'], '%Y-%m-%dT%H:%M:%S.%f')
-                              for m_obj in
-                              self._get_first_and_last_iteration_metrics_for_each_epoch(tuning_details=tuning_details)]
+            if "data" in tuning_details["entity"]["status"]["metrics"][0]:
+                date_times = [
+                    datetime.datetime.strptime(
+                        m_obj["data"]["timestamp"], "%Y-%m-%dT%H:%M:%S.%f"
+                    )
+                    for m_obj in self._get_first_and_last_iteration_metrics_for_each_epoch(
+                        tuning_details=tuning_details
+                    )
+                ]
             else:
-                date_times = [datetime.datetime.strptime(m_obj['timestamp'], '%Y-%m-%dT%H:%M:%S.%f%z')
-                              for m_obj in self._get_first_and_last_iteration_metrics_for_each_epoch(tuning_details=tuning_details)]
+                date_times = [
+                    datetime.datetime.strptime(
+                        m_obj["timestamp"], "%Y-%m-%dT%H:%M:%S.%f%z"
+                    )
+                    for m_obj in self._get_first_and_last_iteration_metrics_for_each_epoch(
+                        tuning_details=tuning_details
+                    )
+                ]
 
             elapsed_time = []
             for i in range(1, len(date_times), 2):
                 elapsed_time.append((date_times[i] - date_times[i - 1]).total_seconds())
 
             fig, axes = plt.subplots(1, 3, figsize=(18, 4))
             if scores:
-                plot_learning_curve(fig=fig, axes=axes, scores=scores, fit_times=elapsed_time,
-                                    xlabels={'first_xlabel': 'Epochs', 'second_xlabel': 'Epochs'},
-                                    titles={'first_plot': 'Loss function'})
+                plot_learning_curve(
+                    fig=fig,
+                    axes=axes,
+                    scores=scores,
+                    fit_times=elapsed_time,
+                    xlabels={"first_xlabel": "Epochs", "second_xlabel": "Epochs"},
+                    titles={"first_plot": "Loss function"},
+                )
         else:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_no_metrics"))
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_no_metrics")
+            )
 
-    def summary(self, scoring: str = 'loss') -> 'DataFrame':
+    def summary(self, scoring: str = "loss") -> DataFrame:
         """Print PromptTuner models details (prompt-tuned models).
 
         :param scoring: scoring metric which user wants to use to sort pipelines by,
             when not provided use loss one
         :type scoring: string, optional
 
         :return: computed models and metrics
@@ -515,60 +634,85 @@
             # Result:
             #                          Enhancements            Base model  ...         loss
             #       Model Name
             # Prompt_tuned_M_1      [prompt_tuning]     google/flan-t5-xl  ...     0.449197
         """
 
         if self.id is None:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_not_scheduled"))
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_not_scheduled")
+            )
 
         from pandas import DataFrame
 
         details = self.get_run_details(include_metrics=True)
 
-        metrics = details['entity']['status'].get('metrics', [{}])[0]
-        is_ml_metrics = 'data' in metrics or 'ml_metrics' in metrics
+        metrics = details["entity"]["status"].get("metrics", [{}])[0]
+        is_ml_metrics = "data" in metrics or "ml_metrics" in metrics
 
         if not is_ml_metrics:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_no_metrics"))
-
-        columns = ['Model Name', 'Enhancements', 'Base model', 'Auto store', 'Epochs', scoring]
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_no_metrics")
+            )
+
+        columns = [
+            "Model Name",
+            "Enhancements",
+            "Base model",
+            "Auto store",
+            "Epochs",
+            scoring,
+        ]
         values = []
-        model_name = 'model_' + self.id
+        model_name = "model_" + self.id
         base_model_name = None
         epochs = None
         enhancements = []
-        if scoring == 'loss':
-            model_metrics = [self._get_average_loss_score_for_each_epoch(tuning_details=details)[-1]]
+        if scoring == "loss":
+            model_metrics = [
+                self._get_average_loss_score_for_each_epoch(tuning_details=details)[-1]
+            ]
         else:
-            if "data" in details['entity']['status']['metrics'][0]:
-                model_metrics = [details['entity']['status'].get('metrics', [{}])[-1].get('data', {})[scoring]]
+            if "data" in details["entity"]["status"]["metrics"][0]:
+                model_metrics = [
+                    details["entity"]["status"]
+                    .get("metrics", [{}])[-1]
+                    .get("data", {})[scoring]
+                ]
             else:
-                model_metrics = [details['entity']['status'].get('metrics', [{}])[-1].get('ml_metrics', {})[scoring]]
-
-        if 'prompt_tuning' in details['entity']:
-            enhancements = [details['entity']['prompt_tuning']['tuning_type']]
-            base_model_name = details['entity']['prompt_tuning']['base_model']['model_id']
-            epochs = details['entity']['prompt_tuning']['num_epochs']
-
-        values.append((
-                [model_name] +
-                [enhancements] +
-                [base_model_name] +
-                [details['entity']['auto_update_model']] +
-                [epochs] +
-                model_metrics
-             ))
+                model_metrics = [
+                    details["entity"]["status"]
+                    .get("metrics", [{}])[-1]
+                    .get("ml_metrics", {})[scoring]
+                ]
+
+        if "prompt_tuning" in details["entity"]:
+            enhancements = [details["entity"]["prompt_tuning"]["tuning_type"]]
+            base_model_name = details["entity"]["prompt_tuning"]["base_model"][
+                "model_id"
+            ]
+            epochs = details["entity"]["prompt_tuning"]["num_epochs"]
+
+        values.append(
+            (
+                [model_name]
+                + [enhancements]
+                + [base_model_name]
+                + [details["entity"]["auto_update_model"]]
+                + [epochs]
+                + model_metrics
+            )
+        )
 
         summary = DataFrame(data=values, columns=columns)
-        summary.set_index('Model Name', inplace=True)
+        summary.set_index("Model Name", inplace=True)
 
         return summary
 
-    def get_model_id(self):
+    def get_model_id(self) -> str:
         """Get model id.
 
         **Example**
 
         .. code-block:: python
 
             from ibm_watsonx_ai.experiment import TuneExperiment
@@ -577,32 +721,36 @@
             prompt_tuner = experiment.prompt_tuner(...)
             prompt_tuner.run(...)
 
             prompt_tuner.get_model_id()
         """
 
         run_details = self.get_run_details()
-        if run_details['entity']['auto_update_model']:
-            return run_details['entity']['model_id']
+        if run_details["entity"]["auto_update_model"]:
+            return run_details["entity"]["model_id"]
         else:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_no_model_id"))
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_no_model_id")
+            )
 
-    def cancel_run(self, hard_delete=False) -> None:
+    def cancel_run(self, hard_delete: bool = False) -> None:
         """Cancels or deletes a Prompt Tuning run.
 
         :param hard_delete: When True then the completed or cancelled prompt tuning run is deleted,
                             if False then the current run is canceled. Default: False
         :type hard_delete: bool, optional
         """
         if self.id is None:
-            raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_not_scheduled"))
+            raise WMLClientError(
+                Messages.get_message(message_id="fm_prompt_tuning_not_scheduled")
+            )
 
-        self._client.training.cancel(training_uid=self.id, hard_delete=hard_delete)
+        self._client.training.cancel(training_id=self.id, hard_delete=hard_delete)
 
-    def get_data_connections(self) -> List['DataConnection']:
+    def get_data_connections(self) -> list[DataConnection]:
         """Create DataConnection objects for further user usage
             (eg. to handle data storage connection).
 
         :return: list of DataConnections
         :rtype: list['DataConnection']
 
         **Example**
@@ -613,17 +761,21 @@
             experiment = TuneExperiment(credentials, ...)
             prompt_tuner = experiment.prompt_tuner(...)
             prompt_tuner.run(...)
 
             data_connections = prompt_tuner.get_data_connections()
         """
 
-        training_data_references = self.get_run_details()['entity']['training_data_references']
+        training_data_references = self.get_run_details()["entity"][
+            "training_data_references"
+        ]
 
         data_connections = [
-            DataConnection._from_dict(_dict=data_connection) for data_connection in training_data_references]
+            DataConnection._from_dict(_dict=data_connection)
+            for data_connection in training_data_references
+        ]
 
         for data_connection in data_connections:
             data_connection.set_client(self._client)
             data_connection._run_id = self.id
 
         return data_connections
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/prompts/prompt_template.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/prompts/prompt_template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,101 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
 from __future__ import annotations
 
-from typing import Optional, List, Dict, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, cast, Any
 
 if TYPE_CHECKING:
     import langchain
+    from langchain.prompts import PromptTemplate as LcPromptTemplate
 from dataclasses import dataclass
 from datetime import datetime
 
 import pandas
 
 import ibm_watsonx_ai._wrappers.requests as requests
-from ibm_watsonx_ai import APIClient
-from ibm_watsonx_ai.wml_client_error import (WMLClientError, ValidationError,
-                                                          InvalidValue, InvalidMultipleArguments, PromptVariablesError)
+from ibm_watsonx_ai import APIClient, Credentials
+from ibm_watsonx_ai.wml_client_error import (
+    WMLClientError,
+    ValidationError,
+    InvalidValue,
+    InvalidMultipleArguments,
+    PromptVariablesError,
+)
 from ibm_watsonx_ai.wml_resource import WMLResource
-from ibm_watsonx_ai.foundation_models.utils.enums import ModelTypes, PromptTemplateFormats
+from ibm_watsonx_ai.foundation_models.utils.enums import (
+    ModelTypes,
+    PromptTemplateFormats,
+)
 from ibm_watsonx_ai.foundation_models.utils.utils import TemplateFormatter
 
 
 @dataclass
 class PromptTemplateLock:
-    """Storage for lock object.
-    """
+    """Storage for lock object."""
+
     locked: bool
-    locked_by: Optional[str] = None
+    locked_by: str | None = None
 
 
 class PromptTemplate:
     """Storage for prompt template parameters.
 
     :param prompt_id: Id of prompt template, defaults to None.
-    :type prompt_id: Optional[str], attribute setting not allowed
+    :type prompt_id: str, attribute setting not allowed
 
     :param created_at: Time the prompt was created (UTC), defaults to None.
-    :type created_at: Optional[str], attribute setting not allowed 
+    :type created_at: str, attribute setting not allowed
 
     :param lock: Locked state of asset, defaults to None.
     :type lock: Optional[PromptTemplateLock], attribute setting not allowed
 
     :param is_template: True if prompt is a template, False otherwise; defaults to None.
-    :type is_template: Optional[bool], attribute setting not allowed 
+    :type is_template: Optional[bool], attribute setting not allowed
 
     :param name: Prompt template name, defaults to None.
-    :type name: Optional[str], optional
+    :type name: str, optional
 
     :param model_id: Foundation model id, defaults to None.
     :type model_id: Optional[ModelTypes], optional
 
     :param model_params: Model parameters, defaults to None.
-    :type model_params: Optional[Dict], optional
+    :type model_params: dict, optional
 
     :param template_version: Semvar version for tracking in IBM AI Factsheets, defaults to None.
-    :type template_version: Optional[str], optional
+    :type template_version: str, optional
 
     :param task_ids: List of task ids, defaults to None.
     :type task_ids: Optional[List[str]], optional
 
     :param description: Prompt template asset description, defaults to None.
-    :type description: Optional[str], optional
+    :type description: str, optional
 
     :param input_text: Input text for prompt, defaults to None.
-    :type input_text: Optional[str], optional
+    :type input_text: str, optional
 
-    :param input_variables: Input variables can be present in fields: `instruction`, 
+    :param input_variables: Input variables can be present in fields: `instruction`,
                             `input_prefix`, `output_prefix`, `input_text`, `examples`
                             and are identified by braces ('{' and '}'), defaults to None.
-    :type input_variables: (List | Dict[str, Dict[str, str]] | None), optional
+    :type input_variables: (list | dict[str, dict[str, str]]), optional
 
     :param instruction: Instruction for model, defaults to None.
-    :type instruction: Optional[str], optional
+    :type instruction: str, optional
 
     :param input_prefix: Prefix string placed before input text, defaults to None.
-    :type input_prefix: Optional[str], optional
+    :type input_prefix: str, optional
 
     :param output_prefix: Prefix before model response, defaults to None.
-    :type output_prefix: Optional[str], optional
+    :type output_prefix: str, optional
 
     :param examples: Examples may help the model to adjust the response; [[input1, output1], ...], defaults to None.
-    :type examples: Optional[List[List[str]]], optional
+    :type examples: list[list[str]]], optional
 
     :param validate_template: If True, the Prompt Template is validated for the presence of input variables, defaults to True.
     :type validate_template: bool, optional
 
     **Examples**
 
     Example of invalid Prompt Template:
@@ -105,103 +114,137 @@
     .. code-block:: python
 
         prompt_template = PromptTemplate(input_text='What are the most famous monuments in {country}?',
                                          input_variables=['country'])
 
     """
 
-    def __init__(self,
-                 name: Optional[str] = None,
-                 model_id: Optional[ModelTypes] = None,
-                 model_params: Optional[Dict] = None,
-                 template_version: Optional[str] = None,
-                 task_ids: Optional[List[str]] = None,
-                 description: Optional[str] = None,
-                 input_text: Optional[str] = None,
-                 input_variables: (List | Dict[str, Dict[str, str]] | None) = None,
-                 instruction: Optional[str] = None,
-                 input_prefix: Optional[str] = None,
-                 output_prefix: Optional[str] = None,
-                 examples: Optional[List[List[str]]] = None,
-                 validate_template: bool = True) -> None:
+    def __init__(
+        self,
+        name: str | None = None,
+        model_id: ModelTypes | None = None,
+        model_params: dict | None = None,
+        template_version: str | None = None,
+        task_ids: list[str] | None = None,
+        description: str | None = None,
+        input_text: str | None = None,
+        input_variables: list | dict[str, dict[str, str]] | None = None,
+        instruction: str | None = None,
+        input_prefix: str | None = None,
+        output_prefix: str | None = None,
+        examples: list[list[str]] | None = None,
+        validate_template: bool = True,
+        **kwargs: Any,
+    ) -> None:
         self.name = name
-        self._prompt_id = None
-        self._created_at = None
-        self._lock = None
-        self._is_template = None
-        self.model_id = model_id
+        self._prompt_id: str | None = None
+        self._created_at: int | None = None
+        self._lock: PromptTemplateLock | None = None
+        self._is_template: bool | None = None
+        self.model_id: ModelTypes | str | None = model_id
         if isinstance(self.model_id, ModelTypes):
             self.model_id = self.model_id.value
-        self.model_params = model_params.copy() if model_params is not None else model_params
+        self.model_params = (
+            model_params.copy() if model_params is not None else model_params
+        )
         self.task_ids = task_ids.copy() if task_ids is not None else task_ids
         self.template_version = template_version
         self.description = description
         self.input_text = input_text
-        self.input_variables = input_variables.copy() if input_variables is not None else input_variables
+        self.input_variables = (
+            input_variables.copy() if input_variables is not None else input_variables
+        )
         self.instruction = instruction
         self.input_prefix = input_prefix
         self.output_prefix = output_prefix
         self.examples = examples.copy() if examples is not None else examples
 
+        supported_pt_kwargs = ["input_mode", "external_information"]
+        unsupported_pt_keys = [
+            key for key in kwargs.keys() if key not in supported_pt_kwargs
+        ]
+        if unsupported_pt_keys:
+            raise WMLClientError(
+                f"Unsupported kwargs: {', '.join(unsupported_pt_keys)}. "
+                f"Supported kwargs are: {', '.join(supported_pt_kwargs)}."
+            )
+
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
         # template validation
         if validate_template:
             self._validation()
-            
-    def __repr__(self):
-        args = [f"{key}={value!r}" for key, value in self.__dict__.items() 
-                if not key.startswith('_') and value is not None]
+
+    def __repr__(self) -> str:
+        args = [
+            f"{key}={value!r}"
+            for key, value in self.__dict__.items()
+            if not key.startswith("_") and value is not None
+        ]
         return f"{type(self).__name__}({ ', '.join(args)})"
 
     @property
-    def prompt_id(self):
+    def prompt_id(self) -> str | None:
         return self._prompt_id
 
     @property
-    def created_at(self):
+    def created_at(self) -> str:
+        self._created_at = cast(int, self._created_at)
         return str(datetime.fromtimestamp(self._created_at / 1000)).split(".")[0]
 
     @property
-    def lock(self):
+    def lock(self) -> PromptTemplateLock | None:
         return self._lock
 
     @property
-    def is_template(self):
+    def is_template(self) -> bool | None:
         return self._is_template
 
-    def _validation(self):
+    def _validation(self) -> None:
         """Validate template structure.
 
         :raises ValidationError: raises when input_variables does not fit placeholders in input body.
         """
-        input_variables = self.input_variables if self.input_variables is not None else []
-        template_text = " ".join(filter(None, [self.instruction,
-                                               self.input_prefix,
-                                               self.output_prefix]))
+        input_variables = (
+            self.input_variables if self.input_variables is not None else []
+        )
+        template_text = " ".join(
+            filter(None, [self.instruction, self.input_prefix, self.output_prefix])
+        )
         if self.examples:
             for example in self.examples:
                 template_text += " ".join(example)
         try:
-            def _validate(input_text):
-                dummy_inputs = {input_variable: "wx" for input_variable in input_variables}
-                TemplateFormatter().format("".join([template_text, input_text]), **dummy_inputs)
+
+            def _validate(input_text: str) -> None:
+                dummy_inputs = {
+                    input_variable: "wx" for input_variable in input_variables
+                }
+                TemplateFormatter().format(
+                    "".join([template_text, input_text]), **dummy_inputs
+                )
 
             if self.input_text:
                 _validate(template_text + self.input_text)
             else:
                 if template_text:
                     _validate(template_text)
         except KeyError as key:
-            raise ValidationError(key, additional_msg="One can turn off validation step setting `validate_template` to False." )
+            raise ValidationError(
+                str(key),
+                additional_msg="One can turn off validation step setting `validate_template` to False.",
+            )
 
 
 class PromptTemplateManager(WMLResource):
     """Instantiate the prompt template manager.
 
     :param credentials: Credentials to watsonx.ai instance.
-    :type credentials: dict
+    :type credentials: Credentials
 
     :param project_id: ID of project
     :type project_id: str
 
     :param space_id: ID of project
     :type space_id: str
 
@@ -215,22 +258,24 @@
     .. note::
         One of these parameters is required: ['project_id ', 'space_id']
 
     **Example**
 
     .. code-block:: python
 
+        from ibm_watsonx_ai import Credentials
+
         from ibm_watsonx_ai.foundation_models.prompts import PromptTemplate, PromptTemplateManager
         from ibm_watsonx_ai.foundation_models.utils.enums import ModelTypes
 
         prompt_mgr = PromptTemplateManager(
-                        credentials={
-                            "apikey": "***",
-                            "url": "https://us-south.ml.cloud.ibm.com"
-                        },
+                        credentials=Credentials(
+                            api_key="***",
+                            url="https://us-south.ml.cloud.ibm.com"
+                        ),
                         project_id="*****"
                         )
 
         prompt_template = PromptTemplate(name="My prompt",
                                          model_id=ModelTypes.GRANITE_13B_CHAT_V2,
                                          input_prefix="Human:",
                                          output_prefix="Assistant:",
@@ -240,273 +285,325 @@
                                                     'A stock market is a place where investors buy and sell shares of publicly traded companies.']])
 
         stored_prompt_template = prompt_mgr.store_prompt(prompt_template)
         print(stored_prompt_template.prompt_id)   # id of prompt template asset
 
     """
 
-    def __init__(self,
-                 credentials: Optional[dict] = None,
-                 *,
-                 project_id: Optional[str] = None,
-                 space_id: Optional[str] = None,
-                 verify=None,
-                 api_client: APIClient = None) -> None:
-
+    def __init__(
+        self,
+        credentials: Credentials | dict | None = None,
+        *,
+        project_id: str | None = None,
+        space_id: str | None = None,
+        verify: str | bool | None = None,
+        api_client: APIClient | None = None,
+    ) -> None:
         self.project_id = project_id
         self.space_id = space_id
         if credentials:
             self._client = APIClient(credentials, verify=verify)
         elif api_client:
+            api_client = cast(APIClient, api_client)
             self._client = api_client
         else:
-            raise InvalidMultipleArguments(params_names_list=["credentials", "api_client"],
-                                           reason="None of the arguments were provided.")
+            raise InvalidMultipleArguments(
+                params_names_list=["credentials", "api_client"],
+                reason="None of the arguments were provided.",
+            )
 
         if self.space_id is not None and self.project_id is not None:
-            raise InvalidMultipleArguments(params_names_list=["project_id", "space_id"],
-                                           reason="Both arguments were provided.")
+            raise InvalidMultipleArguments(
+                params_names_list=["project_id", "space_id"],
+                reason="Both arguments were provided.",
+            )
         self.params = {}
         if self.space_id:
             self._client.set.default_space(space_id)
-            self.params = {'space_id': self.space_id}
+            self.params = {"space_id": self.space_id}
         elif self.project_id:
+            project_id = cast(str, project_id)
             self._client.set.default_project(project_id)
-            self.params = {'project_id': self.project_id}
+            self.params = {"project_id": self.project_id}
         elif api_client:
-            if (project_id := self._client.default_project_id):
-                self.params = {'project_id': project_id}
-            elif (space_id := self._client.default_space_id):
-                self.params = {'space_id': space_id}
+            if project_id := self._client.default_project_id:
+                self.params = {"project_id": project_id}
+            elif space_id := self._client.default_space_id:
+                self.params = {"space_id": space_id}
             else:
                 pass
         elif not api_client:
-            raise InvalidMultipleArguments(params_names_list=["space_id", "project_id"],
-                                           reason="None of the arguments were provided.")
-        
+            raise InvalidMultipleArguments(
+                params_names_list=["space_id", "project_id"],
+                reason="None of the arguments were provided.",
+            )
+
         if not self._client.CLOUD_PLATFORM_SPACES and self._client.CPD_version < 4.8:
             raise WMLClientError(error_msg="Operation is unsupported for this release.")
 
         WMLResource.__init__(self, __name__, self._client)
 
-    def _create_request_body(self, prompt_template: PromptTemplate) -> Dict:
+    def _create_request_body(self, prompt_template: PromptTemplate) -> dict:
         """Method is used to create request body from PromptTemplate object.
 
         :param prompt_template: Object of type PromptTemplate based on which the request
                                 body will be created.
         :type prompt_template: PromptTemplate
 
         :return: Request body
-        :rtype: Dict
+        :rtype: dict
         """
-        json_data: Dict = {'prompt': dict()}
+        json_data: dict = {"prompt": dict()}
         if prompt_template.description is not None:
-            json_data.update({'description': prompt_template.description})
+            json_data.update({"description": prompt_template.description})
         if prompt_template.input_variables is not None:
-            PromptTemplateManager._validate_type(prompt_template.input_variables, u'input_variables', [dict, list],
-                                                 False)
+            PromptTemplateManager._validate_type(
+                prompt_template.input_variables, "input_variables", [dict, list], False
+            )
             if isinstance(prompt_template.input_variables, list):
-                json_data.update({'prompt_variables': {key: {} for key in prompt_template.input_variables}})
+                json_data.update(
+                    {
+                        "prompt_variables": {
+                            key: {} for key in prompt_template.input_variables
+                        }
+                    }
+                )
             else:
-                json_data.update({'prompt_variables': prompt_template.input_variables})
+                json_data.update({"prompt_variables": prompt_template.input_variables})
         if prompt_template.task_ids is not None:
-            PromptTemplateManager._validate_type(prompt_template.task_ids, u'task_ids', list, False)
-            json_data.update({'task_ids': prompt_template.task_ids})
+            PromptTemplateManager._validate_type(
+                prompt_template.task_ids, "task_ids", list, False
+            )
+            json_data.update({"task_ids": prompt_template.task_ids})
         if prompt_template.template_version is not None:
-            json_data.update({"model_version": {"number": prompt_template.template_version}})
+            json_data.update(
+                {"model_version": {"number": prompt_template.template_version}}
+            )
+        if hasattr(prompt_template, "input_mode"):
+            json_data.update({"input_mode": prompt_template.input_mode})
 
         if prompt_template.input_text:
-            PromptTemplateManager._validate_type(prompt_template.input_text, u'input_text', str, False)
-            json_data['prompt'].update({'input': [[prompt_template.input_text, '']]})
-
-        PromptTemplateManager._validate_type(prompt_template.model_id, u'model_id', str, True)
+            PromptTemplateManager._validate_type(
+                prompt_template.input_text, "input_text", str, False
+            )
+            json_data["prompt"].update({"input": [[prompt_template.input_text, ""]]})
+
+        PromptTemplateManager._validate_type(
+            prompt_template.model_id, "model_id", str, True
+        )
         if prompt_template.model_id is not None:
-            json_data['prompt'].update({'model_id': prompt_template.model_id})
+            json_data["prompt"].update({"model_id": prompt_template.model_id})
 
         if prompt_template.model_params is not None:
-            PromptTemplateManager._validate_type(prompt_template.model_params, u'model_parameters', dict, False)
-            json_data['prompt'].update({'model_parameters': prompt_template.model_params})
+            PromptTemplateManager._validate_type(
+                prompt_template.model_params, "model_parameters", dict, False
+            )
+            json_data["prompt"].update(
+                {"model_parameters": prompt_template.model_params}
+            )
+
+        if hasattr(prompt_template, "external_information"):
+            json_data["prompt"].update(
+                {"external_information": prompt_template.external_information}
+            )
 
-        data: Dict = dict()
+        data: dict = dict()
         if prompt_template.instruction is not None:
-            data.update({'instruction': prompt_template.instruction})
+            data.update({"instruction": prompt_template.instruction})
 
         if prompt_template.input_prefix is not None:
-            data.update({'input_prefix': prompt_template.input_prefix})
+            data.update({"input_prefix": prompt_template.input_prefix})
 
         if prompt_template.output_prefix is not None:
-            data.update({'output_prefix': prompt_template.output_prefix})
+            data.update({"output_prefix": prompt_template.output_prefix})
         if prompt_template.examples is not None:
-            PromptTemplateManager._validate_type(prompt_template.examples, u'examples', list, False)
-            data.update({'examples': prompt_template.examples})
+            PromptTemplateManager._validate_type(
+                prompt_template.examples, "examples", list, False
+            )
+            data.update({"examples": prompt_template.examples})
 
-        json_data['prompt'].update({'data': data})
+        json_data["prompt"].update({"data": data})
 
         return json_data
 
-    def _from_json_to_prompt(self, response: Dict) -> PromptTemplate:
+    def _from_json_to_prompt(self, response: dict) -> PromptTemplate:
         """Convert json response to PromptTemplate object.
 
         :param response: Response body after request operation.
-        :type response: Dict
+        :type response: dict
 
         :return: PromptTemplate object with given details.
         :rtype: PromptTemplate
         """
-        prompt_field: Dict = response.get('prompt', dict())
-        data_field: Dict = prompt_field.get('data', dict())
-        prompt_template = PromptTemplate(name=response.get('name'),
-                                         description=response.get('description'),
-                                         model_id=prompt_field.get('model_id'),
-                                         model_params=prompt_field.get('model_parameters'),
-                                         task_ids=response.get("task_ids"),
-                                         template_version=response.get("model_version", dict()).get("number"),
-                                         input_variables=response.get('prompt_variables'),
-                                         input_text=prompt_field.get('input', [[None, None]])[0][0],
-                                         instruction=data_field.get('instruction'),
-                                         input_prefix=data_field.get('input_prefix'),
-                                         output_prefix=data_field.get('output_prefix'),
-                                         examples=data_field.get('examples'),
-                                         validate_template=False
-                                         )
-
-        prompt_template._prompt_id = response.get('id')
-        prompt_template._created_at = response.get('created_at')
-        if "lock_type" in response.get('lock', dict()):
-            del response['lock']["lock_type"]
-        prompt_template._lock = PromptTemplateLock(**response.get('lock', {"locked": None,
-                                                                           "locked_by": None}))
-        prompt_template._is_template = response.get('is_template')
+        prompt_field: dict = response.get("prompt", dict())
+        data_field: dict = prompt_field.get("data", dict())
+        prompt_template = PromptTemplate(
+            name=response.get("name"),
+            description=response.get("description"),
+            model_id=prompt_field.get("model_id"),
+            model_params=prompt_field.get("model_parameters"),
+            task_ids=response.get("task_ids"),
+            template_version=response.get("model_version", dict()).get("number"),
+            input_variables=response.get("prompt_variables"),
+            input_text=prompt_field.get("input", [[None, None]])[0][0],
+            instruction=data_field.get("instruction"),
+            input_prefix=data_field.get("input_prefix"),
+            output_prefix=data_field.get("output_prefix"),
+            examples=data_field.get("examples"),
+            validate_template=False,
+        )
+
+        prompt_template._prompt_id = response.get("id")
+        prompt_template._created_at = response.get("created_at")
+        if "lock_type" in response.get("lock", dict()):
+            del response["lock"]["lock_type"]
+        prompt_template._lock = PromptTemplateLock(
+            **response.get("lock", {"locked": None, "locked_by": None})
+        )
+        prompt_template._is_template = response.get("is_template")
 
         return prompt_template
 
-    def _get_details(self, limit: Optional[int] = None) -> List:
+    def _get_details(self, limit: int | None = None) -> list:
         """Method retrives details of all prompt templates. If limit is set to None
         then all prompt templates are fetched.
 
         :param limit: limit number of fetched records, defaults to None.
-        :type limit: Optional[int]
+        :type limit: int | None
 
-        :return: List of prompts metadata 
+        :return: List of prompts metadata
         :rtype: List
         """
         headers = self._client._get_headers()
         url = self._client.service_instance._href_definitions.get_prompts_all_href()
-        json_data = {"query": u"asset.asset_type:wx_prompt",
-                     u"sort": "-asset.created_at<string>"}
+        json_data: dict[str, int | str] = {
+            "query": "asset.asset_type:wx_prompt",
+            "sort": "-asset.created_at<string>",
+        }
         if limit is not None:
             if limit < 1:
-                raise WMLClientError('Limit cannot be lower than 1.')
+                raise WMLClientError("Limit cannot be lower than 1.")
             elif limit > 200:
-                raise WMLClientError('Limit cannot be larger than 200.')
+                raise WMLClientError("Limit cannot be larger than 200.")
 
-            json_data.update({'limit': limit})
+            json_data.update({"limit": limit})
         else:
-            json_data.update({'limit': 200})
+            json_data.update({"limit": 200})
         prompts_list = []
         bookmark = True
         while bookmark is not None:
-            response = requests.post(url=url, json=json_data,
-                                     headers=headers,
-                                     params=self.params)
+            response = requests.post(
+                url=url, json=json_data, headers=headers, params=self.params
+            )
             details_json = self._handle_response(200, "Get next details", response)
-            bookmark = details_json.get('next', {'href': None}).get('bookmark', None)
-            prompts_list.extend(details_json.get('results', []))
+            bookmark = details_json.get("next", {"href": None}).get("bookmark", None)
+            prompts_list.extend(details_json.get("results", []))
             if limit is not None:
                 break
-            json_data.update({'bookmark': bookmark})
+            json_data.update({"bookmark": bookmark})
         return prompts_list
 
-    def _change_lock(self, prompt_id: str, locked: bool, force: bool = False) -> Dict:
+    def _change_lock(self, prompt_id: str, locked: bool, force: bool = False) -> dict:
         """Change prompt template lock state.
 
         :param prompt_id: Id of prompt template.
         :type prompt_id: str
 
         :param locked: New lock state.
         :type locked: bool
 
         :param force: force lock state overwrite, defaults to False.
         :type force: bool, optional
 
         :return: Response content after lock state change.
-        :rtype: Dict
+        :rtype: dict
         """
         headers = self._client._get_headers()
-        params = (self.params | {"prompt_id": prompt_id, "force": force})
+        params = self.params | {"prompt_id": prompt_id, "force": force}
         json_data = {"locked": locked}
 
-        url = self._client.service_instance._href_definitions.get_prompts_href() + f"/{prompt_id}/lock"
-        response = requests.put(url=url,
-                                json=json_data,
-                                headers=headers,
-                                params=params)
-
-        return self._handle_response(200, u'change_lock', response)
-
-    def load_prompt(self,
-                    prompt_id: str,
-                    astype: PromptTemplateFormats = PromptTemplateFormats.PROMPTTEMPLATE,
-                    *,
-                    prompt_variables: Optional[Dict[str, str]] = None):
+        url = (
+            self._client.service_instance._href_definitions.get_prompts_href()
+            + f"/{prompt_id}/lock"
+        )
+        response = requests.put(url=url, json=json_data, headers=headers, params=params)
+
+        return self._handle_response(200, "change_lock", response)
+
+    def load_prompt(
+        self,
+        prompt_id: str,
+        astype: PromptTemplateFormats | str = PromptTemplateFormats.PROMPTTEMPLATE,
+        *,
+        prompt_variables: dict[str, str] | None = None,
+    ) -> LcPromptTemplate | PromptTemplate | str:
         """Retrive a prompt template asset.
 
         :param prompt_id: Id of prompt template which is processed.
         :type prompt_id: str
 
         :param astype: Type of return object.
         :type astype: PromptTemplateFormats
 
-        :param prompt_variables: Dictionary of input variables and values with which input variables will be replaced.
-        :type prompt_variables: Dict[str, str]
+        :param prompt_variables: dictionary of input variables and values with which input variables will be replaced.
+        :type prompt_variables: dict[str, str]
 
         :return: Prompt template asset.
         :rtype: PromptTemplate | str | langchain.prompts.PromptTemplate
 
         **Example**
 
         .. code-block:: python
 
             loaded_prompt_template = prompt_mgr.load_prompt(prompt_id)
             loaded_prompt_template_lc = prompt_mgr.load_prompt(prompt_id, PromptTemplateFormats.LANGCHAIN)
             loaded_prompt_template_string = prompt_mgr.load_prompt(prompt_id, PromptTemplateFormats.STRING)
         """
         headers = self._client._get_headers()
-        params = (self.params | {"prompt_id": prompt_id})
-        url = self._client.service_instance._href_definitions.get_prompts_href() + f"/{prompt_id}"
+        params = self.params | {"prompt_id": prompt_id}
+        url = (
+            self._client.service_instance._href_definitions.get_prompts_href()
+            + f"/{prompt_id}"
+        )
 
         if isinstance(astype, PromptTemplateFormats):
             astype = astype.value
 
-        if astype == 'prompt':
-            response = requests.get(url=url,
-                                    headers=headers,
-                                    params=params)
-            return self._from_json_to_prompt(self._handle_response(200, u'_load_json_prompt', response))
-        elif astype in ('langchain', 'string'):
-            response = requests.post(url=url + u"/input",
-                                     headers=headers,
-                                     params=params)
-            response_input = self._handle_response(200, u'load_prompt', response).get("input")
-            if astype == 'string':
+        if astype == "prompt":
+            response = requests.get(url=url, headers=headers, params=params)
+            return self._from_json_to_prompt(
+                self._handle_response(200, "_load_json_prompt", response)
+            )
+        elif astype in ("langchain", "string"):
+            response = requests.post(url=url + "/input", headers=headers, params=params)
+            response_input = self._handle_response(200, "load_prompt", response).get(
+                "input"
+            )
+            response_input = cast(str, response_input)
+            if astype == "string":
                 try:
-                    return response_input if prompt_variables is None else response_input.format(**prompt_variables)
+                    return (
+                        response_input
+                        if prompt_variables is None
+                        else response_input.format(**prompt_variables)
+                    )
                 except KeyError as key:
-                    raise PromptVariablesError(key)
+                    raise PromptVariablesError(str(key))
             else:
                 from langchain.prompts import PromptTemplate as LcPromptTemplate
+
                 return LcPromptTemplate.from_template(response_input)
         else:
-            raise InvalidValue(u'astype')
+            raise InvalidValue("astype")
 
-    def list(self, *, limit=None) -> pandas.core.frame.DataFrame:
+    def list(self, *, limit: int | None = None) -> pandas.core.frame.DataFrame:
         """List all available prompt templates in the DataFrame format.
 
         :param limit: limit number of fetched records, defaults to None.
-        :type limit: Optional[int]
+        :type limit: int, optional
 
         :return: Dataframe of fundamental properties of availabale prompts.
         :rtype: pandas.core.frame.DataFram
 
         **Example**
 
         .. code-block:: python
@@ -518,46 +615,69 @@
 
             .. code-block:: python
 
                 df_prompts = prompt_mgr.list()
                 df_prompts.sort_values("LAST MODIFIED", ascending=False)
 
         """
-        details = ['metadata.asset_id', 'metadata.name', 'metadata.created_at', 'metadata.usage.last_updated_at']
+        details = [
+            "metadata.asset_id",
+            "metadata.name",
+            "metadata.created_at",
+            "metadata.usage.last_updated_at",
+        ]
         prompts_details = self._get_details(limit=limit)
 
         data_normalize = pandas.json_normalize(prompts_details)
         prompts_data = data_normalize.reindex(columns=details)
 
         df_details = pandas.DataFrame(prompts_data, columns=details)
 
-        df_details.rename(columns={'metadata.asset_id': 'ID',
-                                   'metadata.name': 'NAME',
-                                   'metadata.created_at': 'CREATED',
-                                   'metadata.usage.last_updated_at': 'LAST MODIFIED',
-                                   }, inplace=True)
+        df_details.rename(
+            columns={
+                "metadata.asset_id": "ID",
+                "metadata.name": "NAME",
+                "metadata.created_at": "CREATED",
+                "metadata.usage.last_updated_at": "LAST MODIFIED",
+            },
+            inplace=True,
+        )
 
         return df_details
 
-    def store_prompt(self, prompt_template: Union[PromptTemplate, langchain.prompts.PromptTemplate]) -> PromptTemplate:
+    def store_prompt(
+        self, prompt_template: PromptTemplate | langchain.prompts.PromptTemplate
+    ) -> PromptTemplate:
         """Store a new prompt template.
 
         :param prompt_template: PromptTemplate to be stored.
         :type prompt_template: (PromptTemplate | langchain.prompts.PromptTemplate)
 
         :return: PromptTemplate object initialized with values provided in the server response object.
         :rtype: PromptTemplate
         """
         if isinstance(prompt_template, PromptTemplate):
             pass
         else:
             from langchain.prompts import PromptTemplate as LcPromptTemplate
+
             if isinstance(prompt_template, LcPromptTemplate):
-                def get_metadata_value(prompt_temp, key, default=None, must_be_list=False, must_be_nested_list=False):
-                    if hasattr(prompt_temp, "metadata") and prompt_temp.metadata and key in prompt_temp.metadata:
+
+                def get_metadata_value(
+                    prompt_temp: LcPromptTemplate,
+                    key: str,
+                    default: ModelTypes | list | bool | str | None = None,
+                    must_be_list: bool = False,
+                    must_be_nested_list: bool = False,
+                ) -> Any:
+                    if (
+                        hasattr(prompt_temp, "metadata")
+                        and prompt_temp.metadata
+                        and key in prompt_temp.metadata
+                    ):
                         if must_be_list:
                             if isinstance(prompt_temp.metadata[key], str):
                                 return [prompt_temp.metadata[key]]
                             return prompt_temp.metadata[key]
                         elif must_be_nested_list:
                             if isinstance(prompt_temp.metadata[key], str):
                                 return [[prompt_temp.metadata[key]]]
@@ -568,189 +688,222 @@
                         else:
                             return prompt_temp.metadata[key]
                     else:
                         return default
 
                 prompt_template = PromptTemplate(
                     name=get_metadata_value(prompt_template, "name", "My prompt"),
-                    model_id=get_metadata_value(prompt_template, "model_id", ModelTypes.FLAN_UL2),
-                    model_params=get_metadata_value(prompt_template, "model_params", None),
-                    template_version=get_metadata_value(prompt_template, "template_version", None),
-                    task_ids=get_metadata_value(prompt_template, "task_ids", None, must_be_list=True),
-                    description=get_metadata_value(prompt_template, "description", None),
-                    input_text=get_metadata_value(prompt_template, "input_text", prompt_template.template),
-                    input_variables=get_metadata_value(prompt_template, "input_variables", prompt_template.input_variables),
-                    instruction=get_metadata_value(prompt_template, "instruction", None),
-                    input_prefix=get_metadata_value(prompt_template, "input_prefix", None),
-                    output_prefix=get_metadata_value(prompt_template, "output_prefix", None),
-                    examples=get_metadata_value(prompt_template, "examples", None, must_be_nested_list=True),
-                    validate_template=get_metadata_value(prompt_template, "validate_template", True)
+                    model_id=get_metadata_value(
+                        prompt_template, "model_id", ModelTypes.FLAN_UL2
+                    ),
+                    model_params=get_metadata_value(
+                        prompt_template, "model_params", None
+                    ),
+                    template_version=get_metadata_value(
+                        prompt_template, "template_version", None
+                    ),
+                    task_ids=get_metadata_value(
+                        prompt_template, "task_ids", None, must_be_list=True
+                    ),
+                    description=get_metadata_value(
+                        prompt_template, "description", None
+                    ),
+                    input_text=get_metadata_value(
+                        prompt_template, "input_text", prompt_template.template
+                    ),
+                    input_variables=get_metadata_value(
+                        prompt_template,
+                        "input_variables",
+                        prompt_template.input_variables,
+                    ),
+                    instruction=get_metadata_value(
+                        prompt_template, "instruction", None
+                    ),
+                    input_prefix=get_metadata_value(
+                        prompt_template, "input_prefix", None
+                    ),
+                    output_prefix=get_metadata_value(
+                        prompt_template, "output_prefix", None
+                    ),
+                    examples=get_metadata_value(
+                        prompt_template, "examples", None, must_be_nested_list=True
+                    ),
+                    validate_template=get_metadata_value(
+                        prompt_template, "validate_template", True
+                    ),
                 )
             else:
                 raise WMLClientError(error_msg="Unsupported type for `prompt_template`")
-            
+
         headers = self._client._get_headers()
 
-        PromptTemplateManager._validate_type(prompt_template.name,
-                                             u'prompt_template.name',
-                                             str, True)
-        json_data: Dict = {
+        PromptTemplateManager._validate_type(
+            prompt_template.name, "prompt_template.name", str, True
+        )
+        json_data: dict = {
             "name": prompt_template.name,
             "lock": {"locked": True},
-            "prompt": dict()
+            "prompt": dict(),
         }
 
         json_data.update(self._create_request_body(prompt_template))
 
         url = self._client.service_instance._href_definitions.get_prompts_href()
-        response = requests.post(url=url,
-                                 json=json_data,
-                                 headers=headers,
-                                 params=self.params)
-        response = self._handle_response(201, u'store_prompt', response)
+        response = requests.post(
+            url=url, json=json_data, headers=headers, params=self.params
+        )
+        response = self._handle_response(201, "store_prompt", response)
 
         return self._from_json_to_prompt(response)
 
     def delete_prompt(self, prompt_id: str, *, force: bool = False) -> str:
         """Remove prompt template from project or space.
 
-        :param prompt_id: Id of prompt template that will be delete. 
+        :param prompt_id: Id of prompt template that will be delete.
         :type prompt_id: str
 
         :param force: If True then prompt template is unlocked and then delete, defaults to False.
         :type force: bool
 
         :return: Status 'SUCESS' if the prompt template is successfully deleted.
         :rtype: str
-        
+
         **Example**
 
         .. code-block:: python
 
             prompt_mgr.delete_prompt(prompt_id)  # delete if asset is unclocked
         """
         if force:
             self.unlock(prompt_id)
 
         headers = self._client._get_headers()
-        params = (self.params | {"prompt_id": prompt_id})
+        params = self.params | {"prompt_id": prompt_id}
 
-        url = self._client.service_instance._href_definitions.get_prompts_href() + f"/{prompt_id}"
-        response = requests.delete(url=url, headers=headers,
-                                   params=params)
+        url = (
+            self._client.service_instance._href_definitions.get_prompts_href()
+            + f"/{prompt_id}"
+        )
+        response = requests.delete(url=url, headers=headers, params=params)
 
-        return self._handle_response(204, u'delete_prompt', response)
+        return self._handle_response(204, "delete_prompt", response)  # type: ignore[return-value]
 
-    def update_prompt(self, prompt_id: str, prompt_template: PromptTemplate) -> Dict:
+    def update_prompt(self, prompt_id: str, prompt_template: PromptTemplate) -> dict:
         """Update prompt template data.
 
         :param prompt_id: Id of the updated prompt template.
         :type prompt_id: str
 
         :param prompt: PromptTemplate with new data.
-        :type prompt: PromptTemplate 
+        :type prompt: PromptTemplate
 
         :return: metadata of updated deployment
         :rtype: dict
 
         **Example**
 
         .. code-block:: python
 
             updataed_prompt_template = PromptTemplate(name="New name")
-            prompt_mgr.update_prompt(prompt_id, prompt_template)  # {'name': 'New name'} in metadata  
-            
+            prompt_mgr.update_prompt(prompt_id, prompt_template)  # {'name': 'New name'} in metadata
+
         """
         headers = self._client._get_headers()
-        params = (self.params | {"prompt_id": prompt_id})
+        params = self.params | {"prompt_id": prompt_id}
 
-        new_body: Dict = dict()
+        new_body: dict = dict()
         current_prompt_template = self.load_prompt(prompt_id)
 
+        current_prompt_template = cast(PromptTemplate, current_prompt_template)
         for attribute in prompt_template.__dict__:
-            if getattr(prompt_template, attribute) is not None and not attribute.startswith("_"):
-                setattr(current_prompt_template, attribute, getattr(prompt_template, attribute))
+            if getattr(
+                prompt_template, attribute
+            ) is not None and not attribute.startswith("_"):
+                setattr(
+                    current_prompt_template,
+                    attribute,
+                    getattr(prompt_template, attribute),
+                )
 
         if current_prompt_template.name is not None:
-            new_body.update({'name': current_prompt_template.name})
+            new_body.update({"name": current_prompt_template.name})
 
         new_body.update(self._create_request_body(current_prompt_template))
 
-        url = self._client.service_instance._href_definitions.get_prompts_href() + f"/{prompt_id}"
-
-        response = requests.patch(url=url,
-                                  json=new_body,
-                                  headers=headers,
-                                  params=params)
-        return self._handle_response(200, u'update_prompt', response)
+        url = (
+            self._client.service_instance._href_definitions.get_prompts_href()
+            + f"/{prompt_id}"
+        )
+
+        response = requests.patch(
+            url=url, json=new_body, headers=headers, params=params
+        )
+        return self._handle_response(200, "update_prompt", response)
 
-    def get_lock(self, prompt_id: str) -> Dict:
+    def get_lock(self, prompt_id: str) -> dict:
         """Get the current locked state of a prompt template.
 
         :param prompt_id: Id of prompt template
         :type prompt_id: str
 
         :return: Information about locked state of prompt template asset.
-        :rtype: Dict
+        :rtype: dict
 
         **Example**
 
         .. code-block:: python
 
             print(prompt_mgr.get_lock(prompt_id))
         """
         headers = self._client._get_headers()
-        params = (self.params | {"prompt_id": prompt_id})
-        url = self._client.service_instance._href_definitions.get_prompts_href() + f"/{prompt_id}/lock"
+        params = self.params | {"prompt_id": prompt_id}
+        url = (
+            self._client.service_instance._href_definitions.get_prompts_href()
+            + f"/{prompt_id}/lock"
+        )
 
-        response = requests.get(url=url,
-                                headers=headers,
-                                params=params)
+        response = requests.get(url=url, headers=headers, params=params)
 
-        return self._handle_response(200, u'get_lock', response)
+        return self._handle_response(200, "get_lock", response)
 
-    def lock(self, prompt_id: str, force: bool = False) -> Dict:
-        """Lock the prompt template if it is unlocked and user has permission to do that. 
+    def lock(self, prompt_id: str, force: bool = False) -> dict:
+        """Lock the prompt template if it is unlocked and user has permission to do that.
 
         :param promp_id: Id of prompt template.
         :type promp_id: str
 
         :param force: If True, method forcefully overwrite a lock.
         :type force: bool
 
         :return: Status 'SUCCESS' or response content after an attempt to lock prompt template.
-        :rtype: (str | Dict)
+        :rtype: dict
 
         **Example**
 
         .. code-block:: python
 
             prompt_mgr.lock(prompt_id)
 
         """
-        return self._change_lock(prompt_id=prompt_id,
-                                 locked=True,
-                                 force=force)
+        return self._change_lock(prompt_id=prompt_id, locked=True, force=force)
 
-    def unlock(self, prompt_id: str) -> Dict:
+    def unlock(self, prompt_id: str) -> dict:
         """Unlock the prompt template if it is locked and user has permission to do that.
 
         :param promp_id: Id of prompt template.
         :type promp_id: str
 
         :return: Response content after an attempt to unlock prompt template.
-        :rtype: Dict
+        :rtype: dict
 
         **Example**
 
         .. code-block:: python
 
             prompt_mgr.unlock(prompt_id)
         """
         # server returns status code 400 after trying to unlock unlocked prompt
         lock_state = self.get_lock(prompt_id)
-        if lock_state['locked']:
-            return self._change_lock(prompt_id=prompt_id,
-                                     locked=False,
-                                     force=False)
+        if lock_state["locked"]:
+            return self._change_lock(prompt_id=prompt_id, locked=False, force=False)
         else:
             return lock_state
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from ibm_watsonx_ai.foundation_models.utils.utils import PromptTuningParams
-from ibm_watsonx_ai.foundation_models.utils.utils import HAPDetectionWarning
-from ibm_watsonx_ai.foundation_models.utils.utils import (get_model_specs, get_model_lifecycle, get_supported_tasks,
-                                                          get_model_specs_with_prompt_tuning_support,
-                                                          get_custom_model_specs, get_embedding_model_specs)
+from .model import Model
+from .prompt_tuner import PromptTuner
+from ibm_watsonx_ai.foundation_models.utils.utils import (
+    get_model_specs,
+    get_model_lifecycle,
+    get_supported_tasks,
+    get_model_specs_with_prompt_tuning_support,
+    get_custom_model_specs,
+    get_embedding_model_specs,
+)
+from ibm_watsonx_ai.foundation_models.inference.model_inference import ModelInference
+from ibm_watsonx_ai.foundation_models.embeddings import Embeddings
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/enums.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/foundation_models/utils/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,50 +8,54 @@
 __all__ = [
     "ModelTypes",
     "DecodingMethods",
     "PromptTuningTypes",
     "PromptTuningInitMethods",
     "TuneExperimentTasks",
     "PromptTemplateFormats",
+    "EmbeddingTypes"
 ]
 
 
 class ModelTypes(Enum):
     """Supported foundation models."""
+
     FLAN_T5_XXL = "google/flan-t5-xxl"
     FLAN_UL2 = "google/flan-ul2"
     MT0_XXL = "bigscience/mt0-xxl"
-    GPT_NEOX = 'eleutherai/gpt-neox-20b'
-    MPT_7B_INSTRUCT2 = 'ibm/mpt-7b-instruct2'
-    STARCODER = 'bigcode/starcoder'
-    LLAMA_2_70B_CHAT = 'meta-llama/llama-2-70b-chat'
-    LLAMA_2_13B_CHAT = 'meta-llama/llama-2-13b-chat'
-    GRANITE_13B_INSTRUCT = 'ibm/granite-13b-instruct-v1'
-    GRANITE_13B_CHAT = 'ibm/granite-13b-chat-v1'
-    FLAN_T5_XL = 'google/flan-t5-xl'
-    GRANITE_13B_CHAT_V2 = 'ibm/granite-13b-chat-v2'
-    GRANITE_13B_INSTRUCT_V2 = 'ibm/granite-13b-instruct-v2'
-    ELYZA_JAPANESE_LLAMA_2_7B_INSTRUCT = 'elyza/elyza-japanese-llama-2-7b-instruct'
-    MIXTRAL_8X7B_INSTRUCT_V01_Q = 'ibm-mistralai/mixtral-8x7b-instruct-v01-q'
+    GPT_NEOX = "eleutherai/gpt-neox-20b"
+    MPT_7B_INSTRUCT2 = "ibm/mpt-7b-instruct2"
+    STARCODER = "bigcode/starcoder"
+    LLAMA_2_70B_CHAT = "meta-llama/llama-2-70b-chat"
+    LLAMA_2_13B_CHAT = "meta-llama/llama-2-13b-chat"
+    GRANITE_13B_INSTRUCT = "ibm/granite-13b-instruct-v1"
+    GRANITE_13B_CHAT = "ibm/granite-13b-chat-v1"
+    FLAN_T5_XL = "google/flan-t5-xl"
+    GRANITE_13B_CHAT_V2 = "ibm/granite-13b-chat-v2"
+    GRANITE_13B_INSTRUCT_V2 = "ibm/granite-13b-instruct-v2"
+    ELYZA_JAPANESE_LLAMA_2_7B_INSTRUCT = "elyza/elyza-japanese-llama-2-7b-instruct"
+    MIXTRAL_8X7B_INSTRUCT_V01_Q = "ibm-mistralai/mixtral-8x7b-instruct-v01-q"
     CODELLAMA_34B_INSTRUCT_HF = "codellama/codellama-34b-instruct-hf"
     GRANITE_20B_MULTILINGUAL = "ibm/granite-20b-multilingual"
-    
+
 
 class DecodingMethods(Enum):
     """Supported decoding methods for text generation."""
+
     SAMPLE = "sample"
     GREEDY = "greedy"
 
 
 class PromptTuningTypes:
     PT = "prompt_tuning"
 
 
 class PromptTuningInitMethods:
     """Supported methods for prompt initialization in prompt tuning."""
+
     RANDOM = "random"
     TEXT = "text"
     # PRESET ?
 
 
 class TuneExperimentTasks(Enum):
     QUESTION_ANSWERING = "question_answering"
@@ -61,16 +65,18 @@
     GENERATION = "generation"
     CODE_GENERATION_AND_CONVERSION = "code"
     EXTRACTION = "extraction"
 
 
 class PromptTemplateFormats(Enum):
     """Supported formats of loaded prompt template."""
+
     PROMPTTEMPLATE = "prompt"
     STRING = "string"
     LANGCHAIN = "langchain"
 
+
 class EmbeddingTypes(Enum):
     """Supported Embedding Models."""
+
     IBM_SLATE_30M_ENG = "ibm/slate-30m-english-rtrvr"
     IBM_SLATE_125M_ENG = "ibm/slate-125m-english-rtrvr"
-
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/foundation_models/utils/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/xgb_fl_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,437 +1,458 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
-import warnings
-from string import Formatter
-from typing import Any, Sequence, List, Dict, Union, Optional, Generator
-from dataclasses import dataclass, KW_ONLY, asdict
-from json import loads as json_loads
-
-from ibm_watsonx_ai._wrappers import requests
-from ibm_watsonx_ai.helpers import DataConnection
-from ibm_watsonx_ai.messages.messages import Messages
-from ibm_watsonx_ai.wml_client_error import WMLClientError, InvalidMultipleArguments, InvalidValue
-from ibm_watsonx_ai.utils import NextResourceGenerator
-from ibm_watsonx_ai.utils.autoai.utils import load_file_from_file_system_nonautoai
-from ibm_watsonx_ai.foundation_models.utils.enums import ModelTypes
-from ibm_watsonx_ai.utils.autoai.enums import DataConnectionTypes
-from ibm_watsonx_ai.lifecycle import SpecStates
-from ibm_watsonx_ai import APIClient
-
-
-@dataclass
-class PromptTuningParams:
-    base_model: dict
-    _: KW_ONLY
-    accumulate_steps: int = None
-    batch_size: int = None
-    init_method: str = None
-    init_text: str = None
-    learning_rate: float = None
-    max_input_tokens: int = None
-    max_output_tokens: int = None
-    num_epochs: int = None
-    task_id: str = None
-    tuning_type: str = None
-    verbalizer: str = None
-
-    def to_dict(self):
-        return {key: value for key, value in asdict(self).items() if value is not None}
-
-
-def _get_foundation_models_spec(url, operation_name, additional_params: dict = None):
-    params = {"version": "2023-09-30"}
-    if additional_params:
-        params.update(additional_params)
-    response = requests.get(url,
-                            params=params,
-                            headers={'X-WML-User-Client': 'PythonClient'})
-    if response.status_code == 200:
-        return response.json()
-    elif response.status_code == 404:
-        raise WMLClientError(Messages.get_message(message_id="fm_prompt_tuning_no_foundation_models"), logg_messages=False)
-    else:
-        msg = f"{operation_name} failed. Reason: {response.text}"
-        raise WMLClientError(msg)
 
+from __future__ import print_function
+import time
+import pickle
+import logging
+
+from sklearn.utils.validation import check_is_fitted
+from sklearn.ensemble._hist_gradient_boosting.loss import *
+from sklearn.ensemble._hist_gradient_boosting.common import *
+from sklearn.preprocessing import OrdinalEncoder, LabelEncoder
+from sklearn.utils.multiclass import check_classification_targets
+from sklearn.metrics import check_scoring, accuracy_score, r2_score
+from sklearn.utils import check_X_y, check_random_state, check_array
+from sklearn.ensemble._hist_gradient_boosting.grower import TreePredictor
+
+from ibmfl.util import fl_metrics
+from ibmfl.util import config
+from ibmfl.model.fl_model import FLModel
+from ibmfl.util.xgboost.utils import is_classifier
+from ibmfl.util.xgboost.export import export_sklearn
+from ibmfl.exceptions import ModelInitializationException, ModelException
+from ibmfl.util.xgboost.hyperparams import init_parameters, \
+    validate_parameters
 
-def get_model_specs(url: str, model_id: Optional[str] = None) -> dict:
-    """
-    Operations to retrieve the list of deployed foundation models specifications.
-
-    :param url: environment url
-    :type url: str
-
-    :param model_id: Id of the model, defaults to None (all models specs are returned).
-    :type model_id: Optional[str, ModelTypes], optional
-
-    :return: list of deployed foundation model specs
-    :rtype: dict
-
-    **Example**
+logger = logging.getLogger(__name__)
 
-    .. code-block:: python
 
-        from ibm_watsonx_ai.foundation_models import get_model_specs
-
-        # GET ALL MODEL SPECS
-        get_model_specs(
-            url="https://us-south.ml.cloud.ibm.com"
-            )
-
-        # GET MODEL SPECS BY MODEL_ID
-        get_model_specs(
-            url="https://us-south.ml.cloud.ibm.com",
-            model_id="google/flan-ul2"
-            )
+class XGBFLModel(FLModel, ABC):
     """
-    try:
-        if model_id:
-            if isinstance(model_id, ModelTypes):
-                model_id = model_id.value
-            try:
-                return [res for res in _get_foundation_models_spec(f"{url}/ml/v1/foundation_model_specs",
-                                                                   "Get available foundation models")['resources']
-                        if res['model_id'] == model_id][0]
-            except WMLClientError:  # Remove on CPD 5.0 release
-                return [res for res in _get_foundation_models_spec(f"{url}/ml/v1-beta/foundation_model_specs",
-                                                                   "Get available foundation models")['resources']
-                        if res['model_id'] == model_id][0]
-        else:
-            try:
-                return _get_foundation_models_spec(f"{url}/ml/v1/foundation_model_specs",
-                                                   "Get available foundation models")
-            except WMLClientError:  # Remove on CPD 5.0 release
-                return _get_foundation_models_spec(f"{url}/ml/v1-beta/foundation_model_specs",
-                                                   "Get available foundation models")
-    except WMLClientError as e:
-        raise WMLClientError(Messages.get_message(url, message_id="fm_prompt_tuning_no_model_specs"), e)
-
-
-def get_custom_model_specs(credentials: dict = None,
-                           api_client: 'APIClient' = None,
-                           model_id: Optional[str] = None,
-                           limit: int = 100, 
-                           asynchronous: bool = False, 
-                           get_all: bool = False,
-                           verify=None) -> Union[dict, Generator[dict, None, None]]:
-    """Get details on available custom model(s) as dict or as generator (``asynchronous``). 
-    If ``asynchronous`` or ``get_all`` is set, then ``model_id`` is ignored.
-
-    :param credentials: credentials to watsonx.ai instance
-    :type credentials: dict, optional
-
-    :param api_client: API client to connect to service
-    :type api_client: APIClient, optional
-
-    :param model_id: Id of the model, defaults to None (all models specs are returned).
-    :type model_id: str, optional
-
-    :param limit:  limit number of fetched records. Possible values: 1 ≤ value ≤ 200, default value: 100
-    :type limit: int, optional
-
-    :param asynchronous:  if True, it will work as a generator
-    :type asynchronous: bool, optional
-
-    :param get_all:  if True, it will get all entries in 'limited' chunks
-    :type get_all: bool, optional
-
-    :param verify: user can pass as verify one of following:
-
-        - the path to a CA_BUNDLE file
-        - the path of directory with certificates of trusted CAs
-        - `True` - default path to truststore will be taken
-        - `False` - no verification will be made
-    :type verify: bool or str, optional
-
-    :return: details of supported custom models
-    :rtype: dict
-
-    **Example**
-
-    .. code-block:: python
-
-        from ibm_watsonx_ai.foundation_models import get_custom_model_specs
-
-        get_custom_models_spec(api_client=client)
-        get_custom_models_spec(credentials=credentials)
-        get_custom_models_spec(api_client=client, model_id='mistralai/Mistral-7B-Instruct-v0.2')
-        get_custom_models_spec(api_client=client, limit=20)
-        get_custom_models_spec(api_client=client, limit=20, get_all=True)
-        for spec in get_custom_model_specs(api_client=client, limit=20, asynchronous=True, get_all=True):
-            print(spec, end="")
-
+    Wrapper class implementation for XGBoost containing the XGBoost Model Object
     """
-    warnings.warn("Model needs to be first stored via client.repository.store_model(model_id, meta_props=metadata)"
-                  " and deployed via client.deployments.create(asset_id, metadata) to be used.")
 
-    if credentials is None and api_client is None:
-        raise InvalidMultipleArguments(params_names_list=["credentials", "api_client"],
-                                       reason="None of the arguments were provided.")
-    elif credentials:
-        client = APIClient(credentials, verify=verify)
-    else:
-        client = api_client
-
-    url = client.wml_credentials['url']
-
-    params = client._params(skip_for_create=True)
-    if limit < 1 or limit > 200:
-        raise InvalidValue(value_name="limit", reason=f"The given value {limit} is not in the range <1, 200>")
-    else:
-        params.update({'limit': limit})
-
-    if asynchronous or get_all:
-        resource_generator = NextResourceGenerator(client,
-                                                   url=url,
-                                                   href="ml/v4/custom_foundation_models",
-                                                   params=params,
-                                                   _all=get_all)
-
-        if asynchronous:
-            return resource_generator
-
-        resources = []
-        for entry in resource_generator:
-            resources.extend(entry['resources'])
-        return {
-            "resources": resources
-        }
-
-    response = requests.get(f"{url}/ml/v4/custom_foundation_models", 
-                            params=params,
-                            headers=client._get_headers()) 
-    if response.status_code == 200:
-        if model_id:
-            resources = [res for res in response.json()['resources'] if res['model_id'] == model_id]
-            return resources[0] if resources else {}
-        else:
-            return response.json()
-    elif response.status_code == 404:
-        raise WMLClientError(Messages.get_message(url, message_id="custom_models_no_model_specs"), url)
-    else:
-        msg = f"Getting failed. Reason: {response.text}"
-        raise WMLClientError(msg)
+    def __init__(self, model_name, model_spec, xgb_model=None, **kwargs):
+        """
+        Create a XGBFLModel instance for XGBoost model based either on an
+        existing model object or an entirely new model object.
+
+        :param model_type: String specifying the name of the model
+        :type model_type: `str`
+        :param model_spec: Hyperparameters associated with the model.
+        :type model_spec: `dict`
+        :param xgb_model: List of predictors existing predictor structures.
+        :type xgb_model: `list`
+        :param kwargs: A dictionary contains other parameter settings on \
+         to initialize a XGBoost model.
+        :type kwargs: `dict`
+        """
+        super().__init__(model_name, model_spec, **kwargs)
+
+        # Initialize Input Model Object Parameters
+        # Note: For model loading process, onboard from `xgb_model` parameter.
+        self._predictors = []
+
+        # Initialize Additional Internal Model Parameters
+        self.model_type = 'XGBFLModel'
+        self._baseline_prediction = None
+        self._raw_predictions = None
+        self.n_features_ = 0
+        self.loss_ = None
+
+        # Validate and Initialize Model Hyperparameters
+        validate_parameters(model_spec)
+        init_parameters(self, model_spec)
+
+    def fit_model(self, train_data, fit_params=None, **kwargs):
+        """
+        This function is not implemented as model training is not operated
+        within the FL Model object and is part of an external process.
+
+        :return: `NotImplementedError`
+        """
+        return NotImplementedError
+
+    def update_model(self, model_update=None, **kwargs):
+        """
+        Updates model using provided `model_update`. Additional arguments
+        specific to the model can be added through `**kwargs`
+
+        :param model_update: Model with update. This is specific to each model \
+        type e.g., `ModelUpdateSGD`. The specific type should be checked by \
+        the corresponding FLModel class.
+        :type `ModelUpdate`
+        :param kwargs: Dictionary of model-specific arguments.
+        :type kwargs: `dict`
+        :return: None
+        """
+        if model_update is not None:
+            if isinstance(model_update.get('xgb_model'), list):
+                # Perform Model Update
+                self._predictors.append(model_update.get('xgb_model'))
+            else:
+                raise ValueError('Provided model object is not of the correct '
+                                 'data type. Should be a `list`. '
+                                 'Type provided: ' + str(type(model_update)))
+
+    def _raw_predict(self, x):
+        """
+        Internal helper function for generating predictions for the model.
+
+        :param x: The input data for the prediction model.
+        :type x: `np.array`
+        :param model: Model object which is used for generating the prediction. \
+        If not provided the default model assigned internally will be used.
+        :type model: `XGBFLModel`
+        :return: raw_predictions
+        :rtype: `np.array`
+        """
+        logger.info('Performing Model Inference Process')
+
+        # Initialize Prediction Object
+        n_samples = x.shape[0]
+        preds = np.zeros(shape=(self.n_trees, n_samples))
+
+        # Append Null Model Predictions
+        if self._baseline_prediction is not None:
+            preds += self._baseline_prediction
+        elif self._raw_predictions is not None:
+            preds += self._raw_predictions
+
+        # Generate Predictions
+        for p in self._predictors:
+            for k, p_i in enumerate(p):
+                preds[k, :] += p_i.predict(x.astype(np.float64))
+
+        return preds
+
+    def get_model_update(self):
+        """
+        Since we are not using the conventional train() function at the local
+        training handler, we respectively do not implement anything within here,
+        nor this function is utilized anywhere else.
+        """
+        return NotImplementedError
+
+    @abstractmethod
+    def predict(self, x):
+        """
+        Given a set of inputs, generate inference for the given set of samples.
+
+        :param x: The input data for the prediction model.
+        :type x: `np.array`
+        :param model: Model object which is used for generating the prediction. \
+        If not provided the default model assigned internally will be used.
+        :type model: `XGBFLModel`
+        :return: `np.array`
+        """
+        return NotImplementedError
+
+    def save_model(self, filename=None, path=None):
+        """
+        Saves a sklearn model to file in the format specific
+        to the framework requirement as a pickle file (only for inference use).
+
+        :param filename: Name of the file where to store the model.
+        :type filename: `str`
+        :param path: Path of the folder where to store the model. If no path \
+        is specified, the model will be stored in the default data location of \
+        the library `DATA_PATH`.
+        :type path: `str`
+        :return: filename
+        """
+        if filename is None:
+            file = self.model_name if self.model_name else self.model_type
+            filename = '{}_{}.pickle'.format(file, time.time())            
+            
+        full_path = super().get_model_absolute_path(filename)
 
+        # Scikit-Learn Export Demo
+        export_sklearn(self, full_path)
 
-def get_model_lifecycle(url: str, model_id: str) -> Union[list, None]:
-    """
-    Operation to retrieve the list of model lifecycle data.
-
-    :param url: environment url
-    :type url: str
-
-    :param model_id: the type of model to use
-    :type model_id: str
-
-    :return: list of deployed foundation model lifecycle data
-    :rtype: list
-
-    **Example**
-
-    .. code-block:: python
-
-        from ibm_watsonx_ai.foundation_models import get_model_lifecycle
-
-        get_model_lifecycle(
-            url="https://us-south.ml.cloud.ibm.com",
-            model_id="ibm/granite-13b-instruct-v2"
-            )
-    """
-    model_specs = get_model_specs(url=url)
-    model_spec = next((model_metadata for model_metadata in model_specs.get('resources', [])
-                       if model_metadata.get('model_id') == model_id), None)
-    return model_spec.get('lifecycle') if model_spec is not None else None
-
-
-def _check_model_state(url, model_id):
-    default_warning_template = (
-        "Model '{model_id}' is in {state} state from {start_date} until {withdrawn_start_date}. "
-        "IDs of alternative models: {alternative_model_ids}. "
-        "Further details: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-lifecycle.html?context=wx&audience=wdp")
-
-    lifecycle = get_model_lifecycle(url, model_id)
-
-    modes_list = [ids.get("id") for ids in (lifecycle or [])]
-    deprecated_or_constricted_warning_template_cpd = (
-            "Model '{model_id}' is in {state} state. "
-            "IDs of alternative models: {alternative_model_ids}. "
-            "Further details: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-lifecycle.html?context=wx&audience=wdp")
-
-    if lifecycle and SpecStates.DEPRECATED.value in modes_list:
-        model_lifecycle = next((el for el in lifecycle if el.get('id') == SpecStates.DEPRECATED.value), None)
-        if model_lifecycle.get('since_version'):
-            warnings.warn(deprecated_or_constricted_warning_template_cpd.format(
-                model_id=model_id,
-                state=(model_lifecycle.get('label') or SpecStates.DEPRECATED.value),
-                alternative_model_ids=', '.join(model_lifecycle.get('alternative_model_ids', ["None"]))
-            ), category=LifecycleWarning)
+        if len(self._predictors) > 0:
+            logger.info('Model saved in path: %s.', full_path)
         else:
-            warnings.warn(default_warning_template.format(
-                model_id=model_id,
-                state=(model_lifecycle.get('label') or SpecStates.DEPRECATED.value),
-                start_date=model_lifecycle.get('start_date'),
-                withdrawn_start_date=next((el.get('start_date') for el in lifecycle if el.get('id') == SpecStates.WITHDRAWN.value), None),
-                alternative_model_ids=', '.join(model_lifecycle.get('alternative_model_ids', ["None"]))
-            ), category=LifecycleWarning)
-
-    elif lifecycle and SpecStates.CONSTRICTED.value in modes_list:
-        model_lifecycle = next((el for el in lifecycle if el.get('id') == SpecStates.CONSTRICTED.value), None)
-        if model_lifecycle.get('since_version'):
-            warnings.warn(deprecated_or_constricted_warning_template_cpd.format(
-                model_id=model_id,
-                state=(model_lifecycle.get('label') or SpecStates.CONSTRICTED.value),
-                alternative_model_ids=', '.join(model_lifecycle.get('alternative_model_ids', ["None"]))
-            ), category=LifecycleWarning)
-        else:
-            warnings.warn(default_warning_template.format(
-                model_id=model_id,
-                state=(model_lifecycle.get('label') or SpecStates.CONSTRICTED.value),
-                start_date=model_lifecycle.get('start_date'),
-                withdrawn_start_date=next((el.get('start_date') for el in lifecycle if el.get('id') == SpecStates.WITHDRAWN.value), None),
-                alternative_model_ids=', '.join(model_lifecycle.get('alternative_model_ids', ["None"]))
-            ), category=LifecycleWarning)
-
-
-def get_model_specs_with_prompt_tuning_support(url: str) -> dict:
-    """
-    Operations to query the details of the deployed foundation models with prompt tuning support.
-
-    :param url: environment url
-    :type url: str
+            logger.info('Persisting empty model in path: %s.', full_path)
 
-    :return: list of deployed foundation model specs with prompt tuning support
-    :rtype: dict
+        return filename
 
-    **Example**
-
-    .. code-block:: python
-
-        from ibm_watsonx_ai.foundation_models import get_model_specs_with_prompt_tuning_support
-
-        get_model_specs_with_prompt_tuning_support(
-            url="https://us-south.ml.cloud.ibm.com"
-            )
-    """
-    try:
-        try:
-            return _get_foundation_models_spec(url=f"{url}/ml/v1/foundation_model_specs",
-                                               operation_name="Get available foundation models",
-                                               additional_params={"filters": "function_prompt_tune_trainable"})
-        except WMLClientError:  # Remove on CPD 5.0 release
-            return _get_foundation_models_spec(url=f"{url}/ml/v1-beta/foundation_model_specs",
-                                               operation_name="Get available foundation models",
-                                               additional_params={"filters": "function_prompt_tune_trainable"})
-    except WMLClientError as e:
-        raise WMLClientError(Messages.get_message(url, message_id="fm_prompt_tuning_no_model_specs"), e)
+    @staticmethod
+    def load_model(filename):
+        """
+        Load model from provided filename
+
+        :param filename: Name of the file where to store the model.
+        :type filename: `str`
+        :param path: Path of the folder where to store the model. If no path \
+        is specified, the model will be stored in the default data location of \
+        the library `DATA_PATH`.
+        :type path: `str`
+        :return: Returns the corresponding model object.
+        :rtype: `XGBFLModel`
+        """
+        absolute_path = config.get_absolute_path(filename)
+
+        with open(absolute_path, 'rb') as f:
+            model = pickle.load(f)
+            self = model
+
+        if len(self._predictors) == 0:
+            logger.info('Model does not contain any predictors.')
+
+        return model
+
+    @abstractmethod
+    def get_loss(self):
+        """
+        Internal helper function used to obtain the corresponding loss function
+        which is dependent on the learning task set by the hyperparameters.
+
+        :return: Returns the loss object used to compute the loss function.
+        :rtype: `BaseLoss` based object
+        """
+        return NotImplementedError
+
+    def evaluate(self, test_dataset, **kwargs):
+        """
+        Evaluates the model given testing data.
+        :param test_dataset: Testing data, a tuple given in the form \
+        (x_test, test) or a datagenerator of of type `keras.utils.Sequence`, \
+        `keras.preprocessing.image.ImageDataGenerator`
+        :type test_dataset: `np.ndarray`
+        :param kwargs: Dictionary of metrics available for the model
+        :type kwargs: `dict`
+        """
+
+        if type(test_dataset) is tuple:
+            x_test = test_dataset[0]
+            y_test = test_dataset[1]
 
+            return self.evaluate_model(x_test, y_test)
 
-def get_supported_tasks(url: str) -> dict:
-    """
-    Operation to retrieve the list of tasks that are supported by the foundation models.
+        else:
+            raise ModelException("Invalid test dataset!")
 
-    :param url: environment url
-    :type url: str
+    @abstractmethod
+    def evaluate_model(self, x, y, **kwargs):
+        """
+        Evaluates model given the samples x and true labels y.
+        Multiple evaluation metrics are returned in a dictionary
+
+        :param x: Samples with shape as expected by the model.
+        :type x: Data structure as expected by the model \
+        :param y: Corresponding labels to x
+        :type y: Data structure the same as the type defines labels \
+        in testing data.
+        :param batch_size: Size of batches.
+        :type batch_size: `int`
+        :param kwargs: Dictionary of model-specific arguments.
+        :type kwargs: `dict`
+        :return: Dictionary with all evaluation metrics provided by specific \
+        implementation.
+        :rtype: `dict`
+        """
+        return NotImplementedError
+
+
+class XGBRegressorFLModel(XGBFLModel):
+    _VALID_LOSSES = ('least_squares', 'least_absolute_deviation')
+
+    def predict(self, x):
+        """
+        Perform prediction for a batch of inputs.
+
+        :param x: Samples with shape as expected by the model.
+        :type x: Data structure as expected by the model
+        :param kwargs: Dictionary of model-specific arguments.
+        :type kwargs: `dict`
+        :return: Predictions
+        :rtype: Data structure the same as the type defines labels
+        in testing data.
+        """
+        if len(self._predictors) > 0:
+            return self._raw_predict(x).ravel()
+        else:
+            raise Exception('Model has not been trained yet.')
 
-    :return: list of tasks that are supported by the foundation models
-    :rtype: dict
+    def encode_target(self, y):
+        """
+        Converts the input y to the expected dtype.
+
+        :param y: The corresponding target data from the dataset to encode.
+        :type y: `np.array`
+        :return: Returns the corresponding encoded y values.
+        :rtype: `np.array`
+        """
+        self.n_trees = 1
+        return y.astype(Y_DTYPE, copy=False)
+
+    def get_loss(self, sample_weight):
+        """
+        Given the initialized loss type defined under the hyerparameters, we
+        return the corresponding loss function to dictate the corresponding
+        learning task of the model.
+
+        :param sample_weight: Weights of training data
+        :type sample_weight: `np.ndarray`
+        :return: Returns the respective loss object as defined in the FL \
+        hyperparameters.
+        :rtype: Derivation of `BaseLoss`
+        """
+        return _LOSSES[self.loss](sample_weight=sample_weight)
+
+    def evaluate_model(self, x, y, **kwargs):
+        """
+        Given an input set of values and their values, generate the prediction
+        and compute the R^2 metric.
+
+        :param x: The input data for the prediction model.
+        :type x: `np.array`
+        :param y: The corresponding target value of the prediction.
+        :type y: `np.array`
+        :return: Return a dictionary containing the R^2 metric for the provided
+        input and target values.
+        :rtype: `dict`
+        """
+        metrics = {}
+        if len(self._predictors) > 0:
+            y_hat = self.predict(x)
+            score = r2_score(y, y_hat)
+            metrics['r2_score'] = score
+            additional_metrics = fl_metrics.get_eval_metrics_for_regression(
+                y, y_hat)
+            metrics = {**metrics, **additional_metrics}
+            return metrics
+        else:
+            logger.info('Model has not been trained yet.')
+            return {}
 
-    **Example**
 
-    .. code-block:: python
+class XGBClassifierFLModel(XGBFLModel):
+    _VALID_LOSSES = ('binary_crossentropy', 'categorical_crossentropy', 'auto')
 
-        from ibm_watsonx_ai.foundation_models import get_supported_tasks
+    def encode_target(self, y):
+        """
+        Converts the input y to the expected dtype and performs a label
+        encoding. Here, we assume that each party has at least one sample of
+        the corresponding class label type for each different classes.
+
+        :param y: The corresponding target data from the dataset to encode.
+        :type  y: `np.array`
+        :return y: Returns the corresponding encoded y values.
+        :rtype  y: `np.array`
+        """
+        # Validate Classification Target Values
+        check_classification_targets(y)
+
+        # Apply Label Encoder Transformation
+        lab_enc = LabelEncoder()
+        enc_y = lab_enc.fit_transform(y).astype(np.float64, copy=False)
+
+        # Extract Encoded Target Sizes
+        self.classes_ = lab_enc.classes_
+        if self.classes_.shape[0] != self.num_classes:
+            raise ValueError('Number of classes defined in configuration file '
+                             'and the classes derived from the data does not '
+                             'match. Found {0} classes, while config file '
+                             'is defined as {1} classes.'.format(
+                             self.classes_.shape[0], self.num_classes))
 
-        get_supported_tasks(
-            url="https://us-south.ml.cloud.ibm.com"
-            )
-    """
-    try:
-        try:
-            return _get_foundation_models_spec(f"{url}/ml/v1/foundation_model_tasks",
-                                               "Get tasks that are supported by the foundation models.")
-        except WMLClientError:  # Remove on CPD 5.0 release
-            return _get_foundation_models_spec(f"{url}/ml/v1-beta/foundation_model_tasks",
-                                               "Get tasks that are supported by the foundation models.")
-    except WMLClientError as e:
-        raise WMLClientError(Messages.get_message(url, message_id="fm_prompt_tuning_no_supported_tasks"), e)
-
-
-def get_all_supported_tasks_dict(url="https://us-south.ml.cloud.ibm.com") -> dict:
-    tasks_dict = dict()
-    for task_spec in get_supported_tasks(url).get('resources', []):
-        tasks_dict[task_spec['label'].replace("-", "_").replace(" ", "_").upper()] = task_spec['task_id']
-    return tasks_dict
-
-
-def load_request_json(run_id, wml_client, run_params = None) -> dict:
-    if run_params is None:
-        run_params = wml_client.training.get_details(run_id)
-
-    model_request_path = run_params['entity'].get('results_reference', {}).get('location', {}).get('model_request_path')
+        if self.loss == 'auto':
+            self.n_trees = 1 if self.classes_.shape[0] <= 2 else self.classes_.shape[0]
+        else:
+            self.n_trees = 1 if self.num_classes <= 2 else self.num_classes
 
-    if model_request_path is None:
-        raise WMLClientError("Missing model_request_path in run_params. Verify if the training run has been completed.")
+        return enc_y
 
-    if wml_client.CLOUD_PLATFORM_SPACES:
-        results_reference = DataConnection._from_dict(run_params['entity']['results_reference'])
+    def get_loss(self, sample_weight):
+        """
+        Given the initialized loss type defined under the hyerparameters, we
+        return the corresponding loss function to dictate the corresponding
+        learning task of the model. If auto is selected, then we will
+        automatically determine whether the classification task is binary or
+        multiclass given the label encoding cardinality.
+
+        :param sample_weight: Weights of training data
+        :type sample_weight: `np.ndarray`
+        :return: Returns the respective loss object as defined in the FL \
+        hyperparameters.
+        :rtype: Derivation of `BaseLoss`
+        """
+        if (self.loss == 'categorical_crossentropy' and self.n_trees == 1):
+            raise ValueError("Incompatible loss and target variable counts.")
+
+        if self.loss == 'auto':
+            return _LOSSES['binary_crossentropy']() if self.n_trees == 1 else \
+                _LOSSES['categorical_crossentropy']()
+        else:
+            return _LOSSES[self.loss](sample_weight=sample_weight)
 
-        if run_params['entity']['results_reference']['type'] == DataConnectionTypes.CA:
-            results_reference.location.file_name = model_request_path
+    def predict(self, x, **kwargs):
+        """
+        Perform prediction for a batch of inputs returned as class values.
+
+        :param x: Samples with shape as expected by the model.
+        :type x: Data structure as expected by the model
+        :param kwargs: Dictionary of model-specific arguments.
+        :type kwargs: `dict`
+        :return: Predictions based on class values.
+        :rtype: Data structure the same as the type defines labels
+        in testing data.
+        """
+        if len(self._predictors) > 0:
+            encoded_classes = np.argmax(self.predict_proba(x), axis=1)
+            return self.classes_[encoded_classes]
         else:
-            results_reference.location.path = model_request_path
+            raise Exception('Model has not been trained yet.')
 
-        results_reference.set_client(wml_client)
-        request_json_bytes = results_reference.read(raw=True, binary=True)
+    def predict_proba(self, x, **kwargs):
+        """
+        Perform prediction for a batch of inputs as probabilities.
+
+        :param x: Samples with shape as expected by the model.
+        :type x: Data structure as expected by the model
+        :param kwargs: Dictionary of model-specific arguments.
+        :type kwargs: `dict`
+        :return: A probabilistic set of predictions
+        :rtype: Data structure the same as the type defines labels \
+        in testing data.
+        """
+        if len(self._predictors) > 0:
+            raw_predictions = self._raw_predict(x)
+            return self.loss_.predict_proba(raw_predictions)
+        else:
+            raise Exception('Model has not been trained yet.')
 
-        # download from cos
+    def evaluate_model(self, x, y, **kwargs):
+        """
+        Given an input set of values and their values, generate the prediction
+        and compute the accuracy.
+
+        :param x: The input data for the prediction model.
+        :type x: `np.array`
+        :param y: The corresponding target value of the prediction.
+        :type y: `np.array`
+        :return: Return a dictionary containing the accuracy for the provided \
+        input and target values.
+        :rtype: `dict`
+        """
+        acc = {}
+        if len(self._predictors) > 0:
+            y_hat = self.predict(x)
+            correct = 0
+            for i in range(x.shape[0]):
+                if y_hat[i] == y[i]:
+                    correct += 1
+
+            acc = {'acc': correct/float(len(y))}
+            additional_metrics = fl_metrics.get_eval_metrics_for_classificaton(
+                y, y_hat)
 
-    elif wml_client.CPD_version >= 4.8:
-        asset_parts = model_request_path.split('/')
-        model_request_asset_url = '/'.join(asset_parts[asset_parts.index('assets') + 1:])
-        request_json_bytes = load_file_from_file_system_nonautoai(api_client=wml_client,
-                                                                  file_path=model_request_asset_url).read()
-    else:
-        raise WMLClientError("Unsupported environment for this action")
-
-    return json_loads(request_json_bytes.decode())
-
-
-def is_training_prompt_tuning(training_id, wml_client):
-    """Returns True if training_id is connected to prompt tuning"""
-    if training_id is None:
-        return False
-    run_params = wml_client.training.get_details(training_uid=training_id)
-    return bool(run_params['entity'].get('prompt_tuning'))
-
-
-class TemplateFormatter(Formatter):
-    def check_unused_args(self, 
-                          used_args: List[(int | str)], 
-                          args: Sequence, 
-                          kwargs: Dict[str, Any]) -> None:
-        """Check for unused args."""
-        extra_args = set(kwargs).difference(used_args)
-        if extra_args:
-            raise KeyError(extra_args)
-
-class HAPDetectionWarning(UserWarning): ...
-class PIIDetectionWarning(UserWarning): ...
-class LifecycleWarning(UserWarning): ...
-class WatsonxLLMDeprecationWarning(UserWarning): ...
-
-
-def _raise_watsonxllm_deprecation_warning() -> None:
-    warnings.warn("ibm_watsonx_ai.foundation_models.extensions.langchain.WatsonxLLM"
-                  " is deprecated and will not be supported in the future. "
-                  "Please import from langchain-ibm instead.\n"
-                  "To install langchain-ibm run `pip install -U langchain-ibm`.",
-                  category=WatsonxLLMDeprecationWarning,
-                  stacklevel=2
-                  )
-    
-def get_embedding_model_specs(url: str) -> dict:
-    return _get_foundation_models_spec(url=f'{url}/ml/v1/foundation_model_specs',
-                                       operation_name='Get available embedding models',
-                                       additional_params={'filters': 'function_embedding'})
+            acc = {**acc, **additional_metrics}
+            return acc
+        else:
+            logger.info('No models have been trained yet.')
+            return {}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/base_connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/base_data_connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/base_data_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from abc import ABC, abstractmethod
 from typing import Union, Tuple, TYPE_CHECKING
 from warnings import warn
 
 import pandas as pd
 
 import ibm_watsonx_ai._wrappers.requests as requests
-from pandas import concat, DataFrame, read_csv
+from pandas import DataFrame, read_csv
 
-from ibm_watsonx_ai.utils.autoai.utils import try_load_dataset, try_load_tar_gz, try_import_autoai_libs
+from ibm_watsonx_ai.utils.autoai.utils import try_load_dataset, try_load_tar_gz
 from ibm_watsonx_ai.utils.autoai.enums import DataConnectionTypes
 from ibm_watsonx_ai.utils.autoai.errors import CannotReadSavedRemoteDataBeforeFit, WrongAssetType
-from ibm_watsonx_ai.wml_client_error import ApiRequestFailure, WMLClientError, DataStreamError
+from ibm_watsonx_ai.wml_client_error import ApiRequestFailure, DataStreamError
 from ibm_watsonx_ai.utils.utils import is_lib_installed
 from ibm_watsonx_ai.data_loaders.datasets.experiment import DEFAULT_SAMPLING_TYPE, DEFAULT_SAMPLE_SIZE_LIMIT
 
 if TYPE_CHECKING:
     from ibm_boto3 import resource
 
 
@@ -141,17 +141,17 @@
                 json_content = json.loads(content.decode('utf-8'))
             except Exception as cos_access_exception:
                 raise ConnectionError(
                     f"Unable to access data object in cloud object storage with credentials supplied. "
                     f"Error: {cos_access_exception}")
         elif self.type == DataConnectionTypes.FS:
             if "prompt_tune" in path:
-                json_url = self._wml_client.service_instance._href_definitions.get_wsd_model_attachment_href() + f"wx_prompt_tune/{path.split('/wx_prompt_tune/')[-1]}"
+                json_url = self._api_client.service_instance._href_definitions.get_wsd_model_attachment_href() + f"wx_prompt_tune/{path.split('/wx_prompt_tune/')[-1]}"
             else:
-                json_url = self._wml_client.service_instance._href_definitions.get_wsd_model_attachment_href() + f"/auto_ml/{path.split('/auto_ml/')[-1]}"
+                json_url = self._api_client.service_instance._href_definitions.get_wsd_model_attachment_href() + f"/auto_ml/{path.split('/auto_ml/')[-1]}"
 
             with requests.get(json_url, params=self._api_client._params(), headers=self._api_client._get_headers(),
                               stream=True) as file_response:
                 if file_response.status_code != 200:
                     raise ApiRequestFailure(u'Failure during {}.'.format("downloading json"), file_response)
 
                 downloaded_asset = file_response.content
@@ -196,15 +196,15 @@
 
         attachments_data_asset_details = data_asset_details.get('attachments', [{}])[0]
         # note: Return attachment details from data asset details if it is not a connected data asset:
         if attachments_data_asset_details and attachments_data_asset_details.get('connection_id') is None:
             return attachments_data_asset_details
         else:
             attachment_id = attachments_data_asset_details.get('id')
-            if not self._api_client.ICP:
+            if not self._api_client.ICP_PLATFORM_SPACES:
                 response = requests.get(
                     self._api_client.service_instance._href_definitions.get_attachment_href(data_asset_id, attachment_id),
                     params=self._api_client._params(),
                     headers=self._api_client._get_headers())
             else:
                 response = requests.get(
                     self._api_client.service_instance._href_definitions.get_attachment_href(data_asset_id, attachment_id),
@@ -294,17 +294,17 @@
             else:
                 raise WrongAssetType(asset_type=self.type)
 
             # Note: Check with project libs if connection points to S3
             if self._api_client is not None:
                 datasource_type = connection_details['entity']['datasource_type']
                 self._datasource_type = datasource_type
-                datasource_type_id_ibm_cos = self._api_client.connections.get_datasource_type_uid_by_name(
+                datasource_type_id_ibm_cos = self._api_client.connections.get_datasource_type_id_by_name(
                     'bluemixcloudobjectstorage')
-                datasource_type_id_aws_cos = self._api_client.connections.get_datasource_type_uid_by_name(
+                datasource_type_id_aws_cos = self._api_client.connections.get_datasource_type_id_by_name(
                     'cloudobjectstorage')
 
                 if (datasource_type == datasource_type_id_ibm_cos or datasource_type == datasource_type_id_aws_cos or
                         datasource_type == 'bluemixcloudobjectstorage' or datasource_type == 'cloudobjectstorage'):
                     cos_type = True
 
                 else:
@@ -442,15 +442,15 @@
                 items = self.location.href.split('/')
             _id = items[-1].split('?')[0]
 
             if self._api_client is not None:
                 attachment_details = self._get_attachemnt_details(_id)
 
                 return ('connection_id' in attachment_details and attachment_details.get(
-                    'datasource_type') == self._api_client.connections.get_datasource_type_uid_by_name('volumes'))
+                    'datasource_type') == self._api_client.connections.get_datasource_type_id_by_name('volumes'))
         return False
 
 
     def _download_indices_from_cos(self, cos_client: 'resource', location_path) -> 'DataFrame':
         """Download indices for this connection. COS version"""
 
         try:
@@ -502,15 +502,15 @@
 
             if response.status_code == 200:
                 try:
                     attachment_details = response.json()
                     if "url" in attachment_details:
                         file_asset_url = attachment_details['url']
                         if not file_asset_url.startswith("http"):
-                            file_asset_url = self._api_client.wml_credentials['url'] + file_asset_url
+                            file_asset_url = self._api_client.credentials.url + file_asset_url
                         csv_response = requests.get(file_asset_url)
 
                         if csv_response.status_code != 200:
                             raise ApiRequestFailure(u'Failure during {}.'.format("downloading model"), csv_response)
 
                         downloaded_asset = csv_response.content
 
@@ -950,15 +950,15 @@
             "project_id": self._api_client.default_project_id,
             "space_id": self._api_client.default_space_id,
             'headers': self._api_client._get_headers() if headers is None else headers
         }
 
         experiment_metadata.update(self.auto_pipeline_params)
         if binary and isinstance(self.location, DatabaseLocation):
-            write_mode = self._wml_client.connections.get_write_mode_by_datasource_type(self._datasource_type)
+            write_mode = self._api_client.connections.get_write_mode_by_datasource_type(self._datasource_type)
             extra_interaction_properties = {'write_mode': write_mode}
         else:
             extra_interaction_properties = {}
 
         iterable_dataset = ExperimentIterableDataset(
             connection=dict_connection,
             experiment_metadata=experiment_metadata,
@@ -1022,20 +1022,14 @@
             token = os.environ.get('USER_ACCESS_TOKEN')
 
         if token:
             token = token.replace('Bearer ', '')
 
         return token
 
-    @staticmethod
-    def _get_url_from_environment():
-        url = os.environ.get('RUNTIME_ENV_APSX_URL')
-
-        return url
-
     def _is_size_acceptable(self):
         """
         Checks if data asset size is acceptable to download based on available memory in pod (MEM env variable)/ T-shirt size.
         Returns: True when data asset size is equal or lower than T-shirt limitation or when limitation is not set (outside autoai pod).
                 False when data asset size is known and is above supported limit.
                 None when data asset size is unknown or data_connection is not data asset type.
         """
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/base_location.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/base_location.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/connections.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,24 @@
 from typing import Union, Tuple, List, TYPE_CHECKING, Optional
 from warnings import warn
 
 from ibm_boto3 import resource
 from ibm_botocore.client import ClientError
 from pandas import DataFrame
 import ibm_watsonx_ai._wrappers.requests as requests
-from ibm_watsonx_ai.utils.autoai.enums import PredictionType, DataConnectionTypes
+from ibm_watsonx_ai.utils.autoai.enums import DataConnectionTypes
 from ibm_watsonx_ai.utils.autoai.errors import (
-    MissingAutoPipelinesParameters, UseWMLClient, MissingCOSStudioConnection, MissingProjectLib,
-    HoldoutSplitNotSupported, InvalidCOSCredentials, MissingLocalAsset, InvalidIdType,
-    NotExistingCOSResource, InvalidDataAsset, CannotReadSavedRemoteDataBeforeFit, NoAutomatedHoldoutSplit
+    MissingAutoPipelinesParameters, MissingCOSStudioConnection, MissingProjectLib, 
+    InvalidCOSCredentials, InvalidIdType,
+    NotExistingCOSResource, CannotReadSavedRemoteDataBeforeFit, NoAutomatedHoldoutSplit
 )
 
 import numpy as np
 from ibm_watsonx_ai.utils.autoai.utils import all_logging_disabled, try_import_autoai_libs, \
     try_import_autoai_ts_libs
-from ibm_watsonx_ai.utils.autoai.watson_studio import get_project
 from ibm_watsonx_ai.data_loaders.datasets.experiment import DEFAULT_SAMPLING_TYPE, DEFAULT_SAMPLE_SIZE_LIMIT
 from ibm_watsonx_ai.wml_client_error import MissingValue, ApiRequestFailure, WMLClientError
 from ibm_watsonx_ai.utils.autoai.errors import ContainerTypeNotSupported
 from ibm_watsonx_ai.messages.messages import Messages
 from .base_connection import BaseConnection
 from .base_data_connection import BaseDataConnection
 from .base_location import BaseLocation
@@ -814,15 +813,15 @@
 
                 except FileNotFoundError as e:
                     raise e
 
                 except Exception as e:
                     # do not try Flight if we are on the cloud
                     if self._api_client is not None:
-                        if not self._api_client.ICP:
+                        if not self._api_client.ICP_PLATFORM_SPACES:
                             raise e
 
                     elif os.environ.get('USER_ACCESS_TOKEN') is None and os.environ.get('RUNTIME_ENV_ACCESS_TOKEN_FILE') is None:
                         raise CannotReadSavedRemoteDataBeforeFit()
 
                     data = self._download_data_from_flight_service(data_location=self,
                                                                    binary=binary,
@@ -838,15 +837,15 @@
                                                                    total_nrows_limit=total_nrows_limit,
                                                                    total_percentage_limit=total_percentage_limit)
 
         elif self.type == DataConnectionTypes.FS:
             data = self._download_training_data_from_file_system()
 
         elif self.type == DataConnectionTypes.CA or self.type == DataConnectionTypes.CN:
-            if getattr(self._api_client, 'ICP', False) and self.type == DataConnectionTypes.CN:
+            if getattr(self._api_client, 'ICP_PLATFORM_SPACES', False) and self.type == DataConnectionTypes.CN:
                 raise ContainerTypeNotSupported()  # block Container type on CPD
 
             if use_flight:
                 # Workaround for container connection type, we need to fetch COS details from space/project
                 if self.type == DataConnectionTypes.CN:
                     # note: update flight parameters only if `connection_properties` was not set earlier
                     #       (e.x. by wml/autoi)
@@ -881,15 +880,15 @@
                                     f"Error: {cos_access_exception}")
                         else:
                             data = self._download_data_from_nfs_connection()
 
                 except Exception as e:
                     # do not try Flight is we are on the cloud
                     if self._api_client is not None:
-                        if not self._api_client.ICP:
+                        if not self._api_client.ICP_PLATFORM_SPACES:
                             raise e
 
                     elif os.environ.get('USER_ACCESS_TOKEN') is None and os.environ.get('RUNTIME_ENV_ACCESS_TOKEN_FILE') is None:
                         raise CannotReadSavedRemoteDataBeforeFit()
 
                     data = self._download_data_from_flight_service(data_location=self,
                                                                    binary=binary,
@@ -1000,20 +999,20 @@
             headers['impersonate'] = impersonate_header
 
         # TODO: Remove S3 implementation
         if self.type == DataConnectionTypes.S3:
             raise ConnectionError("S3 DataConnection is not supported. Please use data_asset_id instead.")
 
         elif self.type == DataConnectionTypes.CA or self.type == DataConnectionTypes.CN:
-            if getattr(self._api_client, 'ICP', False) and self.type == DataConnectionTypes.CN:
+            if getattr(self._api_client, 'ICP_PLATFORM_SPACES', False) and self.type == DataConnectionTypes.CN:
                 raise ContainerTypeNotSupported()  # block Container type on CPD
 
             if self._check_if_connection_asset_is_s3():
                 # do not try Flight if we are on the cloud
-                if self._api_client is not None and not self._api_client.ICP and not use_flight:  # CLOUD
+                if self._api_client is not None and not self._api_client.ICP_PLATFORM_SPACES and not use_flight:  # CLOUD
                     if remote_name is None and self._to_dict().get('location', {}).get('path'):
                         updated_remote_name = data.split('/')[-1]
                     else:
                         updated_remote_name = self._get_path_with_remote_name(self._to_dict(), remote_name)
                     cos_resource_client = self._init_cos_client()
                     if isinstance(data, str):
                         with open(data, "rb") as file_data:
@@ -1056,15 +1055,15 @@
                                                              flight_parameters=flight_parameters,
                                                              headers=headers)
 
                     else:
                         raise TypeError("data should be either of type \"str\" or \"pandas.DataFrame\"")
 
             else:
-                if self._api_client is not None and not self._api_client.ICP and not use_flight:  # CLOUD
+                if self._api_client is not None and not self._api_client.ICP_PLATFORM_SPACES and not use_flight:  # CLOUD
                     raise ConnectionError("Connections other than COS are not supported on a cloud yet.")
                 # CP4D
                 else:
                     if isinstance(data, str):
                         self._upload_data_via_flight_service(file_path=data,
                                                              data_location=self,
                                                              remote_name=remote_name,
@@ -1087,15 +1086,15 @@
                 pass  # don't remove additional params if client is used internally
             else:
                 # note: remove additional params and inline credentials added by _check_if_connection_asset_is_s3:
                 [delattr(self.connection, attr) for attr in ['secret_access_key', 'access_key_id', 'endpoint_url', 'cos_type'] if
                     hasattr(self.connection, attr)]
                 # end note
         elif self.type == DataConnectionTypes.DS:
-            if self._api_client is not None and not self._api_client.ICP and not use_flight:  # CLOUD
+            if self._api_client is not None and not self._api_client.ICP_PLATFORM_SPACES and not use_flight:  # CLOUD
                 raise ConnectionError("Write of data for Data Asset is not supported on Cloud.")
 
             elif self._api_client is not None:
                 if isinstance(data, str):
                     self._upload_data_via_flight_service(file_path=data,
                                                          data_location=self,
                                                          remote_name=remote_name,
@@ -1331,15 +1330,15 @@
         return location
 
     def _save_file_as_data_asset(self, workspace: 'WorkSpace') -> 'str':
 
         asset_name = self.path.split('/')[-1]
         if self.path:
             data_asset_details = workspace.api_client.data_assets.create(asset_name, self.path)
-            return workspace.api_client.data_assets.get_uid(data_asset_details)
+            return workspace.api_client.data_assets.get_id(data_asset_details)
         else:
             raise MissingValue('path', reason="Incorrect initialization of class FSLocation")
 
     def _get_file_size(self, workspace: 'WorkSpace') -> 'int':
         # note if path is not file then returned size is 0
         try:
             # note: try to get file size from remote server
@@ -1400,15 +1399,15 @@
 
         else:
             attachment_id = asset_details['attachments'][0]['id']
 
         attachment_url = client.service_instance._href_definitions.get_data_asset_href(self.id)
         attachment_url = f"{attachment_url}/attachments/{attachment_id}"
 
-        if client.ICP:
+        if client.ICP_PLATFORM_SPACES:
             attachment = requests.get(attachment_url, headers=client._get_headers(),
                                       params=client._params())
 
         else:
             attachment = requests.get(attachment_url, headers=client._get_headers(),
                                       params=client._params())
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/flight_service.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/flight_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,19 +325,19 @@
             self.read_status_change.notify_all()
 
     def _set_default_flight_location(self) -> None:
         """Try to set default flight location and port from WS."""
         if not os.environ.get(
                 'FLIGHT_SERVICE_LOCATION') and self._api_client and self._api_client.CLOUD_PLATFORM_SPACES:
             try:
-                flight_location = self._api_client.PLATFORM_URLS_MAP[self._api_client.wml_credentials['url']].replace(
+                flight_location = self._api_client.PLATFORM_URLS_MAP[self._api_client.credentials.url].replace(
                     'https://', '')
             except Exception as e:
-                if self._api_client.wml_credentials['url'] in self._api_client.PLATFORM_URLS_MAP.values():
-                    flight_location = self._api_client.wml_credentials['url'].replace('https://', '')
+                if self._api_client.credentials.url in self._api_client.PLATFORM_URLS_MAP.values():
+                    flight_location = self._api_client.credentials.url.replace('https://', '')
                 else:
                     raise e
             flight_port = 443
         else:
             host = os.environ.get('ASSET_API_SERVICE_HOST', os.environ.get('CATALOG_API_SERVICE_HOST'))
 
             if host is None or 'api.' not in host:
@@ -429,16 +429,16 @@
                                  f" attempting to retry the authentication. ")
                     waiting_time = 2**count_auth_retries_power
                     real_waiting_time += waiting_time
                     time.sleep(waiting_time)
                     count_auth_retries_power += 1
                 else:
                     # suggest CPD users to check the Flight variables
-                    if hasattr(self._api_client, 'ICP'):
-                        if self._api_client.ICP:
+                    if hasattr(self._api_client, 'ICP_PLATFORM_SPACES'):
+                        if self._api_client.ICP_PLATFORM_SPACES:
                             raise ConnectionError(
                                 f"Cannot connect to the Flight service. Please make sure you set correct "
                                 f"FLIGHT_SERVICE_LOCATION and FLIGHT_SERVICE_PORT environmental variables.\n"
                                 f"If you are trying to connect to FIPS-enabled cluster, "
                                 f"please set the following as environment variable and try again:\n"
                                 f"GRPC_SSL_CIPHER_SUITES="
                                 f"ECDHE-RSA-AES128-SHA256:ECDHE-RSA-AES128-GCM-SHA256:ECDHE-RSA-AES256-GCM-SHA384 "
@@ -1235,15 +1235,15 @@
             del command['interaction_properties']['path']
 
         if 'connection_properties' not in command:
             logger.debug(f"Command: {command}")
 
         return [json.dumps(command)]
 
-    def read_binary_data(self, read_to_file=None) -> None:
+    def read_binary_data(self, read_to_file: str | None = None) -> Generator | list:
         """Try to read data from flight service using the 'read_raw' parameter. This will allow to fetch binary data.
         Binary read should be used for small data, like json files, zip files etc. not for the big datasets as
         each data batch is joined to the previous one in-memory.
         """
         self.read_binary = True
 
         if self.flight_parameters.get('num_partitions') is None:
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/connections/local.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/connections/local.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/helpers/helpers.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/href_definitions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/href_definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,591 +1,730 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
+from __future__ import annotations
+from typing import TYPE_CHECKING
 
 import re
 
-TRAINING_MODEL_HREF_PATTERN = u'{}/v4/trainings/{}'
-TRAINING_MODELS_HREF_PATTERN = u'{}/v4/trainings'
-REPO_MODELS_FRAMEWORKS_HREF_PATTERN = u'{}/v3/models/frameworks'
-
-INSTANCE_ENDPOINT_HREF_PATTERN = u'{}/v3/wml_instance'
-INSTANCE_BY_ID_ENDPOINT_HREF_PATTERN = u'{}/v3/wml_instances/{}'
-TOKEN_ENDPOINT_HREF_PATTERN = u'{}/v3/identity/token'
-CPD_TOKEN_ENDPOINT_HREF_PATTERN = u'{}/icp4d-api/v1/authorize'
-CPD_BEDROCK_TOKEN_ENDPOINT_HREF_PATTERN = u'{}/idprovider/v1/auth/identitytoken'
-CPD_VALIDATION_TOKEN_ENDPOINT_HREF_PATTERN = u'{}/v1/preauth/validateAuth'
-EXPERIMENTS_HREF_PATTERN = u'{}/v4/experiments'
-EXPERIMENT_HREF_PATTERN = u'{}/v4/experiments/{}'
-EXPERIMENT_RUNS_HREF_PATTERN = u'{}/v3/experiments/{}/runs'
-EXPERIMENT_RUN_HREF_PATTERN = u'{}/v3/experiments/{}/runs/{}'
-
-PUBLISHED_MODEL_HREF_PATTERN = u'{}/v4/models/{}'
-PUBLISHED_MODELS_HREF_PATTERN = u'{}/v4/models'
-LEARNING_CONFIGURATION_HREF_PATTERN = u'{}/v3/wml_instances/{}/published_models/{}/learning_configuration'
-LEARNING_ITERATION_HREF_PATTERN = u'{}/v3/wml_instances/{}/published_models/{}/learning_iterations/{}'
-LEARNING_ITERATIONS_HREF_PATTERN = u'{}/v3/wml_instances/{}/published_models/{}/learning_iterations'
-EVALUATION_METRICS_HREF_PATTERN = u'{}/v3/wml_instances/{}/published_models/{}/evaluation_metrics'
-FEEDBACK_HREF_PATTERN = u'{}/v3/wml_instances/{}/published_models/{}/feedback'
-
-DEPLOYMENTS_HREF_PATTERN = u'{}/v4/deployments'
-DEPLOYMENT_HREF_PATTERN = u'{}/v4/deployments/{}'
-DEPLOYMENT_JOB_HREF_PATTERN = u'{}/v4/deployment_jobs'
-DEPLOYMENT_JOBS_HREF_PATTERN = u'{}/v4/deployment_jobs/{}'
-DEPLOYMENT_ENVS_HREF_PATTERN = u'{}/v4/deployments/environments'
-DEPLOYMENT_ENV_HREF_PATTERN = u'{}/v4/deployments/environments/{}'
-
-MODEL_LAST_VERSION_HREF_PATTERN = u'{}/v4/models/{}'
-DEFINITION_HREF_PATTERN = u'{}/v3/ml_assets/training_definitions/{}'
-DEFINITIONS_HREF_PATTERN = u'{}/v3/ml_assets/training_definitions'
-
-FUNCTION_HREF_PATTERN = u'{}/v4/functions/{}'
-FUNCTION_LATEST_CONTENT_HREF_PATTERN = u'{}/v4/functions/{}/content'
-FUNCTIONS_HREF_PATTERN = u'{}/v4/functions'
-
-IAM_TOKEN_API = u'{}&grant_type=urn%3Aibm%3Aparams%3Aoauth%3Agrant-type%3Aapikey'
-IAM_TOKEN_URL = u'{}/oidc/token'
-PROD_SVT_URL = ['https://us-south.ml.cloud.ibm.com',
-                'https://eu-gb.ml.cloud.ibm.com',
-                'https://eu-de.ml.cloud.ibm.com',
-                'https://jp-tok.ml.cloud.ibm.com',
-                'https://ibm-watson-ml.mybluemix.net',
-                'https://ibm-watson-ml.eu-gb.bluemix.net',
-                'https://private.us-south.ml.cloud.ibm.com',
-                'https://private.eu-gb.ml.cloud.ibm.com',
-                'https://private.eu-de.ml.cloud.ibm.com',
-                'https://private.jp-tok.ml.cloud.ibm.com',
-                'https://yp-qa.ml.cloud.ibm.com',
-                'https://private.yp-qa.ml.cloud.ibm.com',
-                'https://yp-cr.ml.cloud.ibm.com',
-                'https://private.yp-cr.ml.cloud.ibm.com']
-
-PIPELINES_HREF_PATTERN=u'{}/v4/pipelines'
-PIPELINE_HREF_PATTERN=u'{}/v4/pipelines/{}'
-
-
-SPACES_HREF_PATTERN = u'{}/v4/spaces'
-SPACE_HREF_PATTERN = u'{}/v4/spaces/{}'
-MEMBER_HREF_PATTERN=u'{}/v4/spaces/{}/members/{}'
-MEMBERS_HREF_PATTERN=u'{}/v4/spaces/{}/members'
-
-SPACES_PLATFORM_HREF_PATTERN = u'{}/v2/spaces'
-SPACE_PLATFORM_HREF_PATTERN = u'{}/v2/spaces/{}'
-SPACES_MEMBERS_HREF_PATTERN = u'{}/v2/spaces/{}/members'
-SPACES_MEMBER_HREF_PATTERN = u'{}/v2/spaces/{}/members/{}'
-
-V4_INSTANCE_ID_HREF_PATTERN = u'{}/ml/v4/instances/{}'
-
-API_VERSION = u'/v4'
-SPACES=u'/spaces'
-PIPELINES=u'/pipelines'
-EXPERIMENTS=u'/experiments'
-LIBRARIES=u'/libraries'
-RUNTIMES=u'/runtimes'
-SOFTWARE_SPEC=u'/software_specifications'
-DEPLOYMENTS = u'/deployments'
-ASSET = u'{}/v2/assets/{}'
-ASSETS = u'{}/v2/assets'
-ASSET_TYPE = u'{}/v2/asset_types'
-ASSET_FILES = u'{}/v2/asset_files/'
-ATTACHMENT = u'{}/v2/assets/{}/attachments/{}'
-ATTACHMENT_COMPLETE = u'{}/v2/assets/{}/attachments/{}/complete'
-ATTACHMENTS = u'{}/v2/assets/{}/attachments'
-SEARCH_ASSETS = u'{}/v2/asset_types/{}/search'
-SEARCH_MODEL_DEFINITIONS = u'{}/v2/asset_types/wml_model_definition/search'
-SEARCH_DATA_ASSETS = u'{}/v2/asset_types/data_asset/search'
-SEARCH_SHINY = u'{}/v2/asset_types/shiny_asset/search'
-SEARCH_SCRIPT = u'{}/v2/asset_types/script/search'
-GIT_BASED_PROJECT_ASSET = u'{}/userfs/v2/assets/{}'
-GIT_BASED_PROJECT_ASSETS = u'{}/userfs/v2/assets'
-GIT_BASED_PROJECT_ASSET_TYPE = u'{}/userfs/v2/asset_types'
-GIT_BASED_PROJECT_ASSET_FILES = u'{}/v2/asset_files/'
-GIT_BASED_PROJECT_ATTACHMENT = u'{}/userfs/v2/assets/{}/attachments/{}'
-GIT_BASED_PROJECT_ATTACHMENT_COMPLETE = u'{}/userfs/v2/assets/{}/attachments/{}/complete'
-GIT_BASED_PROJECT_ATTACHMENTS = u'{}/userfs/v2/assets/{}/attachments'
-GIT_BASED_PROJECT_SEARCH_ASSETS = u'{}/userfs/v2/asset_types/{}/search'
-GIT_BASED_PROJECT_SEARCH_MODEL_DEFINITIONS = u'{}/userfs/v2/asset_types/wml_model_definition/search'
-GIT_BASED_PROJECT_SEARCH_DATA_ASSETS = u'{}/userfs/v2/asset_types/data_asset/search'
-GIT_BASED_PROJECT_SEARCH_SHINY = u'{}/userfs/v2/asset_types/shiny_asset/search'
-GIT_BASED_PROJECT_SEARCH_SCRIPT = u'{}/userfs/v2/asset_types/script/search'
-DATA_SOURCE_TYPE = u'{}/v2/datasource_types'
-DATA_SOURCE_TYPE_BY_ID = u'{}/v2/datasource_types/{}'
-CONNECTION_ASSET = u'{}/v2/connections'
-CONNECTION_ASSET_SEARCH = u'{}/v2/connections'
-CONNECTION_BY_ID = u'{}/v2/connections/{}'
-CONNECTIONS_FILES = u'{}/v2/connections/files'
-CONNECTIONS_FILE = u'{}/v2/connections/files/{}'
-SOFTWARE_SPECIFICATION = u'{}/v2/software_specifications/{}'
-SOFTWARE_SPECIFICATIONS = u'{}/v2/software_specifications'
-HARDWARE_SPECIFICATION = u'{}/v2/hardware_specifications/{}'
-HARDWARE_SPECIFICATIONS = u'{}/v2/hardware_specifications'
-PACKAGE_EXTENSION = u'{}/v2/package_extensions/{}'
-PACKAGE_EXTENSIONS = u'{}/v2/package_extensions'
-PARAMETER_SET = u'{}/v2/parameter_sets/{}'
-PARAMETER_SETS = u'{}/v2/parameter_sets'
-PROJECT = u'{}/v2/projects/{}'
-LIST_SOFTWARE_SPECIFICATIONS = '{}/ml/v4/list/software_specifications'
-
-V4GA_CLOUD_MIGRATION = u'{}/ml/v4/repository'
-V4GA_CLOUD_MIGRATION_ID = u'{}/ml/v4/repository/{}'
-
-REMOTE_TRAINING_SYSTEM = u'{}/v4/remote_training_systems'
-REMOTE_TRAINING_SYSTEM_ID = u'{}/v4/remote_training_systems/{}'
-
-FM_GENERATION = u'{}/ml/v1/text/generation'
-FM_GENERATION_BETA = u'{}/ml/v1-beta/generation/{}'  # Remove on CPD 5.0 release
-FM_GENERATION_STREAM = u'{}/ml/v1/text/generation_stream'
-FM_GET_SPECS = u'{}/ml/v1/foundation_model_specs?limit={}'
-FM_GET_SPECS_BETA = u'{}/ml/v1-beta/foundation_model_specs?version=2022-08-01&limit={}'  # Remove on CPD 5.0 release
-FM_GET_TASKS = u'{}/ml/v1/foundation_model_tasks?limit={}'
-FM_TOKENIZE = u'{}/ml/v1/text/tokenization'
-FM_TOKENIZE_BETA = u'{}/ml/v1-beta/text/tokenization'  # Remove on CPD 5.0 release
-FM_EMBEDDINGS = u'{}/ml/v1/text/embeddings'
-
-FM_DEPLOYMENT_GENERATION = u'{}/ml/v1/deployments/{}/text/generation'
-FM_DEPLOYMENT_GENERATION_STREAM = u'{}/ml/v1/deployments/{}/text/generation_stream'
-FM_DEPLOYMENT_GENERATION_BETA = u'{}/ml/v1-beta/deployments/{}/generation/{}'  # Remove on CPD 5.0 release
-
-PROMPTS = u'{}/wx/v1-beta/prompts'
-PROMPTS_GET_ALL = u'{}/v2/asset_types/wx_prompt/search'
-
-EXPORTS = u'{}/v2/asset_exports'
-EXPORT_ID = u'{}/v2/asset_exports/{}'
-EXPORT_ID_CONTENT = u'{}/v2/asset_exports/{}/content'
-
-IMPORTS = u'{}/v2/asset_imports'
-IMPORT_ID = u'{}/v2/asset_imports/{}'
-
-VOLUMES = u'{}/zen-data/v3/service_instances'
-VOLUME_ID = u'{}/zen-data/v3/service_instances/{}'
-VOLUME_SERVICE = u'{}/zen-data/v1/volumes/volume_services/{}'
-VOLUME_SERVICE_FILE_UPLOAD = u'{}/zen-volumes/{}/v1/volumes/files/'
-VOLUME_MONITOR = u'{}/zen-volumes/{}/v1/monitor'
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
 
-PROMOTE_ASSET = u'{}/projects/api/rest/catalogs/assets/{}/promote'
+TRAINING_MODEL_HREF_PATTERN = "{}/v4/trainings/{}"
+TRAINING_MODELS_HREF_PATTERN = "{}/v4/trainings"
+REPO_MODELS_FRAMEWORKS_HREF_PATTERN = "{}/v3/models/frameworks"
+
+INSTANCE_ENDPOINT_HREF_PATTERN = "{}/v3/wml_instance"
+INSTANCE_BY_ID_ENDPOINT_HREF_PATTERN = "{}/v3/wml_instances/{}"
+TOKEN_ENDPOINT_HREF_PATTERN = "{}/v3/identity/token"
+CPD_TOKEN_ENDPOINT_HREF_PATTERN = "{}/icp4d-api/v1/authorize"
+CPD_BEDROCK_TOKEN_ENDPOINT_HREF_PATTERN = "{}/idprovider/v1/auth/identitytoken"
+CPD_VALIDATION_TOKEN_ENDPOINT_HREF_PATTERN = "{}/v1/preauth/validateAuth"
+EXPERIMENTS_HREF_PATTERN = "{}/v4/experiments"
+EXPERIMENT_HREF_PATTERN = "{}/v4/experiments/{}"
+EXPERIMENT_RUNS_HREF_PATTERN = "{}/v3/experiments/{}/runs"
+EXPERIMENT_RUN_HREF_PATTERN = "{}/v3/experiments/{}/runs/{}"
+
+PUBLISHED_MODEL_HREF_PATTERN = "{}/v4/models/{}"
+PUBLISHED_MODELS_HREF_PATTERN = "{}/v4/models"
+LEARNING_CONFIGURATION_HREF_PATTERN = (
+    "{}/v3/wml_instances/{}/published_models/{}/learning_configuration"
+)
+LEARNING_ITERATION_HREF_PATTERN = (
+    "{}/v3/wml_instances/{}/published_models/{}/learning_iterations/{}"
+)
+LEARNING_ITERATIONS_HREF_PATTERN = (
+    "{}/v3/wml_instances/{}/published_models/{}/learning_iterations"
+)
+EVALUATION_METRICS_HREF_PATTERN = (
+    "{}/v3/wml_instances/{}/published_models/{}/evaluation_metrics"
+)
+FEEDBACK_HREF_PATTERN = "{}/v3/wml_instances/{}/published_models/{}/feedback"
+
+DEPLOYMENTS_HREF_PATTERN = "{}/v4/deployments"
+DEPLOYMENT_HREF_PATTERN = "{}/v4/deployments/{}"
+DEPLOYMENT_JOB_HREF_PATTERN = "{}/v4/deployment_jobs"
+DEPLOYMENT_JOBS_HREF_PATTERN = "{}/v4/deployment_jobs/{}"
+DEPLOYMENT_ENVS_HREF_PATTERN = "{}/v4/deployments/environments"
+DEPLOYMENT_ENV_HREF_PATTERN = "{}/v4/deployments/environments/{}"
+
+MODEL_LAST_VERSION_HREF_PATTERN = "{}/v4/models/{}"
+DEFINITION_HREF_PATTERN = "{}/v3/ml_assets/training_definitions/{}"
+DEFINITIONS_HREF_PATTERN = "{}/v3/ml_assets/training_definitions"
+
+FUNCTION_HREF_PATTERN = "{}/v4/functions/{}"
+FUNCTION_LATEST_CONTENT_HREF_PATTERN = "{}/v4/functions/{}/content"
+FUNCTIONS_HREF_PATTERN = "{}/v4/functions"
+
+IAM_TOKEN_API = "{}&grant_type=urn%3Aibm%3Aparams%3Aoauth%3Agrant-type%3Aapikey"
+IAM_TOKEN_URL = "{}/oidc/token"
+PROD_SVT_URL = [
+    "https://us-south.ml.cloud.ibm.com",
+    "https://eu-gb.ml.cloud.ibm.com",
+    "https://eu-de.ml.cloud.ibm.com",
+    "https://jp-tok.ml.cloud.ibm.com",
+    "https://ibm-watson-ml.mybluemix.net",
+    "https://ibm-watson-ml.eu-gb.bluemix.net",
+    "https://private.us-south.ml.cloud.ibm.com",
+    "https://private.eu-gb.ml.cloud.ibm.com",
+    "https://private.eu-de.ml.cloud.ibm.com",
+    "https://private.jp-tok.ml.cloud.ibm.com",
+    "https://yp-qa.ml.cloud.ibm.com",
+    "https://private.yp-qa.ml.cloud.ibm.com",
+    "https://yp-cr.ml.cloud.ibm.com",
+    "https://private.yp-cr.ml.cloud.ibm.com",
+]
+
+PIPELINES_HREF_PATTERN = "{}/v4/pipelines"
+PIPELINE_HREF_PATTERN = "{}/v4/pipelines/{}"
+
+
+SPACES_HREF_PATTERN = "{}/v4/spaces"
+SPACE_HREF_PATTERN = "{}/v4/spaces/{}"
+MEMBER_HREF_PATTERN = "{}/v4/spaces/{}/members/{}"
+MEMBERS_HREF_PATTERN = "{}/v4/spaces/{}/members"
+
+SPACES_PLATFORM_HREF_PATTERN = "{}/v2/spaces"
+SPACE_PLATFORM_HREF_PATTERN = "{}/v2/spaces/{}"
+SPACES_MEMBERS_HREF_PATTERN = "{}/v2/spaces/{}/members"
+SPACES_MEMBER_HREF_PATTERN = "{}/v2/spaces/{}/members/{}"
+
+V4_INSTANCE_ID_HREF_PATTERN = "{}/ml/v4/instances/{}"
+
+API_VERSION = "/v4"
+SPACES = "/spaces"
+PIPELINES = "/pipelines"
+EXPERIMENTS = "/experiments"
+LIBRARIES = "/libraries"
+RUNTIMES = "/runtimes"
+SOFTWARE_SPEC = "/software_specifications"
+DEPLOYMENTS = "/deployments"
+ASSET = "{}/v2/assets/{}"
+ASSETS = "{}/v2/assets"
+ASSET_TYPE = "{}/v2/asset_types"
+ASSET_FILES = "{}/v2/asset_files/"
+ATTACHMENT = "{}/v2/assets/{}/attachments/{}"
+ATTACHMENT_COMPLETE = "{}/v2/assets/{}/attachments/{}/complete"
+ATTACHMENTS = "{}/v2/assets/{}/attachments"
+SEARCH_ASSETS = "{}/v2/asset_types/{}/search"
+SEARCH_MODEL_DEFINITIONS = "{}/v2/asset_types/wml_model_definition/search"
+SEARCH_DATA_ASSETS = "{}/v2/asset_types/data_asset/search"
+SEARCH_SHINY = "{}/v2/asset_types/shiny_asset/search"
+SEARCH_SCRIPT = "{}/v2/asset_types/script/search"
+GIT_BASED_PROJECT_ASSET = "{}/userfs/v2/assets/{}"
+GIT_BASED_PROJECT_ASSETS = "{}/userfs/v2/assets"
+GIT_BASED_PROJECT_ASSET_TYPE = "{}/userfs/v2/asset_types"
+GIT_BASED_PROJECT_ASSET_FILES = "{}/v2/asset_files/"
+GIT_BASED_PROJECT_ATTACHMENT = "{}/userfs/v2/assets/{}/attachments/{}"
+GIT_BASED_PROJECT_ATTACHMENT_COMPLETE = "{}/userfs/v2/assets/{}/attachments/{}/complete"
+GIT_BASED_PROJECT_ATTACHMENTS = "{}/userfs/v2/assets/{}/attachments"
+GIT_BASED_PROJECT_SEARCH_ASSETS = "{}/userfs/v2/asset_types/{}/search"
+GIT_BASED_PROJECT_SEARCH_MODEL_DEFINITIONS = (
+    "{}/userfs/v2/asset_types/wml_model_definition/search"
+)
+GIT_BASED_PROJECT_SEARCH_DATA_ASSETS = "{}/userfs/v2/asset_types/data_asset/search"
+GIT_BASED_PROJECT_SEARCH_SHINY = "{}/userfs/v2/asset_types/shiny_asset/search"
+GIT_BASED_PROJECT_SEARCH_SCRIPT = "{}/userfs/v2/asset_types/script/search"
+DATA_SOURCE_TYPE = "{}/v2/datasource_types"
+DATA_SOURCE_TYPE_BY_ID = "{}/v2/datasource_types/{}"
+CONNECTION_ASSET = "{}/v2/connections"
+CONNECTION_ASSET_SEARCH = "{}/v2/connections"
+CONNECTION_BY_ID = "{}/v2/connections/{}"
+CONNECTIONS_FILES = "{}/v2/connections/files"
+CONNECTIONS_FILE = "{}/v2/connections/files/{}"
+SOFTWARE_SPECIFICATION = "{}/v2/software_specifications/{}"
+SOFTWARE_SPECIFICATIONS = "{}/v2/software_specifications"
+HARDWARE_SPECIFICATION = "{}/v2/hardware_specifications/{}"
+HARDWARE_SPECIFICATIONS = "{}/v2/hardware_specifications"
+PACKAGE_EXTENSION = "{}/v2/package_extensions/{}"
+PACKAGE_EXTENSIONS = "{}/v2/package_extensions"
+PARAMETER_SET = "{}/v2/parameter_sets/{}"
+PARAMETER_SETS = "{}/v2/parameter_sets"
+PROJECT = "{}/v2/projects/{}"
+LIST_SOFTWARE_SPECIFICATIONS = "{}/ml/v4/list/software_specifications"
+
+V4GA_CLOUD_MIGRATION = "{}/ml/v4/repository"
+V4GA_CLOUD_MIGRATION_ID = "{}/ml/v4/repository/{}"
+
+REMOTE_TRAINING_SYSTEM = "{}/v4/remote_training_systems"
+REMOTE_TRAINING_SYSTEM_ID = "{}/v4/remote_training_systems/{}"
+
+FM_GENERATION = "{}/ml/v1/text/generation"
+FM_GENERATION_BETA = "{}/ml/v1-beta/generation/{}"  # Remove on CPD 5.0 release
+FM_GENERATION_STREAM = "{}/ml/v1/text/generation_stream"
+FM_GET_SPECS = "{}/ml/v1/foundation_model_specs"
+FM_GET_SPECS_BETA = "{}/ml/v1-beta/foundation_model_specs?version=2022-08-01"  # Remove on CPD 5.0 release
+FM_GET_CUSTOM_FOUNDATION_MODELS = "{}/ml/v4/custom_foundation_models"
+FM_GET_TASKS = "{}/ml/v1/foundation_model_tasks?limit={}"
+FM_TOKENIZE = "{}/ml/v1/text/tokenization"
+FM_TOKENIZE_BETA = "{}/ml/v1-beta/text/tokenization"  # Remove on CPD 5.0 release
+FM_EMBEDDINGS = "{}/ml/v1/text/embeddings"
+
+FM_DEPLOYMENT_GENERATION = "{}/ml/v1/deployments/{}/text/generation"
+FM_DEPLOYMENT_GENERATION_STREAM = "{}/ml/v1/deployments/{}/text/generation_stream"
+FM_DEPLOYMENT_GENERATION_BETA = (
+    "{}/ml/v1-beta/deployments/{}/generation/{}"  # Remove on CPD 5.0 release
+)
+
+PROMPTS = "{}/wx/v1-beta/prompts"
+PROMPTS_GET_ALL = "{}/v2/asset_types/wx_prompt/search"
+
+EXPORTS = "{}/v2/asset_exports"
+EXPORT_ID = "{}/v2/asset_exports/{}"
+EXPORT_ID_CONTENT = "{}/v2/asset_exports/{}/content"
+
+IMPORTS = "{}/v2/asset_imports"
+IMPORT_ID = "{}/v2/asset_imports/{}"
+
+VOLUMES = "{}/zen-data/v3/service_instances"
+VOLUME_ID = "{}/zen-data/v3/service_instances/{}"
+VOLUME_SERVICE = "{}/zen-data/v1/volumes/volume_services/{}"
+VOLUME_SERVICE_FILE_UPLOAD = "{}/zen-volumes/{}/v1/volumes/files/"
+VOLUME_MONITOR = "{}/zen-volumes/{}/v1/monitor"
+
+PROMOTE_ASSET = "{}/projects/api/rest/catalogs/assets/{}/promote"
 
 DATAPLATFORM_URLS_MAP = {
-            'https://wml-fvt.ml.test.cloud.ibm.com': 'https://dataplatform.dev.cloud.ibm.com',
-            'https://yp-qa.ml.cloud.ibm.com': 'https://dataplatform.test.cloud.ibm.com',
-            'https://private.yp-qa.ml.cloud.ibm.com': 'https://dataplatform.test.cloud.ibm.com',
-            'https://yp-cr.ml.cloud.ibm.com': 'https://dataplatform.test.cloud.ibm.com',
-            'https://private.yp-cr.ml.cloud.ibm.com': 'https://dataplatform.test.cloud.ibm.com',
-            'https://jp-tok.ml.cloud.ibm.com': 'https://jp-tok.dataplatform.cloud.ibm.com',
-            'https://eu-gb.ml.cloud.ibm.com': 'https://eu-gb.dataplatform.cloud.ibm.com',
-            'https://eu-de.ml.cloud.ibm.com': 'https://eu-de.dataplatform.cloud.ibm.com',
-            'https://us-south.ml.cloud.ibm.com': 'https://dataplatform.cloud.ibm.com'
-        }
-
-WKC_MODEL_REGISTER = u"{}/v1/aigov/model_inventory/models/{}/model_entry"
-WKC_MODEL_LIST_FROM_CATALOG = u"{}/v1/aigov/model_inventory/{}/model_entries"
-WKC_MODEL_LIST_ALL = u"{}/v1/aigov/model_inventory/model_entries"
-TASK_CREDENTIALS = u"{}/v1/task_credentials/{}"
-TASK_CREDENTIALS_ALL = u"{}/v1/task_credentials"
+    "https://wml-fvt.ml.test.cloud.ibm.com": "https://dataplatform.dev.cloud.ibm.com",
+    "https://yp-qa.ml.cloud.ibm.com": "https://dataplatform.test.cloud.ibm.com",
+    "https://private.yp-qa.ml.cloud.ibm.com": "https://dataplatform.test.cloud.ibm.com",
+    "https://yp-cr.ml.cloud.ibm.com": "https://dataplatform.test.cloud.ibm.com",
+    "https://private.yp-cr.ml.cloud.ibm.com": "https://dataplatform.test.cloud.ibm.com",
+    "https://jp-tok.ml.cloud.ibm.com": "https://jp-tok.dataplatform.cloud.ibm.com",
+    "https://eu-gb.ml.cloud.ibm.com": "https://eu-gb.dataplatform.cloud.ibm.com",
+    "https://eu-de.ml.cloud.ibm.com": "https://eu-de.dataplatform.cloud.ibm.com",
+    "https://us-south.ml.cloud.ibm.com": "https://dataplatform.cloud.ibm.com",
+}
+
+WKC_MODEL_REGISTER = "{}/v1/aigov/model_inventory/models/{}/model_entry"
+WKC_MODEL_LIST_FROM_CATALOG = "{}/v1/aigov/model_inventory/{}/model_entries"
+WKC_MODEL_LIST_ALL = "{}/v1/aigov/model_inventory/model_entries"
+TASK_CREDENTIALS = "{}/v1/task_credentials/{}"
+TASK_CREDENTIALS_ALL = "{}/v1/task_credentials"
+
 
-def is_url(s):
-    res = re.match('https?:\/\/.+', s)
+def is_url(s: str) -> bool:
+    res = re.match("https?:\/\/.+", s)
     return res is not None
 
 
-def is_uid(s):
-    res = re.match('[a-z0-9\-]{36}', s)
+def is_id(s: str) -> bool:
+    res = re.match("[a-z0-9\-]{36}", s)
     return res is not None
 
 
 class HrefDefinitions:
-    def __init__(self, client, cloud_platform_spaces=False, platform_url=None, cams_url=None,
-                 cp4d_platform_spaces=False):
-        self._credentials = client.wml_credentials
+    def __init__(
+        self,
+        client: APIClient,
+        cloud_platform_spaces: bool = False,
+        platform_url: str | None = None,
+        cp4d_platform_spaces: bool = False,
+    ):
+        self._credentials = client.credentials
         self._client = client
         self.cloud_platform_spaces = cloud_platform_spaces
         self.cp4d_platform_spaces = cp4d_platform_spaces
         self.platform_url = platform_url
-        self.cams_url = cams_url
-
-        if self.cloud_platform_spaces or self.cp4d_platform_spaces:
-            self.prepend = '/ml'
-        else:
-            self.prepend = ''
+        self.prepend = "/ml"
 
-    def _is_git_based_project(self):
+    def _is_git_based_project(self) -> bool:
         return self._client.project_type == "local_git_storage"
 
-    def _get_platform_url_if_exists(self):
-        return self.platform_url if self.platform_url else self._credentials['url']
-
-    def _get_cams_url_if_exists(self):
-        return self.cams_url if self.cams_url else self._credentials['url']
-
-    def get_training_href(self, model_uid):
-        return TRAINING_MODEL_HREF_PATTERN.format(self._credentials['url'] + self.prepend, model_uid)
-
-    def get_trainings_href(self):
-        return TRAINING_MODELS_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_repo_models_frameworks_href(self):
-        return REPO_MODELS_FRAMEWORKS_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_instance_endpoint_href(self):
-        return INSTANCE_ENDPOINT_HREF_PATTERN.format(self._credentials['url'])
-
-    def get_instance_by_id_endpoint_href(self):
-        return INSTANCE_BY_ID_ENDPOINT_HREF_PATTERN.format(self._credentials['url'], self._credentials['instance_id'])
-
-    def get_token_endpoint_href(self):
-        return TOKEN_ENDPOINT_HREF_PATTERN.format(self._credentials['url'])
-
-    def get_cpd_token_endpoint_href(self):
-        return CPD_TOKEN_ENDPOINT_HREF_PATTERN.format(self._credentials['url'].replace(':31002', ':31843'))
-
-    def get_cpd_bedrock_token_endpoint_href(self):
-        return CPD_BEDROCK_TOKEN_ENDPOINT_HREF_PATTERN.format(self._credentials['bedrock_url'])
-
-    def get_cpd_validation_token_endpoint_href(self):
-        return CPD_VALIDATION_TOKEN_ENDPOINT_HREF_PATTERN.format(self._credentials['url'])
-
-    def get_published_model_href(self, model_uid):
-        return PUBLISHED_MODEL_HREF_PATTERN.format(self._credentials['url'] + self.prepend, model_uid)
-
-    def get_published_models_href(self):
-        return PUBLISHED_MODELS_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_learning_configuration_href(self, model_uid):
-        return LEARNING_CONFIGURATION_HREF_PATTERN.format(self._credentials['url'], self._credentials['instance_id'], model_uid)
-
-    def get_learning_iterations_href(self, model_uid):
-        return LEARNING_ITERATIONS_HREF_PATTERN.format(self._credentials['url'], self._credentials['instance_id'], model_uid)
-
-    def get_learning_iteration_href(self, model_uid, iteration_uid):
-        return LEARNING_ITERATION_HREF_PATTERN.format(self._credentials['url'], self._credentials['instance_id'], model_uid, iteration_uid)
-
-    def get_evaluation_metrics_href(self, model_uid):
-        return EVALUATION_METRICS_HREF_PATTERN.format(self._credentials['url'], self._credentials['instance_id'], model_uid)
-
-    def get_feedback_href(self, model_uid):
-        return FEEDBACK_HREF_PATTERN.format(self._credentials['url'], self._credentials['instance_id'], model_uid)
-
-    def get_model_last_version_href(self, artifact_uid):
-        return MODEL_LAST_VERSION_HREF_PATTERN.format(self._credentials['url'] + self.prepend, artifact_uid)
-
-    def get_deployments_href(self):
-        return DEPLOYMENTS_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_experiments_href(self):
-        return EXPERIMENTS_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_experiment_href(self, experiment_uid):
-        return EXPERIMENT_HREF_PATTERN.format(self._credentials['url'] + self.prepend, experiment_uid)
-
-    def get_experiment_runs_href(self, experiment_uid):
-        return EXPERIMENT_RUNS_HREF_PATTERN.format(self._credentials['url'], experiment_uid)
-
-    def get_experiment_run_href(self, experiment_uid, experiment_run_uid):
-        return EXPERIMENT_RUN_HREF_PATTERN.format(self._credentials['url'], experiment_uid, experiment_run_uid)
-
-    def get_deployment_href(self, deployment_uid):
-        return DEPLOYMENT_HREF_PATTERN.format(self._credentials['url'] + self.prepend, deployment_uid)
-
-    def get_definition_href(self, definition_uid):
-        return DEFINITION_HREF_PATTERN.format(self._credentials['url'], definition_uid)
-
-    def get_definitions_href(self):
-        return DEFINITIONS_HREF_PATTERN.format(self._credentials['url'])
-
-    def get_function_href(self, ai_function_uid):
-        return FUNCTION_HREF_PATTERN.format(self._credentials['url'] + self.prepend, ai_function_uid)
-
-    def get_function_latest_revision_content_href(self, ai_function_uid):
-        return FUNCTION_LATEST_CONTENT_HREF_PATTERN.format(self._credentials['url'], ai_function_uid)
+    def _get_platform_url_if_exists(self) -> str:
+        return self.platform_url if self.platform_url else self._credentials.url
 
-    def get_functions_href(self):
-        return FUNCTIONS_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
+    def get_training_href(self, model_id: str) -> str:
+        return TRAINING_MODEL_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, model_id
+        )
+
+    def get_trainings_href(self) -> str:
+        return TRAINING_MODELS_HREF_PATTERN.format(self._credentials.url + self.prepend)
+
+    def get_repo_models_frameworks_href(self) -> str:
+        return REPO_MODELS_FRAMEWORKS_HREF_PATTERN.format(
+            self._credentials.url + self.prepend
+        )
+
+    def get_instance_endpoint_href(self) -> str:
+        return INSTANCE_ENDPOINT_HREF_PATTERN.format(self._credentials.url)
+
+    def get_instance_by_id_endpoint_href(self) -> str:
+        return INSTANCE_BY_ID_ENDPOINT_HREF_PATTERN.format(
+            self._credentials.url, self._credentials.instance_id
+        )
+
+    def get_token_endpoint_href(self) -> str:
+        return TOKEN_ENDPOINT_HREF_PATTERN.format(self._credentials.url)
+
+    def get_cpd_token_endpoint_href(self) -> str:
+        return CPD_TOKEN_ENDPOINT_HREF_PATTERN.format(
+            self._credentials.url.replace(":31002", ":31843")
+        )
+
+    def get_cpd_bedrock_token_endpoint_href(self) -> str:
+        return CPD_BEDROCK_TOKEN_ENDPOINT_HREF_PATTERN.format(
+            self._credentials.bedrock_url
+        )
+
+    def get_cpd_validation_token_endpoint_href(self) -> str:
+        return CPD_VALIDATION_TOKEN_ENDPOINT_HREF_PATTERN.format(self._credentials.url)
+
+    def get_published_model_href(self, model_id: str) -> str:
+        return PUBLISHED_MODEL_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, model_id
+        )
+
+    def get_published_models_href(self) -> str:
+        return PUBLISHED_MODELS_HREF_PATTERN.format(
+            self._credentials.url + self.prepend
+        )
+
+    def get_learning_configuration_href(self, model_id: str) -> str:
+        return LEARNING_CONFIGURATION_HREF_PATTERN.format(
+            self._credentials.url, self._credentials.instance_id, model_id
+        )
+
+    def get_learning_iterations_href(self, model_id: str) -> str:
+        return LEARNING_ITERATIONS_HREF_PATTERN.format(
+            self._credentials.url, self._credentials.instance_id, model_id
+        )
+
+    def get_learning_iteration_href(self, model_id: str, iteration_id: str) -> str:
+        return LEARNING_ITERATION_HREF_PATTERN.format(
+            self._credentials.url,
+            self._credentials.instance_id,
+            model_id,
+            iteration_id,
+        )
+
+    def get_evaluation_metrics_href(self, model_id: str) -> str:
+        return EVALUATION_METRICS_HREF_PATTERN.format(
+            self._credentials.url, self._credentials.instance_id, model_id
+        )
+
+    def get_feedback_href(self, model_id: str) -> str:
+        return FEEDBACK_HREF_PATTERN.format(
+            self._credentials.url, self._credentials.instance_id, model_id
+        )
+
+    def get_model_last_version_href(self, artifact_id: str) -> str:
+        return MODEL_LAST_VERSION_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, artifact_id
+        )
+
+    def get_deployments_href(self) -> str:
+        return DEPLOYMENTS_HREF_PATTERN.format(self._credentials.url + self.prepend)
+
+    def get_experiments_href(self) -> str:
+        return EXPERIMENTS_HREF_PATTERN.format(self._credentials.url + self.prepend)
+
+    def get_experiment_href(self, experiment_id: str) -> str:
+        return EXPERIMENT_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, experiment_id
+        )
+
+    def get_experiment_runs_href(self, experiment_id: str) -> str:
+        return EXPERIMENT_RUNS_HREF_PATTERN.format(self._credentials.url, experiment_id)
+
+    def get_experiment_run_href(
+        self, experiment_id: str, experiment_run_id: str
+    ) -> str:
+        return EXPERIMENT_RUN_HREF_PATTERN.format(
+            self._credentials.url, experiment_id, experiment_run_id
+        )
+
+    def get_deployment_href(self, deployment_id: str) -> str:
+        return DEPLOYMENT_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, deployment_id
+        )
+
+    def get_definition_href(self, definition_id: str) -> str:
+        return DEFINITION_HREF_PATTERN.format(self._credentials.url, definition_id)
+
+    def get_definitions_href(self) -> str:
+        return DEFINITIONS_HREF_PATTERN.format(self._credentials.url)
+
+    def get_function_href(self, ai_function_id: str) -> str:
+        return FUNCTION_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, ai_function_id
+        )
+
+    def get_function_latest_revision_content_href(self, ai_function_id: str) -> str:
+        return FUNCTION_LATEST_CONTENT_HREF_PATTERN.format(
+            self._credentials.url, ai_function_id
+        )
+
+    def get_functions_href(self) -> str:
+        return FUNCTIONS_HREF_PATTERN.format(self._credentials.url + self.prepend)
+
+    def get_pipeline_href(self, pipeline_id: str) -> str:
+        return PIPELINE_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, pipeline_id
+        )
+
+    def get_pipelines_href(self) -> str:
+        return PIPELINES_HREF_PATTERN.format(self._credentials.url + self.prepend)
+
+    def get_space_href(self, spaces_id: str) -> str:
+        return SPACE_HREF_PATTERN.format(self._credentials.url, spaces_id)
+
+    def get_spaces_href(self) -> str:
+        return SPACES_HREF_PATTERN.format(self._credentials.url)
+
+    def get_platform_space_href(self, spaces_id: str) -> str:
+        return SPACE_PLATFORM_HREF_PATTERN.format(
+            self._get_platform_url_if_exists(), spaces_id
+        )
 
-    def get_pipeline_href(self, pipeline_uid):
-        return PIPELINE_HREF_PATTERN.format(self._credentials['url'] + self.prepend, pipeline_uid)
-
-    def get_pipelines_href(self):
-        return PIPELINES_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_space_href(self, spaces_uid):
-        return SPACE_HREF_PATTERN.format(self._credentials['url'], spaces_uid)
-
-    def get_spaces_href(self):
-        return SPACES_HREF_PATTERN.format(self._credentials['url'])
-
-    def get_platform_space_href(self, spaces_id):
-        return SPACE_PLATFORM_HREF_PATTERN.format(self._get_platform_url_if_exists(), spaces_id)
-
-    def get_platform_spaces_href(self):
+    def get_platform_spaces_href(self) -> str:
         return SPACES_PLATFORM_HREF_PATTERN.format(self._get_platform_url_if_exists())
 
-    def get_platform_spaces_member_href(self, spaces_id, member_id):
-        return SPACES_MEMBER_HREF_PATTERN.format(self._get_platform_url_if_exists(), spaces_id, member_id)
-
-    def get_platform_spaces_members_href(self,spaces_id):
-        return SPACES_MEMBERS_HREF_PATTERN.format(self._get_platform_url_if_exists(), spaces_id)
-
-    def get_v4_instance_id_href(self):
-        return V4_INSTANCE_ID_HREF_PATTERN.format(self._credentials['url'],
-                                                  self._credentials['instance_id'])
-
-    def get_async_deployment_job_href(self):
-        return DEPLOYMENT_JOB_HREF_PATTERN.format(self._credentials['url'] + self.prepend)
-
-    def get_async_deployment_jobs_href(self, job_uid):
-        return DEPLOYMENT_JOBS_HREF_PATTERN.format(self._credentials['url'] + self.prepend, job_uid)
-
-    def get_iam_token_api(self):
-        return IAM_TOKEN_API.format(self._credentials['apikey'])
-
-    def get_iam_token_url(self):
-        if self._credentials['url'] in PROD_SVT_URL:
-            return IAM_TOKEN_URL.format('https://iam.cloud.ibm.com')
+    def get_platform_spaces_member_href(self, spaces_id: str, member_id: str) -> str:
+        return SPACES_MEMBER_HREF_PATTERN.format(
+            self._get_platform_url_if_exists(), spaces_id, member_id
+        )
+
+    def get_platform_spaces_members_href(self, spaces_id: str) -> str:
+        return SPACES_MEMBERS_HREF_PATTERN.format(
+            self._get_platform_url_if_exists(), spaces_id
+        )
+
+    def get_v4_instance_id_href(self, instance_id: str) -> str:
+        return V4_INSTANCE_ID_HREF_PATTERN.format(
+            self._credentials.url, instance_id
+        )
+
+    def get_async_deployment_job_href(self) -> str:
+        return DEPLOYMENT_JOB_HREF_PATTERN.format(self._credentials.url + self.prepend)
+
+    def get_async_deployment_jobs_href(self, job_id: str) -> str:
+        return DEPLOYMENT_JOBS_HREF_PATTERN.format(
+            self._credentials.url + self.prepend, job_id
+        )
+
+    def get_iam_token_api(self) -> str:
+        return IAM_TOKEN_API.format(self._credentials.api_key)
+
+    def get_iam_token_url(self) -> str:
+        if self._credentials.url in PROD_SVT_URL:
+            return IAM_TOKEN_URL.format("https://iam.cloud.ibm.com")
         else:
-            return IAM_TOKEN_URL.format('https://iam.test.cloud.ibm.com')
-
-    def get_member_href(self, spaces_uid,member_id):
-        return MEMBER_HREF_PATTERN.format(self._credentials['url'], spaces_uid,member_id)
-
-    def get_members_href(self,spaces_uid):
-        return MEMBERS_HREF_PATTERN.format(self._credentials['url'],spaces_uid)
-
-    def get_data_asset_href(self,asset_id):
-        return (ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET)\
-            .format(self._get_cams_url_if_exists(), asset_id)
-
-    def get_data_assets_href(self):
-        return (ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS)\
-            .format(self._get_cams_url_if_exists())
-
-    def get_assets_href(self):
-        return (ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS)\
-            .format(self._get_cams_url_if_exists())
+            return IAM_TOKEN_URL.format("https://iam.test.cloud.ibm.com")
 
-    def get_asset_href(self,asset_id):
-        return (ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET)\
-            .format(self._get_cams_url_if_exists(), asset_id)
+    def get_member_href(self, spaces_id: str, member_id: str) -> str:
+        return MEMBER_HREF_PATTERN.format(self._credentials.url, spaces_id, member_id)
 
-    def get_base_asset_href(self,asset_id):
-        return (ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET).format('', asset_id)
+    def get_members_href(self, spaces_id: str) -> str:
+        return MEMBERS_HREF_PATTERN.format(self._credentials.url, spaces_id)
 
-    def get_base_assets_href(self):
-        return (ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS).format('')
-
-    def get_base_asset_with_type_href(self,asset_type, asset_id):
-        return (ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET).format('', asset_type) + '/' + asset_id
-
-    def get_attachment_href(self,asset_id,attachment_id):
-        return (ATTACHMENT if not self._is_git_based_project() else GIT_BASED_PROJECT_ATTACHMENT)\
-            .format(self._get_cams_url_if_exists(), asset_id, attachment_id)
-
-    def get_attachments_href(self, asset_id):
-        return (ATTACHMENTS if not self._is_git_based_project() else GIT_BASED_PROJECT_ATTACHMENTS)\
-            .format(self._get_cams_url_if_exists(), asset_id)
-
-    def get_attachment_complete_href(self,asset_id,attachment_id):
-        return (ATTACHMENT_COMPLETE if not self._is_git_based_project() else GIT_BASED_PROJECT_ATTACHMENT_COMPLETE)\
-            .format(self._get_cams_url_if_exists(), asset_id, attachment_id)
-
-    def get_search_asset_href(self):
-        return (SEARCH_DATA_ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_SEARCH_DATA_ASSETS)\
-            .format(self._get_cams_url_if_exists())
-
-    def get_search_shiny_href(self):
-        return (SEARCH_SHINY if not self._is_git_based_project() else GIT_BASED_PROJECT_SEARCH_SHINY)\
-            .format(self._get_cams_url_if_exists())
-
-    def get_search_script_href(self):
-        return (SEARCH_SCRIPT if not self._is_git_based_project() else GIT_BASED_PROJECT_SEARCH_SCRIPT)\
-            .format(self._get_cams_url_if_exists())
-
-    def get_model_definition_assets_href(self):
-        return (ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS)\
-            .format(self._get_cams_url_if_exists())
-
-    def get_model_definition_search_asset_href(self):
-        return (SEARCH_MODEL_DEFINITIONS if not self._is_git_based_project() else GIT_BASED_PROJECT_SEARCH_MODEL_DEFINITIONS)\
-            .format(self._get_cams_url_if_exists())
+    def get_data_asset_href(self, asset_id: str) -> str:
+        return (
+            ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET
+        ).format(self._get_platform_url_if_exists(), asset_id)
+
+    def get_data_assets_href(self) -> str:
+        return (
+            ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS
+        ).format(self._get_platform_url_if_exists())
+
+    def get_assets_href(self) -> str:
+        return (
+            ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS
+        ).format(self._get_platform_url_if_exists())
+
+    def get_asset_href(self, asset_id: str) -> str:
+        return (
+            ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET
+        ).format(self._get_platform_url_if_exists(), asset_id)
+
+    def get_base_asset_href(self, asset_id: str) -> str:
+        return (
+            ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET
+        ).format("", asset_id)
+
+    def get_base_assets_href(self) -> str:
+        return (
+            ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS
+        ).format("")
+
+    def get_base_asset_with_type_href(self, asset_type: str, asset_id: str) -> str:
+        return (
+            (
+                ASSET if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET
+            ).format("", asset_type)
+            + "/"
+            + asset_id
+        )
+
+    def get_attachment_href(self, asset_id: str, attachment_id: str) -> str:
+        return (
+            ATTACHMENT
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_ATTACHMENT
+        ).format(self._get_platform_url_if_exists(), asset_id, attachment_id)
+
+    def get_attachments_href(self, asset_id: str) -> str:
+        return (
+            ATTACHMENTS
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_ATTACHMENTS
+        ).format(self._get_platform_url_if_exists(), asset_id)
+
+    def get_attachment_complete_href(self, asset_id: str, attachment_id: str) -> str:
+        return (
+            ATTACHMENT_COMPLETE
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_ATTACHMENT_COMPLETE
+        ).format(self._get_platform_url_if_exists(), asset_id, attachment_id)
+
+    def get_search_asset_href(self) -> str:
+        return (
+            SEARCH_DATA_ASSETS
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_SEARCH_DATA_ASSETS
+        ).format(self._get_platform_url_if_exists())
+
+    def get_search_shiny_href(self) -> str:
+        return (
+            SEARCH_SHINY
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_SEARCH_SHINY
+        ).format(self._get_platform_url_if_exists())
+
+    def get_search_script_href(self) -> str:
+        return (
+            SEARCH_SCRIPT
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_SEARCH_SCRIPT
+        ).format(self._get_platform_url_if_exists())
+
+    def get_model_definition_assets_href(self) -> str:
+        return (
+            ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSETS
+        ).format(self._get_platform_url_if_exists())
+
+    def get_model_definition_search_asset_href(self) -> str:
+        return (
+            SEARCH_MODEL_DEFINITIONS
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_SEARCH_MODEL_DEFINITIONS
+        ).format(self._get_platform_url_if_exists())
 
     # note: leave `wsd` in name since APIClient is still wrapped
-    def get_wsd_model_attachment_href(self):
-        return (ASSET_FILES if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET_FILES)\
-            .format(self._credentials['url'])
-
-    def get_asset_search_href(self, asset_type):
-        return (SEARCH_ASSETS if not self._is_git_based_project() else GIT_BASED_PROJECT_SEARCH_ASSETS)\
-            .format(self._get_cams_url_if_exists(), asset_type)
-
-    def get_wsd_asset_type_href(self):
-        return (ASSET_TYPE if not self._is_git_based_project() else GIT_BASED_PROJECT_ASSET_TYPE)\
-            .format(self._credentials['url'])
+    def get_wsd_model_attachment_href(self) -> str:
+        return (
+            ASSET_FILES
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_ASSET_FILES
+        ).format(self._credentials.url)
+
+    def get_asset_search_href(self, asset_type: str) -> str:
+        return (
+            SEARCH_ASSETS
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_SEARCH_ASSETS
+        ).format(self._get_platform_url_if_exists(), asset_type)
+
+    def get_wsd_asset_type_href(self) -> str:
+        return (
+            ASSET_TYPE
+            if not self._is_git_based_project()
+            else GIT_BASED_PROJECT_ASSET_TYPE
+        ).format(self._credentials.url)
 
-    def get_connections_href(self):
+    def get_connections_href(self) -> str:
         return CONNECTION_ASSET.format(self._get_platform_url_if_exists())
 
-    def get_connection_by_id_href(self, connection_id):
-        return CONNECTION_BY_ID.format(self._get_platform_url_if_exists(), connection_id)
+    def get_connection_by_id_href(self, connection_id: str) -> str:
+        return CONNECTION_BY_ID.format(
+            self._get_platform_url_if_exists(), connection_id
+        )
 
-    def get_connections_files_href(self):
+    def get_connections_files_href(self) -> str:
         return CONNECTIONS_FILES.format(self._get_platform_url_if_exists())
 
-    def get_connections_file_href(self, file_name):
+    def get_connections_file_href(self, file_name: str) -> str:
         return CONNECTIONS_FILE.format(self._get_platform_url_if_exists(), file_name)
 
-    def get_connection_data_types_href(self):
+    def get_connection_data_types_href(self) -> str:
         return DATA_SOURCE_TYPE.format(self._get_platform_url_if_exists())
 
-    def get_connection_data_type_by_id_href(self, datasource_type_id):
-        return DATA_SOURCE_TYPE_BY_ID.format(self._get_platform_url_if_exists(), datasource_type_id)
-
-    def get_sw_spec_href(self, sw_spec_id):
-        return SOFTWARE_SPECIFICATION.format(self._get_platform_url_if_exists(), sw_spec_id)
+    def get_connection_data_type_by_id_href(self, datasource_type_id: str) -> str:
+        return DATA_SOURCE_TYPE_BY_ID.format(
+            self._get_platform_url_if_exists(), datasource_type_id
+        )
+
+    def get_sw_spec_href(self, sw_spec_id: str) -> str:
+        return SOFTWARE_SPECIFICATION.format(
+            self._get_platform_url_if_exists(), sw_spec_id
+        )
 
-    def get_sw_specs_href(self):
+    def get_sw_specs_href(self) -> str:
         return SOFTWARE_SPECIFICATIONS.format(self._get_platform_url_if_exists())
 
-    def get_hw_spec_href(self, hw_spec_id):
-        return HARDWARE_SPECIFICATION.format(self._get_platform_url_if_exists(), hw_spec_id)
+    def get_hw_spec_href(self, hw_spec_id: str) -> str:
+        return HARDWARE_SPECIFICATION.format(
+            self._get_platform_url_if_exists(), hw_spec_id
+        )
 
-    def get_hw_specs_href(self):
+    def get_hw_specs_href(self) -> str:
         return HARDWARE_SPECIFICATIONS.format(self._get_platform_url_if_exists())
 
-    def get_pkg_extn_href(self, pkg_extn_id):
+    def get_pkg_extn_href(self, pkg_extn_id: str) -> str:
         return PACKAGE_EXTENSION.format(self._get_platform_url_if_exists(), pkg_extn_id)
 
-    def get_pkg_extns_href(self):
+    def get_pkg_extns_href(self) -> str:
         return PACKAGE_EXTENSIONS.format(self._get_platform_url_if_exists())
 
-    def get_project_href(self, project_id):
+    def get_project_href(self, project_id: str) -> str:
         return PROJECT.format(self._get_platform_url_if_exists(), project_id)
 
-    def get_software_specifications_list_href(self):
-        return LIST_SOFTWARE_SPECIFICATIONS.format(self._credentials['url'])
+    def get_software_specifications_list_href(self) -> str:
+        return LIST_SOFTWARE_SPECIFICATIONS.format(self._credentials.url)
 
-    def v4ga_cloud_migration_href(self):
-        return V4GA_CLOUD_MIGRATION.format(self._credentials['url'])
+    def v4ga_cloud_migration_href(self) -> str:
+        return V4GA_CLOUD_MIGRATION.format(self._credentials.url)
 
-    def v4ga_cloud_migration_id_href(self, migration_id):
-        return V4GA_CLOUD_MIGRATION_ID.format(self._credentials['url'], migration_id)
+    def v4ga_cloud_migration_id_href(self, migration_id: str) -> str:
+        return V4GA_CLOUD_MIGRATION_ID.format(self._credentials.url, migration_id)
 
-    def exports_href(self):
+    def exports_href(self) -> str:
         return EXPORTS.format(self._get_platform_url_if_exists())
 
-    def export_href(self, export_id):
+    def export_href(self, export_id: str) -> str:
         return EXPORT_ID.format(self._get_platform_url_if_exists(), export_id)
 
-    def export_content_href(self, export_id):
+    def export_content_href(self, export_id: str) -> str:
         return EXPORT_ID_CONTENT.format(self._get_platform_url_if_exists(), export_id)
 
-    def imports_href(self):
+    def imports_href(self) -> str:
         return IMPORTS.format(self._get_platform_url_if_exists())
 
-    def import_href(self, export_id):
+    def import_href(self, export_id: str) -> str:
         return IMPORT_ID.format(self._get_platform_url_if_exists(), export_id)
 
-    def remote_training_systems_href(self):
-        return REMOTE_TRAINING_SYSTEM.format(self._credentials['url'] + self.prepend)
+    def remote_training_systems_href(self) -> str:
+        return REMOTE_TRAINING_SYSTEM.format(self._credentials.url + self.prepend)
 
-    def remote_training_system_href(self, remote_training_systems_id):
-        return REMOTE_TRAINING_SYSTEM_ID.format(self._credentials['url'] + self.prepend, remote_training_systems_id)
+    def remote_training_system_href(self, remote_training_systems_id: str) -> str:
+        return REMOTE_TRAINING_SYSTEM_ID.format(
+            self._credentials.url + self.prepend, remote_training_systems_id
+        )
 
-    def volumes_href(self):
-        return VOLUMES.format(self._credentials['url'])
+    def volumes_href(self) -> str:
+        return VOLUMES.format(self._credentials.url)
 
-    def volume_href(self,volume_id):
-        return VOLUME_ID.format(self._credentials['url'], volume_id)
+    def volume_href(self, volume_id: str) -> str:
+        return VOLUME_ID.format(self._credentials.url, volume_id)
 
-    def volume_service_href(self,volume_name):
-        return VOLUME_SERVICE.format(self._credentials['url'], volume_name)
+    def volume_service_href(self, volume_name: str) -> str:
+        return VOLUME_SERVICE.format(self._credentials.url, volume_name)
 
-    def volume_upload_href(self, volume_name):
-        return VOLUME_SERVICE_FILE_UPLOAD.format(self._credentials['url'], volume_name)
+    def volume_upload_href(self, volume_name: str) -> str:
+        return VOLUME_SERVICE_FILE_UPLOAD.format(self._credentials.url, volume_name)
 
-    def volume_monitor_href(self, volume_name):
-        return VOLUME_MONITOR.format(self._credentials['url'], volume_name)
+    def volume_monitor_href(self, volume_name: str) -> str:
+        return VOLUME_MONITOR.format(self._credentials.url, volume_name)
 
-    def promote_asset_href(self, asset_id):
+    def promote_asset_href(self, asset_id: str) -> str:
         if self.cloud_platform_spaces:
-            data_platform_url = DATAPLATFORM_URLS_MAP[self._credentials['url']]
+            data_platform_url = DATAPLATFORM_URLS_MAP[self._credentials.url]
             return PROMOTE_ASSET.format(data_platform_url, asset_id)
         else:
-            promote_href = PROMOTE_ASSET.format(self._credentials['url'], asset_id)
+            promote_href = PROMOTE_ASSET.format(self._credentials.url, asset_id)
             try:
                 # note: For CPD older than 4.0 we need to roll back to older endpoint.
-                if float(self._credentials.get("version")) < 4.0:
+                if float(self._credentials.version) < 4.0:
                     promote_href = promote_href.replace("/projects", "")
                 # --- end note
             finally:
                 return promote_href
 
-    def get_wkc_model_register_href(self, model_id) -> str:
+    def get_wkc_model_register_href(self, model_id: str) -> str:
         return WKC_MODEL_REGISTER.format(self._get_platform_url_if_exists(), model_id)
 
-    def get_wkc_model_list_from_catalog_href(self, catalog_id) -> str:
-        return WKC_MODEL_LIST_FROM_CATALOG.format(self._get_platform_url_if_exists(), catalog_id)
+    def get_wkc_model_list_from_catalog_href(self, catalog_id: str) -> str:
+        return WKC_MODEL_LIST_FROM_CATALOG.format(
+            self._get_platform_url_if_exists(), catalog_id
+        )
 
     def get_wkc_model_list_all_href(self) -> str:
         return WKC_MODEL_LIST_ALL.format(self._get_platform_url_if_exists())
 
-    def get_wkc_model_delete_href(self, asset_id) -> str:
+    def get_wkc_model_delete_href(self, asset_id: str) -> str:
         return WKC_MODEL_REGISTER.format(self._get_platform_url_if_exists(), asset_id)
 
-    def get_task_credentials_href(self, task_credentials_uid) -> str:
-        return TASK_CREDENTIALS.format(self._get_platform_url_if_exists(), task_credentials_uid)
+    def get_task_credentials_href(self, task_credentials_id: str) -> str:
+        return TASK_CREDENTIALS.format(
+            self._get_platform_url_if_exists(), task_credentials_id
+        )
 
     def get_task_credentials_all_href(self) -> str:
         return TASK_CREDENTIALS_ALL.format(self._get_platform_url_if_exists())
 
-    def get_fm_specifications_href(self, limit):
+    def get_fm_specifications_href(self) -> str:
         if self._client._use_fm_ga_api:
-            return FM_GET_SPECS.format(self._credentials['url'], limit)
+            return FM_GET_SPECS.format(self._credentials.url)
         else:
-            return FM_GET_SPECS_BETA.format(self._credentials['url'], limit)  # Remove on CPD 5.0 release
+            return FM_GET_SPECS_BETA.format(
+                self._credentials.url
+            )  # Remove on CPD 5.0 release
 
-    def get_fm_tasks_href(self, limit):
-        return FM_GET_TASKS.format(self._credentials['url'], limit)
+    def get_fm_custom_foundation_models_href(self) -> str:
+        return FM_GET_CUSTOM_FOUNDATION_MODELS.format(self._credentials.url)
 
-    def get_fm_generation_href(self, item=None):
+    def get_fm_tasks_href(self, limit: str) -> str:
+        return FM_GET_TASKS.format(self._credentials.url, limit)
+
+    def get_fm_generation_href(self, item: str | None = None) -> str:
         if self._client._use_fm_ga_api:
-            return FM_GENERATION.format(self._credentials['url'])
+            return FM_GENERATION.format(self._credentials.url)
         else:
-            return FM_GENERATION_BETA.format(self._credentials['url'], item)  # Remove on CPD 5.0 release
+            return FM_GENERATION_BETA.format(
+                self._credentials.url, item
+            )  # Remove on CPD 5.0 release
 
-    def get_fm_generation_stream_href(self):
-        return FM_GENERATION_STREAM.format(self._credentials['url'])
+    def get_fm_generation_stream_href(self) -> str:
+        return FM_GENERATION_STREAM.format(self._credentials.url)
 
-    def get_fm_tokenize_href(self):
+    def get_fm_tokenize_href(self) -> str:
         if self._client._use_fm_ga_api:
-            return FM_TOKENIZE.format(self._credentials['url'])
+            return FM_TOKENIZE.format(self._credentials.url)
         else:
-            return FM_TOKENIZE_BETA.format(self._credentials['url'])  # Remove on CPD 5.0 release
-
-    def get_fm_deployment_generation_href(self, deployment_id, item=None):
+            return FM_TOKENIZE_BETA.format(
+                self._credentials.url
+            )  # Remove on CPD 5.0 release
+
+    def get_fm_deployment_generation_href(
+        self, deployment_id: str, item: str | None = None
+    ) -> str:
         if self._client._use_fm_ga_api:
-            return FM_DEPLOYMENT_GENERATION.format(self._credentials['url'], deployment_id)
+            return FM_DEPLOYMENT_GENERATION.format(self._credentials.url, deployment_id)
         else:
-            return FM_DEPLOYMENT_GENERATION_BETA.format(self._credentials['url'], deployment_id, item)  # Remove on CPD 5.0 release
+            return FM_DEPLOYMENT_GENERATION_BETA.format(
+                self._credentials.url, deployment_id, item
+            )  # Remove on CPD 5.0 release
+
+    def get_fm_deployment_generation_stream_href(self, deployment_id: str) -> str:
+        return FM_DEPLOYMENT_GENERATION_STREAM.format(
+            self._credentials.url, deployment_id
+        )
 
-    def get_fm_deployment_generation_stream_href(self, deployment_id):
-        return FM_DEPLOYMENT_GENERATION_STREAM.format(self._credentials['url'], deployment_id)
-
-    def get_prompts_href(self):
+    def get_prompts_href(self) -> str:
         return PROMPTS.format(self._get_platform_url_if_exists())
-    
-    def get_prompts_all_href(self):
-        return PROMPTS_GET_ALL.format(self._get_platform_url_if_exists())
 
-    # def get_envs_href(self):
-    #     return DEPLOYMENT_ENVS_HREF_PATTERN.format(self._wml_credentials['url'])
-    #
-    # def get_env_href(self, env_id):
-    #     return DEPLOYMENT_ENV_HREF_PATTERN.format(self._wml_credentials['url'],env_id)
+    def get_prompts_all_href(self) -> str:
+        return PROMPTS_GET_ALL.format(self._get_platform_url_if_exists())
 
-    def get_parameter_set_href(self, parameter_sets_id):
-        return PARAMETER_SET.format(self._get_platform_url_if_exists(), parameter_sets_id)
+    def get_parameter_set_href(self, parameter_sets_id: str) -> str:
+        return PARAMETER_SET.format(
+            self._get_platform_url_if_exists(), parameter_sets_id
+        )
 
-    def get_parameter_sets_href(self):
+    def get_parameter_sets_href(self) -> str:
         return PARAMETER_SETS.format(self._get_platform_url_if_exists())
-    
+
     def get_fm_embeddings_href(self):
-        return FM_EMBEDDINGS.format(self._credentials['url'])
-    
+        return FM_EMBEDDINGS.format(self._credentials.url)
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/route_declarations.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/route_declarations.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/websockets_connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/connection/websockets_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_util.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/data/data_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/pytorch_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/pytorch_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/tensorflow_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/tensorflow_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/xgb_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/v2/xgb_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/model/xgb_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/xgb_fl_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
 from __future__ import print_function
 import time
+import uuid
 import pickle
 import logging
+from functools import partial
 
 from sklearn.utils.validation import check_is_fitted
 from sklearn.ensemble._hist_gradient_boosting.loss import *
 from sklearn.ensemble._hist_gradient_boosting.common import *
 from sklearn.preprocessing import OrdinalEncoder, LabelEncoder
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.metrics import check_scoring, accuracy_score, r2_score
 from sklearn.utils import check_X_y, check_random_state, check_array
 from sklearn.ensemble._hist_gradient_boosting.grower import TreePredictor
+from sklearn.ensemble._hist_gradient_boosting.common import X_DTYPE, X_BINNED_DTYPE
 
 from ibmfl.util import fl_metrics
 from ibmfl.util import config
 from ibmfl.model.fl_model import FLModel
 from ibmfl.util.xgboost.utils import is_classifier
 from ibmfl.util.xgboost.export import export_sklearn
 from ibmfl.exceptions import ModelInitializationException, ModelException
@@ -57,19 +60,23 @@
 
         # Initialize Additional Internal Model Parameters
         self.model_type = 'XGBFLModel'
         self._baseline_prediction = None
         self._raw_predictions = None
         self.n_features_ = 0
         self.loss_ = None
-
+        self._in_fit = False
+        self.bin_mapper_ = None
         # Validate and Initialize Model Hyperparameters
         validate_parameters(model_spec)
         init_parameters(self, model_spec)
 
+        # Generate Party-Based UUID (For Model + Metrics Persistence)
+        self.party_uuid = str(uuid.uuid4())
+
     def fit_model(self, train_data, fit_params=None, **kwargs):
         """
         This function is not implemented as model training is not operated
         within the FL Model object and is part of an external process.
 
         :return: `NotImplementedError`
         """
@@ -109,26 +116,30 @@
         :return: raw_predictions
         :rtype: `np.array`
         """
         logger.info('Performing Model Inference Process')
 
         # Initialize Prediction Object
         n_samples = x.shape[0]
-        preds = np.zeros(shape=(self.n_trees, n_samples))
+        is_binned = getattr(self, '_in_fit', False)
 
-        # Append Null Model Predictions
+        # Generate Predictions
+        preds = np.zeros(shape=(self.n_trees, n_samples))
         if self._baseline_prediction is not None:
             preds += self._baseline_prediction
-        elif self._raw_predictions is not None:
-            preds += self._raw_predictions
-
-        # Generate Predictions
         for p in self._predictors:
             for k, p_i in enumerate(p):
-                preds[k, :] += p_i.predict(x.astype(np.float64))
+                if is_binned and self.bin_mapper_:
+                    predict = partial(
+                        p_i.predict_binned,
+                        missing_values_bin_idx=self.bin_mapper_.missing_values_bin_idx_
+                    )
+                else:
+                    predict = p_i.predict
+                preds[k, :] += predict(x)
 
         return preds
 
     def get_model_update(self):
         """
         Since we are not using the conventional train() function at the local
         training handler, we respectively do not implement anything within here,
@@ -161,16 +172,16 @@
         is specified, the model will be stored in the default data location of \
         the library `DATA_PATH`.
         :type path: `str`
         :return: filename
         """
         if filename is None:
             file = self.model_name if self.model_name else self.model_type
-            filename = '{}_{}.pickle'.format(file, time.time())            
-            
+            filename = '{}_{}.pickle'.format(file, self.party_uuid)
+
         full_path = super().get_model_absolute_path(filename)
 
         # Scikit-Learn Export Demo
         export_sklearn(self, full_path)
 
         if len(self._predictors) > 0:
             logger.info('Model saved in path: %s.', full_path)
@@ -223,16 +234,16 @@
         `keras.preprocessing.image.ImageDataGenerator`
         :type test_dataset: `np.ndarray`
         :param kwargs: Dictionary of metrics available for the model
         :type kwargs: `dict`
         """
 
         if type(test_dataset) is tuple:
-            x_test = test_dataset[0]
-            y_test = test_dataset[1]
+            x_test = test_dataset[0].astype(X_DTYPE)
+            y_test = test_dataset[1].astype(Y_DTYPE)
 
             return self.evaluate_model(x_test, y_test)
 
         else:
             raise ModelException("Invalid test dataset!")
 
     @abstractmethod
@@ -438,21 +449,21 @@
         :return: Return a dictionary containing the accuracy for the provided \
         input and target values.
         :rtype: `dict`
         """
         acc = {}
         if len(self._predictors) > 0:
             y_hat = self.predict(x)
+
             correct = 0
             for i in range(x.shape[0]):
                 if y_hat[i] == y[i]:
                     correct += 1
 
             acc = {'acc': correct/float(len(y))}
             additional_metrics = fl_metrics.get_eval_metrics_for_classificaton(
                 y, y_hat)
-
             acc = {**acc, **additional_metrics}
             return acc
         else:
             logger.info('No models have been trained yet.')
             return {}
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/metrics_recorder.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/metrics/metrics_recorder.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party_protocol_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/party_protocol_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/fedavg_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/fedavg_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/pfnm_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/pfnm_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/xgboost_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/v2/xgboost_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/xgboost_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/party/training/xgboost_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/config.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/config.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/core.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/core.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/matching.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/matching.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/pfnm/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/export.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/export.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/hyperparams.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/hyperparams.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd35/ibmfl/util/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/websockets_connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/connection/websockets_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/metrics_recorder.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/metrics/metrics_recorder.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party_protocol_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/party/party_protocol_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/config.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/cpd403/ibmfl/util/config.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/party_env_validator.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/party_env_validator.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/route_declarations.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/connection/route_declarations.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_enumeration.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_enumeration.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_exceptions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_library.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/crypto_library.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/fhe.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/helayer/fhe.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_asym_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_cert_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_he_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/infra/crypto_sym_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/exceptions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/message_type.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/message/message_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/pytorch_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/pytorch_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/tensorflow_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/tensorflow_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/xgb_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/model/xgb_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party_protocol_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/party_protocol_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/crypto_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/crypto_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/pfnm_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/pfnm_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/xgboost_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/party/training/xgboost_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/export.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/export.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/hyperparams.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/hyperparams.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf212-pt20-sk11/ibmfl/util/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/route_declarations.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/connection/route_declarations.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_enumeration.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_enumeration.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_exceptions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_library.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/crypto_library.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/fhe.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/helayer/fhe.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_imp_rsa.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_asym_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_imp_rsa.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_cert_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_imp_hely.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_he_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_imp_fernet.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/infra/crypto_sym_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_dst.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_key_mng_int.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/crypto/keys_mng/crypto_keys_proto_party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/exceptions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/message_type.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/message/message_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/pytorch_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/pytorch_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/tensorflow_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/tensorflow_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/xgb_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/model/xgb_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party_protocol_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/party_protocol_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/crypto_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/crypto_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/pfnm_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/pfnm_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/xgboost_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/party/training/xgboost_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/export.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/export.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/hyperparams.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/hyperparams.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py310-tf29-pt112-sk11/ibmfl/util/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/route_declarations.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/route_declarations.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/router_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/router_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/websockets_connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/connection/websockets_connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_util.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/data_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_data_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_spec.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/env_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/pandas_data_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/data/pandas_data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/envs.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/envs.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/exceptions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/json_serializer.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/json_serializer.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message_type.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/message_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/pickle_serializer.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer_factory.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/message/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/model_update.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/model_update.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/naive_bayes_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/naive_bayes_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/pytorch_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/pytorch_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_SGD_linear_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_SGD_linear_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_kmeans_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/sklearn_kmeans_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/tensorflow_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/tensorflow_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/model/xgb_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/xgb_fl_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     Wrapper class implementation for XGBoost containing the XGBoost Model Object
     """
 
     def __init__(self, model_name, model_spec, xgb_model=None, **kwargs):
         """
         Create a XGBFLModel instance for XGBoost model based either on an
         existing model object or an entirely new model object.
-
         :param model_type: String specifying the name of the model
         :type model_type: `str`
         :param model_spec: Hyperparameters associated with the model.
         :type model_spec: `dict`
         :param xgb_model: List of predictors existing predictor structures.
         :type xgb_model: `list`
         :param kwargs: A dictionary contains other parameter settings on \
@@ -73,24 +72,22 @@
         # Generate Party-Based UUID (For Model + Metrics Persistence)
         self.party_uuid = str(uuid.uuid4())
 
     def fit_model(self, train_data, fit_params=None, **kwargs):
         """
         This function is not implemented as model training is not operated
         within the FL Model object and is part of an external process.
-
         :return: `NotImplementedError`
         """
         return NotImplementedError
 
     def update_model(self, model_update=None, **kwargs):
         """
         Updates model using provided `model_update`. Additional arguments
         specific to the model can be added through `**kwargs`
-
         :param model_update: Model with update. This is specific to each model \
         type e.g., `ModelUpdateSGD`. The specific type should be checked by \
         the corresponding FLModel class.
         :type `ModelUpdate`
         :param kwargs: Dictionary of model-specific arguments.
         :type kwargs: `dict`
         :return: None
@@ -103,15 +100,14 @@
                 raise ValueError('Provided model object is not of the correct '
                                  'data type. Should be a `list`. '
                                  'Type provided: ' + str(type(model_update)))
 
     def _raw_predict(self, x):
         """
         Internal helper function for generating predictions for the model.
-
         :param x: The input data for the prediction model.
         :type x: `np.array`
         :param model: Model object which is used for generating the prediction. \
         If not provided the default model assigned internally will be used.
         :type model: `XGBFLModel`
         :return: raw_predictions
         :rtype: `np.array`
@@ -131,15 +127,15 @@
                 if is_binned and self.bin_mapper_:
                     predict = partial(
                         p_i.predict_binned,
                         missing_values_bin_idx=self.bin_mapper_.missing_values_bin_idx_
                     )
                 else:
                     predict = p_i.predict
-                preds[k, :] += predict(x)
+                preds[k, :] += predict(x, self.known_cat_bitsets, self.f_idx_map, self.loss_.n_threads)
 
         return preds
 
     def get_model_update(self):
         """
         Since we are not using the conventional train() function at the local
         training handler, we respectively do not implement anything within here,
@@ -147,29 +143,27 @@
         """
         return NotImplementedError
 
     @abstractmethod
     def predict(self, x):
         """
         Given a set of inputs, generate inference for the given set of samples.
-
         :param x: The input data for the prediction model.
         :type x: `np.array`
         :param model: Model object which is used for generating the prediction. \
         If not provided the default model assigned internally will be used.
         :type model: `XGBFLModel`
         :return: `np.array`
         """
         return NotImplementedError
 
     def save_model(self, filename=None, path=None):
         """
         Saves a sklearn model to file in the format specific
         to the framework requirement as a pickle file (only for inference use).
-
         :param filename: Name of the file where to store the model.
         :type filename: `str`
         :param path: Path of the folder where to store the model. If no path \
         is specified, the model will be stored in the default data location of \
         the library `DATA_PATH`.
         :type path: `str`
         :return: filename
@@ -190,15 +184,14 @@
 
         return filename
 
     @staticmethod
     def load_model(filename):
         """
         Load model from provided filename
-
         :param filename: Name of the file where to store the model.
         :type filename: `str`
         :param path: Path of the folder where to store the model. If no path \
         is specified, the model will be stored in the default data location of \
         the library `DATA_PATH`.
         :type path: `str`
         :return: Returns the corresponding model object.
@@ -216,15 +209,14 @@
         return model
 
     @abstractmethod
     def get_loss(self):
         """
         Internal helper function used to obtain the corresponding loss function
         which is dependent on the learning task set by the hyperparameters.
-
         :return: Returns the loss object used to compute the loss function.
         :rtype: `BaseLoss` based object
         """
         return NotImplementedError
 
     def evaluate(self, test_dataset, **kwargs):
         """
@@ -247,15 +239,14 @@
             raise ModelException("Invalid test dataset!")
 
     @abstractmethod
     def evaluate_model(self, x, y, **kwargs):
         """
         Evaluates model given the samples x and true labels y.
         Multiple evaluation metrics are returned in a dictionary
-
         :param x: Samples with shape as expected by the model.
         :type x: Data structure as expected by the model \
         :param y: Corresponding labels to x
         :type y: Data structure the same as the type defines labels \
         in testing data.
         :param batch_size: Size of batches.
         :type batch_size: `int`
@@ -265,20 +256,19 @@
         implementation.
         :rtype: `dict`
         """
         return NotImplementedError
 
 
 class XGBRegressorFLModel(XGBFLModel):
-    _VALID_LOSSES = ('least_squares', 'least_absolute_deviation')
+    _VALID_LOSSES = ('squared_error')
 
     def predict(self, x):
         """
         Perform prediction for a batch of inputs.
-
         :param x: Samples with shape as expected by the model.
         :type x: Data structure as expected by the model
         :param kwargs: Dictionary of model-specific arguments.
         :type kwargs: `dict`
         :return: Predictions
         :rtype: Data structure the same as the type defines labels
         in testing data.
@@ -287,42 +277,39 @@
             return self._raw_predict(x).ravel()
         else:
             raise Exception('Model has not been trained yet.')
 
     def encode_target(self, y):
         """
         Converts the input y to the expected dtype.
-
         :param y: The corresponding target data from the dataset to encode.
         :type y: `np.array`
         :return: Returns the corresponding encoded y values.
         :rtype: `np.array`
         """
         self.n_trees = 1
         return y.astype(Y_DTYPE, copy=False)
 
     def get_loss(self, sample_weight):
         """
         Given the initialized loss type defined under the hyerparameters, we
         return the corresponding loss function to dictate the corresponding
         learning task of the model.
-
         :param sample_weight: Weights of training data
         :type sample_weight: `np.ndarray`
         :return: Returns the respective loss object as defined in the FL \
         hyperparameters.
         :rtype: Derivation of `BaseLoss`
         """
         return _LOSSES[self.loss](sample_weight=sample_weight)
 
     def evaluate_model(self, x, y, **kwargs):
         """
         Given an input set of values and their values, generate the prediction
         and compute the R^2 metric.
-
         :param x: The input data for the prediction model.
         :type x: `np.array`
         :param y: The corresponding target value of the prediction.
         :type y: `np.array`
         :return: Return a dictionary containing the R^2 metric for the provided
         input and target values.
         :rtype: `dict`
@@ -345,15 +332,14 @@
     _VALID_LOSSES = ('binary_crossentropy', 'categorical_crossentropy', 'auto')
 
     def encode_target(self, y):
         """
         Converts the input y to the expected dtype and performs a label
         encoding. Here, we assume that each party has at least one sample of
         the corresponding class label type for each different classes.
-
         :param y: The corresponding target data from the dataset to encode.
         :type  y: `np.array`
         :return y: Returns the corresponding encoded y values.
         :rtype  y: `np.array`
         """
         # Validate Classification Target Values
         check_classification_targets(y)
@@ -365,15 +351,15 @@
         # Extract Encoded Target Sizes
         self.classes_ = lab_enc.classes_
         if self.classes_.shape[0] != self.num_classes:
             raise ValueError('Number of classes defined in configuration file '
                              'and the classes derived from the data does not '
                              'match. Found {0} classes, while config file '
                              'is defined as {1} classes.'.format(
-                             self.classes_.shape[0], self.num_classes))
+                self.classes_.shape[0], self.num_classes))
 
         if self.loss == 'auto':
             self.n_trees = 1 if self.classes_.shape[0] <= 2 else self.classes_.shape[0]
         else:
             self.n_trees = 1 if self.num_classes <= 2 else self.num_classes
 
         return enc_y
@@ -381,15 +367,14 @@
     def get_loss(self, sample_weight):
         """
         Given the initialized loss type defined under the hyerparameters, we
         return the corresponding loss function to dictate the corresponding
         learning task of the model. If auto is selected, then we will
         automatically determine whether the classification task is binary or
         multiclass given the label encoding cardinality.
-
         :param sample_weight: Weights of training data
         :type sample_weight: `np.ndarray`
         :return: Returns the respective loss object as defined in the FL \
         hyperparameters.
         :rtype: Derivation of `BaseLoss`
         """
         if (self.loss == 'categorical_crossentropy' and self.n_trees == 1):
@@ -400,15 +385,14 @@
                 _LOSSES['categorical_crossentropy']()
         else:
             return _LOSSES[self.loss](sample_weight=sample_weight)
 
     def predict(self, x, **kwargs):
         """
         Perform prediction for a batch of inputs returned as class values.
-
         :param x: Samples with shape as expected by the model.
         :type x: Data structure as expected by the model
         :param kwargs: Dictionary of model-specific arguments.
         :type kwargs: `dict`
         :return: Predictions based on class values.
         :rtype: Data structure the same as the type defines labels
         in testing data.
@@ -418,15 +402,14 @@
             return self.classes_[encoded_classes]
         else:
             raise Exception('Model has not been trained yet.')
 
     def predict_proba(self, x, **kwargs):
         """
         Perform prediction for a batch of inputs as probabilities.
-
         :param x: Samples with shape as expected by the model.
         :type x: Data structure as expected by the model
         :param kwargs: Dictionary of model-specific arguments.
         :type kwargs: `dict`
         :return: A probabilistic set of predictions
         :rtype: Data structure the same as the type defines labels \
         in testing data.
@@ -437,15 +420,14 @@
         else:
             raise Exception('Model has not been trained yet.')
 
     def evaluate_model(self, x, y, **kwargs):
         """
         Given an input set of values and their values, generate the prediction
         and compute the accuracy.
-
         :param x: The input data for the prediction model.
         :type x: `np.array`
         :param y: The corresponding target value of the prediction.
         :type y: `np.array`
         :return: Return a dictionary containing the accuracy for the provided \
         input and target values.
         :rtype: `dict`
@@ -462,8 +444,8 @@
             acc = {'acc': correct/float(len(y))}
             additional_metrics = fl_metrics.get_eval_metrics_for_classificaton(
                 y, y_hat)
             acc = {**acc, **additional_metrics}
             return acc
         else:
             logger.info('No models have been trained yet.')
-            return {}
+            return {}
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/metrics_recorder.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/metrics/metrics_recorder.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party_protocol_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/party_protocol_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/status_type.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/status_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/fedavg_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/fedavg_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/pfnm_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/pfnm_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/xgboost_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/party/training/xgboost_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/config.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/config.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/fl_metrics.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/fl_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/log_config.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/log_config.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/core.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/core.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/matching.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/matching.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/pfnm/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/export.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/export.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/hyperparams.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/hyperparams.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py38-tf24-pt17-sk23/ibmfl/util/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/pytorch_fl_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/model/pytorch_fl_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/xgboost_local_training_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/xgboost_local_training_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/export.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/export.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/hyperparams.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/hyperparams.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/TestRepoSaveLoad.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/TestRepoSaveLoad.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,17 @@
 # mlUrl = service_path
 # mlUser = user
 # mlPassword = password
 #
 # auth64 = mlUser + ":" + mlPassword
 # wml_url = mlUrl + "/v2/identity/token"
 # token_response = requests.get(wml_url, auth=(mlUser, mlPassword))
-# wml_token = json.loads(token_response.text).get('token')
-# print(wml_token)
-# bearer = "Bearer "+ wml_token
+# token = json.loads(token_response.text).get('token')
+# print(token)
+# bearer = "Bearer "+ token
 #
 # details_json = {'href': 'https://ibm-watson-ml-fvt.stage1.mybluemix.net/v3/ml_assets/models/f81ad6bd-26f6-4c6f-aae9-3fe82be5d318/versions/4cdc20a2-f1a1-445f-b43a-f12fc88b93b7',
 #                 'mltoken': bearer }
 #
 # saved_dir = get_model_archive("reqid_2", "depid_2", details_json)
 # print(saved_dir)
 ## End of Save
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/base_constants.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/base_constants.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/ml_api_client.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/ml_api_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/ml_authorization.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/ml_authorization.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/artifact_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_pipeline_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/generic_archive_pipeline_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/hybrid_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/hybrid_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/meta_names.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/meta_names.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/meta_props.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/meta_props.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/pipeline_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/pipeline_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/scikit_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/scikit_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/tensorflow_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/tensorflow_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_experiment_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_experiment_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_function_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_function_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_libraries_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_libraries_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/wml_runtimes_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/wml_runtimes_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepository/xgboost_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepository/xgboost_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/content_loaders.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/content_loaders.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/experiment_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/experiment_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/function_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_archive_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/generic_file_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/hybrid_pipeline_model_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/libraries_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/ml_repository_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/ml_repository_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/runtimes_artifact_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/scikit_pipeline_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_pipeline_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_version.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/spark_version.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_artifact_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_artifact.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_model_loader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/tensorflow_pipeline_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/version_helper.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/version_helper.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/xgboost_model_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryartifact/xgboost_model_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/content_reader.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/content_reader.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_adapter.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_collection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/experiment_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_adapter.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_collection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/function_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_adapter.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_collection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/libraries_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_api.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_api.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_client.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/ml_repository_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_adapter.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_collection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/model_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_adapter.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_collection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/runtimes_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_adapter.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_adapter.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_collection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/mlrepositoryclient/wml_experiment_collection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/api_client.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/apis/repository_api.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/apis/repository_api.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/apis/token_api.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/apis/token_api.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/configuration.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/__init__.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_data_input_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_data_input_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_metrics_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_metrics_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_metrics_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_model_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_version_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_pipeline_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/array_training_output_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/array_training_output_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_author.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_author.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_short_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/artifact_version_short_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/author_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/author_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/author_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/author_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_entity_execution.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_meta.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_deploy_output_meta.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/batch_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/cols_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/cols_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/compute_configuration_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/compute_configuration_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_source_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_source_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_target_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_target_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_with_name_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/connection_object_with_name_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/content_location.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/content_location.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/content_status.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/content_status.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/custom_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/custom_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/deploy_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/deploy_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_bad_request_libraries_target.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_bad_request_libraries_target.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments_target.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_experiments_target.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_message.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_message.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository_target.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_repository_target.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/error_schema_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_metrics.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/evaluation_definition_repository_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input_settings.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_input_settings.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array_first.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_patch.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_patch.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_status_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/experiment_status_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_libraries.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_runtimes.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/framework_output_repository_runtimes.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_double_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_double_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_int_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_inner_values_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_experiments_int_range.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_for_status_experiments_inner.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/hyper_parameters_optimization_experiments_method_parameters.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/input_data_schema.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/input_data_schema.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_input_batch.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_input_batch.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_output_batch.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/internal_output_batch.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/json_patch_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input_platform.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/libraries_definition_input_platform.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_experiments_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_functions_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_functions_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/meta_object_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/metric_object_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/metric_object_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/metrics_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/metrics_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_experiment_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_function_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_function_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_functions_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_libraries_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_model_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_patch_libraries_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_create_runtime_spec_output_array_first.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_get_presigned_url_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_model_size_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_model_size_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_function.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_function.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_libraries_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_patch_runtime_spec_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/ml_assets_upload_content_output_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_content_location.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_content_location.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_definition_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_definition_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics_values.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_metrics_values.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_output_entity_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_schemas.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_schemas.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_training_data_ref.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_training_data_ref.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_type.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_metrics_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_metrics_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity_model.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/model_version_output_entity_model.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/online_deploy_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/online_deploy_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/online_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/output_data_schema.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/output_data_schema.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_functions.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_functions.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_libraries.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_runtime_spec.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/patch_operation_runtime_spec.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_type.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_type.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/pipeline_version_output_entity_parent.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_environment.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_output_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_output_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_custom_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_platform.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_public_libraries.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/runtime_spec_definition_input_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/sample_scoring_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/sample_scoring_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/schemas.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/schemas.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/score_input.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/score_input.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/score_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/score_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/size_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/size_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/software_spec_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/software_spec_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/space_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/space_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/spark_service.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/spark_service.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_input_internal.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_input_internal.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_internal.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_internal.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_array.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_array.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_internal.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/stream_output_internal.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/tag_repository.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/tag_repository.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/token_response.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_data_schema.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_data_schema.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_models.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_models.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_output_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_output_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_reference_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_reference_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments_result.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/models/training_status_experiments_result.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/swagger_client/rest.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/base_singleton.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/base_singleton.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/compression_util.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/compression_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/file_system_ops.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/file_system_ops.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/generic_archive_file_check.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/generic_archive_file_check.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/json_2_object_mapper.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/json_2_object_mapper.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/library_imports.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/library_imports.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/libs/repo/util/spark_util.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/libs/repo/util/spark_util.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/messages.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
 import json
 import os
+from typing import Any
 
 from .globalization_util import GlobalizationUtil
 import ibm_watsonx_ai.messages
 
 
-def get_message_dict(locale):
+def get_message_dict(locale: str) -> dict[str, str]:
     file_name = "messages_" + locale + ".json"
     message_dict = {}
     path = os.path.dirname(ibm_watsonx_ai.messages.__file__)
     messages = []
     # try to load the respective json file for the locale
     try:
         with open(os.path.join(path, file_name)) as f:
@@ -22,41 +23,44 @@
     # load the english dictionary if the json file for the locale doesn't exist
     except:
         try:
             return get_message_dict("en")
         except:
             raise Exception(
                 "An error occurred while trying to load the message json file for the {} locale. "
-                "Make sure the json file exists and is located in the correct folder.".format(locale))
+                "Make sure the json file exists and is located in the correct folder.".format(
+                    locale
+                )
+            )
 
-    messages_list = [{item["code"]:item["message"]} for item in messages]
+    messages_list = [{item["code"]: item["message"]} for item in messages]
     for i in range(len(messages_list)):
         message_dict.update(messages_list[i])
     return message_dict
 
 
 MESSAGE_DICT = get_message_dict(GlobalizationUtil.get_language())
 
 
-def replace_args_in_message(message, *args):
+def replace_args_in_message(message: str, *args: Any) -> str:
     if args:
         varss = []
         for x in args:
             if x is not None and type(x) is not Exception:
                 varss.append(x)
-        if '{0}' in message:
+        if "{0}" in message:
             message = message.format(*varss)
         else:
             message = message % tuple(varss)
     return message
 
 
 class Messages:
 
     @classmethod
-    def get_message(cls, *args, message_id):
+    def get_message(cls, *args: Any, message_id: str) -> str:
         message = MESSAGE_DICT.get(message_id)
 
         if args and message:
             message = replace_args_in_message(message, *args)
 
-        return message
+        return str(message)
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/messages/messages_en.json` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/messages/messages_en.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156863%*

 * *Differences: {'8': '{\'message\': "The product version {0} is not supported yet in the ibm-watsonx-ai package '*

 * *      "release {1}. Please check for package's updates, install the most recent ibm-watsonx-ai "*

 * *      'package release, and try again."}'}*

```diff
@@ -29,15 +29,15 @@
     },
     {
         "code": "invalid_version",
         "message": "Invalid value for 'version' provided in wml_credentials. Update the wml_credentials and try again. Supported value for version field are: {0}"
     },
     {
         "code": "invalid_version_from_automated_check",
-        "message": "The product version {0} is not supported yet in the ibm-watson-machine-learning package release {1}. Please check for package's updates, install the most recent ibm-watson-machine-learning package release, and try again."
+        "message": "The product version {0} is not supported yet in the ibm-watsonx-ai package release {1}. Please check for package's updates, install the most recent ibm-watsonx-ai package release, and try again."
     },
     {
         "code": "instance_id_in_cloud_scenario",
         "message": "Specified credentials are invalid. Do not specify `instance_id` for Cloud Pak for Data as a Service. Update your wml_credentials and try again. See https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/ml-authentication.html ."
     },
     {
         "code": "invalid_instance_id",
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/parameter_sets.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/parameter_sets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from typing import Literal, List, Union
+from __future__ import annotations
+from typing import Literal, TYPE_CHECKING, TypeAlias
 
 from ibm_watsonx_ai._wrappers import requests
 from ibm_watsonx_ai.wml_resource import WMLResource
 from ibm_watsonx_ai.metanames import ParameterSetsMetaNames
 
 _DEFAULT_LIST_LENGTH = 50
+ListType: TypeAlias = list
+
+if TYPE_CHECKING:
+    from ibm_watsonx_ai import APIClient
+    from pandas import DataFrame
 
 
 class ParameterSets(WMLResource):
     """Store and manage parameter sets."""
 
     ConfigurationMetaNames = ParameterSetsMetaNames()
     """MetaNames for Parameter Sets creation."""
 
-    def __init__(self, client):
+    def __init__(self, client: APIClient) -> None:
         WMLResource.__init__(self, __name__, client)
-        self._ICP = client.ICP
 
     @staticmethod
     def _prepare_parameter_sets_payload(meta_data: dict) -> dict:
-        payload = {
-            "parameter_set": meta_data
-        }
+        payload = {"parameter_set": meta_data}
 
         return payload
 
     @staticmethod
-    def _prepare_parameter_sets_payload_to_update(meta_data: Union[List, str], path: str, operation: str = "replace") -> list:
+    def _prepare_parameter_sets_payload_to_update(
+        meta_data: ListType | str, path: str, operation: str = "replace"
+    ) -> ListType:
         payload = [
             {
                 "op": operation,
                 "path": f"/entity/parameter_set/{path}",
-                "value": meta_data
+                "value": meta_data,
             }
         ]
         return payload
 
-    def get_details(self, parameter_set_id: str = None) -> dict:
+    def get_details(self, parameter_set_id: str | None = None) -> dict:
         """Get parameter set details. If no parameter_sets_id is passed, details for all parameter sets
         will be returned.
 
-        :param parameter_set_id: UID of software specification
+        :param parameter_set_id: ID of software specification
         :type parameter_set_id: str, optional
 
         :return: metadata of the stored parameter set(s)
         :rtype:
           - **dict** - if `parameter_set_id` is not None
           - **{"parameter_sets": [dict]}** - if `parameter_set_id` is None
 
@@ -64,33 +69,37 @@
         if `parameter_set_id` is given
 
         .. code-block:: python
 
             parameter_sets_details = client.parameter_sets.get_details(parameter_set_id)
 
         """
-        ParameterSets._validate_type(parameter_set_id, u'sw_spec_uid', str, False)
+        ParameterSets._validate_type(parameter_set_id, "parameter_set_id", str, False)
 
         if parameter_set_id:
             try:  # TODO remove when get_parameter_sets_href() available
-                href = self._client.service_instance._href_definitions.get_parameter_set_href(parameter_set_id)
+                href = self._client.service_instance._href_definitions.get_parameter_set_href(
+                    parameter_set_id
+                )
             except AttributeError:
                 href = f"{self._client.service_instance._href_definitions._get_platform_url_if_exists()}/v2/parameter_sets/{parameter_set_id}"
 
         else:
             try:  # TODO remove when get_parameter_sets_href() available
-                href = self._client.service_instance._href_definitions.get_parameter_sets_href()
+                href = (
+                    self._client.service_instance._href_definitions.get_parameter_sets_href()
+                )
             except AttributeError:
                 href = f"{self._client.service_instance._href_definitions._get_platform_url_if_exists()}/v2/parameter_sets"
 
-        response = requests.get(url=href,
-                                params=self._client._params(),
-                                headers=self._client._get_headers())
+        response = requests.get(
+            url=href, params=self._client._params(), headers=self._client._get_headers()
+        )
 
-        return self._handle_response(200, u'get parameter set(s) details', response)
+        return self._handle_response(200, "get parameter set(s) details", response)
 
     def create(self, meta_props: dict) -> dict:
         """Create a parameter set.
 
         :param meta_props: metadata of the space configuration. To see available meta names use:
 
             .. code-block:: python
@@ -134,78 +143,94 @@
                     }
                 ]
             }
 
             parameter_sets_details = client.parameter_sets.create(meta_props)
         """
 
-        ParameterSets._validate_type(meta_props, u'meta_props', dict, True)
+        ParameterSets._validate_type(meta_props, "meta_props", dict, True)
 
-        parameter_sets_meta_data = self.ConfigurationMetaNames._generate_resource_metadata(
-            meta_props,
-            with_validation=True,
-            client=self._client)
+        parameter_sets_meta_data = (
+            self.ConfigurationMetaNames._generate_resource_metadata(
+                meta_props, with_validation=True, client=self._client
+            )
+        )
 
         payload = self._prepare_parameter_sets_payload(parameter_sets_meta_data)
 
         try:  # TODO remove when get_parameter_sets_href() available
-            href = self._client.service_instance._href_definitions.get_parameter_sets_href()
+            href = (
+                self._client.service_instance._href_definitions.get_parameter_sets_href()
+            )
         except AttributeError:
             href = f"{self._client.service_instance._href_definitions._get_platform_url_if_exists()}/v2/parameter_sets"
 
-        creation_response = requests.post(url=href,
-                                          json=payload,
-                                          params=self._client._params(),
-                                          headers=self._client._get_headers())
-
-        parameter_sets_details = self._handle_response(201, u'creating parameter set', creation_response)
+        creation_response = requests.post(
+            url=href,
+            json=payload,
+            params=self._client._params(),
+            headers=self._client._get_headers(),
+        )
+
+        parameter_sets_details = self._handle_response(
+            201, "creating parameter set", creation_response
+        )
 
         return parameter_sets_details
 
-    def list(self, limit: int = None, return_as_df: bool = True):
-        """Print parameter sets in a table format.
+    def list(self, limit: int | None = None) -> DataFrame:
+        """Lists parameter sets in a table format.
 
         :param limit: limit number of fetched records
         :type limit: int, optional
 
-        :param return_as_df: determinate if table should be returned as pandas.DataFrame object, default: True
-        :type return_as_df: bool, optional
-
-        :return: pandas.DataFrame with listed parameter sets or None if return_as_df is False
-        :rtype: pandas.DataFrame or None
+        :return: pandas.DataFrame with listed parameter sets
+        :rtype: pandas.DataFrame
 
         **Example**
 
         .. code-block:: python
 
             client.parameter_sets.list()
         """
 
         try:  # TODO remove when get_parameter_sets_href() available
-            href = self._client.service_instance._href_definitions.get_parameter_sets_href()
+            href = (
+                self._client.service_instance._href_definitions.get_parameter_sets_href()
+            )
         except AttributeError:
             href = f"{self._client.service_instance._href_definitions._get_platform_url_if_exists()}/v2/parameter_sets"
 
-        response = requests.get(url=href,
-                                params=self._client._params(),
-                                headers=self._client._get_headers())
-
-        parameter_sets_details = self._handle_response(200, u'list assets', response)['parameter_sets']
+        response = requests.get(
+            url=href, params=self._client._params(), headers=self._client._get_headers()
+        )
+
+        parameter_sets_details = self._handle_response(
+            200, "parameter sets asset", response
+        )["parameter_sets"]
 
         parameter_sets_values = [
-            (m['metadata']['name'],
-             m['metadata']['asset_id'],
-             m['metadata']['create_time']) for m in parameter_sets_details]
+            (
+                m["metadata"]["name"],
+                m["metadata"]["asset_id"],
+                m["metadata"]["create_time"],
+            )
+            for m in parameter_sets_details
+        ]
 
-        table = self._list(parameter_sets_values, ['NAME', 'ID', 'CREATED'], limit, _DEFAULT_LIST_LENGTH)
+        table = self._list(
+            parameter_sets_values,
+            ["NAME", "ID", "CREATED"],
+            limit,
+            _DEFAULT_LIST_LENGTH,
+        )
 
-        if return_as_df:
-            return table
+        return table
 
-    def delete(self, parameter_set_id: str):
+    def delete(self, parameter_set_id: str) -> str:
         """Delete a parameter set.
 
         :param parameter_set_id: Unique id of parameter set
         :type parameter_set_id: str
 
         :return: status ("SUCCESS" or "FAILED")
         :rtype: str
@@ -213,57 +238,70 @@
         **Example**
 
         .. code-block:: python
 
             client.parameter_sets.delete(parameter_set_id)
 
         """
-        ParameterSets._validate_type(parameter_set_id, u'sw_spec_uid', str, True)
+        ParameterSets._validate_type(parameter_set_id, "parameter_set_id", str, True)
 
         try:  # TODO remove when get_parameter_sets_href() available
-            href = self._client.service_instance._href_definitions.get_parameter_set_href(parameter_set_id)
+            href = (
+                self._client.service_instance._href_definitions.get_parameter_set_href(
+                    parameter_set_id
+                )
+            )
         except AttributeError:
             href = f"{self._client.service_instance._href_definitions._get_platform_url_if_exists()}/v2/parameter_sets/{parameter_set_id}"
 
-        response = requests.delete(url=href,
-                                   params=self._client._params(),
-                                   headers=self._client._get_headers())
+        response = requests.delete(
+            url=href, params=self._client._params(), headers=self._client._get_headers()
+        )
 
         if response.status_code == 200:
             return response.json()
         else:
-            return self._handle_response(204, u'delete parameter set', response)
+            return self._handle_response(204, "delete parameter set", response)
 
     def get_id_by_name(self, parameter_set_name: str) -> str:
         """Get Unique Id of parameter set.
 
         :param parameter_set_name: name of the parameter sets
         :type parameter_set_name: str
 
         :return: Unique Id of parameter set
         :rtype: str
 
         **Example**
 
         .. code-block:: python
 
-            asset_uid = client.parameter_sets.get_id_by_name(parameter_set_name)
+            asset_id = client.parameter_sets.get_id_by_name(parameter_set_name)
 
         """
-        ParameterSets._validate_type(parameter_set_name, u'parameter_sets_id', str, True)
+        ParameterSets._validate_type(
+            parameter_set_name, "parameter_set_name", str, True
+        )
 
         details = self.get_details().get("parameter_sets") or []
 
-        parameter_sets_id = [parameter["metadata"]['asset_id'] for parameter in details if
-                             parameter["metadata"]["name"] == parameter_set_name]
+        parameter_sets_id = [
+            parameter["metadata"]["asset_id"]
+            for parameter in details
+            if parameter["metadata"]["name"] == parameter_set_name
+        ]
 
         return parameter_sets_id[0] if parameter_sets_id else "Not Found"
 
-    def update(self, parameter_set_id: str, new_data: Union[str, List],
-               file_path: Literal["description", "parameters", "value_sets"]) -> dict:
+    def update(
+        self,
+        parameter_set_id: str,
+        new_data: ListType[dict] | str,
+        file_path: Literal["description", "parameters", "value_sets"],
+    ) -> dict:
         """Update parameter sets.
 
         :param parameter_set_id: Unique id of parameter sets
         :type parameter_set_id: str
 
         :param new_data: Parameters new data.
         :type new_data: str, list
@@ -314,25 +352,35 @@
                         }
                     ]
                 }
             ]
             parameter_set_details = client.parameter_sets.update_value_sets(parameter_set_id, new_value_sets_data, "value_sets")
 
         """
-        ParameterSets._validate_type(parameter_set_id, u'sw_spec_uid', str, True)
-        ParameterSets._validate_type(new_data, u'meta_props', [list, str], True)
+        ParameterSets._validate_type(parameter_set_id, "parameter_set_id", str, True)
+        ParameterSets._validate_type(new_data, "new_data", [ListType, str], True)
 
         try:  # TODO remove when get_parameter_sets_href() available
-            href = self._client.service_instance._href_definitions.get_parameter_set_href(parameter_set_id)
+            href = (
+                self._client.service_instance._href_definitions.get_parameter_set_href(
+                    parameter_set_id
+                )
+            )
         except AttributeError:
             href = f"{self._client.service_instance._href_definitions._get_platform_url_if_exists()}/v2/parameter_sets/{parameter_set_id}"
 
-        payload = self._prepare_parameter_sets_payload_to_update(meta_data=new_data, path=file_path)
-
-        response = requests.patch(url=href,
-                                  json=payload,
-                                  params=self._client._params(),
-                                  headers=self._client._get_headers())
-
-        parameter_sets_details = self._handle_response(200, u'update parameter set', response)
+        payload = self._prepare_parameter_sets_payload_to_update(
+            meta_data=new_data, path=file_path
+        )
+
+        response = requests.patch(
+            url=href,
+            json=payload,
+            params=self._client._params(),
+            headers=self._client._get_headers(),
+        )
+
+        parameter_sets_details = self._handle_response(
+            200, "update parameter set", response
+        )
 
         return parameter_sets_details
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/connection.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 def validate_source_data_connections(source_data_connections: List['DataConnection'],
                                      workspace: 'WorkSpace',
                                      deployment=False) -> List['DataConnection']:
     for data_connection in source_data_connections:
 
         if isinstance(data_connection.location, FSLocation):
             # note: save data as an data asset
-            if workspace.api_client.ICP:
+            if workspace.api_client.ICP_PLATFORM_SPACES:
                 asset_id = data_connection.location._save_file_as_data_asset(workspace=workspace)
                 data_connection.location = AssetLocation(asset_id)
                 data_connection.type = DataConnectionTypes.DS
             # --- end note
 
         elif isinstance(data_connection.location, ContainerLocation):
-            if workspace.api_client.ICP:
+            if workspace.api_client.ICP_PLATFORM_SPACES:
                 raise ContainerTypeNotSupported() # block Container type on CPD
             elif isinstance(data_connection.connection, S3Connection):
                 # note: remove S3 inline credential from data asset before training
                 data_connection.connection = None
                 if hasattr(data_connection.location, 'bucket'):
                     delattr(data_connection.location, 'bucket')
                 # --- end note
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/enums.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/enums.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/errors.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,18 @@
     "LocalInstanceButRemoteParameter",
     "DataFormatNotSupported",
     "HoldoutSplitNotSupported",
     'LibraryNotCompatible',
     'CannotInstallLibrary',
     'InvalidCOSCredentials',
     'CannotDownloadTrainingDetails',
-    'NotInWatsonStudio',
-    'CredentialsNotFound,'
     'TShirtSizeNotSupported',
     'MissingPositiveLabel',
     'MissingDataPreprocessingStep',
     'CannotDownloadWMLPipelineDetails',
-    'NotInWatsonStudio',
     'SetIDFailed',
     'MissingLocalAsset',
     'DataSourceSizeNotSupported',
     'TrainingDataSourceIsNotFile',
     'VisualizationFailed',
     'InvalidPredictionType',
     'InvalidIdType',
@@ -68,15 +65,15 @@
     "ContainerTypeNotSupported",
     "InvalidSizeLimit",
     "CorruptedData"
 ]
 
 
 from ibm_watsonx_ai.wml_client_error import WMLClientError
-from ibm_watsonx_ai.utils.autoai.enums import PredictionType, ImputationStrategy
+from ibm_watsonx_ai.utils.autoai.enums import PredictionType
 
 
 class MissingPipeline(WMLClientError, ValueError):
     def __init__(self, value_name, reason=None):
         WMLClientError.__init__(self, f"There is no such a Pipeline like: {value_name}", reason)
 
 
@@ -157,22 +154,14 @@
 
 
 class CannotDownloadTrainingDetails(WMLClientError, ValueError):
     def __init__(self, value_name, reason=None):
         WMLClientError.__init__(self, f"Cannot download training details, training is not done yet. "
                                       f"Please try again after training is finished.", reason)
 
-class NotInWatsonStudio(WMLClientError, ValueError):
-    def __init__(self, value_name=None, reason=None):
-        WMLClientError.__init__(self, f"Wrong environment.", reason)
-
-class CredentialsNotFound(WMLClientError, ValueError):
-    def __init__(self, value_name=None, reason=None):
-        WMLClientError.__init__(self, f"Cannot find WMLS credentials in WSD.", reason)
-
 class TShirtSizeNotSupported(WMLClientError, ValueError):
     def __init__(self, value_name=None, reason=None):
         WMLClientError.__init__(self, f"This t-shirt size: \"{value_name}\" is not supported on this environment.",
                                 reason)
 
 
 class MissingPositiveLabel(WMLClientError, ValueError):
@@ -185,20 +174,14 @@
         WMLClientError.__init__(self, f"Data preprocessing step not performed.", reason)
 
 
 class CannotDownloadWMLPipelineDetails(WMLClientError, ValueError):
     def __init__(self, value_name, reason=None):
         WMLClientError.__init__(self, f"Cannot download WML pipeline details ", reason)
 
-
-class NotInWatsonStudio(WMLClientError, ValueError):
-    def __init__(self, value_name=None, reason=None):
-        WMLClientError.__init__(self, f"Wrong environment.", reason)
-
-
 class SetIDFailed(WMLClientError, ValueError):
     def __init__(self, value_name=None, reason=None):
         WMLClientError.__init__(self, f"Cannot set {value_name}.", reason)
 
 
 class MissingLocalAsset(WMLClientError, ValueError):
     def __init__(self, value_name=None, reason=None):
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/fairness.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/fairness.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/incremental.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/incremental.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/local_training_message_handler.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/local_training_message_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/progress_bar.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/progress_bar.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/training.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/training.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/autoai/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/autoai/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
-
+from __future__ import annotations
 
 __all__ = [
     'fetch_pipelines',
     'load_file_from_file_system',
     'load_file_from_file_system_nonautoai',
     'NextRunDetailsGenerator',
     'prepare_auto_ai_model_to_publish_normal_scenario',
@@ -180,15 +180,15 @@
 
     path = os.path.abspath(path)
     pipelines_names = []
     pipelines = {}
     check_lale = True
     is_ts_metrics = 'timeseries' in run_params['entity']['status'].get('metrics', [None])[0]['context']
 
-    if api_client.ICP:
+    if api_client.ICP_PLATFORM_SPACES:
         model_paths = []
 
         # note: iterate over all computed pipelines
         for pipeline in run_params['entity']['status'].get('metrics', []):
             model_number = pipeline['context']['intermediate_model']['name'].split('P')[-1]
             model_phase = chose_model_output(model_number=model_number, is_ts_metrics=is_ts_metrics, run_params=run_params)
 
@@ -358,15 +358,15 @@
     if wml_client is None and api_client is None:
         raise WMLClientError("No API client provided")
     # --- end note
             
     path = os.path.abspath(path)
     is_ts_metrics = 'timeseries' in run_params['entity']['status'].get('metrics', [None])[0]['context']
 
-    if api_client.ICP:
+    if api_client.ICP_PLATFORM_SPACES:
         # note: iterate over all computed pipelines
         for pipeline in run_params['entity']['status'].get('metrics', []):
             model_number = pipeline['context']['intermediate_model']['name'].split('P')[-1]
             if pipeline_name == f"Pipeline_{model_number}":
                 model_phase = chose_model_output(model_number=model_number, is_ts_metrics=is_ts_metrics, run_params=run_params)
 
                 # note: populate available pipeline names
@@ -561,15 +561,15 @@
     
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.next_href is not None:
             response = requests.get(
-                url=f"{self.api_client.api_credentials['url']}{self.next_href}",
+                url=f"{self.api_client.credentials.url}{self.next_href}",
                 headers=self.api_client._get_headers())
             details = response.json()
             self.next_href = details.get('next', {'href': None})['href']
             return details.get('resources', [])
 
         else:
             raise StopIteration
@@ -633,15 +633,15 @@
 
 def prepare_auto_ai_model_to_publish_notebook_normal_scenario(
         pipeline_model: Union['Pipeline', 'TrainablePipeline'],
         result_connection,
         cos_client,
         run_params: Dict,
         space_id: str,
-        auto_pipelines_parameters=None) -> Tuple[str, Dict[str, dict]]:
+        auto_pipelines_parameters=None) -> tuple[str, dict[str, Any]]:
     """Prepares autoai model to publish in Watson Studio via COS.
     Option only for auto-gen notebooks with correct result references on COS.
 
     :param pipeline_model: model object to publish
     :type pipeline_model: Pipeline or TrainablePipeline
     :param result_connection: connection object with COS credentials and all needed locations for jsons
     :type result_connection: DataConnection
@@ -705,15 +705,15 @@
         pipeline_model: Union['Pipeline', 'TrainablePipeline'],
         run_params: dict,
         run_id: str,
         api_client: Optional['APIClient'] = None,
         space_id: Optional[str] = None,
         result_reference: 'DataConnection' = None,
         auto_pipelines_parameters: dict = None,
-        **kwargs) -> Union[Tuple[str, Dict[str, dict]]]:
+        **kwargs) -> tuple[str, dict[str, Any]]:
     """Helper function to specify `content_location` statement for AutoAI models to store in repository.
 
     :param pipeline_model: model that will be prepared for an upload
     :type pipeline_model: Pipeline or TrainablePipeline
     :param run_params: fetched details of the run/fit
     :type run_params: dict
     :param run_id: fit/run ID associated with the model
@@ -764,16 +764,16 @@
 
 
 # TODO: remove this function
 def prepare_auto_ai_model_to_publish(
         pipeline_model: Union['Pipeline', 'TrainablePipeline'],
         run_params: dict,
         run_id: str,
-        api_client: Optional['APIClient'] = None,
-        **kwargs) -> Union[Tuple[Dict[str, dict], str], str]:
+        api_client: APIClient | None = None,
+        **kwargs) -> tuple[dict[str, dict], str]:
     """Helper function to download and load computed AutoAI pipelines (sklearn pipelines).
 
     :param pipeline_model: model that will be prepared for an upload
     :type pipeline_model: Pipeline or TrainablePipeline
     :param run_params: fetched details of the run/fit
     :type run_params: dict
     :param run_id: fit/run ID associated with the model
@@ -802,29 +802,29 @@
     is_ml_metrics = 'ml_metrics' in run_params['entity']['status'].get('metrics')[-1]
     is_ts_metrics = 'ts_metrics' in run_params['entity']['status'].get('metrics')[-1]
     is_tsad_metrics = 'tsad_metrics' in run_params['entity']['status'].get('metrics')[-1]
 
     if not is_ml_metrics and not is_ts_metrics and not is_tsad_metrics:
         raise NoAvailableMetrics()
 
-    artifact_type = ".tar.gz" if api_client.ICP else ".gzip"
+    artifact_type = ".tar.gz" if api_client.ICP_PLATFORM_SPACES else ".gzip"
 
     artifact_name = f"artifact_auto_ai_model{artifact_type}"
     model_artifact_name = f"model_{run_id}.tar.gz"
     pipeline_definition_name = "pipeline-model.json"
     temp_model_name = '__temp_model.pickle'
     temp_ts_model_name = "model.gzip"
 
     # note: prepare file paths of pipeline-model and schema (COS / file system location)
     pipeline_info = run_params['entity']['status'].get('metrics')[-1]
     pipeline_model_path = f"{pipeline_info['context']['intermediate_model']['location']['pipeline_model']}"
     schema_path = f"{pipeline_info['context']['intermediate_model']['schema_location']}"
     # --- end note
 
-    if api_client.ICP:
+    if api_client.ICP_PLATFORM_SPACES:
         # note: downloading pipeline-model.json and schema.json from file system on CP4D
         schema_json = load_file_from_file_system(api_client=api_client, file_path=schema_path).read().decode()
         pipeline_model_json = load_file_from_file_system(api_client=api_client,
                                                          file_path=pipeline_model_path).read().decode()
         with open(pipeline_definition_name, 'w') as f:
             f.write(pipeline_model_json)
         # --- end note
@@ -1935,15 +1935,15 @@
     if is_ml_metrics:
         model_output = chose_model_output(model_number=model_number, run_params=run_params)
     elif is_ts_metrics or is_tsad_metrics:
         model_output = 'after_final_pipelines_generation'
 
     request_path = f"{schema_path.rsplit('/data/', 1)[0]}/assets/{run_id}_P{model_number}_{model_output}/resources/wml_model/request.json"
 
-    if api_client.ICP:
+    if api_client.ICP_PLATFORM_SPACES:
         request_bytes = load_file_from_file_system(api_client=api_client, file_path=request_path).read()
         try:
             request_str = request_bytes.decode()
         except Exception as e:
             if auto_pipelines_parameters:
                 request_str = request_bytes.decode(encoding=auto_pipelines_parameters.get('encoding'))
             else:
@@ -2271,15 +2271,15 @@
 
             if estimator.endswith('Estimator)') and estimator[:-10] + ")" in alg_names:
                 return alg(estimator[:-10] + ")")
 
     return estimator
 
 
-def convert_dataframe_to_fields_values_payload(df: 'DataFrame', return_values_only=False) -> Dict[str, List]:
+def convert_dataframe_to_fields_values_payload(df: 'DataFrame', return_values_only=False) -> dict[str, Any]:
     if isinstance(df, pd.DataFrame):
 
         data = df.where(pd.notnull(df), None)
         data.fillna(json.dumps(float("nan")), inplace=True)
         values = data.values
 
         # note: scoring endpoint could not recognize NaN values, convert NaN to None
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/cpd_version.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/cpd_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from typing import Optional
+from typing import cast
 
 from ibm_watsonx_ai.wml_client_error import WMLClientError
 from ibm_watsonx_ai.messages.messages import Messages
 
 
 class CPDVersion:
-    """Storage for cpd version. Comparison operators are 
-    overloaded to allow comparison with numeric values. 
+    """Storage for cpd version. Comparison operators are
+    overloaded to allow comparison with numeric values.
 
     Class attribute:
     :param supported_version_list: List of supported CPD versions.
     :type supported_version_list: list
 
     Attribute:
     :param cpd_version: Store CPD version.
@@ -32,63 +32,68 @@
 
         version.cpd_version = '4.5'
 
         if version > 4:
             print("version greater than 4.0")
 
     """
-    supported_version_list = ['4.0', '4.5', '4.6', '4.7', '4.8', '5.0']
 
-    def __init__(self, version: Optional[str] = None):
+    supported_version_list = ["4.0", "4.5", "4.6", "4.7", "4.8", "5.0"]
+
+    def __init__(self, version: str | None = None):
         self.cpd_version = version
 
-    def __str__(self):
-        version = self.__cpd_version
+    def __str__(self) -> str:
+        version = self.__cpd_version  # type: ignore[has-type]
         return f"CPD version {version}" if version is not None else ""
 
     @property
-    def cpd_version(self):
+    def cpd_version(self) -> float:
         """Attribute that stores cpd version. Before the value is set,
-          validation is performed against a supported versions.
+        validation is performed against a supported versions.
         """
-        return self.__cpd_version
+        return self.__cpd_version  # type: ignore[has-type]
 
     @cpd_version.setter
-    def cpd_version(self, value):
+    def cpd_version(self, value: float | str) -> None:
         if value is None:
             self.__cpd_version = value
         elif str(value) in CPDVersion.supported_version_list:
-            self.__cpd_version = str(value)
+            self.__cpd_version = str(value)  # type: ignore[has-type]
         else:
-            raise WMLClientError(Messages.get_message(', '.join(CPDVersion.supported_version_list),
-                                                      message_id="invalid_version"))
+            raise WMLClientError(
+                Messages.get_message(
+                    ", ".join(CPDVersion.supported_version_list),
+                    message_id="invalid_version",
+                )
+            )
 
     @cpd_version.getter
-    def cpd_version(self):
-        value = self.__cpd_version
+    def cpd_version(self) -> float | None:
+        value = self.__cpd_version  # type: ignore[has-type]
         if value is None:
             return None
         else:
             dot_index = value.find(".")
-            value = value[:dot_index + 1] + value[dot_index + 1:].replace(".", "")
+            value = value[: dot_index + 1] + value[dot_index + 1 :].replace(".", "")
             return float(value)
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self.cpd_version)
 
-    def __eq__(self, value):
+    def __eq__(self, value: float) -> bool:  # type: ignore[override]
         return self.cpd_version == value
 
-    def __ne__(self, value):
+    def __ne__(self, value: float) -> bool:  # type: ignore[override]
         return not self.__eq__(value)
 
-    def __lt__(self, value):
+    def __lt__(self, value: float) -> bool:
         return bool(self) and self.cpd_version.__lt__(value)
 
-    def __le__(self, value):
+    def __le__(self, value: float) -> bool:
         return bool(self) and (self.__lt__(value) or self.__eq__(value))
 
-    def __gt__(self, value):
+    def __gt__(self, value: float) -> bool:
         return bool(self) and not self.__le__(value)
 
-    def __ge__(self, value):
+    def __ge__(self, value: float) -> bool:
         return bool(self) and not self.__lt__(value)
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/enums.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/utils/utils.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,263 +1,330 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
-from __future__ import print_function
+from __future__ import annotations
 import re
 import os
 import sys
 import shutil
 import tarfile
 import logging
 import importlib.util
 import json
 import numpy
+import importlib
 
-from typing import Optional
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Type,
+    Generator,
+    TypeAlias,
+    cast,
+)
 from subprocess import check_call
 from packaging import version
+from warnings import warn
 
 import ibm_watsonx_ai._wrappers.requests as requests
 
-from ibm_watsonx_ai.wml_client_error import WMLClientError, CannotInstallLibrary
-
-INSTANCE_DETAILS_TYPE = u'instance_details_type'
-PIPELINE_DETAILS_TYPE = u'pipeline_details_type'
-DEPLOYMENT_DETAILS_TYPE = u'deployment_details_type'
-EXPERIMENT_RUN_DETAILS_TYPE = u'experiment_run_details_type'
-MODEL_DETAILS_TYPE = u'model_details_type'
-DEFINITION_DETAILS_TYPE = u'definition_details_type'
-EXPERIMENT_DETAILS_TYPE = u'experiment_details_type'
-TRAINING_RUN_DETAILS_TYPE = u'training_run_details_type'
-FUNCTION_DETAILS_TYPE = u'function_details_type'
-DATA_ASSETS_DETAILS_TYPE = u'data_assets_details_type'
-SW_SPEC_DETAILS_TYPE = u'sw_spec_details_type'
-HW_SPEC_DETAILS_TYPE = u'hw_spec_details_type'
-RUNTIME_SPEC_DETAILS_TYPE = u'runtime_spec_details_type'
-LIBRARY_DETAILS_TYPE = u'library_details_type'
-SPACES_DETAILS_TYPE = u'spaces_details_type'
-MEMBER_DETAILS_TYPE = u'member_details_type'
-CONNECTION_DETAILS_TYPE = u'connection_details_type'
-PKG_EXTN_DETAILS_TYPE = u'pkg_extn_details_type'
-UNKNOWN_ARRAY_TYPE = u'resource_type'
-UNKNOWN_TYPE = u'unknown_type'
-SPACES_IMPORTS_DETAILS_TYPE = u'spaces_imports_details_type'
-SPACES_EXPORTS_DETAILS_TYPE = u'spaces_exports_details_type'
-
-SPARK_MLLIB = u'mllib'
-SPSS_FRAMEWORK = u'spss-modeler'
-TENSORFLOW_FRAMEWORK = u'tensorflow'
-XGBOOST_FRAMEWORK = u'xgboost'
-SCIKIT_LEARN_FRAMEWORK = u'scikit-learn'
-PMML_FRAMEWORK = u'pmml'
-
-
-def is_python_2():
-    return sys.version_info[0] == 2
-
-
-def get_url(url, headers, params=None, isIcp=False):
-    import ibm_watsonx_ai._wrappers.requests as requests
+from ibm_watsonx_ai.wml_client_error import (
+    WMLClientError,
+    CannotInstallLibrary,
+)
+
+if TYPE_CHECKING:
+    import pyspark
+    import collections
+    from types import TracebackType
+    from ibm_watsonx_ai import APIClient
+    from IPython.display import HTML
+    from requests import Response
+
+    PipelineType: TypeAlias = Any
+    MLModelType: TypeAlias = Any
+
+INSTANCE_DETAILS_TYPE = "instance_details_type"
+PIPELINE_DETAILS_TYPE = "pipeline_details_type"
+DEPLOYMENT_DETAILS_TYPE = "deployment_details_type"
+EXPERIMENT_RUN_DETAILS_TYPE = "experiment_run_details_type"
+MODEL_DETAILS_TYPE = "model_details_type"
+DEFINITION_DETAILS_TYPE = "definition_details_type"
+EXPERIMENT_DETAILS_TYPE = "experiment_details_type"
+TRAINING_RUN_DETAILS_TYPE = "training_run_details_type"
+FUNCTION_DETAILS_TYPE = "function_details_type"
+DATA_ASSETS_DETAILS_TYPE = "data_assets_details_type"
+SW_SPEC_DETAILS_TYPE = "sw_spec_details_type"
+HW_SPEC_DETAILS_TYPE = "hw_spec_details_type"
+RUNTIME_SPEC_DETAILS_TYPE = "runtime_spec_details_type"
+LIBRARY_DETAILS_TYPE = "library_details_type"
+SPACES_DETAILS_TYPE = "spaces_details_type"
+MEMBER_DETAILS_TYPE = "member_details_type"
+CONNECTION_DETAILS_TYPE = "connection_details_type"
+PKG_EXTN_DETAILS_TYPE = "pkg_extn_details_type"
+UNKNOWN_ARRAY_TYPE = "resource_type"
+UNKNOWN_TYPE = "unknown_type"
+SPACES_IMPORTS_DETAILS_TYPE = "spaces_imports_details_type"
+SPACES_EXPORTS_DETAILS_TYPE = "spaces_exports_details_type"
+
+SPARK_MLLIB = "mllib"
+SPSS_FRAMEWORK = "spss-modeler"
+TENSORFLOW_FRAMEWORK = "tensorflow"
+XGBOOST_FRAMEWORK = "xgboost"
+SCIKIT_LEARN_FRAMEWORK = "scikit-learn"
+PMML_FRAMEWORK = "pmml"
+
+
+def _get_id_from_deprecated_uid(
+    kwargs: dict, resource_id: str | None, resource_name: str, can_be_none: bool = False
+) -> str:
+    if (resource_uid := kwargs.get(resource_name + "_uid")) is not None:
+        warn(
+            f"`{resource_name}_uid` parameter is deprecated, please use `{resource_name}_id`",
+            category=DeprecationWarning,
+        )
+        if not resource_id:
+            resource_id = resource_uid
+    elif not can_be_none and resource_uid is None and resource_id is None:
+        raise TypeError(
+            f"Function missing 1 required positional argument: '{resource_name}_id'"
+        )
+
+    return resource_id
+
+
+def get_url(
+    url: str, headers: dict, params: dict | None = None, isIcp: bool = False
+) -> Response:
 
     if isIcp:
         return requests.get(url, headers=headers, params=params)
     else:
         return requests.get(url, headers=headers, params=params)
 
 
-def print_text_header_h1(title):
-    print(u'\n\n' + (u'#' * len(title)) + u'\n')
+def print_text_header_h1(title: str) -> None:
+    print("\n\n" + ("#" * len(title)) + "\n")
     print(title)
-    print(u'\n' + (u'#' * len(title)) + u'\n\n')
+    print("\n" + ("#" * len(title)) + "\n\n")
 
 
-def print_text_header_h2(title):
-    print(u'\n\n' + (u'-' * len(title)))
+def print_text_header_h2(title: str) -> None:
+    print("\n\n" + ("-" * len(title)))
     print(title)
-    print((u'-' * len(title)) + u'\n\n')
+    print(("-" * len(title)) + "\n\n")
 
 
-def get_type_of_details(details):
-    if 'resources' in details:
+def get_type_of_details(details: dict) -> str:
+    if "resources" in details:
         return UNKNOWN_ARRAY_TYPE
     elif details is None:
-        raise WMLClientError('Details doesn\'t exist.')
+        raise WMLClientError("Details doesn't exist.")
     else:
         try:
-            plan = 'plan' in details[u'entity']
+            plan = "plan" in details["entity"]
 
             if plan:
                 return INSTANCE_DETAILS_TYPE
 
-            if re.search(u'\/wml_instances\/[^\/]+$', details[u'metadata'][u'url']) is not None:
+            if (
+                re.search("\/wml_instances\/[^\/]+$", details["metadata"]["url"])
+                is not None
+            ):
                 return INSTANCE_DETAILS_TYPE
         except:
             pass
         try:
-            if re.search(u'\/pipelines\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search("\/pipelines\/[^\/]+$", details["metadata"]["href"])
+                is not None
+            ):
                 return PIPELINE_DETAILS_TYPE
         except:
             pass
         try:
-            if 'href' in details[u'metadata'] and re.search(u'\/deployments\/[^\/]+$', details[u'metadata'][u'href']) is not None \
-                    or re.search(u'\/deployments\/[^\/]+$', details[u'metadata'][u'id']) is not None \
-                    or u'virtual_deployment_downloads' in details[u'entity'][u'status']:
+            if (
+                "href" in details["metadata"]
+                and re.search("\/deployments\/[^\/]+$", details["metadata"]["href"])
+                is not None
+                or re.search("\/deployments\/[^\/]+$", details["metadata"]["id"])
+                is not None
+                or "virtual_deployment_downloads" in details["entity"]["status"]
+            ):
                 return DEPLOYMENT_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/experiments\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search("\/experiments\/[^\/]+$", details["metadata"]["href"])
+                is not None
+            ):
                 return EXPERIMENT_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/trainings\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search("\/trainings\/[^\/]+$", details["metadata"]["href"])
+                is not None
+            ):
                 return TRAINING_RUN_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/models\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/models\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return MODEL_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/functions\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search("\/functions\/[^\/]+$", details["metadata"]["href"])
+                is not None
+            ):
                 return FUNCTION_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/runtimes\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search("\/runtimes\/[^\/]+$", details["metadata"]["href"])
+                is not None
+            ):
                 return RUNTIME_SPEC_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/libraries\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search("\/libraries\/[^\/]+$", details["metadata"]["href"])
+                is not None
+            ):
                 return LIBRARY_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/spaces\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/spaces\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return SPACES_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/members\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/members\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return MEMBER_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/members\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/members\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return MEMBER_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/assets\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/assets\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return DATA_ASSETS_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/software_specifications\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search(
+                    "\/software_specifications\/[^\/]+$", details["metadata"]["href"]
+                )
+                is not None
+            ):
                 return SW_SPEC_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/hardware_specifications\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if (
+                re.search(
+                    "\/hardware_specifications\/[^\/]+$", details["metadata"]["href"]
+                )
+                is not None
+            ):
                 return HW_SPEC_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/package_extension\/[^\/]+$', details[u'entity'][u'package_extension'][u'href']) is not None:
+            if (
+                re.search(
+                    "\/package_extension\/[^\/]+$",
+                    details["entity"]["package_extension"]["href"],
+                )
+                is not None
+            ):
                 return PKG_EXTN_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/imports\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/imports\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return SPACES_IMPORTS_DETAILS_TYPE
         except:
             pass
 
         try:
-            if re.search(u'\/exports\/[^\/]+$', details[u'metadata'][u'href']) is not None:
+            if re.search("\/exports\/[^\/]+$", details["metadata"]["href"]) is not None:
                 return SPACES_EXPORTS_DETAILS_TYPE
         except:
             pass
 
         return UNKNOWN_TYPE
 
 
-def load_model_from_directory(framework, directory_path):
+def load_model_from_directory(
+    framework: dict, directory_path: str
+) -> pyspark.ml.pipeline.PipelineModel | None:
     if "mllib" in framework:
-     from pyspark.ml import PipelineModel
-     return PipelineModel.read().load(directory_path)
+        from pyspark.ml import PipelineModel
+
+        return PipelineModel.read().load(directory_path)
     if "spss" in framework:
-     pass
+        pass
     if "tensorflow" in framework:
-     pass
+        pass
     if "scikit" in framework or "xgboost" in framework:
         try:
             try:
                 from sklearn.externals import joblib
             except ImportError:
                 import joblib
-            pkl_files = [x for x in os.listdir(directory_path) if x.endswith('.pkl')]
+            pkl_files = [x for x in os.listdir(directory_path) if x.endswith(".pkl")]
 
             if len(pkl_files) < 1:
-                raise WMLClientError('No pkl files in directory.')
+                raise WMLClientError("No pkl files in directory.")
 
             model_id = pkl_files[0]
             return joblib.load(os.path.join(directory_path, model_id))
         except Exception as e:
-            raise WMLClientError('Cannot load model from pkl file.', e)
+            raise WMLClientError("Cannot load model from pkl file.", e)
     if "pmml" in framework:
-     pass
+        return None
     else:
-        raise WMLClientError(u'Invalid framework specified: \'{}\'.'.format(framework))
+        raise WMLClientError("Invalid framework specified: '{}'.".format(framework))
 
 
-# def load_model_from_directory(framework, directory_path):
-#     if framework == SPARK_MLLIB:
-#         from pyspark.ml import PipelineModel
-#         return PipelineModel.read().load(directory_path)
-#     elif framework == SPSS_FRAMEWORK:
-#         pass
-#     elif framework == TENSORFLOW_FRAMEWORK:
-#         pass
-#     elif framework == SCIKIT_LEARN_FRAMEWORK or framework == XGBOOST_FRAMEWORK:
-#         from sklearn.externals import joblib
-#         model_id = directory_path[directory_path.rfind('/') + 1:] + ".pkl"
-#         return joblib.load(os.path.join(directory_path, model_id))
-#     elif framework == PMML_MODEL:
-#         pass
-#     else:
-#         raise WMLClientError('Invalid framework specified: \'{}\'.'.format(framework))
-
-
-def save_model_to_file(model, framework, base_path, filename):
-    if filename.find('.') != -1:
-        base_name = filename[:filename.find('.') + 1]
-        file_extension = filename[filename.find('.'):]
+def save_model_to_file(
+    model: MLModelType, framework: str, base_path: str, filename: str
+) -> None:
+    if filename.find(".") != -1:
+        base_name = filename[: filename.find(".") + 1]
     else:
         base_name = filename
-        file_extension = 'tar.gz'
 
     if framework == SPARK_MLLIB:
         model.write.overwrite.save(os.path.join(base_path, base_name))
     elif framework == SPSS_FRAMEWORK:
         pass
     elif framework == TENSORFLOW_FRAMEWORK:
         pass
@@ -269,328 +336,386 @@
             from sklearn.externals import joblib
         except ImportError:
             import joblib
         joblib.dump(model, os.path.join(base_path, base_name, base_name + ".pkl"))
     elif framework == PMML_FRAMEWORK:
         pass
     else:
-        raise WMLClientError(u'Invalid framework specified: \'{}\'.'.format(framework))
+        raise WMLClientError("Invalid framework specified: '{}'.".format(framework))
 
 
-def format_metrics(latest_metrics_list):
-    formatted_metrics = u''
+def format_metrics(latest_metrics_list: list[dict]) -> str:
+    formatted_metrics = ""
 
     for i in latest_metrics_list:
 
-        values = i[u'values']
+        values = i["values"]
 
         if len(values) > 0:
-            sorted_values = sorted(values, key=lambda k: k[u'name'])
+            sorted_values = sorted(values, key=lambda k: k["name"])
         else:
             sorted_values = values
 
         for j in sorted_values:
-            formatted_metrics = formatted_metrics + i[u'phase'] + ':' + j[u'name']+'='+'{0:.4f}'.format(j[u'value']) + '\n'
+            formatted_metrics = (
+                formatted_metrics
+                + i["phase"]
+                + ":"
+                + j["name"]
+                + "="
+                + "{0:.4f}".format(j["value"])
+                + "\n"
+            )
 
     return formatted_metrics
 
 
-def inherited_docstring(f, mapping={}):
-    def dec(obj):
+def inherited_docstring(f: Callable, mapping: dict = {}) -> Callable:
+    def dec(obj: Callable) -> Callable:
         if not obj.__doc__:
-            possible_types = {'model': 'model',
-                              'function': 'function',
-                              'space': 'space',
-                              'pipeline': 'pipeline',
-                              'experiment': 'experiment',
-                              'member': 'space'}
-
-            available_metanames = {'model': 'ModelMetaNames',
-                                   'experiment': 'ExperimentMetaNames',
-                                   'function': 'FunctionMetaNames',
-                                   'pipeline': 'PipelineMetaNames'}
+            possible_types = {
+                "model": "model",
+                "function": "function",
+                "space": "space",
+                "pipeline": "pipeline",
+                "experiment": "experiment",
+                "member": "space",
+            }
+
+            available_metanames = {
+                "model": "ModelMetaNames",
+                "experiment": "ExperimentMetaNames",
+                "function": "FunctionMetaNames",
+                "pipeline": "PipelineMetaNames",
+            }
 
             actual_type = None
 
             for t in possible_types:
                 if t in obj.__name__:
                     actual_type = possible_types[t]
 
-            docs = f.__doc__
+            docs = cast(str, f.__doc__)
 
             if actual_type:
-                docs = docs.replace(f'client.{actual_type}s.{f.__name__}', 'client.repository.' + obj.__name__)
-                docs = docs.replace(f'client._{actual_type}s.{f.__name__}', 'client.repository.' + obj.__name__)
+                docs = docs.replace(
+                    f"client.{actual_type}s.{f.__name__}",
+                    "client.repository." + obj.__name__,
+                )
+                docs = docs.replace(
+                    f"client._{actual_type}s.{f.__name__}",
+                    "client.repository." + obj.__name__,
+                )
 
                 if actual_type in available_metanames:
                     repository_meta_names = available_metanames[actual_type]
-                    docs = docs.replace(f'_{actual_type}s.ConfigurationMetaNames', f'repository.{repository_meta_names}')
-                    docs = docs.replace(f'{actual_type}s.ConfigurationMetaNames', f'repository.{repository_meta_names}')
-                    docs = docs.replace('ConfigurationMetaNames', repository_meta_names)
+                    docs = docs.replace(
+                        f"_{actual_type}s.ConfigurationMetaNames",
+                        f"repository.{repository_meta_names}",
+                    )
+                    docs = docs.replace(
+                        f"{actual_type}s.ConfigurationMetaNames",
+                        f"repository.{repository_meta_names}",
+                    )
+                    docs = docs.replace("ConfigurationMetaNames", repository_meta_names)
 
                 for k in mapping:
                     docs = docs.replace(k, mapping[k])
             obj.__doc__ = docs
         return obj
+
     return dec
 
 
-def group_metrics(metrics):
-    grouped_metrics = []
+def group_metrics(metrics: list[dict]) -> list | collections.defaultdict:
+    grouped_metrics: list | collections.defaultdict = []
 
     if len(metrics) > 0:
         import collections
+
         grouped_metrics = collections.defaultdict(list)
         for d in metrics:
-            k = d[u'phase']
+            k = d["phase"]
             grouped_metrics[k].append(d)
 
     return grouped_metrics
 
 
 class StatusLogger:
-    def __init__(self, initial_state):
+    def __init__(self, initial_state: str):
         self.last_state = initial_state
-        print(initial_state, end='')
+        print(initial_state, end="")
 
-    def log_state(self, state):
+    def log_state(self, state: str) -> None:
         if state == self.last_state:
-            print('.', end='')
+            print(".", end="")
         else:
-            print('\n{}'.format(state), end='')
+            print("\n{}".format(state), end="")
             self.last_state = state
 
-    def __enter__(self):
+    def __enter__(self) -> StatusLogger:
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(
+        self,
+        exc_type: Type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         pass
 
 
-def get_file_from_cos(cos_credentials):
+def get_file_from_cos(cos_credentials: dict) -> str:
     import ibm_boto3
     from ibm_botocore.client import Config
 
-    client_cos = ibm_boto3.client(service_name='s3',
-        ibm_api_key_id=cos_credentials['IBM_API_KEY_ID'],
-        ibm_auth_endpoint=cos_credentials['IBM_AUTH_ENDPOINT'],
-        config=Config(signature_version='oauth'),
-        endpoint_url=cos_credentials['ENDPOINT'])
-
-    streaming_body = client_cos.get_object(Bucket=cos_credentials['BUCKET'], Key=cos_credentials['FILE'])['Body']
+    client_cos = ibm_boto3.client(
+        service_name="s3",
+        ibm_api_key_id=cos_credentials["IBM_API_KEY_ID"],
+        ibm_auth_endpoint=cos_credentials["IBM_AUTH_ENDPOINT"],
+        config=Config(signature_version="oauth"),
+        endpoint_url=cos_credentials["ENDPOINT"],
+    )
+
+    streaming_body = client_cos.get_object(
+        Bucket=cos_credentials["BUCKET"], Key=cos_credentials["FILE"]
+    )["Body"]
     training_definition_bytes = streaming_body.read()
     streaming_body.close()
-    filename = cos_credentials['FILE']
-    f = open(filename, 'wb')
+    filename = cos_credentials["FILE"]
+    f = open(filename, "wb")
     f.write(training_definition_bytes)
     f.close()
 
     return filename
 
 
-def extract_model_from_repository(model_uid, client):
+def extract_model_from_repository(
+    model_id: str, client: APIClient, **kwargs: Any
+) -> str:
     """Download and extract archived model from wml repository.
 
-    :param model_uid: UID of model
-    :type model_uid: str
+    :param model_id: ID of model
+    :type model_id: str
     :param client: client instance
     :type client: APIClient
 
     :return: extracted directory path
     :rtype: str
     """
-    create_empty_directory(model_uid)
+    model_id = _get_id_from_deprecated_uid(kwargs, model_id, "model")
+    create_empty_directory(model_id)
     current_dir = os.getcwd()
 
-    os.chdir(model_uid)
+    os.chdir(model_id)
     model_dir = os.getcwd()
 
-    fname = 'downloaded_' + model_uid + '.tar.gz'
-    client.repository.download(model_uid, filename=fname)
+    fname = "downloaded_" + model_id + ".tar.gz"
+    client.repository.download(model_id, filename=fname)
 
     if fname.endswith("tar.gz"):
         tar = tarfile.open(fname)
         tar.extractall()
         tar.close()
     else:
-        raise WMLClientError('Invalid type. Expected tar.gz')
+        raise WMLClientError("Invalid type. Expected tar.gz")
 
     os.chdir(current_dir)
     return model_dir
 
 
-def extract_mlmodel_from_archive(archive_path, model_uid):
-    """Extract archived model under model uid directory.
+def extract_mlmodel_from_archive(
+    archive_path: str, model_id: str, **kwargs: Any
+) -> str:
+    """Extract archived model under model id directory.
 
-    :param model_uid: UID of model
-    :type model_uid: str
+    :param model_id: ID of model
+    :type model_id: str
     :param archive_path: path to archived model
     :type archive_path: str
 
     :return: extracted directory path
     :rtype: str
     """
-    create_empty_directory(model_uid)
+    model_id = _get_id_from_deprecated_uid(kwargs, model_id, "model")
+    create_empty_directory(model_id)
     current_dir = os.getcwd()
 
-    os.rename(archive_path, os.path.join(model_uid, archive_path))
+    os.rename(archive_path, os.path.join(model_id, archive_path))
 
-    os.chdir(model_uid)
-    model_dir = os.getcwd()
+    os.chdir(model_id)
 
     if archive_path.endswith("tar.gz"):
         tar = tarfile.open(archive_path)
         tar.extractall()
         tar.close()
     else:
-        raise WMLClientError('Invalid type. Expected tar.gz')
+        raise WMLClientError("Invalid type. Expected tar.gz")
 
     os.chdir(current_dir)
-    return os.path.join(model_uid, 'model.mlmodel')
+    return os.path.join(model_id, "model.mlmodel")
 
 
-def get_model_filename(directory, model_extension):
+def get_model_filename(directory: str, model_extension: str) -> str:
     logger = logging.getLogger(__name__)
     model_filepath = None
 
     for file in os.listdir(directory):
         if file.endswith(model_extension):
             if model_filepath is None:
                 model_filepath = os.path.join(directory, file)
             else:
-                logger.warning('More than one file with extension \'{}\'.'.format(model_extension))
+                logger.warning(
+                    "More than one file with extension '{}'.".format(model_extension)
+                )
 
     if model_filepath is None:
-        raise WMLClientError('No file with extension \'{}\'.'.format(model_extension))
+        raise WMLClientError("No file with extension '{}'.".format(model_extension))
 
     return model_filepath
 
 
-def delete_directory(directory):
+def delete_directory(directory: str) -> None:
     if os.path.exists(directory):
         shutil.rmtree(directory)
 
 
-def create_empty_directory(directory):
+def create_empty_directory(directory: str) -> None:
     delete_directory(directory)
     os.makedirs(directory)
 
 
-def install_package(package):
+def install_package(package: str) -> None:
     import importlib
+
     try:
         importlib.import_module(package)
     except ImportError:
         import pip
-        pip.main(['install', package])
+
+        pip.main(["install", package])
 
 
-def is_ipython():
+def is_ipython() -> bool:
     # checks if the code is run in the notebook
     try:
-        get_ipython
+        get_ipython  # type: ignore[name-defined]
         return True
     except Exception:
         return False
 
 
-def create_download_link(file_path, title="Download file."):
+def create_download_link(file_path: str, title: str = "Download file.") -> HTML | None:
     # creates download link for binary files on notebook filesystem (Watson Studio)
 
     if is_ipython():
         from IPython.display import HTML
         import base64
 
         filename = os.path.basename(file_path)
 
-        with open(file_path, 'rb') as file:
+        with open(file_path, "rb") as file:
             b_model = file.read()
         b64 = base64.b64encode(b_model)
         payload = b64.decode()
         html = '<a download="{file_path}" href="data:binary;base64,{payload}" target="_blank">{title}</a>'
         html = html.format(payload=payload, title=title, file_path=filename)
 
         return HTML(html)
 
+    return None
 
-def convert_metadata_to_parameters(meta_data):
+
+def convert_metadata_to_parameters(meta_data: dict) -> list:
     parameters = []
 
     if meta_data is not None:
-        if is_python_2():
-            for key, value in meta_data.iteritems():
-                parameters.append({'name': str(key), 'value': value})
-        else:
-            for key, value in meta_data.items():
-                parameters.append({'name': str(key), 'value': value})
+        for key, value in meta_data.items():
+            parameters.append({"name": str(key), "value": value})
 
     return parameters
 
 
-def is_of_python_basic_type(el):
-    if type(el) in [int, float, bool, str]:
+def is_of_python_basic_type(el: object | list | None) -> bool:
+    if el is None:
+        return True
+    elif type(el) in [int, float, bool, str]:
         return True
     elif type(el) in [list, tuple]:
-        return all([is_of_python_basic_type(t) for t in el])
+        return all([is_of_python_basic_type(t) for t in cast(Iterable, el)])
     elif type(el) is dict:
         if not all(type(k) == str for k in el.keys()):
             return False
 
         return is_of_python_basic_type(list(el.values()))
     else:
         return False
 
 
 class NextResourceGenerator:
     """Generator class to produce next list of resources from REST API."""
 
-    def __init__(self, wml_client: 'APIClient', url: str, href: str, params: dict = None, _all=False,
-                 _filter_func=None) -> None:
+    def __init__(
+        self,
+        client: APIClient,
+        url: str,
+        href: str,
+        params: dict | None = None,
+        _all: bool = False,
+        _filter_func: Callable | None = None,
+    ) -> None:
         """
-        :param wml_client: WML Client Instance
-        :type wml_client: APIClient
+        :param client: Client Instance
+        :type client: APIClient
 
         :param href: href to the resource
         :type href: str
         """
-        self.wml_client = wml_client
+        self.client = client
         self.url = url
-        self.next_href = href
+        self.next_href: str | None = href
         self.params = params
         self.all = _all
         self._filter_func = _filter_func
 
-    def __iter__(self):
+    def __iter__(self) -> Generator:
         while self.next_href is not None:
             if "http" not in self.next_href:
                 self.next_href = f"{self.url}/{self.next_href}"
             response = requests.get(
-                # url=f"{self.url}/{self.next_href}",
                 url=self.next_href,
-                headers=self.wml_client._get_headers(),
-                params=self.params if self.params is not None else self.wml_client.params()
+                headers=self.client._get_headers(),
+                params=(
+                    self.params if self.params is not None else self.client.params()
+                ),
+            )
+            details_json = self.client.training._handle_response(
+                200, "Get next details", response
             )
-            details_json = self.wml_client.training._handle_response(200, "Get next details", response)
 
             if self.all:
-                self.next_href = details_json.get('next', {'href': None})['href']
+                self.next_href = details_json.get("next", {"href": None})["href"]
 
             else:
                 self.next_href = None
 
-            if 'resources' in details_json:
-                resources = details_json['resources']
+            if "resources" in details_json:
+                resources = details_json["resources"]
 
-            elif 'metadata' in details_json:
+            elif "metadata" in details_json:
                 resources = [details_json]
 
             else:
-                resources = details_json.get('results', [])
+                resources = details_json.get("results", [])
 
-            yield {'resources': self._filter_func(resources) if self._filter_func else resources}
+            yield {
+                "resources": (
+                    self._filter_func(resources) if self._filter_func else resources
+                )
+            }
 
 
 class DisableWarningsLogger:
     """Class which disables logging warnings (for example for silent handling WMLClientErrors in try except).
 
     **Example**
 
@@ -599,22 +724,32 @@
         try:
             with DisableWarningsLogger():
                 throw_wml_error()
         except WMLClientError:
             success = False
 
     """
-    def __enter__(self):
+
+    def __enter__(self) -> None:
         logging.disable(logging.WARNING)
 
-    def __exit__(self, exit_type, exit_value, exit_traceback):
+    def __exit__(
+        self,
+        exit_type: Type[BaseException] | None,
+        exit_value: BaseException | None,
+        exit_traceback: TracebackType | None,
+    ) -> None:
         logging.disable(logging.NOTSET)
 
 
-def is_lib_installed(lib_name: str, minimum_version: Optional[str] = None, install: Optional[bool] = False) -> bool:
+def is_lib_installed(
+    lib_name: str,
+    minimum_version: str | None = None,
+    install: bool = False,
+) -> bool:
     """Check if provided library is installed on user environment. If not, tries to install it.
 
     :param lib_name: library name to check
     :type lib_name: str
 
     :param minimum_version: minimum version of library to check, default: None - check if library is installed in overall
     :type minimum_version: str, optional
@@ -636,39 +771,51 @@
 
     if installed:
         installed_module_version = get_module_version(lib_name)
 
         if minimum_version is not None:
             if version.parse(installed_module_version) < version.parse(minimum_version):
                 if install:
-                    install_library(lib_name=lib_name, version=minimum_version, strict=False)
+                    install_library(
+                        lib_name=lib_name, version=minimum_version, strict=False
+                    )
 
     else:
         if install:
             install_library(lib_name=lib_name, version=minimum_version, strict=False)
             installed = True
 
     return installed
 
 
-def install_library(lib_name: str, version: Optional[str] = None, strict: Optional[bool] = False) -> None:
+def install_library(
+    lib_name: str, version: str | None = None, strict: bool = False
+) -> None:
     """Try to install library.
 
     :param lib_name: library name to install
     :type lib_name: str
 
     :param version: version of the library to install
     :type version: str, optional
 
     :param strict: indicates if we want to install specific version or higher version if available
     :type strict: bool, optional
     """
     try:
         if version is not None:
-            check_call([sys.executable, "-m", "pip", "install", f"{lib_name}{'==' if strict else '>='}{version}"])
+            check_call(
+                [
+                    sys.executable,
+                    "-m",
+                    "pip",
+                    "install",
+                    f"{lib_name}{'==' if strict else '>='}{version}",
+                ]
+            )
 
         else:
             check_call([sys.executable, "-m", "pip", "install", lib_name])
 
     except Exception as e:
         raise CannotInstallLibrary(lib_name=lib_name, reason=str(e))
 
@@ -699,29 +846,31 @@
     encoding = source_params.get("encoding", None)
 
     if ".xls" in file_name or ".xlsx" in file_name:
         file_format = "excel"
         if source_params.get("excel_sheet"):
             interaction_properties["sheet_name"] = str(source_params.get("excel_sheet"))
 
-    elif '.csv' in file_name:
+    elif ".csv" in file_name:
         if source_params.get("quote_character"):
-            interaction_properties["quote_character"] = str(source_params.get("quote_character"))
+            interaction_properties["quote_character"] = str(
+                source_params.get("quote_character")
+            )
         if encoding is not None:
             interaction_properties["encoding"] = encoding
 
         input_file_separator = source_params.get("input_file_separator", ",")
         if input_file_separator != ",":
             file_format = "delimited"
             interaction_properties["field_delimiter"] = input_file_separator
         else:
             file_format = "csv"
 
-    elif '.parquet' in file_name or '.prq' in file_name:
-        file_format = 'parquet'
+    elif ".parquet" in file_name or ".prq" in file_name:
+        file_format = "parquet"
 
     if file_format is not None:
         interaction_properties["file_format"] = file_format
 
     return interaction_properties
 
 
@@ -732,30 +881,35 @@
     :param details_from_get: details of script/shiny app acquired using GET method
     :type details_from_get: dict
 
     :return: details with 'guid' and 'href' key added to 'metadata'
     :rtype: dict
     """
     try:
-        details_from_get[u'metadata'][u'href'] = details_from_get[u'href']
-        details_from_get[u'metadata'][u'guid'] = details_from_get[u'metadata'][u'asset_id']
+        details_from_get["metadata"]["href"] = details_from_get["href"]
+        details_from_get["metadata"]["guid"] = details_from_get["metadata"]["asset_id"]
     except KeyError:
         pass
 
     return details_from_get
 
 
-def is_lale_pipeline(pipeline):
-    return type(pipeline).__module__ == 'lale.operators' and type(pipeline).__qualname__ == 'TrainedPipeline'
+def is_lale_pipeline(pipeline: PipelineType) -> bool:
+    return (
+        type(pipeline).__module__ == "lale.operators"
+        and type(pipeline).__qualname__ == "TrainedPipeline"
+    )
 
 
- 
 class NumpyTypeEncoder(json.JSONEncoder):
     """Extended json.JSONEncoder to encode correctly numpy types."""
-    def default(self, obj):
+
+    def default(
+        self, obj: numpy.integer | numpy.bool_ | numpy.floating | numpy.ndarray
+    ) -> int | bool | float | list | None:
         if isinstance(obj, numpy.integer):
             return int(obj)
         elif isinstance(obj, numpy.bool_):
             return bool(obj)
         elif isinstance(obj, numpy.floating):
             return None if numpy.isnan(obj) else float(obj)
         elif isinstance(obj, numpy.ndarray):
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai/workspace/workspace.py` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai/workspace/workspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 #  -----------------------------------------------------------------------------------------
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
-
+from copy import copy
 from warnings import warn
 
 from ibm_watsonx_ai import APIClient
 from ibm_watsonx_ai.wml_client_error import MissingArgument, WrongEnvironmentVersion
 from ibm_watsonx_ai.wml_client_error import WMLClientError
+from ..credentials import Credentials
 from ..utils.autoai.enums import TShirtSize
 from ..utils.autoai.errors import TShirtSizeNotSupported, SetIDFailed
 from ..utils.autoai.utils import is_ipython
 
 
 class WorkSpace:
     """WorkSpace class for Service authentication and project/space manipulation."""
 
-    def __init__(self,
-                 credentials: dict = None,
-                 project_id: str = None,
-                 space_id: str = None,
-                 verify=None,
-                 **kwargs) -> None:
+    def __init__(
+        self,
+        credentials: Credentials = None,
+        project_id: str = None,
+        space_id: str = None,
+        verify=None,
+        **kwargs,
+    ) -> None:
         """
         :param credentials: credentials to Service instance
         :type credentials: dict
 
         :param project_id: ID of the Watson Studio project
         :type project_id: str, optional
 
@@ -33,155 +36,185 @@
         :type space_id: str, optional
 
         **Example**
 
         .. code-block: python
 
             from ibm_watsonx_ai.workspace import WorkSpace
+            from ibm_watsonx_ai import Credentials
 
             ws = WorkSpace(
-                credentials={
-                    "apikey": "...",
-                    "iam_apikey_description": "...",
-                    "iam_apikey_name": "...",
-                    "iam_role_crn": "...",
-                    "iam_serviceid_crn": "...",
-                    "instance_id": "...",
-                    "url": "https://us-south.ml.cloud.ibm.com"
-                },
+                credentials=Credentials(
+                    api_key= "...",
+                    iam_serviceid_crn = "...",
+                    instance_id = "...",
+                    url = "https://us-south.ml.cloud.ibm.com"
+                ),
                 project_id="...",
                 space_id="...")
         """
         # note: backward compatibility
-        if (wml_credentials:=kwargs.get('wml_credentials')) is not None:
+        if (wml_credentials := kwargs.get("wml_credentials")) is not None:
             credentials = wml_credentials
-            warn(("`wml_credentials` is deprecated and will be removed in future. "
-                  "Instead, please use `credentials`."), category=DeprecationWarning)
+            warn(
+                (
+                    "`wml_credentials` is deprecated and will be removed in future. "
+                    "Instead, please use `credentials`."
+                ),
+                category=DeprecationWarning,
+            )
         if wml_credentials is None and credentials is None:
             raise WMLClientError("No `credentials` provided")
         # --- end note
-        self.credentials = credentials.copy()
+        self.credentials = copy(credentials)
         self.project_id = project_id
         self.space_id = space_id
 
-        self.api_client = APIClient(wml_credentials=self.credentials, verify=verify)
+        self.api_client = APIClient(credentials=self.credentials, verify=verify)
 
-        if not credentials.get('instance_id'):
+        if credentials.instance_id is None:
             if self.space_id is not None:
                 self.api_client.set.default_space(self.space_id)
 
             elif self.project_id is not None:
                 self.api_client.set.default_project(self.project_id)
 
             else:
                 raise SetIDFailed(
-                    f'project_id and space_id',
-                    reason=f'project_id and space_id cannot be None at the same time.')
-
-        elif credentials.get('instance_id', '').lower() in ('icp', 'openshift'):
+                    f"project_id and space_id",
+                    reason=f"project_id and space_id cannot be None at the same time.",
+                )
+
+        elif credentials.instance_id and credentials.instance_id.lower() in (
+            "icp",
+            "openshift",
+        ):
             if self.project_id is None and self.space_id is None:
                 raise MissingArgument(
-                    'project_id',
+                    "project_id",
                     reason="These credentials are from CP4D environment, "
-                           "please specify \"project_id\"")
+                    'please specify "project_id"',
+                )
             else:
                 if self.project_id is not None:
                     outcome = self.api_client.set.default_project(self.project_id)
 
                 else:
                     outcome = self.api_client.set.default_space(self.space_id)
 
-                if outcome == 'FAILURE':
+                if outcome == "FAILURE":
                     raise SetIDFailed(
                         f'{"project_id" if self.project_id is not None else "space_id"}',
                         reason=f'This {"project_id" if self.project_id is not None else "space_id"}: '
                                f'{self.project_id if self.project_id is not None else self.space_id} '
                                f'cannot be found in current environment.')
 
             supported_versions = ('4.0', '4.5', '4.6', '4.7', '4.8', '5.0')
-            if credentials[u'version'] not in supported_versions:
-                raise WrongEnvironmentVersion(credentials[u'version'], credentials[u'instance_id'].lower(),
+            if credentials.version not in supported_versions:
+                raise WrongEnvironmentVersion(credentials.version, credentials.instance_id.lower(),
                                               supported_versions)
 
     def __str__(self):
-        return f'credentials: {self.credentials} project_id: {self.project_id} space_id = {self.space_id}'
+        return f"credentials: {self.credentials} project_id: {self.project_id} space_id = {self.space_id}"
 
     def __repr__(self):
         return self.__str__()
-    
+
     @property
     def wml_credentials(self):
-        warn(("`wml_credentials` is deprecated and will be removed in future. "
-              "Instead, please use `credentials`."), category=DeprecationWarning)
-        return self.credentials
-    
+        warn(
+            (
+                "`wml_credentials` is deprecated and will be removed in future. "
+                "Instead, please use `credentials`."
+            ),
+            category=DeprecationWarning,
+        )
+        return self.credentials.to_dict()
+
     @wml_credentials.setter
     def wml_credentials(self, var):
-        warn(("`wml_credentials` is deprecated and will be removed in future. "
-              "Instead, please use `credentials`."), category=DeprecationWarning)
-        self.credentials = var
+        warn(
+            (
+                "`wml_credentials` is deprecated and will be removed in future. "
+                "Instead, please use `credentials`."
+            ),
+            category=DeprecationWarning,
+        )
+        self.credentials = Credentials.from_dict(var)
 
     @property
     def wml_client(self):
-        warn(("`wml_client` is deprecated and will be removed in future. "
-              "Instead, please use `api_client`."), category=DeprecationWarning)
+        warn(
+            (
+                "`wml_client` is deprecated and will be removed in future. "
+                "Instead, please use `api_client`."
+            ),
+            category=DeprecationWarning,
+        )
         return self.api_client
-    
+
     @wml_client.setter
     def wml_client(self, var):
-        warn(("`wml_client` is deprecated and will be removed in future. "
-              "Instead, please use `api_client`."), category=DeprecationWarning)
+        warn(
+            (
+                "`wml_client` is deprecated and will be removed in future. "
+                "Instead, please use `api_client`."
+            ),
+            category=DeprecationWarning,
+        )
         self.api_client = var
 
-
-    def restrict_pod_size(self, t_shirt_size: 'TShirtSize') -> 'TShirtSize':
+    def restrict_pod_size(self, t_shirt_size: "TShirtSize") -> "TShirtSize":
         """Check t_shirt_size for AutoAI POD. Restrict sizes per environment.
 
         :param t_shirt_size: TShirt size to be validated and restricted
         :type t_shirt_size: TShirtSize
 
         :return: validated and restricted TShirt size
         :rtype: TShirtSize
         """
         # note: for testing purposes
-        if self.credentials.get('development', False):
+        if self.credentials.__dict__.get("development", False):
             return t_shirt_size
         # --- end note
 
         default_cloud = TShirtSize.L
         default_cp4d = TShirtSize.M
         default_server = TShirtSize.M
 
         supported_cp4d = (TShirtSize.S, TShirtSize.M, TShirtSize.L, TShirtSize.XL)
         supported_server = (TShirtSize.S, TShirtSize.M, TShirtSize.L)
 
         # note: check CP4D and Server pod sizes
-        if self.api_client.ICP:
+        if self.api_client.ICP_PLATFORM_SPACES:
             if t_shirt_size not in supported_cp4d:
-                message = (f"This t-shirt-size: \"{t_shirt_size}\" is not supported in CP4D. "
-                           f"Supported sizes: {supported_cp4d} "
-                           f"Continuing work with default size {default_cp4d}")
+                message = (
+                    f'This t-shirt-size: "{t_shirt_size}" is not supported in CP4D. '
+                    f"Supported sizes: {supported_cp4d} "
+                    f"Continuing work with default size {default_cp4d}"
+                )
 
                 warn(message=message)
                 if is_ipython():
                     print(message)
 
                 return default_cp4d
 
             else:
                 return t_shirt_size
 
         else:
             # note: allow every size in test envs
-            if 'test' in self.credentials.get('url', ''):
+            if self.credentials.url and "test" in self.credentials.url:
                 return t_shirt_size
 
             else:
                 # note: raise an error for cloud if pod size is different, other just return
                 if t_shirt_size != default_cloud:
                     raise TShirtSizeNotSupported(
                         t_shirt_size,
-                        reason=f"This t-shirt size is not supported. Please use the default one: {default_cloud}")
+                        reason=f"This t-shirt size is not supported. Please use the default one: {default_cloud}",
+                    )
 
                 else:
                     return default_cloud
                 # --- end note
```

### Comparing `ibm_watsonx_ai-0.2.6/ibm_watsonx_ai.egg-info/SOURCES.txt` & `ibm_watsonx_ai-1.0.1/ibm_watsonx_ai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 setup.cfg
 setup.py
 ibm_watsonx_ai/Set.py
 ibm_watsonx_ai/__init__.py
 ibm_watsonx_ai/assets.py
 ibm_watsonx_ai/client.py
 ibm_watsonx_ai/connections.py
+ibm_watsonx_ai/credentials.py
 ibm_watsonx_ai/deployments.py
 ibm_watsonx_ai/experiments.py
 ibm_watsonx_ai/export_assets.py
 ibm_watsonx_ai/factsheets.py
+ibm_watsonx_ai/foundation_models_manager.py
 ibm_watsonx_ai/functions.py
 ibm_watsonx_ai/hpo.py
 ibm_watsonx_ai/href_definitions.py
 ibm_watsonx_ai/hw_spec.py
 ibm_watsonx_ai/import_assets.py
-ibm_watsonx_ai/instance_new_plan.py
 ibm_watsonx_ai/lifecycle.py
 ibm_watsonx_ai/metanames.py
-ibm_watsonx_ai/migration_v4ga_cloud.py
 ibm_watsonx_ai/model_definition.py
 ibm_watsonx_ai/models.py
 ibm_watsonx_ai/parameter_sets.py
 ibm_watsonx_ai/party_wrapper.py
 ibm_watsonx_ai/pipelines.py
 ibm_watsonx_ai/pkg_extn.py
-ibm_watsonx_ai/platform_spaces.py
 ibm_watsonx_ai/remote_training_system.py
 ibm_watsonx_ai/repository.py
 ibm_watsonx_ai/script.py
+ibm_watsonx_ai/service_instance.py
 ibm_watsonx_ai/shiny.py
+ibm_watsonx_ai/spaces.py
 ibm_watsonx_ai/sw_spec.py
 ibm_watsonx_ai/task_credentials.py
 ibm_watsonx_ai/training.py
 ibm_watsonx_ai/volumes.py
 ibm_watsonx_ai/wml_client_error.py
 ibm_watsonx_ai/wml_resource.py
 ibm_watsonx_ai.egg-info/PKG-INFO
@@ -80,17 +81,29 @@
 ibm_watsonx_ai/federated_learning/data_util.py
 ibm_watsonx_ai/foundation_models/__init__.py
 ibm_watsonx_ai/foundation_models/model.py
 ibm_watsonx_ai/foundation_models/prompt_tuner.py
 ibm_watsonx_ai/foundation_models/embeddings/__init__.py
 ibm_watsonx_ai/foundation_models/embeddings/base_embeddings.py
 ibm_watsonx_ai/foundation_models/embeddings/embeddings.py
+ibm_watsonx_ai/foundation_models/embeddings/sentence_transformer_embeddings.py
 ibm_watsonx_ai/foundation_models/extensions/__init__.py
 ibm_watsonx_ai/foundation_models/extensions/langchain/__init__.py
 ibm_watsonx_ai/foundation_models/extensions/langchain/llm.py
+ibm_watsonx_ai/foundation_models/extensions/rag/__init__.py
+ibm_watsonx_ai/foundation_models/extensions/rag/pattern/__init__.py
+ibm_watsonx_ai/foundation_models/extensions/rag/pattern/default_deployable_function.py
+ibm_watsonx_ai/foundation_models/extensions/rag/pattern/pattern.py
+ibm_watsonx_ai/foundation_models/extensions/rag/utils/__init__.py
+ibm_watsonx_ai/foundation_models/extensions/rag/utils/utils.py
+ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/__init__.py
+ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/base_vector_store.py
+ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/langchain_vector_store_adapter.py
+ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/vector_store.py
+ibm_watsonx_ai/foundation_models/extensions/rag/vector_stores/vector_store_connector.py
 ibm_watsonx_ai/foundation_models/inference/__init__.py
 ibm_watsonx_ai/foundation_models/inference/base_model_inference.py
 ibm_watsonx_ai/foundation_models/inference/deployment_model_inference.py
 ibm_watsonx_ai/foundation_models/inference/fm_model_inference.py
 ibm_watsonx_ai/foundation_models/inference/model_inference.py
 ibm_watsonx_ai/foundation_models/prompts/__init__.py
 ibm_watsonx_ai/foundation_models/prompts/prompt_template.py
@@ -315,30 +328,14 @@
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/__init__.py
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/__init__.py
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/party/training/xgboost_local_training_handler.py
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/__init__.py
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/__init__.py
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/export.py
 ibm_watsonx_ai/libs/ibmfl/py39-tf27-pt110-sk10/ibmfl/util/xgboost/hyperparams.py
-ibm_watsonx_ai/libs/mlpipelinepy/__init__.py
-ibm_watsonx_ai/libs/mlpipelinepy/edge.py
-ibm_watsonx_ai/libs/mlpipelinepy/exception.py
-ibm_watsonx_ai/libs/mlpipelinepy/javaproxy.py
-ibm_watsonx_ai/libs/mlpipelinepy/mlpipeline.py
-ibm_watsonx_ai/libs/mlpipelinepy/serialization.py
-ibm_watsonx_ai/libs/mlpipelinepy/utils.py
-ibm_watsonx_ai/libs/mlpipelinepy/version.py
-ibm_watsonx_ai/libs/pipeline/DAG.py
-ibm_watsonx_ai/libs/pipeline/IBMSparkPipeline.py
-ibm_watsonx_ai/libs/pipeline/IBMSparkPipelineModel.py
-ibm_watsonx_ai/libs/pipeline/Result.py
-ibm_watsonx_ai/libs/pipeline/Sink.py
-ibm_watsonx_ai/libs/pipeline/Source.py
-ibm_watsonx_ai/libs/pipeline/Wrapper.py
-ibm_watsonx_ai/libs/pipeline/__init__.py
 ibm_watsonx_ai/libs/repo/TestRepoSaveLoad.py
 ibm_watsonx_ai/libs/repo/__init__.py
 ibm_watsonx_ai/libs/repo/base_constants.py
 ibm_watsonx_ai/libs/repo/ml_api_client.py
 ibm_watsonx_ai/libs/repo/ml_authorization.py
 ibm_watsonx_ai/libs/repo/mlrepository/__init__.py
 ibm_watsonx_ai/libs/repo/mlrepository/artifact.py
@@ -604,29 +601,27 @@
 ibm_watsonx_ai/libs/repo/util/unique_id_gen.py
 ibm_watsonx_ai/messages/__init__.py
 ibm_watsonx_ai/messages/globalization_util.py
 ibm_watsonx_ai/messages/messages.py
 ibm_watsonx_ai/messages/messages_en.json
 ibm_watsonx_ai/utils/API_VERSION_PARAM
 ibm_watsonx_ai/utils/__init__.py
-ibm_watsonx_ai/utils/change_methods_docstring.py
 ibm_watsonx_ai/utils/cpd_version.py
 ibm_watsonx_ai/utils/enums.py
 ibm_watsonx_ai/utils/utils.py
 ibm_watsonx_ai/utils/autoai/__init__.py
 ibm_watsonx_ai/utils/autoai/connection.py
 ibm_watsonx_ai/utils/autoai/enums.py
 ibm_watsonx_ai/utils/autoai/errors.py
 ibm_watsonx_ai/utils/autoai/fairness.py
 ibm_watsonx_ai/utils/autoai/incremental.py
 ibm_watsonx_ai/utils/autoai/local_training_message_handler.py
 ibm_watsonx_ai/utils/autoai/progress_bar.py
 ibm_watsonx_ai/utils/autoai/training.py
 ibm_watsonx_ai/utils/autoai/utils.py
-ibm_watsonx_ai/utils/autoai/watson_studio.py
 ibm_watsonx_ai/utils/deployment/__init__.py
 ibm_watsonx_ai/utils/deployment/errors.py
 ibm_watsonx_ai/workspace/__init__.py
 ibm_watsonx_ai/workspace/workspace.py
 ibmfl/__init__.py
 ibmfl/party_env_validator.py
 ibmfl/data/__init__.py
```

### Comparing `ibm_watsonx_ai-0.2.6/ibmfl/data/data_handler.py` & `ibm_watsonx_ai-1.0.1/ibmfl/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/ibmfl/party/party.py` & `ibm_watsonx_ai-1.0.1/ibmfl/party/party.py`

 * *Files identical despite different names*

### Comparing `ibm_watsonx_ai-0.2.6/setup.py` & `ibm_watsonx_ai-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,88 +2,29 @@
 #  (C) Copyright IBM Corp. 2023-2024.
 #  https://opensource.org/licenses/BSD-3-Clause
 #  -----------------------------------------------------------------------------------------
 
 from setuptools import setup, find_packages
 import os
 
-with open('VERSION', 'r') as f_ver:
+with open("VERSION", "r") as f_ver:
     VERSION = f_ver.read()
 
 
 def read(fname):
-    with open(os.path.join(os.path.dirname(__file__), fname)) as  f:
+    with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 # read the contents of README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 extras_require = {
-    "fl": [
-        "tensorflow==2.4.4",
-        "scikit-learn==0.23.2",
-        "torch==1.7.1",
-        "numpy==1.19.2",
-        "pandas==1.3.4",
-        "pytest==6.2.5",
-        "pyYAML==5.4.1",
-        "parse==1.19.0",
-        "websockets==8.1",
-        "jsonpickle==1.4.2",
-        "requests==2.27.1",
-        "scipy==1.6.3",
-        "environs==9.5.0",
-        "pathlib2==2.3.6",
-        "diffprivlib==0.5.1",
-        "numcompress==0.1.2",
-        "psutil",
-        "setproctitle",
-        "tabulate==0.8.9",
-        "lz4",
-        "gym",
-        "cloudpickle==1.3.0",
-        "image==1.5.33",
-        "ddsketch==1.1.2",
-        "skorch==0.11.0",
-    ],
-
-    "fl-rt22.1": [
-        "tensorflow==2.7.2",
-        "scikit-learn==1.0.2",
-        "torch==1.10.2",
-        "numpy==1.20.3",
-        "pandas==1.3.4",
-        "pytest==6.2.5",
-        "pyYAML==5.4.1",
-        "parse==1.19.0",
-        "websockets==10.1",
-        "jsonpickle==1.4.2",
-        "requests==2.27.1",
-        "scipy==1.7.3",
-        "environs==9.5.0",
-        "pathlib2==2.3.6",
-        "diffprivlib==0.5.1",
-        "numcompress==0.1.2",
-        "psutil",
-        "setproctitle",
-        "tabulate==0.8.9",
-        "lz4",
-        "gym",
-        "cloudpickle==1.3.0",
-        "image==1.5.33",
-        "ddsketch==1.1.2",
-        "skorch==0.11.0",
-        "protobuf==3.19.5",
-        "GPUtil",
-        "joblib==1.1.1",
-    ],
-
     "fl-rt22.2-py3.10": [
         "tensorflow==2.9.3",
         "scikit-learn==1.1.1",
         "torch==1.12.1",
         "numpy==1.23.1",
         "pandas==1.4.3",
         "pytest==6.2.5",
@@ -105,17 +46,16 @@
         "cloudpickle==1.3.0",
         "image==1.5.33",
         "ddsketch==1.1.2",
         "skorch==0.12.0",
         "protobuf==3.19.5",
         "GPUtil",
         "joblib==1.1.1",
-        "cryptography==39.0.1"
+        "cryptography==39.0.1",
     ],
-
     "fl-rt23.1-py3.10": [
         "tensorflow==2.12.0",
         "scikit-learn==1.1.1",
         "torch==2.0.0",
         "numpy==1.23.5",
         "pandas==1.5.3",
         "pytest==6.2.5",
@@ -137,64 +77,87 @@
         "cloudpickle==1.3.0",
         "image==1.5.33",
         "ddsketch==1.1.2",
         "skorch==0.12.0",
         "protobuf==4.22.1",
         "GPUtil",
         "joblib==1.1.1",
-        "cryptography==39.0.1"
-    ],
-
-    "fl-crypto": [
-        "pyhelayers==1.5.0.3"
+        "cryptography==39.0.1",
     ],
+    "fl-crypto": ["pyhelayers==1.5.0.3"],
 }
 
 
 def retrieve_all_files_from_path_and_sub_paths(path):
     listOfFiles = list()
     for (dirpath, dirnames, filenames) in os.walk(path):
         listOfFiles += [os.path.join(dirpath, file) for file in filenames]
 
     return listOfFiles
 
 
-with open('MANIFEST.in', 'a') as f:
-    f.writelines([f"exclude {line}\n" for line in
-                  retrieve_all_files_from_path_and_sub_paths('ibm_watsonx_ai/tests')])
+with open("MANIFEST.in", "a") as f:
+    f.writelines(
+        [
+            f"exclude {line}\n"
+            for line in retrieve_all_files_from_path_and_sub_paths(
+                "ibm_watsonx_ai/tests"
+            )
+        ]
+    )
 
 setup(
-    name='ibm_watsonx_ai',
+    name="ibm_watsonx_ai",
     version=VERSION,
-    python_requires='>=3.10',
-    author='IBM',
-    author_email='lukasz.cmielowski@pl.ibm.com, dorota.laczak@ibm.com',
-    description='IBM watsonx.ai API Client',
+    python_requires=">=3.10",
+    author="IBM",
+    author_email="lukasz.cmielowski@pl.ibm.com, dorota.laczak@ibm.com",
+    description="IBM watsonx.ai API Client",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    license='BSD-3-Clause',
-    classifiers=['Development Status :: 5 - Production/Stable',
-                 'Natural Language :: English',
-                 'License :: OSI Approved :: BSD License',
-                 'Programming Language :: Python :: 3.10',
-                 'Operating System :: MacOS :: MacOS X',
-                 'Operating System :: POSIX :: Linux',
-                 'Operating System :: Microsoft :: Windows',
-                 'Intended Audience :: Science/Research',
-                 'Intended Audience :: Developers',
-                 'Intended Audience :: Information Technology',
-                 'Topic :: Software Development :: Libraries',
-                 'Topic :: Software Development :: Libraries :: Python Modules',
-                 'Topic :: Scientific/Engineering :: Artificial Intelligence',
-                 'Topic :: Scientific/Engineering :: Information Analysis',
-                 'Topic :: Internet'],
-    keywords=["watsonx.ai", "machine learning", "IBM", "Bluemix", "client", "API", "IBM Cloud"],
-    url='https://ibm.github.io/watsonx-ai-python-sdk',
+    long_description_content_type="text/markdown",
+    license="BSD-3-Clause",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Natural Language :: English",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python :: 3.10",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: POSIX :: Linux",
+        "Operating System :: Microsoft :: Windows",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Information Technology",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Internet",
+    ],
+    keywords=[
+        "watsonx.ai",
+        "machine learning",
+        "IBM",
+        "Bluemix",
+        "client",
+        "API",
+        "IBM Cloud",
+    ],
+    url="https://ibm.github.io/watsonx-ai-python-sdk",
     packages=find_packages(),
-    package_data={'': ['messages/messages_en.json'],
-                  'api_version_param': ['utils/API_VERSION_PARAM']},
+    package_data={
+        "": ["messages/messages_en.json"],
+        "api_version_param": ["utils/API_VERSION_PARAM"],
+    },
     install_requires=[
-        'ibm-watson-machine-learning>=1.0.349'
+        "requests",
+        "urllib3",
+        "pandas<2.2.0,>=0.24.2",
+        "certifi",
+        "lomond",
+        "tabulate",
+        "packaging",
+        "ibm-cos-sdk<2.14.0,>=2.12.0",
+        "importlib-metadata",
     ],
     extras_require=extras_require,
-    include_package_data=True
+    include_package_data=True,
 )
```

