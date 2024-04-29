# Comparing `tmp/datarobot-3.3.2.tar.gz` & `tmp/datarobot-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot-3.3.2.tar", last modified: Mon Apr  8 17:20:56 2024, max compression
+gzip compressed data, was "datarobot-3.4.0.tar", last modified: Thu Apr 25 18:49:37 2024, max compression
```

## Comparing `datarobot-3.3.2.tar` & `datarobot-3.4.0.tar`

### file list

```diff
@@ -1,168 +1,198 @@
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   195398 2024-04-08 17:17:24.000000 datarobot-3.3.2/CHANGES.rst
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7555 2023-07-24 12:53:40.000000 datarobot-3.3.2/LICENSE.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      421 2023-10-25 11:01:02.000000 datarobot-3.3.2/MANIFEST.in
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3438 2024-04-08 17:20:56.000000 datarobot-3.3.2/PKG-INFO
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8911 2023-10-25 11:01:02.000000 datarobot-3.3.2/README.md
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5760 2024-04-08 17:17:19.000000 datarobot-3.3.2/common_setup.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2443 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      687 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/_compat.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      311 2024-04-08 17:17:24.000000 datarobot-3.3.2/datarobot/_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5241 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/analytics.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21787 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/client.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4664 2024-01-12 10:49:15.000000 datarobot-3.3.2/datarobot/context.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    29414 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/enums.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8984 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/errors.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot/helpers/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    25496 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/helpers/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13002 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/binary_data_utils.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1156 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/eligibility_result.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14350 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/feature_discovery.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8696 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/helpers/image_utils.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   101561 2023-10-25 11:01:02.000000 datarobot-3.3.2/datarobot/helpers/partitioning_methods.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot/mixins/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/mixins/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1134 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/mixins/browser_mixin.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1112 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/mixins/update_attributes_mixin.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4266 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     9166 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/advanced_tuning.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    27075 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/anomaly_assessment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2925 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/api_object.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8969 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/application.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15447 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/automated_documentation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    20521 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/batch_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    37053 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/batch_monitoring_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    82734 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/batch_prediction_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11451 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/blueprint.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    23822 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/calendar_file.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13301 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/change_request.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3978 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/cluster.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7233 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/cluster_insight.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12910 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/compliance_doc_template.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4887 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/confusion_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6953 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/connector.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13004 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/credential.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    33397 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/custom_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12413 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/custom_model_test.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    59820 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/custom_model_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15411 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/custom_task.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    22991 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/custom_task_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2315 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/custom_task_version_dependency_build.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17613 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/data_engine_query_generator.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17013 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/data_slice.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    16402 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/data_source.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    20035 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/data_store.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    73460 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/dataset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    30524 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/datetime_trend_plots.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/deployment/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      417 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/deployment/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    16779 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/deployment/accuracy.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5688 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/deployment/bias_and_fairness.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    12650 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/data_drift.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   104548 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/deployment/deployment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1131 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/mixins.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10065 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/service_stats.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3450 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/deployment/sharing.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/documentai/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/documentai/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    27024 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/documentai/document.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6583 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/driver.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     9411 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/execution_environment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11344 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/execution_environment_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5374 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/external_baseline_validation.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      355 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6403 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4915 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4523 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5208 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4521 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6789 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    53938 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      237 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2600 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6177 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4753 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18187 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/feature_effect.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7003 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/feature_impact.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    17463 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/featurelist.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7336 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/imported_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21166 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6516 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/lift_chart.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5468 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/missing_report.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   283117 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/model.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/model_registry/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      204 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/model_registry/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      408 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/model_registry/common.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3453 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/model_registry/deployment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    26372 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/model_registry/registered_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    21702 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/model_registry/registered_model_version.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7215 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/modeljob.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14320 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/pairwise_statistics.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5438 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/pareto_front.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8726 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/payoff_matrix.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7403 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/predict_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10218 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/prediction_dataset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10973 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/prediction_environment.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    34876 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/prediction_explanations.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2426 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/prediction_server.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15940 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/predictions.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2655 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/prime_file.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)   204934 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/project.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    56833 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/project_options.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8774 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/rating_table.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4337 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/recommended_model.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    19064 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/relationships_configuration.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6645 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/residuals.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4524 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/restore_discarded_features.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    11692 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/roc_curve.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2927 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/ruleset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    19381 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/secondary_dataset.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    14217 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/segmentation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4070 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/shap_impact.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7057 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/shap_matrix.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2645 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/shap_matrix_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     7314 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/sharing.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     6267 2023-12-19 16:42:00.000000 datarobot-3.3.2/datarobot/models/status_check_job.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1431 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/trafarets.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    28260 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/training_predictions.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1822 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/types.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/use_cases/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      262 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/use_cases/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    24589 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/use_cases/use_case.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13520 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/use_cases/utils.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/user_blueprints/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)       49 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/user_blueprints/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    69649 2024-04-08 17:17:19.000000 datarobot-3.3.2/datarobot/models/user_blueprints/models.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     8758 2023-07-24 12:53:40.000000 datarobot-3.3.2/datarobot/models/user_blueprints/trafarets.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2749 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/validators.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/models/visualai/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      226 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18528 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/augmentation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    10521 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/images.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    13615 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/visualai/insights.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4936 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/models/word_cloud.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        0 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/py.typed
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    18404 2023-12-14 18:07:41.000000 datarobot-3.3.2/datarobot/rest.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:56.000000 datarobot-3.3.2/datarobot/utils/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)    15618 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/__init__.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     2997 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/deprecation.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      495 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/logger.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1200 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/pagination.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1461 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/retry.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1282 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/source.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4109 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/sourcedata.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     4193 2023-10-25 11:01:03.000000 datarobot-3.3.2/datarobot/utils/waiters.py
-drwxr-xr-x   0 volodymyr.onofriichuk   (503) staff       (20)        0 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3438 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/PKG-INFO
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     5539 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/SOURCES.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)        1 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/dependency_links.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1128 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/requires.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)       10 2024-04-08 17:20:55.000000 datarobot-3.3.2/datarobot.egg-info/top_level.txt
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     3066 2023-10-25 11:01:03.000000 datarobot-3.3.2/pyproject.toml
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      123 2024-04-08 17:20:56.000000 datarobot-3.3.2/setup.cfg
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)      965 2023-10-25 11:01:03.000000 datarobot-3.3.2/setup.py
--rw-r--r--   0 volodymyr.onofriichuk   (503) staff       (20)     1213 2023-10-25 11:01:03.000000 datarobot-3.3.2/setup_major.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.202417 datarobot-3.4.0/
+-rw-r--r--   0 aj         (502) staff       (20)   226178 2024-04-25 18:23:24.000000 datarobot-3.4.0/CHANGES.rst
+-rw-r--r--   0 aj         (502) staff       (20)     7555 2023-10-16 23:33:18.000000 datarobot-3.4.0/LICENSE.txt
+-rw-r--r--   0 aj         (502) staff       (20)      421 2024-04-08 18:17:57.000000 datarobot-3.4.0/MANIFEST.in
+-rw-r--r--   0 aj         (502) staff       (20)     6533 2024-04-25 18:49:37.202074 datarobot-3.4.0/PKG-INFO
+-rw-r--r--   0 aj         (502) staff       (20)     8911 2024-04-08 18:17:57.000000 datarobot-3.4.0/README.md
+-rw-r--r--   0 aj         (502) staff       (20)     5852 2024-04-08 18:17:57.000000 datarobot-3.4.0/common_setup.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.030285 datarobot-3.4.0/datarobot/
+-rw-r--r--   0 aj         (502) staff       (20)     2546 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)      687 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/_compat.py
+-rw-r--r--   0 aj         (502) staff       (20)      311 2024-04-25 18:23:24.000000 datarobot-3.4.0/datarobot/_version.py
+-rw-r--r--   0 aj         (502) staff       (20)     5241 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/analytics.py
+-rw-r--r--   0 aj         (502) staff       (20)    14682 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/client.py
+-rw-r--r--   0 aj         (502) staff       (20)    12682 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/config.py
+-rw-r--r--   0 aj         (502) staff       (20)     4664 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/context.py
+-rw-r--r--   0 aj         (502) staff       (20)    40318 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/enums.py
+-rw-r--r--   0 aj         (502) staff       (20)     8984 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/errors.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.038590 datarobot-3.4.0/datarobot/helpers/
+-rw-r--r--   0 aj         (502) staff       (20)    27055 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/helpers/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    13002 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/helpers/binary_data_utils.py
+-rw-r--r--   0 aj         (502) staff       (20)     1156 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/helpers/eligibility_result.py
+-rw-r--r--   0 aj         (502) staff       (20)    14350 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/helpers/feature_discovery.py
+-rw-r--r--   0 aj         (502) staff       (20)     8744 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/helpers/image_utils.py
+-rw-r--r--   0 aj         (502) staff       (20)   101561 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/helpers/partitioning_methods.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.042306 datarobot-3.4.0/datarobot/insights/
+-rw-r--r--   0 aj         (502) staff       (20)      200 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/insights/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     9262 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/insights/base.py
+-rw-r--r--   0 aj         (502) staff       (20)     2698 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/insights/shap_impact.py
+-rw-r--r--   0 aj         (502) staff       (20)     1409 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/insights/shap_matrix.py
+-rw-r--r--   0 aj         (502) staff       (20)     1622 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/insights/shap_preview.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.044069 datarobot-3.4.0/datarobot/mixins/
+-rw-r--r--   0 aj         (502) staff       (20)        0 2023-10-17 19:18:59.000000 datarobot-3.4.0/datarobot/mixins/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     1134 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/mixins/browser_mixin.py
+-rw-r--r--   0 aj         (502) staff       (20)     1112 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/mixins/update_attributes_mixin.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.116274 datarobot-3.4.0/datarobot/models/
+-rw-r--r--   0 aj         (502) staff       (20)     4381 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     9166 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/advanced_tuning.py
+-rw-r--r--   0 aj         (502) staff       (20)    27075 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/anomaly_assessment.py
+-rw-r--r--   0 aj         (502) staff       (20)     2925 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/api_object.py
+-rw-r--r--   0 aj         (502) staff       (20)     9076 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/application.py
+-rw-r--r--   0 aj         (502) staff       (20)    15457 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/automated_documentation.py
+-rw-r--r--   0 aj         (502) staff       (20)    20521 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/batch_job.py
+-rw-r--r--   0 aj         (502) staff       (20)    37053 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/batch_monitoring_job.py
+-rw-r--r--   0 aj         (502) staff       (20)    86467 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/batch_prediction_job.py
+-rw-r--r--   0 aj         (502) staff       (20)    11451 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/blueprint.py
+-rw-r--r--   0 aj         (502) staff       (20)    23822 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/calendar_file.py
+-rw-r--r--   0 aj         (502) staff       (20)    13301 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/change_request.py
+-rw-r--r--   0 aj         (502) staff       (20)     3978 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/cluster.py
+-rw-r--r--   0 aj         (502) staff       (20)     7233 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/cluster_insight.py
+-rw-r--r--   0 aj         (502) staff       (20)    12910 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/compliance_doc_template.py
+-rw-r--r--   0 aj         (502) staff       (20)     4889 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/confusion_chart.py
+-rw-r--r--   0 aj         (502) staff       (20)     7244 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/connector.py
+-rw-r--r--   0 aj         (502) staff       (20)    20307 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/credential.py
+-rw-r--r--   0 aj         (502) staff       (20)    34090 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/custom_model.py
+-rw-r--r--   0 aj         (502) staff       (20)    12413 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/custom_model_test.py
+-rw-r--r--   0 aj         (502) staff       (20)    63934 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/custom_model_version.py
+-rw-r--r--   0 aj         (502) staff       (20)    15411 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/custom_task.py
+-rw-r--r--   0 aj         (502) staff       (20)    22991 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/custom_task_version.py
+-rw-r--r--   0 aj         (502) staff       (20)     2315 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/custom_task_version_dependency_build.py
+-rw-r--r--   0 aj         (502) staff       (20)    17613 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/data_engine_query_generator.py
+-rw-r--r--   0 aj         (502) staff       (20)    17068 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/data_slice.py
+-rw-r--r--   0 aj         (502) staff       (20)    17063 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/data_source.py
+-rw-r--r--   0 aj         (502) staff       (20)    20149 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/data_store.py
+-rw-r--r--   0 aj         (502) staff       (20)    75540 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/dataset.py
+-rw-r--r--   0 aj         (502) staff       (20)    30524 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/datetime_trend_plots.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.137912 datarobot-3.4.0/datarobot/models/deployment/
+-rw-r--r--   0 aj         (502) staff       (20)      544 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    16779 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/accuracy.py
+-rw-r--r--   0 aj         (502) staff       (20)     5698 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/bias_and_fairness.py
+-rw-r--r--   0 aj         (502) staff       (20)     7095 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/challenger.py
+-rw-r--r--   0 aj         (502) staff       (20)     6170 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/champion_model_package.py
+-rw-r--r--   0 aj         (502) staff       (20)    57732 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/custom_metrics.py
+-rw-r--r--   0 aj         (502) staff       (20)    12650 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/data_drift.py
+-rw-r--r--   0 aj         (502) staff       (20)    24249 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/data_exports.py
+-rw-r--r--   0 aj         (502) staff       (20)   121466 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/deployment.py
+-rw-r--r--   0 aj         (502) staff       (20)     1131 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/mixins.py
+-rw-r--r--   0 aj         (502) staff       (20)    10065 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/service_stats.py
+-rw-r--r--   0 aj         (502) staff       (20)     3450 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/deployment/sharing.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.139693 datarobot-3.4.0/datarobot/models/documentai/
+-rw-r--r--   0 aj         (502) staff       (20)        0 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/documentai/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    27024 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/documentai/document.py
+-rw-r--r--   0 aj         (502) staff       (20)     8427 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/driver.py
+-rw-r--r--   0 aj         (502) staff       (20)     9411 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/execution_environment.py
+-rw-r--r--   0 aj         (502) staff       (20)    11344 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/execution_environment_version.py
+-rw-r--r--   0 aj         (502) staff       (20)     5376 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_baseline_validation.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.146616 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/
+-rw-r--r--   0 aj         (502) staff       (20)      355 2023-03-22 21:37:35.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     6403 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-r--r--   0 aj         (502) staff       (20)     4915 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-r--r--   0 aj         (502) staff       (20)     4523 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-r--r--   0 aj         (502) staff       (20)     5208 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-r--r--   0 aj         (502) staff       (20)     4521 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-r--r--   0 aj         (502) staff       (20)     6789 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-r--r--   0 aj         (502) staff       (20)    53938 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/feature.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.150027 datarobot-3.4.0/datarobot/models/feature_association_matrix/
+-rw-r--r--   0 aj         (502) staff       (20)      237 2023-03-22 21:37:35.000000 datarobot-3.4.0/datarobot/models/feature_association_matrix/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     2600 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-r--r--   0 aj         (502) staff       (20)     7052 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-r--r--   0 aj         (502) staff       (20)     4753 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-r--r--   0 aj         (502) staff       (20)    18312 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/feature_effect.py
+-rw-r--r--   0 aj         (502) staff       (20)     7003 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/feature_impact.py
+-rw-r--r--   0 aj         (502) staff       (20)    17463 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/featurelist.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.162287 datarobot-3.4.0/datarobot/models/genai/
+-rw-r--r--   0 aj         (502) staff       (20)      455 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     5647 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/chat.py
+-rw-r--r--   0 aj         (502) staff       (20)    18029 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/chat_prompt.py
+-rw-r--r--   0 aj         (502) staff       (20)     5925 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/comparison_chat.py
+-rw-r--r--   0 aj         (502) staff       (20)    12076 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/comparison_prompt.py
+-rw-r--r--   0 aj         (502) staff       (20)     2168 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/custom_model_llm_validation.py
+-rw-r--r--   0 aj         (502) staff       (20)    16900 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/custom_model_validation.py
+-rw-r--r--   0 aj         (502) staff       (20)    10350 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/llm.py
+-rw-r--r--   0 aj         (502) staff       (20)    22572 2024-04-25 18:23:24.000000 datarobot-3.4.0/datarobot/models/genai/llm_blueprint.py
+-rw-r--r--   0 aj         (502) staff       (20)     7299 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/playground.py
+-rw-r--r--   0 aj         (502) staff       (20)     1200 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/user_limits.py
+-rw-r--r--   0 aj         (502) staff       (20)    26873 2024-04-24 21:55:41.000000 datarobot-3.4.0/datarobot/models/genai/vector_database.py
+-rw-r--r--   0 aj         (502) staff       (20)     7336 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/imported_model.py
+-rw-r--r--   0 aj         (502) staff       (20)    21315 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/job.py
+-rw-r--r--   0 aj         (502) staff       (20)    13141 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/key_values.py
+-rw-r--r--   0 aj         (502) staff       (20)     6516 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/lift_chart.py
+-rw-r--r--   0 aj         (502) staff       (20)     5468 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/missing_report.py
+-rw-r--r--   0 aj         (502) staff       (20)   305975 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/model.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.166643 datarobot-3.4.0/datarobot/models/model_registry/
+-rw-r--r--   0 aj         (502) staff       (20)      204 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/model_registry/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)      408 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/model_registry/common.py
+-rw-r--r--   0 aj         (502) staff       (20)     3453 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/model_registry/deployment.py
+-rw-r--r--   0 aj         (502) staff       (20)    26475 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/model_registry/registered_model.py
+-rw-r--r--   0 aj         (502) staff       (20)    22985 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/model_registry/registered_model_version.py
+-rw-r--r--   0 aj         (502) staff       (20)     7215 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/modeljob.py
+-rw-r--r--   0 aj         (502) staff       (20)    14320 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/pairwise_statistics.py
+-rw-r--r--   0 aj         (502) staff       (20)     5438 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/pareto_front.py
+-rw-r--r--   0 aj         (502) staff       (20)     8726 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/payoff_matrix.py
+-rw-r--r--   0 aj         (502) staff       (20)     7403 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/predict_job.py
+-rw-r--r--   0 aj         (502) staff       (20)    10218 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/prediction_dataset.py
+-rw-r--r--   0 aj         (502) staff       (20)    10918 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/prediction_environment.py
+-rw-r--r--   0 aj         (502) staff       (20)    39753 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/prediction_explanations.py
+-rw-r--r--   0 aj         (502) staff       (20)     2426 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/prediction_server.py
+-rw-r--r--   0 aj         (502) staff       (20)    15940 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/predictions.py
+-rw-r--r--   0 aj         (502) staff       (20)     2655 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/prime_file.py
+-rw-r--r--   0 aj         (502) staff       (20)   224363 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/project.py
+-rw-r--r--   0 aj         (502) staff       (20)    57175 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/project_options.py
+-rw-r--r--   0 aj         (502) staff       (20)     8774 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/rating_table.py
+-rw-r--r--   0 aj         (502) staff       (20)     4337 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/recommended_model.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.169833 datarobot-3.4.0/datarobot/models/registry/
+-rw-r--r--   0 aj         (502) staff       (20)      345 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/registry/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    16789 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/registry/job.py
+-rw-r--r--   0 aj         (502) staff       (20)    10379 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/registry/job_run.py
+-rw-r--r--   0 aj         (502) staff       (20)    19064 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/relationships_configuration.py
+-rw-r--r--   0 aj         (502) staff       (20)     6645 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/residuals.py
+-rw-r--r--   0 aj         (502) staff       (20)     4524 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/restore_discarded_features.py
+-rw-r--r--   0 aj         (502) staff       (20)    11692 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/roc_curve.py
+-rw-r--r--   0 aj         (502) staff       (20)     2927 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/ruleset.py
+-rw-r--r--   0 aj         (502) staff       (20)     5008 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/runtime_parameters.py
+-rw-r--r--   0 aj         (502) staff       (20)    19381 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/secondary_dataset.py
+-rw-r--r--   0 aj         (502) staff       (20)    14217 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/segmentation.py
+-rw-r--r--   0 aj         (502) staff       (20)     4722 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/shap_impact.py
+-rw-r--r--   0 aj         (502) staff       (20)     8216 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/shap_matrix.py
+-rw-r--r--   0 aj         (502) staff       (20)     2676 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/shap_matrix_job.py
+-rw-r--r--   0 aj         (502) staff       (20)     7314 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/sharing.py
+-rw-r--r--   0 aj         (502) staff       (20)     6267 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/status_check_job.py
+-rw-r--r--   0 aj         (502) staff       (20)     1431 2023-10-16 23:33:18.000000 datarobot-3.4.0/datarobot/models/trafarets.py
+-rw-r--r--   0 aj         (502) staff       (20)    28260 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/training_predictions.py
+-rw-r--r--   0 aj         (502) staff       (20)     2029 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/types.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.172465 datarobot-3.4.0/datarobot/models/use_cases/
+-rw-r--r--   0 aj         (502) staff       (20)      262 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/use_cases/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    24890 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/use_cases/use_case.py
+-rw-r--r--   0 aj         (502) staff       (20)    13496 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/use_cases/utils.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.174752 datarobot-3.4.0/datarobot/models/user_blueprints/
+-rw-r--r--   0 aj         (502) staff       (20)       49 2023-03-22 21:37:35.000000 datarobot-3.4.0/datarobot/models/user_blueprints/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    69649 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/user_blueprints/models.py
+-rw-r--r--   0 aj         (502) staff       (20)     8758 2023-10-16 23:33:18.000000 datarobot-3.4.0/datarobot/models/user_blueprints/trafarets.py
+-rw-r--r--   0 aj         (502) staff       (20)     2749 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/validators.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.178198 datarobot-3.4.0/datarobot/models/visualai/
+-rw-r--r--   0 aj         (502) staff       (20)      226 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/visualai/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)    18528 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/visualai/augmentation.py
+-rw-r--r--   0 aj         (502) staff       (20)    10521 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/visualai/images.py
+-rw-r--r--   0 aj         (502) staff       (20)    13615 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/visualai/insights.py
+-rw-r--r--   0 aj         (502) staff       (20)     4936 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/models/word_cloud.py
+-rw-r--r--   0 aj         (502) staff       (20)        0 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/py.typed
+-rw-r--r--   0 aj         (502) staff       (20)    18404 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/rest.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.185932 datarobot-3.4.0/datarobot/utils/
+-rw-r--r--   0 aj         (502) staff       (20)    15618 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/__init__.py
+-rw-r--r--   0 aj         (502) staff       (20)     2997 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/deprecation.py
+-rw-r--r--   0 aj         (502) staff       (20)      495 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/logger.py
+-rw-r--r--   0 aj         (502) staff       (20)     1200 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/pagination.py
+-rw-r--r--   0 aj         (502) staff       (20)     1461 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/retry.py
+-rw-r--r--   0 aj         (502) staff       (20)     1282 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/source.py
+-rw-r--r--   0 aj         (502) staff       (20)     4109 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/sourcedata.py
+-rw-r--r--   0 aj         (502) staff       (20)     4193 2024-04-08 18:17:57.000000 datarobot-3.4.0/datarobot/utils/waiters.py
+drwxr-xr-x   0 aj         (502) staff       (20)        0 2024-04-25 18:49:37.186888 datarobot-3.4.0/datarobot.egg-info/
+-rw-r--r--   0 aj         (502) staff       (20)     6533 2024-04-25 18:49:36.000000 datarobot-3.4.0/datarobot.egg-info/PKG-INFO
+-rw-r--r--   0 aj         (502) staff       (20)     6565 2024-04-25 18:49:36.000000 datarobot-3.4.0/datarobot.egg-info/SOURCES.txt
+-rw-r--r--   0 aj         (502) staff       (20)        1 2024-04-25 18:49:36.000000 datarobot-3.4.0/datarobot.egg-info/dependency_links.txt
+-rw-r--r--   0 aj         (502) staff       (20)     1207 2024-04-25 18:49:36.000000 datarobot-3.4.0/datarobot.egg-info/requires.txt
+-rw-r--r--   0 aj         (502) staff       (20)       10 2024-04-25 18:49:36.000000 datarobot-3.4.0/datarobot.egg-info/top_level.txt
+-rw-r--r--   0 aj         (502) staff       (20)     3066 2024-04-08 18:17:58.000000 datarobot-3.4.0/pyproject.toml
+-rw-r--r--   0 aj         (502) staff       (20)      123 2024-04-25 18:49:37.203200 datarobot-3.4.0/setup.cfg
+-rw-r--r--   0 aj         (502) staff       (20)      965 2024-04-08 18:17:58.000000 datarobot-3.4.0/setup.py
+-rw-r--r--   0 aj         (502) staff       (20)     1213 2024-04-08 18:17:58.000000 datarobot-3.4.0/setup_major.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datarobot-3.3.2/CHANGES.rst` & `datarobot-3.4.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,282 @@
 #########
 Changelog
 #########
+3.4.0
+=====
 
-3.3.2
-========
+New features
+************
+- Added the following classes for generative AI. Importing these from `datarobot._experimental.models.genai` is deprecated and will be removed by the release of DataRobot 10.1 and SDK 3.5.
+  - :class:`Playground <datarobot.models.genai.playground.Playground>` to manage generative AI playgrounds.
+  - :class:`LLMDefinition <datarobot.models.genai.llm.LLMDefinition>` to get information about supported LLMs.
+  - :class:`LLMBlueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint>` to manage LLM blueprints.
+  - :class:`Chat <datarobot.models.genai.chat.Chat>` to manage chats for LLM blueprints.
+  - :class:`ChatPrompt <datarobot.models.genai.chat_prompt.ChatPrompt>` to submit prompts within a chat.
+  - :class:`ComparisonChat <datarobot.models.genai.comparison_chat.ComparisonChat>` to manage comparison chats across multiple LLM blueprints within a playground.
+  - :class:`ComparisonPrompt <datarobot.models.genai.comparison_prompt.ComparisonPrompt>` to submit a prompt to multiple LLM blueprints within a comparison chat.
+  - :class:`VectorDatabase <datarobot.models.genai.vector_database.VectorDatabase>` to create vector databases from datasets in the AI Catalog for retrieval augmented generation with an LLM blueprint.
+  - :class:`CustomModelVectorDatabaseValidation <datarobot.models.genai.vector_database.CustomModelVectorDatabaseValidation>` to validate a deployment for use as a vector database.
+  - :class:`CustomModelLLMValidation <datarobot.models.genai.custom_model_llm_validation.CustomModelLLMValidation>` to validate a deployment for use as an LLM.
+  - :class:`UserLimits <datarobot.models.genai.user_limits.UserLimits>` to get counts of vector databases and LLM requests for a user.
 
-Bugfixes
-********
-- Fix `per_ngram_text_explanations` retrieving.  In some cases `per_ngram_text_explanations` are missing in prediction explanations, causing SDK to fail when trying to retrieve the values.
+- Extended the advanced options available when setting a target to include new
+  parameter: 'incrementalLearningEarlyStoppingRounds'(part of the AdvancedOptions object).
+  This parameter allows you to specify when to stop for incremental learning automation.
+- Added experimental support for Chunking Service:
+  - :class:`DatasetChunkDefinition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition>` for defining how chunks are created from a data source.
+
+    - :meth:`DatasetChunkDefinition.create <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create>` to create a new dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.get <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to get a specific dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.list <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to list all dataset chunk definitions.
+    - :meth:`DatasetChunkDefinition.get_datasource_definition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_datasource_definition>` to retrieve the data source definition.
+    - :meth:`DatasetChunkDefinition.get_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_chunk>` to get specific chunk metadata belonging to a dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.list_chunks <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.list_chunks>` to list all chunk metadata belonging to a dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.create_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk>` to submit a job to retrieve the data from the origin data source.
+    - :meth:`DatasetChunkDefinition.create_chunk_by_index <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk_by_index>` to submit a job to retrieve data from the origin data source by index.
+
+  - :class:`OriginStorageType <datarobot._experimental.models.chunking_service.OriginStorageType>`
+  - :class:`Chunk <datarobot._experimental.models.chunking_service.Chunk>`
+  - :class:`ChunkStorageType <datarobot._experimental.models.chunking_service.ChunkStorageType>`
+  - :class:`ChunkStorage <datarobot._experimental.models.chunking_service.ChunkStorage>`
+  - :class:`DatasourceDefinition <datarobot._experimental.models.chunking_service.DatasourceDefinition>`
+  - :class:`DatasourceAICatalogInfo <datarobot._experimental.models.chunking_service.DatasourceAICatalogInfo>` to define the datasource AI catalog information to create a new dataset chunk definition.
+  - :class:`DatasourceDataWarehouseInfo <datarobot._experimental.models.chunking_service.DatasourceDataWarehouseInfo>` to define the datasource data warehouse (snowflake, big query, etc) information to create a new dataset chunk definition.
+  - :class:`RuntimeParameter <datarobot.models.custom_model_version.RuntimeParameter>` for retrieving runtime parameters assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+  - :class:`RuntimeParameterValue <datarobot.models.custom_model_version.RuntimeParameterValue>` to define runtime parameter override value, to be assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+
+- Added Snowflake Key Pair authentication for uploading datasets from Snowflake or creating a project from Snowflake data
+- Added :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>` to retrieve models.
+  Method :meth:`Project.get_models <datarobot.models.Project.get_models>` is deprecated and will be removed soon in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
+- Extended the advanced options available when setting a target to include new
+  parameter: 'chunkDefinitionId'(part of the AdvancedOptions object). This parameter allows you to specify the chunking definition needed for incremental learning automation.
+- Extended the advanced options available when setting a target to include new Autopilot
+  parameters: 'incrementalLearningOnlyMode' and 'incrementalLearningOnBestModel' (part of the AdvancedOptions object). These parameters allow you to specify how Autopilot is performed with the chunking service.
+- Added a new method :meth:`DatetimeModel.request_lift_chart<datarobot.models.DatetimeModel.request_lift_chart>` to support Lift Chart calculations for datetime partitioned projects with support of Sliced Insights.
+- Added a new method :meth:`DatetimeModel.get_lift_chart<datarobot.models.DatetimeModel.get_lift_chart>` to support Lift chart retrieval for datetime partitioned projects with support of Sliced Insights.
+- Added a new method :meth:`DatetimeModel.request_roc_curve<datarobot.models.DatetimeModel.request_roc_curve>` to support ROC curve calculation for datetime partitioned projects with support of Sliced Insights.
+- Added a new method :meth:`DatetimeModel.get_roc_curve<datarobot.models.DatetimeModel.get_roc_curve>` to support ROC curve retrieval for datetime partitioned projects with support of Sliced Insights.
+- Update method :meth:`DatetimeModel.request_feature_impact<datarobot.models.DatetimeModel.request_feature_impact>` to support use of Sliced Insights.
+- Update method :meth:`DatetimeModel.get_feature_impact<datarobot.models.DatetimeModel.get_feature_impact>` to support use of Sliced Insights.
+- Update method :meth:`DatetimeModel.get_or_request_feature_impact<datarobot.models.DatetimeModel.get_or_request_feature_impact>` to support use of Sliced Insights.
+- Update method :meth:`DatetimeModel.request_feature_effect<datarobot.models.DatetimeModel.request_feature_effect>` to support use of Sliced Insights.
+- Update method :meth:`DatetimeModel.get_feature_effect<datarobot.models.DatetimeModel.get_feature_effect>` to support use of Sliced Insights.
+- Update method :meth:`DatetimeModel.get_or_request_feature_effect<datarobot.models.DatetimeModel.get_or_request_feature_effect>` to support use of Sliced Insights.
+- Added a new method :meth:`FeatureAssociationMatrix.create<datarobot.models.FeatureAssociationMatrix.create>` to support the creation of FeatureAssociationMatricies for Featurelists.
+- Introduced a new method :meth:`Deployment.perform_model_replace<datarobot.models.Deployment.perform_model_replace>` as a replacement for :meth:`Deployment.replace_model<datarobot.models.Deployment.replace_model>`.
+- Introduced a new property, `model_package`, which provides an overview of the currently used model package in :class:`datarobot.models.Deployment`.
+- Added new parameter `prediction_threshold` to :meth:`BatchPredictionJob.score_with_leaderboard_model <datarobot.models.BatchPredictionJob.score_with_leaderboard_model>`
+  and :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>` that automatically assigns the positive class label to any prediction exceeding the threshold.
+- Added two new enum values to  :class: `datarobot.models.data_slice.DataSlicesOperators`, "BETWEEN" and "NOT_BETWEEN", which are used to allow slicing.
+- Added a new class :class:`Challenger <datarobot.models.deployment.challenger.Challenger>` for interacting with DataRobot challengers to support the following methods:
+  :meth:`Challenger.get <datarobot.models.deployment.challenger.Challenger.get>` to retrieve challenger objects by ID.
+  :meth:`Challenger.list <datarobot.models.deployment.challenger.Challenger.list>` to list all challengers.
+  :meth:`Challenger.create <datarobot.models.deployment.challenger.Challenger.create>` to create a new challenger.
+  :meth:`Challenger.update <datarobot.models.deployment.challenger.Challenger.update>` to update a challenger.
+  :meth:`Challenger.delete <datarobot.models.deployment.challenger.Challenger.delete>` to delete a challenger.
+- Added a new method :meth:`Deployment.get_challenger_replay_settings <datarobot.models.Deployment.get_challenger_replay_settings>` to retrieve the challenger replay settings of a deployment.
+- Added a new method :meth:`Deployment.list_challengers <datarobot.models.Deployment.list_challengers>` to retrieve the challengers of a deployment.
+- Added a new method :meth:`Deployment.get_champion_model_package <datarobot.models.Deployment.get_champion_model_package>` to retrieve the champion model package from a deployment.
+- Added a new method :meth:`Deployment.list_prediction_data_exports <datarobot.models.Deployment.list_prediction_data_exports>` to retrieve deployment prediction data exports.
+- Added a new method :meth:`Deployment.list_actuals_data_exports <datarobot.models.Deployment.list_actuals_data_exports>` to retrieve deployment actuals data exports.
+- Added a new method :meth:`Deployment.list_training_data_exports <datarobot.models.Deployment.list_training_data_exports>` to retrieve deployment training data exports.
+- Manage deployment health settings with the following methods:
+  - Get health settings :meth:`Deployment.get_health_settings <datarobot.models.Deployment.get_health_settings>`
+  - Update health settings :meth:`Deployment.update_health_settings <datarobot.models.Deployment.update_health_settings>`
+  - Get default health settings :meth:`Deployment.get_default_health_settings <datarobot.models.Deployment.get_default_health_settings>`
+- Added new enum value to ``datarobot.enums._SHARED_TARGET_TYPE`` to support Text Generation use case.
+- Added new enum value ``datarobotServerless`` to ``datarobot.enums.PredictionEnvironmentPlatform`` to support DataRobot Serverless prediction environments.
+- Added new enum value ``notApplicable`` to ``datarobot.enums.PredictionEnvironmentHealthType`` to support new health status from DataRobot API.
+- Added new enum value to ``datarobot.enums.TARGET_TYPE`` and ``datarobot.enums.CUSTOM_MODEL_TARGET_TYPE`` to support text generation custom inference models.
+- Updated ``datarobot.CustomModel`` to support the creation of text generation custom models.
+- Added a new class :class:`CustomMetric <datarobot.models.deployment.custom_metrics.CustomMetric>` for interacting with DataRobot custom metrics to support the following methods:
+  :meth:`CustomMetric.get <datarobot.models.deployment.custom_metrics.CustomMetric.get>` to retrieve a custom metric object by ID from a given deployment.
+  :meth:`CustomMetric.list <datarobot.models.deployment.custom_metrics.CustomMetric.list>` to list all custom metrics from a given deployment.
+  :meth:`CustomMetric.create <datarobot.models.deployment.custom_metrics.CustomMetric.create>` to create a new custom metric for a given deployment.
+  :meth:`CustomMetric.update <datarobot.models.deployment.custom_metrics.CustomMetric.update>` to update a custom metric for a given deployment.
+  :meth:`CustomMetric.delete <datarobot.models.deployment.custom_metrics.CustomMetric.delete>` to delete a custom metric for a given deployment.
+  :meth:`CustomMetric.unset_baseline <datarobot.models.deployment.custom_metrics.CustomMetric.unset_baseline>` to remove baseline for a given custom metric.
+  :meth:`CustomMetric.submit_values <datarobot.models.deployment.custom_metrics.CustomMetric.submit_values>` to submit aggregated custom metrics values from code. The provided data should be in the form of a dict or a Pandas DataFrame.
+  :meth:`CustomMetric.submit_single_value <datarobot.models.deployment.custom_metrics.CustomMetric.submit_single_value>` to submit a single custom metric value.
+  :meth:`CustomMetric.submit_values_from_catalog <datarobot.models.deployment.custom_metrics.CustomMetric.submit_values_from_catalog>` to submit aggregated custom metrics values from a dataset via the AI Catalog.
+  :meth:`CustomMetric.get_values_over_time <datarobot.models.deployment.custom_metrics.CustomMetric.get_values_over_time>` to retrieve values of a custom metric over a time period.
+  :meth:`CustomMetric.get_summary <datarobot.models.deployment.custom_metrics.CustomMetric.get_summary>` to retrieve the summary of a custom metric over a time period.
+  :meth:`CustomMetric.get_values_over_batch <datarobot.models.deployment.custom_metrics.CustomMetric.get_values_over_batch>` to retrieve values of a custom metric over batches.
+  :meth:`CustomMetric.get_batch_summary <datarobot.models.deployment.custom_metrics.CustomMetric.get_batch_summary>` to retrieve the summary of a custom metric over batches.
+- Added :class:`CustomMetricValuesOverTime <datarobot.models.deployment.custom_metrics.CustomMetricValuesOverTime>` to retrieve custom metric over time information.
+- Added :class:`CustomMetricSummary <datarobot.models.deployment.custom_metrics.CustomMetricSummary>` to retrieve custom metric over time summary.
+- Added :class:`CustomMetricValuesOverBatch <datarobot.models.deployment.custom_metrics.CustomMetricValuesOverBatch>` to retrieve custom metric over batch information.
+- Added :class:`CustomMetricBatchSummary <datarobot.models.deployment.custom_metrics.CustomMetricBatchSummary>` to retrieve custom metric batch summary.
+- Added :class:`Job <datarobot.models.registry.job.Job>` and  :class:`JobRun <datarobot.models.registry.job_run.JobRun>`  to create, read, update, run, and delete jobs in the Registry.
+- Added :class:`KeyValue <datarobot.models.key_values.KeyValue>` to create, read, update, and delete key values.
+- Added a new class :class:`PredictionDataExport <datarobot.models.deployment.data_exports.PredictionDataExport>` for interacting with DataRobot deployment data export to support the following methods:
+  :meth:`PredictionDataExport.get <datarobot.models.deployment.data_exports.PredictionDataExport.get>` to retrieve a prediction data export object by ID from a given deployment.
+  :meth:`PredictionDataExport.list <datarobot.models.deployment.data_exports.PredictionDataExport.list>` to list all prediction data exports from a given deployment.
+  :meth:`PredictionDataExport.create <datarobot.models.deployment.data_exports.PredictionDataExport.create>` to create a new prediction data export for a given deployment.
+  :meth:`PredictionDataExport.fetch_data <datarobot.models.deployment.data_exports.PredictionDataExport.fetch_data>` to retrieve a prediction export data as a DataRobot dataset.
+- Added a new class :class:`ActualsDataExport <datarobot.models.deployment.data_exports.ActualsDataExport>` for interacting with DataRobot deployment data export to support the following methods:
+  :meth:`ActualsDataExport.get <datarobot.models.deployment.data_exports.ActualsDataExport.get>` to retrieve an actuals data export object by ID from a given deployment.
+  :meth:`ActualsDataExport.list <datarobot.models.deployment.data_exports.ActualsDataExport.list>` to list all actuals data exports from a given deployment.
+  :meth:`ActualsDataExport.create <datarobot.models.deployment.data_exports.ActualsDataExport.create>` to create a new actuals data export for a given deployment.
+  :meth:`ActualsDataExport.fetch_data <datarobot.models.deployment.data_exports.ActualsDataExport.fetch_data>` to retrieve an actuals export data  as a DataRobot dataset.
+- Added a new class :class:`TrainingDataExport <datarobot.models.deployment.data_exports.TrainingDataExport>` for interacting with DataRobot deployment data export to support the following methods:
+  :meth:`TrainingDataExport.get <datarobot.models.deployment.data_exports.TrainingDataExport.get>` to retrieve a training data export object by ID from a given deployment.
+  :meth:`TrainingDataExport.list <datarobot.models.deployment.data_exports.TrainingDataExport.list>` to list all training data exports from a given deployment.
+  :meth:`TrainingDataExport.create <datarobot.models.deployment.data_exports.TrainingDataExport.create>` to create a new training data export for a given deployment.
+  :meth:`TrainingDataExport.fetch_data <datarobot.models.deployment.data_exports.TrainingDataExport.fetch_data>` to retrieve a training export data as a DataRobot dataset.
+- Added a new parameter `base_environment_version_id` to :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` for overriding the default environment version selection behavior.
+- Added a new parameter `base_environment_version_id` to :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` for overriding the default environment version selection behavior.
+- Added a new class :class:`PromptTrace <datarobot._experimental.models.genai.prompt_trace.PromptTrace>` for interacting with DataRobot prompt trace to support the following methods:
+  :meth:`PromptTrace.list <datarobot._experimental.models.genai.prompt_trace.PromptTrace.list>` to list all prompt traces from a given playground.
+  :meth:`PromptTrace.export_to_ai_catalog <datarobot._experimental.models.genai.prompt_trace.PromptTrace.export_to_ai_catalog>` to export prompt traces for the playground to AI catalog.
+- Added a new class :class: `InsightsConfiguration <datarobot._experimental.models.genai.insights_configuration.InsightsConfiguration>` for describing available insights and configured insights for a playground.
+  :meth:`InsightsConfiguration.list <datarobot._experimental.models.genai.insights_configuration.InsightsConfiguration.list>` to list the insights that are available to be configured.
+- Added a new class :class: `Insights <datarobot._experimental.models.genai.insights_configuration.Insights>` for configuring insights for a playground.
+  :meth:`Insights.get <datarobot._experimental.models.genai.insights_configuration.Insights.get>` to get the current insights configuration for a playground.
+  :meth:`Insights.create <datarobot._experimental.models.genai.insights_configuration.Insights.create>` to create or update the insights configuration for a playground.
+- Added a new class :class: `CostMetricConfiguration <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration>` for describing available cost metrics and configured cost metrics for a Use Case.
+  :meth:`CostMetricConfiguration.get <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.get>` to get the cost metric configuration.
+  :meth:`CostMetricConfiguration.create <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.create>` to create a cost metric configuration.
+  :meth:`CostMetricConfiguration.update <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.update>` to update the cost metric configuration.
+  :meth:`CostMetricConfiguration.delete <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.delete>` to delete the cost metric configuration.Key
+- Added a new class :class: `LLMCostConfiguration <datarobot._experimental.models.genai.cost_metric_configurations.LLMCostConfiguration>` for the cost configuration of a specific llm within a Use Case.
+
+API changes
+***********
+- Parameter Overrides: Users can now override most of the previously set configuration values directly through parameters when initializing the Client. Exceptions: The endpoint and token values must be initialized from one source (client params, environment, or config file) and cannot be overridden individually, for security and consistency reasons. The new configuration priority is as follows:
+  1.  Client Params
+  2.  Client config_path param
+  3.  Environment Variables
+  4.  Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
+- `DATAROBOT_API_CONSUMER_TRACKING_ENABLED` now always defaults to `True`.
+- Added Databricks personal access token and service principal (also shared credentials via secure config) authentication for uploading datasets from Databricks or creating a project from Databricks data.
+- Added secure config support for AWS long term credentials.
+- Implemented support for `dr-database-v1` to `DataStore <datarobot.models.DataStore>`, `DataSource <datarobot.models.DataStore>`, and  `DataDriver <datarobot.models.DataDriver>.` Added enum classes to support the changes.
+- You can retrieve the canonical URI for a Use Case using :meth:`UseCase.get_uri <datarobot.UseCase.get_uri>`.
+- You can open a Use Case in a browser using :meth:`UseCase.open_in_browser <datarobot.UseCase.open_in_browser>`.
+
+Enhancements
+************
+- Added a new parameter to :meth:`Dataset.create_from_url <datarobot.models.Dataset.create_from_url>` to support fast dataset registration:
+  - `sample_size`
+- Added a new parameter to :meth:`Dataset.create_from_data_source <datarobot.models.Dataset.create_from_data_source>` to support fast dataset registration:
+  - `sample_size`
+- :meth:`Job.get_result_when_complete <datarobot.models.Job.get_result_when_complete>`
+  returns :class:`datarobot.models.DatetimeModel` instead of the :class:`datarobot.models.Model`
+  if a datetime model was trained.
+- :meth:`Dataset.get_as_dataframe <datarobot.models.Dataset.get_as_dataframe>` can handle
+  downloading parquet files as well as csv files.
+- Implement support for `dr-database-v1` in `DataStore <datarobot.models.DataStore>`
+- Added two new parameters to :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` for paginating long job definitions lists:
+  - `offset`
+  - `limit`
+- Added two new parameters to :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` for filtering the job definitions:
+  - `deployment_id`
+  - `search_name`
+- Added new parameter to :meth:`Deployment.validate_replacement_model<datarobot.models.Deployment.validate_replacement_model>` to support replacement validation based on model package ID:
+  - `new_registered_model_version_id`
+- Added support for Native Connectors to `Connector <datarobot.models.Connector>` for everything other than :meth:` Connector.create <datarobot.models.Connector.create>` and :meth:` Connector.update <datarobot.models.Connector.update>`
+
+Deprecation summary
+*******************
+- Removed `Model.get_leaderboard_ui_permalink` and `Model.open_model_browser`
+- Deprecated :meth:`Project.get_models <datarobot.models.Project.get_models>` in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
+- :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` will no longer return all job definitions after version 3.6 is released.
+  To preserve current behavior please pass limit=0.
+- `new_model_id` parameter in :meth:`Deployment.validate_replacement_model<datarobot.models.Deployment.validate_replacement_model>` will be removed after version 3.6 is released.
+- :meth:`Deployment.replace_model<datarobot.models.Deployment.replace_model>` will be removed after version 3.6 is released.
+  Method :meth:`Deployment.perform_model_replace<datarobot.models.Deployment.perform_model_replace>` should be used instead.
+- :meth:`CustomInferenceModel.assign_training_data <datarobot.CustomInferenceModel.assign_training_data>` was marked as deprecated in v3.2. The deprecation period has been extended, and the feature will now be removed in v3.5.
+  Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
 
-3.3.1
-========
+Documentation changes
+*********************
+- Updated `genai_example.rst` to utilize latest genAI features and methods introduced most recently in the API client.
 
-Bugfixes
-********
-- Fixed setting ssl_verify by env variables in :meth: `config_from_env <datarobot.client._config_from_env>`
+Experimental changes
+*********************
+- Added new attribute, `prediction_timeout` to :class:`CustomModelValidation <datarobot.models.genai.custom_model_validation.CustomModelValidation>`.
+- Added new attributes, `feedback_result`, `metrics`, and `final_prompt` to :class:`ResultMetadata <datarobot._experimental.models.genai.chat_prompt.ResultMetadata>`.
+- Added `use_case_id` to :class:`CustomModelValidation <datarobot.models.genai.custom_model_validation.CustomModelValidation>`.
+- Added `llm_blueprints_count` and `user_name` to :class:`Playground <datarobot.models.genai.playground.Playground>`.
+- Added `custom_model_embedding_validations` to :class:`SupportedEmbeddings <datarobot._experimental.models.genai.vector_database.SupportedEmbeddings>`.
+- Added `embedding_validation_id` and `is_separator_regex` to :class:`VectorDatabase <datarobot._experimental.models.genai.vector_database.VectorDatabase>`.
+
+- Added optional parameters, `use_case`, `name`, and `model` to :meth:`CustomModelValidation.create <datarobot.models.genai.custom_model_validation.CustomModelValidation.create>`.
+- Added a method :meth:`CustomModelValidation.list <datarobot.models.genai.custom_model_validation.CustomModelValidation.list>`, to list custom model validations available to a user with several optional parameters to filter the results.
+- Added a method :meth:`CustomModelValidation.update <datarobot.models.genai.custom_model_validation.CustomModelValidation.update>`, to update a custom model validation.
+
+- Added an optional parameter, `use_case`, to :meth:`LLMDefinition.list <datarobot.models.genai.llm.LLMDefinition.list>`,
+  to include in the returned LLMs the external LLMs available for the specified `use_case` as well.
+
+- Added optional parameter, `playground` to :meth:`VectorDatabase.list <datarobot.models.genai.vector_database.VectorDatabase.list>`
+  to list vector databases by playground.
+
+- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.list <datarobot.models.genai.comparison_prompt.ComparisonPrompt.list>`, to list comparison prompts by comparison chat.
+- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.create <datarobot.models.genai.comparison_prompt.ComparisonPrompt.create>`, to specify the comparison chat to create the comparison prompt in.
+- Added optional parameter, `feedback_result`, to :meth:`ComparisonPrompt.update <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.update>`, to update a comparison prompt with feedback.
+
+- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.update <datarobot.models.genai.llm_blueprint.LLMBlueprint.update>`
+  to update the LLM Blueprint's starred status.
+- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.list <datarobot.models.genai.llm_blueprint.LLMBlueprint.list>`
+  to filter the returned LLM blueprints to those matching `is_starred`.
+
+- Added a new enum PromptType, :class:`PromptType <datarobot.enums.PromptType>` to identify the LLMBlueprint's prompting type.
+- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.create <datarobot.models.genai.llm_blueprint.LLMBlueprint.create>`,
+  to specify the LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot.enums.PromptType>`.
+- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.update <datarobot.models.genai.llm_blueprint.LLMBlueprint.update>`,
+  to specify the updated LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot.enums.PromptType>`.
+
+- Added a new class, :class:`ComparisonChat <datarobot.models.genai.comparison_chat.ComparisonChat>`, for interacting with DataRobot generative AI comparison chats.
+  :meth:`ComparisonChat.get <datarobot.models.genai.comparison_chat.ComparisonChat.get>` retrieves a comparison chat object by ID.
+  :meth:`ComparisonChat.list <datarobot.models.genai.comparison_chat.ComparisonChat.list>` lists all comparison chats available to the user.
+  :meth:`ComparisonChat.create <datarobot.models.genai.comparison_chat.ComparisonChat.create>` creates a new comparison chat.
+  :meth:`ComparisonChat.update <datarobot.models.genai.comparison_chat.ComparisonChat.update>` updates the name of a comparison chat.
+  :meth:`ComparisonChat.delete <datarobot.models.genai.comparison_chat.ComparisonChat.delete>` deletes a single comparison chat.
+
+- Added optional parameters, `playground` and `chat` to :meth:`ChatPrompt.list <datarobot.models.genai.chat_prompt.ChatPrompt.list>`, to list chat prompts by playground and chat.
+- Added optional parameter, `chat` to :meth:`ChatPrompt.create <datarobot.models.genai.chat_prompt.ChatPrompt.create>`, to specify the chat to create the chat prompt in.
+- Added a new method, :meth:`ChatPrompt.update <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.update>`, to update a chat prompt with custom metrics and feedback.
+
+- Added a new class, :class:`Chat <datarobot.models.genai.chat.Chat>`, for interacting with DataRobot generative AI chats.
+  :meth:`Chat.get <datarobot.models.genai.chat.Chat.get>` retrieves a chat object by ID.
+  :meth:`Chat.list <datarobot.models.genai.chat.Chat.list>` lists all chats available to the user.
+  :meth:`Chat.create <datarobot.models.genai.chat.Chat.create>` creates a new chat.
+  :meth:`Chat.update <datarobot.models.genai.chat.Chat.update>` updates the name of a chat.
+  :meth:`Chat.delete <datarobot.models.genai.chat.Chat.delete>` deletes a single chat.
+
+- Removed the `model_package` module. Use :class:`RegisteredModelVersion <datarobot.models.RegisteredModelVersion>` instead.
+- Added new class :class:`UserLimits <datarobot.models.genai.user_limits.UserLimits>`
+  - Added support to get the count of users' LLM API requests. :meth:`UserLimits.get_llm_requests_count <datarobot.models.genai.user_limits.UserLimits.get_llm_requests_count>`
+  - Added support to get the count of users' vector databases. :meth:`UserLimits.get_vector_database_count <datarobot.models.genai.user_limits.UserLimits.get_vector_database_count>`
+- Added new methods to the class :class:`Notebook <datarobot._experimental.models.notebooks.Notebook>` which includes :meth:`Notebook.run <datarobot._experimental.models.notebooks.Notebook.run>` and :meth:`Notebook.download_revision <datarobot._experimental.models.notebooks.Notebook.download_revision>`. See the documentation for example usage.
+- Added new class :class:`NotebookScheduledJob <datarobot._experimental.models.notebooks.NotebookScheduledJob>`.
+- Added new class :class:`NotebookScheduledRun <datarobot._experimental.models.notebooks.NotebookScheduledRun>`.
+- Added a new method :meth:`Model.get_incremental_learning_metadata <datarobot._experimental.models.model.Model.get_incremental_learning_metadata>` that retrieves incremental learning metadata for a model.
+- Added a new method :meth:`Model.start_incremental_learning <datarobot._experimental.models.model.Model.start_incremental_learning>` that starts incremental learning for a model.
+- Updated the API endpoint prefix for all GenerativeAI routes to align with the publicly documented routes.
+
+Bugfixes
+********
+- Fixed how async url is build in :meth:`Model.get_or_request_feature_impact <datarobot.models.Model.get_or_request_feature_impact>`
+- Fixed setting ssl_verify by env variables.
+- Resolved a problem related to tilde-based paths in the Client's 'config_path' attribute.
+- Changed the force_size default of :class:`ImageOptions <datarobot.helpers.image_utils.ImageOptions>` to apply the same transformations by default, which are applied when image archive datasets are uploaded to DataRobot.
 
 3.3.0
 =====
 
-New Features
+New features
 ************
 - Added support for Python 3.11.
 - Added new library "strenum" to add `StrEnum` support while maintaining backwards compatibility with Python 3.7-3.10. DataRobot does not use the native `StrEnum` class in Python 3.11.
 - Added a new class :class:`PredictionEnvironment <datarobot.models.PredictionEnvironment>` for interacting with DataRobot Prediction environments.
 - Extended the advanced options available when setting a target to include new
   parameters: 'modelGroupId', 'modelRegimeId', and 'modelBaselines' (part of the AdvancedOptions object). These parameters allow you to specify the user columns required to run time series models without feature derivation in OTV projects.
+- Added a new method :meth:`PredictionExplanations.create_on_training_data <datarobot.PredictionExplanations.create_on_training_data>`, for computing prediction explanation on training data.
 
 - Added a new class :class:`RegisteredModel <datarobot.models.RegisteredModel>` for interacting with DataRobot registered models to support the following methods:
   :meth:`RegisteredModel.get <datarobot.models.RegisteredModel.get>` to retrieve RegisteredModel object by ID.
   :meth:`RegisteredModel.list <datarobot.models.RegisteredModel.list>` to list all registered models.
   :meth:`RegisteredModel.archive <datarobot.models.RegisteredModel.archive>` to permanently archive registered model.
   :meth:`RegisteredModel.update <datarobot.models.RegisteredModel.update>` to update registered model.
   :meth:`RegisteredModel.get_shared_roles <datarobot.models.RegisteredModel.get_shared_roles>` to retrieve access control information for registered model.
@@ -62,96 +309,95 @@
   :class:`datarobot.enums.CustomTaskOutgoingNetworkPolicy`.
 
 - Added a new method :meth:`BatchPredictionJob.score_with_leaderboard_model <datarobot.models.BatchPredictionJob.score_with_leaderboard_model>` to run batch predictions using a Leaderboard model instead of a deployment.
 - Set :class:`IntakeSettings <datarobot.models.batch_job.IntakeSettings>` and :class:`OutputSettings <datarobot.models.batch_job.OutputSettings>` to use `IntakeAdapters` and `OutputAdapters` enum values respectively for the property `type`.
 
 - Added method meth:`Deployment.get_predictions_vs_actuals_over_time <datarobot.models.Deployment.get_predictions_vs_actuals_over_time>` to retrieve a deployment's predictions vs actuals over time data.
 
-Enhancements
-************
-- Implement support for `dr-database-v1` in `DataStore <datarobot.models.DataStore>`
-
 Bugfixes
 ********
 - Payload property `subset` renamed to `source` in :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>`
 - Fixed an issue where Context.trace_context was not being set from environment variables or DR config files.
 - :meth:`Project.refresh <datarobot.models.Project.refresh>` no longer sets ``Project.advanced_options`` to a dictionary.
 - Fixed :meth:`Dataset.modify <datarobot.models.Dataset.modify>` to clarify behavior of when to preserve or clear categories.
 - Fixed an issue with enums in f-strings resulting in the enum class and property being printed instead of the enum property's value in Python 3.11 environments.
 
-Deprecation Summary
+Deprecation summary
 *******************
-- :meth:`Project.refresh <datarobot.models.Project.refresh>` will no longer set ``Project.advanced_options`` to a dictionary after version 3.5 is released. All interactions with ``Project.advanced_options`` should be expected to be through the :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` class.
-- `Project.set_advanced_options <datarobot.models.Project.set_advanced_options>` has been removed. Use :meth:`Project.set_options <datarobot.models.Project.set_options>` instead.
-- `Project.get_leaderboard_ui_permalink <datarobot.models.Project.get_leaderboard_ui_permalink>` has been removed. Use :meth:`Project.get_uri <datarobot.models.Project.get_uri>` instead.
-- `Model.get_leaderboard_ui_permalink <datarobot.models.Model.get_leaderboard_ui_permalink>` has been removed. Use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
-- `Model.open_model_browser <datarobot.models.Model.open_model_browser>` has been removed. Use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
+- :meth:`Project.refresh <datarobot.models.Project.refresh>` will no longer set ``Project.advanced_options`` to a dictionary after version 3.5 is released.
+   All interactions with ``Project.advanced_options`` should be expected to be through the :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` class.
 
 Experimental changes
-*********************
-- Added a new class, :class:`VectorDatabase <datarobot._experimental.models.genai.vector_database.VectorDatabase>`, for interacting with DataRobot vector databases.
-  :meth:`VectorDatabase.get <datarobot._experimental.models.genai.vector_database.VectorDatabase.get>` retrieves a VectorDatabase object by ID.
-  :meth:`VectorDatabase.list <datarobot._experimental.models.genai.vector_database.VectorDatabase.list>` lists all VectorDatabases available to the user.
-  :meth:`VectorDatabase.create <datarobot._experimental.models.genai.vector_database.VectorDatabase.create>` creates a new VectorDatabase.
-  :meth:`VectorDatabase.create <datarobot._experimental.models.genai.vector_database.VectorDatabase.create_from_custom_model>` allows you to use a validated deployment of a custom model as your own Vector Database.
-  :meth:`VectorDatabase.update <datarobot._experimental.models.genai.vector_database.VectorDatabase.update>` updates the name of a VectorDatabase.
-  :meth:`VectorDatabase.delete <datarobot._experimental.models.genai.vector_database.VectorDatabase.delete>` deletes a single VectorDatabase.
-  :meth:`VectorDatabase.get_supported_embeddings <datarobot._experimental.models.genai.vector_database.VectorDatabase.get_supported_embeddings>` retrieves all supported embedding models.
-  :meth:`VectorDatabase.get_supported_text_chunkings <datarobot._experimental.models.genai.vector_database.VectorDatabase.get_supported_text_chunkings>` retrieves all supported text chunking configurations.
-  :meth:`VectorDatabase.download_text_and_embeddings_asset <datarobot._experimental.models.genai.vector_database.VectorDatabase.download_text_and_embeddings_asset>` download a parquet file with internal vector database data.
-
-- Added a new class, :class:`CustomModelVectorDatabaseValidation <datarobot._experimental.models.genai.vector_database.CustomModelVectorDatabaseValidation>`, for validating custom model deployments for use as a vector database.
-  :meth:`CustomModelVectorDatabaseValidation.get <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelVectorDatabaseValidation object by ID.
-  :meth:`CustomModelVectorDatabaseValidation.get_by_values <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelVectorDatabaseValidation object by field values.
-  :meth:`CustomModelVectorDatabaseValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
-  :meth:`CustomModelVectorDatabaseValidation.revalidate <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external vector database.
-
-- Added a new class, :class:`Playground <datarobot._experimental.models.genai.playground.Playground>`, for interacting with DataRobot generative AI playgrounds.
-  :meth:`Playground.get <datarobot._experimental.models.genai.playground.Playground.get>` retrieves a playground object by ID.
-  :meth:`Playground.list <datarobot._experimental.models.genai.playground.Playground.list>` lists all playgrounds available to the user.
-  :meth:`Playground.create <datarobot._experimental.models.genai.playground.Playground.create>` creates a new playground.
-  :meth:`Playground.update <datarobot._experimental.models.genai.playground.Playground.update>` updates the name and description of a playground.
-  :meth:`Playground.delete <datarobot._experimental.models.genai.playground.Playground.delete>` deletes a single playground.
-
-- Added a new class, :class:`LLMDefinition <datarobot._experimental.models.genai.llm.LLMDefinition>`, for interacting with DataRobot generative AI LLMs.
-  :meth:`LLMDefinition.list <datarobot._experimental.models.genai.llm.LLMDefinition.list>` lists all LLMs available to the user.
-
-- Added a new class, :class:`LLMBlueprint <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint>`, for interacting with DataRobot generative AI LLM blueprints.
-  :meth:`LLMBlueprint.get <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.get>` retrieves an LLM blueprint object by ID.
-  :meth:`LLMBlueprint.list <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.list>` lists all LLM blueprints available to the user.
-  :meth:`LLMBlueprint.create <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.create>` creates a new LLM blueprint.
-  :meth:`LLMBlueprint.create_from_llm_blueprint <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.create_from_llm_blueprint>` creates a new LLM blueprint from an existing one.
-  :meth:`LLMBlueprint.update <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.update>` updates an LLM blueprint.
-  :meth:`LLMBlueprint.delete <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.delete>` deletes a single LLM blueprint.
-
-- Added a new class, :class:`ChatPrompt <datarobot._experimental.models.genai.chat_prompt.ChatPrompt>`, for interacting with DataRobot generative AI chat prompts.
-  :meth:`ChatPrompt.get <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.get>` retrieves a chat prompt object by ID.
-  :meth:`ChatPrompt.list <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.list>` lists all chat prompts available to the user.
-  :meth:`ChatPrompt.create <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.create>` creates a new chat prompt.
-  :meth:`ChatPrompt.delete <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.delete>` deletes a single chat prompt.
-
-- Added a new class, :class:`CustomModelLLMValidation <datarobot._experimental.models.genai.custom_model_llm_validation.CustomModelLLMValidation>`, for validating custom model deployments for use as a custom model LLM.
-  :meth:`CustomModelLLMValidation.get <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelLLMValidation object by ID.
-  :meth:`CustomModelLLMValidation.get_by_values <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelLLMValidation object by field values.
-  :meth:`CustomModelLLMValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
-  :meth:`CustomModelLLMValidation.revalidate <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external custom model LLM.
-
-- Added a new class, :class:`ComparisonPrompt <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt>`, for interacting with DataRobot generative AI comparison prompts.
-  :meth:`ComparisonPrompt.get <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.get>` retrieves a comparison prompt object by ID.
-  :meth:`ComparisonPrompt.list <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.list>` lists all comparison prompts available to the user.
-  :meth:`ComparisonPrompt.create <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.create>` creates a new comparison prompt.
-  :meth:`ComparisonPrompt.update <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.update>` updates a comparison prompt.
-  :meth:`ComparisonPrompt.delete <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.delete>` deletes a single comparison prompt.
+********************
+- Added a new class, :class:`VectorDatabase <datarobot.models.genai.vector_database.VectorDatabase>`, for interacting with DataRobot vector databases.
+  :meth:`VectorDatabase.get <datarobot.models.genai.vector_database.VectorDatabase.get>` retrieves a VectorDatabase object by ID.
+  :meth:`VectorDatabase.list <datarobot.models.genai.vector_database.VectorDatabase.list>` lists all VectorDatabases available to the user.
+  :meth:`VectorDatabase.create <datarobot.models.genai.vector_database.VectorDatabase.create>` creates a new VectorDatabase.
+  :meth:`VectorDatabase.create <datarobot.models.genai.vector_database.VectorDatabase.create_from_custom_model>` allows you to use a validated deployment of a custom model as your own Vector Database.
+  :meth:`VectorDatabase.update <datarobot.models.genai.vector_database.VectorDatabase.update>` updates the name of a VectorDatabase.
+  :meth:`VectorDatabase.delete <datarobot.models.genai.vector_database.VectorDatabase.delete>` deletes a single VectorDatabase.
+  :meth:`VectorDatabase.get_supported_embeddings <datarobot.models.genai.vector_database.VectorDatabase.get_supported_embeddings>` retrieves all supported embedding models.
+  :meth:`VectorDatabase.get_supported_text_chunkings <datarobot.models.genai.vector_database.VectorDatabase.get_supported_text_chunkings>` retrieves all supported text chunking configurations.
+  :meth:`VectorDatabase.download_text_and_embeddings_asset <datarobot.models.genai.vector_database.VectorDatabase.download_text_and_embeddings_asset>` download a parquet file with internal vector database data.
+
+- Added a new class, :class:`CustomModelVectorDatabaseValidation <datarobot.models.genai.vector_database.CustomModelVectorDatabaseValidation>`, for validating custom model deployments for use as a vector database.
+  :meth:`CustomModelVectorDatabaseValidation.get <datarobot.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelVectorDatabaseValidation object by ID.
+  :meth:`CustomModelVectorDatabaseValidation.get_by_values <datarobot.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelVectorDatabaseValidation object by field values.
+  :meth:`CustomModelVectorDatabaseValidation.create <datarobot.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
+  :meth:`CustomModelVectorDatabaseValidation.revalidate <datarobot.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external vector database.
+
+- Added a new class, :class:`Playground <datarobot.models.genai.playground.Playground>`, for interacting with DataRobot generative AI playgrounds.
+  :meth:`Playground.get <datarobot.models.genai.playground.Playground.get>` retrieves a playground object by ID.
+  :meth:`Playground.list <datarobot.models.genai.playground.Playground.list>` lists all playgrounds available to the user.
+  :meth:`Playground.create <datarobot.models.genai.playground.Playground.create>` creates a new playground.
+  :meth:`Playground.update <datarobot.models.genai.playground.Playground.update>` updates the name and description of a playground.
+  :meth:`Playground.delete <datarobot.models.genai.playground.Playground.delete>` deletes a single playground.
+
+- Added a new class, :class:`LLMDefinition <datarobot.models.genai.llm.LLMDefinition>`, for interacting with DataRobot generative AI LLMs.
+  :meth:`LLMDefinition.list <datarobot.models.genai.llm.LLMDefinition.list>` lists all LLMs available to the user.
+
+- Added a new class, :class:`LLMBlueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint>`, for interacting with DataRobot generative AI LLM blueprints.
+  :meth:`LLMBlueprint.get <datarobot.models.genai.llm_blueprint.LLMBlueprint.get>` retrieves an LLM blueprint object by ID.
+  :meth:`LLMBlueprint.list <datarobot.models.genai.llm_blueprint.LLMBlueprint.list>` lists all LLM blueprints available to the user.
+  :meth:`LLMBlueprint.create <datarobot.models.genai.llm_blueprint.LLMBlueprint.create>` creates a new LLM blueprint.
+  :meth:`LLMBlueprint.create_from_llm_blueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint.create_from_llm_blueprint>` creates a new LLM blueprint from an existing one.
+  :meth:`LLMBlueprint.update <datarobot.models.genai.llm_blueprint.LLMBlueprint.update>` updates an LLM blueprint.
+  :meth:`LLMBlueprint.delete <datarobot.models.genai.llm_blueprint.LLMBlueprint.delete>` deletes a single LLM blueprint.
+
+- Added a new class, :class:`ChatPrompt <datarobot.models.genai.chat_prompt.ChatPrompt>`, for interacting with DataRobot generative AI chat prompts.
+  :meth:`ChatPrompt.get <datarobot.models.genai.chat_prompt.ChatPrompt.get>` retrieves a chat prompt object by ID.
+  :meth:`ChatPrompt.list <datarobot.models.genai.chat_prompt.ChatPrompt.list>` lists all chat prompts available to the user.
+  :meth:`ChatPrompt.create <datarobot.models.genai.chat_prompt.ChatPrompt.create>` creates a new chat prompt.
+  :meth:`ChatPrompt.delete <datarobot.models.genai.chat_prompt.ChatPrompt.delete>` deletes a single chat prompt.
+
+- Added a new class, :class:`CustomModelLLMValidation <datarobot.models.genai.custom_model_llm_validation.CustomModelLLMValidation>`, for validating custom model deployments for use as a custom model LLM.
+  :meth:`CustomModelLLMValidation.get <datarobot.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelLLMValidation object by ID.
+  :meth:`CustomModelLLMValidation.get_by_values <datarobot.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelLLMValidation object by field values.
+  :meth:`CustomModelLLMValidation.create <datarobot.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
+  :meth:`CustomModelLLMValidation.revalidate <datarobot.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external custom model LLM.
+
+- Added a new class, :class:`ComparisonPrompt <datarobot.models.genai.comparison_prompt.ComparisonPrompt>`, for interacting with DataRobot generative AI comparison prompts.
+  :meth:`ComparisonPrompt.get <datarobot.models.genai.comparison_prompt.ComparisonPrompt.get>` retrieves a comparison prompt object by ID.
+  :meth:`ComparisonPrompt.list <datarobot.models.genai.comparison_prompt.ComparisonPrompt.list>` lists all comparison prompts available to the user.
+  :meth:`ComparisonPrompt.create <datarobot.models.genai.comparison_prompt.ComparisonPrompt.create>` creates a new comparison prompt.
+  :meth:`ComparisonPrompt.update <datarobot.models.genai.comparison_prompt.ComparisonPrompt.update>` updates a comparison prompt.
+  :meth:`ComparisonPrompt.delete <datarobot.models.genai.comparison_prompt.ComparisonPrompt.delete>` deletes a single comparison prompt.
 
 - Extended :class:`UseCase <datarobot.UseCase>`, adding two new fields to represent the count of vector databases and playgrounds.
 
+- Added a new method, :meth:`ChatPrompt.create_llm_blueprint <datarobot.models.genai.chat_prompt.ChatPrompt.create_llm_blueprint>`, to create an LLM blueprint from a chat prompt.
+
+- Added a new method, :meth:`CustomModelLLMValidation.delete <datarobot.models.genai.custom_model_validation.CustomModelValidation.delete>`, to delete a custom model LLM validation record.
+
+- Added a new method, :meth:`LLMBlueprint.register_custom_model <datarobot.models.genai.llm_blueprint.LLMBlueprint.register_custom_model>`, for registering a custom model from a generative AI LLM blueprint.
+
 3.2.0
 =====
 
-New Features
+New features
 ************
 - Added new methods to trigger batch monitoring jobs without providing a job definition.
   :meth:`BatchMonitoringJob.run <datarobot.models.BatchMonitoringJob.run>`
   :meth:`BatchMonitoringJob.get_status <datarobot.models.BatchMonitoringJob.get_status>`
   :meth:`BatchMonitoringJob.cancel <datarobot.models.BatchMonitoringJob.cancel>`
   :meth:`BatchMonitoringJob.download <datarobot.models.BatchMonitoringJob.download>`
 
@@ -248,15 +494,15 @@
   :meth:`DataSlice.list <datarobot.models.data_slice.DataSlice.list>` to retrieve all data slices in a project.
   :meth:`DataSlice.create <datarobot.models.data_slice.DataSlice.create>` to create a new data slice.
   :meth:`DataSlice.delete <datarobot.models.data_slice.DataSlice.delete>` to delete the data slice calling this method.
   :meth:`DataSlice.request_size <datarobot.models.data_slice.DataSlice.request_size>` to submit a request to calculate a data slice size on a source.
   :meth:`DataSlice.get_size_info <datarobot.models.data_slice.DataSlice.get_size_info>` to get the data slice's info when applied to a source.
   :meth:`DataSlice.get <datarobot.models.data_slice.DataSlice.get>` to retrieve a specific data slice.
 - Added new :class:`DataSliceSizeInfo <datarobot.models.data_slice.DataSliceSizeInfo>` to define the result of a data slice applied to a source.
-- Added new method for retrieving all available feature impacts for the model :meth: `Model.get_all_feature_impacts <datarobot.models.Model.get_all_feature_impacts>`
+- Added new method for retrieving all available feature impacts for the model :meth:`Model.get_all_feature_impacts <datarobot.models.Model.get_all_feature_impacts>`.
 - Added new method for StatusCheckJob to wait and return the completed object once it is generated :meth:`datarobot.models.StatusCheckJob.get_result_when_complete`
 
 
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
@@ -296,20 +542,20 @@
 Bugfixes
 ********
 - Fixed incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
 - Fixed a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 - Fixed an issue where failed authentication when invoking `datarobot.client.Client()` raises a misleading error about client-server compatibility.
 - Fixed incompatibilities with Pandas 2.0 in :meth:`AccuracyOverTime.get_as_dataframe <datarobot.models.deployment.AccuracyOverTime.get_as_dataframe>`. The method will now throw a `ValueError` if an empty list is passed to the parameter `metrics`.
 
-API Changes
+API changes
 ***********
 - Added parameter ``unsupervised_type`` to the class :class:`DatetimePartitioning <datarobot.DatetimePartitioning>`.
 - The sliced insight API endpoint `GET: api/v2/insights/<insight_name>/` returns a paginated response. This means that it returns an empty response if no insights data is found, unlike `GET: api/v2/projects/<pid>/models/<lid>/<insight_name>/`, which returns 404 NOT FOUND in this case. To maintain backwards-compatibility, all methods that retrieve insights data raise 404 NOT FOUND if the insights API returns an empty response.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``Model.get_feature_fit_metadata`` has been removed.
   Use :meth:`Model.get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>` instead.
 - ``DatetimeModel.get_feature_fit_metadata`` has been removed.
   Use :meth:`DatetimeModel.get_feature_effect_metadata <datarobot.models.DatetimeModel.get_feature_effect_metadata>` instead.
 - ``Model.request_feature_fit`` has been removed.
   Use :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>` instead.
@@ -326,29 +572,29 @@
 - Deprecated the use of :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` in favor of :class:`SharingRole <datarobot.models.sharing.SharingRole>` for sharing in the following classes:
   - :meth:`DataStore.share <datarobot.DataStore.share>`
 - Deprecated the following methods for retrieving :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` information.
   - :meth:`DataStore.get_access_list <datarobot.DataStore.get_access_list>`. Please use :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>` instead.
 - :meth:`CustomInferenceModel.assign_training_data <datarobot.CustomInferenceModel.assign_training_data>` was marked as deprecated and will be removed in v3.4.
   Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Deprecated parameter `user_agent_suffix` in `datarobot.Client`. `user_agent_suffix` will be removed in v3.4. Please use `trace_context` instead.
 
-Documentation Changes
+Documentation changes
 *********************
 - Fixed in-line documentation of `DataRobotClientConfig`.
 - Fixed documentation around client configuration from environment variables or config file.
 
 Experimental changes
-*********************
+********************
 - Added experimental support for data matching:
 
   - :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`
   - :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>`
 
 - Added new method :meth:`DataMatchingQuery.get_result <datarobot._experimental.models.data_matching.DataMatchingQuery.get_result>` for returning data matching query results as pandas dataframes to :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>` .
 - Changed behavior for returning results in the :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. Instead of saving the results as a file, a pandas dataframe will be returned in the following methods:
@@ -368,25 +614,22 @@
 
   - :class:`Recipe <datarobot._experimental.models.recipes.Recipe>`
 
 
 3.1.1
 =====
 
-Configuration Changes
+Configuration changes
 *********************
 - Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
 - Update `typing-extensions <https://pypi.org/project/typing-extensions/>`_ to be inclusive of versions from 4.3.0 to < 5.0.0.
 
 3.1.0
 =====
 
-New Features
-************
-
 Enhancements
 ************
 - Added new methods :meth:`BatchPredictionJob.apply_time_series_data_prep_and_score<datarobot.models.BatchPredictionJob.apply_time_series_data_prep_and_score>`
   and :meth:`BatchPredictionJob.apply_time_series_data_prep_and_score_to_file<datarobot.models.BatchPredictionJob.apply_time_series_data_prep_and_score_to_file>`
   that apply time series data prep to a file or dataset and make batch predictions with a deployment.
 - Added new methods :meth:`DataEngineQueryGenerator.prepare_prediction_dataset<datarobot.DataEngineQueryGenerator.prepare_prediction_dataset>`
   and :meth:`DataEngineQueryGenerator.prepare_prediction_dataset_from_catalog<datarobot.DataEngineQueryGenerator.prepare_prediction_dataset_from_catalog>`
@@ -410,38 +653,32 @@
   :meth:`ImageAugmentationList.list<datarobot.models.visualai.ImageAugmentationList.list>`,
   :meth:`ImageAugmentationList.update<datarobot.models.visualai.ImageAugmentationList.update>`
 
 Bugfixes
 ********
 - Added `format` key to Batch Prediction intake and output settings for S3, GCP and Azure
 
-API Changes
+API changes
 ***********
 - The method :meth:`PredictionExplanations.is_multiclass <datarobot.PredictionExplanations.is_multiclass>` now adds an additional API call to check for multiclass target validity, which adds a small delay.
 - :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` parameter ``blend_best_models`` defaults to false
 - :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` parameter ``consider_blenders_in_recommendation`` defaults to false
 - :class:`DatetimePartitioning <datarobot.DatetimePartitioning>` has parameter ``unsupervised_mode``
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Deprecated method :meth:`Project.create_from_hdfs<datarobot.models.Project.create_from_hdfs>`.
 - Deprecated method :meth:`DatetimePartitioning.generate <datarobot.DatetimePartitioning.generate>`.
 - Deprecated parameter ``in_use`` from :meth:`ImageAugmentationList.create<datarobot.models.visualai.ImageAugmentationList.create>` as DataRobot will take care of it automatically.
 - Deprecated property ``Deployment.capabilities`` from :class:`Deployment <datarobot.models.Deployment>`.
 - ``ImageAugmentationSample.compute`` was removed in v3.1. You
   can get the same information with the method ``ImageAugmentationList.compute_samples``.
 - ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead.
 
-Configuration Changes
-*********************
-
-Experimental changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 - Update the documentation to suggest that setting `use_backtest_start_end_format` of :py:meth:`DatetimePartitioning.to_specification <datarobot.DatetimePartitioning.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 - Update the documentation to suggest setting `use_start_end_format` of :py:meth:`Backtest.to_specification <datarobot.helpers.partitioning_methods.Backtest.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 3.0.3
 =====
@@ -452,36 +689,33 @@
 
 3.0.2
 =====
 
 Bugfixes
 ********
 - Restored `Model.get_leaderboard_ui_permalink`, `Model.open_model_browser`,
-  `Project.get_leaderboard_ui_permalink`, and `Project.open_leaderboard_browser <datarobot.models.Project.open_leaderboard_browser>`.
   These methods were accidentally removed instead of deprecated.
 - Fix for ipykernel < 6.0.0 which does not persist contextvars across cells
 
-Deprecation Summary
+Deprecation summary
 *******************
-- Deprecated method `Model.get_leaderboard_ui_permalink <datarobot.models.Model.get_leaderboard_ui_permalink>`. Please use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
-- Deprecated method `Model.open_model_browser <datarobot.models.Model.open_model_browser>`. Please use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
-- Deprecated method `Project.get_leaderboard_ui_permalink <datarobot.models.Project.get_leaderboard_ui_permalink>`. Please use :meth:`Project.get_uri <datarobot.models.Project.get_uri>` instead.
-- Deprecated method `Project.open_leaderboard_browser <datarobot.models.Project.open_leaderboard_browser>`. Please use :meth:`Project.open_in_browser <datarobot.models.Project.open_in_browser>` instead.
+- Deprecated method `Model.get_leaderboard_ui_permalink`. Please use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
+- Deprecated method `Model.open_model_browser`. Please use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
 
 3.0.1
 =====
 
 Bugfixes
 ********
 - Added `typing-extensions` as a required dependency for the DataRobot Python SDK.
 
 3.0.0
 =====
 
-New Features
+New features
 ************
 - Version 3.0 of the Python client does not support Python 3.6 and earlier versions. Version 3.0 currently supports Python 3.7+.
 
 - The default Autopilot mode for :meth:`project.start_autopilot <datarobot.models.Project.start_autopilot>` has changed to Quick mode.
 
 - For datetime-aware models, you can now calculate and retrieve feature impact for backtests other than zero and holdout:
 
@@ -566,21 +800,21 @@
 Bugfixes
 ********
 - :meth:`Dataset.list <datarobot.models.Dataset.list>` no longer throws errors when listing datasets with no owner.
 - Fixed an issue with the creation of ``BatchPredictionJobDefinitions`` containing a schedule.
 - Fixed error handling in ``datarobot.helpers.partitioning_methods.get_class``.
 - Fixed issue with portions of the payload not using camelCasing in :meth:`Project.upload_dataset_from_catalog<datarobot.models.Project.upload_dataset_from_catalog>`.
 
-API Changes
+API changes
 ***********
 - The Python client now outputs a `DataRobotProjectDeprecationWarning` when you attempt to access certain resources (projects, models, deployments, etc.) that are deprecated or disabled as a result of the DataRobot platform's migration to Python 3.
 - The Python client now raises a `TypeError` when you try to retrieve a labelwise ROC on a binary model or a binary ROC on a multilabel model.
 - The method :meth:`Dataset.create_from_data_source<datarobot.models.Dataset.create_from_data_source>` now raises ``InvalidUsageError`` if ``username`` and ``password`` are not passed as a pair together.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``Model.get_leaderboard_ui_permalink`` has been removed.
   Use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
 - ``Model.open_model_browser`` has been removed.
   Use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
 - ``Project.get_leaderboard_ui_permalink`` has been removed.
   Use :meth:`Project.get_uri <datarobot.models.Project.get_uri>` instead.
@@ -601,21 +835,21 @@
 - The :class:`Deployment <datarobot.models.Deployment>` method ``create_from_custom_model_image`` was removed. Use :meth:`Deployment.create_from_custom_model_version <datarobot.models.Deployment.create_from_custom_model_version>` instead.
 - ``PredictJob.create`` has been removed. Use :meth:`Model.request_predictions <datarobot.models.Model.request_predictions>` instead.
 - ``Model.fetch_resource_data`` has been removed. Use :meth:`Model.get <datarobot.models.Model.get>` instead.
 - The class ``CustomInferenceImage`` was removed. Use :class:`CustomModelVersion <datarobot.CustomModelVersion>` with ``base_environment_id`` instead.
 - ``Project.set_target`` has been deprecated. Use :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>` instead.
 
 
-Configuration Changes
+Configuration changes
 *********************
 - Added a context manager :meth:`client_configuration <datarobot.client.client_configuration>` that can be used to change the connection configuration temporarily, for use in asynchronous or multithreaded code.
 - Upgraded the `Pillow` library to version 9.2.0. Users installing DataRobot with the "images" extra (``pip install datarobot[images]``) should note that this is a required library.
 
 Experimental changes
-*********************
+********************
 
 - Added experimental support for retrieving document thumbnails:
 
   - :class:`DocumentThumbnail <datarobot.models.documentai.document.DocumentThumbnail>`
   - :class:`DocumentPageFile <datarobot.models.documentai.document.DocumentPageFile>`
 
 - Added experimental support to retrieve document text extraction samples using:
@@ -632,15 +866,15 @@
 - Added new methods to :class:`RetrainingPolicy <datarobot._experimental.models.retraining.RetrainingPolicy>`:
   - Use :meth:`RetrainingPolicy.get <datarobot._experimental.models.retraining.RetrainingPolicy.get>` to get a retraining policy associated with a deployment.
   -  Use :meth:`RetrainingPolicy.delete <datarobot._experimental.models.retraining.RetrainingPolicy.delete>` to delete a retraining policy associated with a deployment.
 
 2.29.0b0
 ========
 
-New Features
+New features
 ************
 - Added support to pass `max_ngram_explanations` parameter in batch predictions that will trigger the
   compute of text prediction explanations.
 
   - :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`
 
 - Added support to pass calculation mode to prediction explanations
@@ -712,38 +946,38 @@
 ********
 - Don't include holdout start date, end date, or duration in datetime partitioning payload when
   holdout is disabled.
 - Removed ICE Plot capabilities from Feature Fit.
 - Handle undefined calendar_name in CalendarFile.create_calendar_from_dataset
 - Raise ValueError for submitted calendar names that are not strings
 
-API Changes
+API changes
 ***********
 - `version` field is removed from `ImportedModel` object
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Reason Codes objects deprecated in 2.13 version were removed.
   Please use Prediction Explanations instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - The upper version constraint on pandas has been removed.
 
-Documentation Changes
+Documentation changes
 *********************
 - Fixed a minor typo in the example for Dataset.create_from_data_source.
 
 - Update the documentation to suggest that `feature_derivation_window_end` of :py:class:`datarobot.DatetimePartitioningSpecification` class should be a negative or zero.
 
 
 2.28.0
 ======
 
-New Features
+New features
 ************
 - Added new parameter `upload_read_timeout` to :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`
   and :meth:`BatchPredictionJob.score_to_file <datarobot.models.BatchPredictionJob.score_to_file>` to indicate how many seconds to wait
   until intake dataset uploads to server. Default value 600s.
 
 - Added the ability to turn off supervised feature reduction for Time Series projects. Option
   `use_supervised_feature_reduction` can be set in :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>`.
@@ -804,18 +1038,18 @@
 - Added support for governance, owners, predictionEnvironment, and fairnessHealth fields when querying for a Deployment object.
 
 - Added helper methods for working with files, images and documents. Methods support conversion of
   file contents into base64 string representations. Methods for images provide also image resize and
   transformation support.
 
   Functionality:
-    - `datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_urls.`
-    - `datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_paths`
-    - `datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_paths`
-    - `datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_urls`
+    - :meth:`get_encoded_file_contents_from_urls <datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_urls>`
+    - :meth:`get_encoded_file_contents_from_paths <datarobot.helpers.binary_data_utils.get_encoded_file_contents_from_paths>`
+    - :meth:`get_encoded_image_contents_from_paths <datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_paths>`
+    - :meth:`get_encoded_image_contents_from_urls <datarobot.helpers.binary_data_utils.get_encoded_image_contents_from_urls>`
 
 Enhancements
 ************
 - Requesting metadata instead of actual data of :class:`datarobot.PredictionExplanations` to reduce the amount of data transfer
 
 Bugfixes
 ********
@@ -826,47 +1060,47 @@
 - Fix a bug where credentials were incorrectly formatted in
   :meth:`Project.upload_dataset_from_catalog <datarobot.models.Project.upload_dataset_from_catalog>`
   and
   :meth:`Project.upload_dataset_from_data_source <datarobot.models.Project.upload_dataset_from_data_source>`
 - Rejecting downloads of Batch Prediction data that was not written to the localfile output adapter
 - Fix a bug in :meth:`datarobot.models.BatchPredictionJobDefinition.create` where `schedule` was not optional for all cases
 
-API Changes
+API changes
 ***********
 
 - User can include ICE plots data in the response when requesting Feature Effects/Feature Fit. Extended methods are
     - :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>`,
     - ``Model.get_feature_fit <datarobot.models.Model.get_feature_fit>``,
     - :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` and
     - ``DatetimeModel.get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>``.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - `attrs` library is removed from library dependencies
 - ``ImageAugmentationSample.compute`` was marked as deprecated and will be removed in v2.30. You
   can get the same information with newly introduced method ``ImageAugmentationList.compute_samples``
 - ``ImageAugmentationSample.list`` using ``sample_id``
 - Deprecating scaleout parameters for projects / models. Includes ``scaleout_modeling_mode``,
   ``scaleout_max_train_pct``, and ``scaleout_max_train_rows``
 
-Configuration Changes
+Configuration changes
 *********************
 - `pandas` upper version constraint is updated to include version 1.3.5.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Fixed "from datarobot.enums" import in Unsupervised Clustering example provided in docs.
 
 
 2.27.0
 ========
 
-New Features
+New features
 ************
 - :class:`datarobot.UserBlueprint` is now mature with full support of functionality. Users
   are encouraged to use the `Blueprint Workshop <blueprint-workshop.datarobot.com>`_ instead of
   this class directly.
 - Added the arguments attribute in :class:`datarobot.CustomTaskVersion`.
 - Added the ability to retrieve detected errors in the potentially multicategorical feature types that prevented the
   feature to be identified as multicategorical.
@@ -967,41 +1201,38 @@
 
 Bugfixes
 ********
 - fix :class:`datarobot.CustomTaskVersion` and :class:`datarobot.CustomModelVersion` to correctly format ``required_metadata_values``
   before sending them via API
 - Fixed response validation that could cause `DataError` when using :class:`datarobot.models.Dataset` for a dataset with a description that is an empty string.
 
-API Changes
+API changes
 ***********
 - :meth:`RelationshipsConfiguration.create <datarobot.models.RelationshipsConfiguration.create>` will include a
   new key ``data_source_id`` in `data_source` field when applicable
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``Model.get_all_labelwise_roc_curves`` has been removed.
   You can get the same information with multiple calls of
   :meth:`Model.get_labelwise_roc_curves <datarobot.models.Model.get_labelwise_roc_curves>`, one per data source.
 - ``Model.get_all_multilabel_lift_charts`` has been removed.
   You can get the same information with multiple calls of
   :meth:`Model.get_multilabel_lift_charts <datarobot.models.Model.get_multilabel_lift_charts>`, one per data source.
 
-Configuration Changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 - This release introduces a new documentation organization. The organization has been modified to better reflect the end-to-end modeling workflow. The new "Tutorials" section has 5 major topics that outline the major components of modeling: Data, Modeling, Predictions, MLOps, and Administration.
 - The Getting Started workflow is now hosted at `DataRobot's API Documentation Home <https://docs.datarobot.com/en/docs/api/index.html>`_.
 - Added an example of how to set up optimized datetime partitioning for time series projects.
 
 2.26.0
 ========
 
-New Features
+New features
 ************
 - Added the ability to use external baseline predictions for time series project. External
   dataset can be validated using :meth:`datarobot.models.Project.validate_external_time_series_baseline`.
   Option can be set in :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` to scale
   datarobot models' accuracy performance using external dataset's accuracy performance.
   See the :ref:`external baseline predictions documentation <external_baseline_predictions>`
   for more information.
@@ -1080,52 +1311,52 @@
 - :meth:`RelationshipsConfiguration.create <datarobot.models.RelationshipsConfiguration.create>` will return a ``catalog``
   in `data_source` field
 - Argument ``required_metadata_keys`` was not properly being sent in the update and create requests for
   :class:`datarobot.ExecutionEnvironment`.
 - Fix issue with :class:`datarobot.ExecutionEnvironment` create method failing when used against older versions of the application
 - :class:`datarobot.CustomTaskVersion` was not properly handling ``required_metadata_values`` from the API response
 
-API Changes
+API changes
 ***********
 
 - Updated :meth:`Project.start <datarobot.models.Project.start>` to use ``AUTOPILOT_MODE.QUICK`` when the
   ``autopilot_on`` param is set to True. This brings it in line with :meth:`Project.set_target
   <datarobot.models.Project.set_target>`.
 - Updated :meth:`project.start_autopilot <datarobot.models.Project.start_autopilot>` to accept
   the following new GA parameters that are already in the public API: ``consider_blenders_in_recommendation``,
   ``run_leakage_removed_feature_list``
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - The ``required_metadata`` property of :class:`datarobot.CustomModelVersion` has been deprecated.
   ``required_metadata_values`` should be used instead.
 
 - The ``required_metadata`` property of :class:`datarobot.CustomTaskVersion` has been deprecated.
   ``required_metadata_values`` should be used instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - Now requires dependency on package `scikit-learn <https://pypi.org/project/scikit-learn/>`_  rather than
   `sklearn <https://pypi.org/project/scikit-learn/>`_. Note: This dependency is only used in example code. See
   `this scikit-learn issue <https://github.com/scikit-learn/scikit-learn/issues/8215>`_ for more information.
 - Now permits dependency on package `attrs <https://pypi.org/project/attrs/>`_  to be less than version 21. This
   fixes compatibility with apache-airflow.
 
 - Allow to setup ``Authorization: <type> <token>`` type header for OAuth2 Bearer tokens.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Update the documentation with respect to the permission that controls AI Catalog dataset snapshot behavior.
 
 2.25.0
 ======
 
-New Features
+New features
 ************
 - There is a new :class:`AnomalyAssessmentRecord<datarobot.models.anomaly_assessment.AnomalyAssessmentRecord>` object that
   implements public API routes to work with anomaly assessment insight. This also adds explanations
   and predictions preview classes. The insight is available for anomaly detection models in time
   series unsupervised projects which also support calculation of Shapley values.
 
     - :class:`AnomalyAssessmentPredictionsPreview<datarobot.models.anomaly_assessment.AnomalyAssessmentPredictionsPreview>`
@@ -1210,15 +1441,15 @@
 
 - Ensure that if a configured endpoint ends in a trailing slash, the resulting full URL does
   not end up with double slashes in the path.
 
 - :meth:`Model.request_frozen_datetime_model <datarobot.models.Model.request_frozen_datetime_model>` is now implementing correct
   validation of input parameter ``training_start_date``.
 
-API Changes
+API changes
 ***********
 
 - Arguments ``secondary_datasets`` now accept :py:class:`SecondaryDataset <datarobot.helpers.feature_discovery.SecondaryDataset>`
   to create secondary dataset configurations
   - :meth:`SecondaryDatasetConfigurations.create <datarobot.models.SecondaryDatasetConfigurations.create>`
 
 - Arguments ``dataset_definitions`` and ``relationships`` now accept :py:class:`DatasetDefinition <datarobot.helpers.feature_discovery.DatasetDefinition>` :py:class:`Relationship <datarobot.helpers.feature_discovery.Relationship>`
@@ -1235,15 +1466,15 @@
 - Argument ``required_metadata`` has been added to :class:`datarobot.CustomModelVersion`.  This should be set with
   relevant values defined by the base environment's ``required_metadata_keys``
 
 
 2.24.0
 =========
 
-New Features
+New features
 ************
 
 - Partial history predictions can be made with time series time series multiseries models using the
   ``allow_partial_history_time_series_predictions`` attribute of the
   :py:class:`datarobot.DatetimePartitioningSpecification
   <datarobot.DatetimePartitioningSpecification>`.
   See the :ref:`Time Series <time_series>` documentation for more info.
@@ -1295,48 +1526,45 @@
 Bugfixes
 ********
 - Fixed response validation that could cause `DataError` when using
   :meth:`TrainingPredictions.list <datarobot.models.training_predictions.TrainingPredictions.list>` and
   :meth:`TrainingPredictions.get_all_as_dataframe <datarobot.models.training_predictions.TrainingPredictions.get_all_as_dataframe>`
   methods if there are training predictions computed with `explanation_algorithm`.
 
-API Changes
+API changes
 ***********
 - Remove `desired_memory` param from the following classes: :class:`datarobot.CustomInferenceModel`,
   :class:`datarobot.CustomModelVersion`, :class:`datarobot.CustomModelTest`
 - Remove ``desired_memory`` param from the following methods:
   :meth:`CustomInferenceModel.create <datarobot.CustomInferenceModel.create>`,
   :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>`,
   :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>`,
   :meth:`CustomModelTest.create <datarobot.CustomModelTest.create>` and
   :meth:`CustomModelTest.create <datarobot.CustomModelTest.create>`
 
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - class ``ComplianceDocumentation``
   will be deprecated in v2.24 and will be removed entirely in v2.27. Use
   :class:`AutomatedDocument<datarobot.models.automated_documentation.AutomatedDocument>`
   instead. To start off, see the
   :ref:`Automated Documentation overview<automated_documentation_overview>` for details.
 
-Configuration Changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 
 - Remove reference to S3 for :meth:`Project.upload_dataset <datarobot.models.Project.upload_dataset>` since it is not supported by the server
 
 
 2.23.0
 ======
 
-New Features
+New features
 ************
 - Calendars for time series projects can now be automatically generated by providing a country code to the method
   :meth:`CalendarFile.create_calendar_from_country_code<datarobot.CalendarFile.create_calendar_from_country_code>`.
   A list of allowed country codes can be retrieved using :meth:`CalendarFile.get_allowed_country_codes<datarobot.CalendarFile.get_allowed_country_codes>`
   For more information, see the :ref:`calendar documentation <preloaded_calendar_files>`.
 
 - Added `calculate_all_series`` param to
@@ -1423,49 +1651,49 @@
 - Using :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.download>` could in some circumstances
   result in a crash from trying to abort the job if it fails to start
 
 - Using :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.download>` or
   :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score_to_file>` would produce incomplete
   results in case a job was aborted while downloading. This will now raise an exception.
 
-API Changes
+API changes
 ***********
 - New ``sampling_method`` param in :meth:`Model.train_datetime <datarobot.models.Model.train_datetime>`,
   :meth:`Project.train_datetime <datarobot.models.Project.train_datetime>`,
   :meth:`Model.train_datetime <datarobot.models.Model.request_frozen_datetime_model>` and
   :meth:`Model.train_datetime <datarobot.models.Model.retrain>`.
 - New ``target_type`` param in :class:`datarobot.CustomInferenceModel`
 - New arguments ``secondary_datasets``, ``name``, ``creator_full_name``, ``creator_user_id``, ``created``,
     ``featurelist_id``, ``credentials_ids``, ``project_version`` and ``is_default`` in :class:`datarobot.models.SecondaryDatasetConfigurations`
 - New arguments ``secondary_datasets``, ``name``, ``featurelist_id`` to
     :meth:`SecondaryDatasetConfigurations.create <datarobot.models.SecondaryDatasetConfigurations.create>`
 - Class ``FeatureEngineeringGraph`` has been removed. Use :class:`datarobot.models.RelationshipsConfiguration` instead.
 - Param ``feature_engineering_graphs`` removed from :meth:`Project.set_target<datarobot.models.Project.set_target>`.
 - Param ``config`` removed from :meth:`SecondaryDatasetConfigurations.create<datarobot.models.SecondaryDatasetConfigurations.create>`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - ``supports_binary_classification`` and  ``supports_regression`` are deprecated
     for :class:`datarobot.CustomInferenceModel` and will be removed in v2.24
 - Argument ``config`` and  ``supports_regression`` are deprecated
     for :class:`datarobot.models.SecondaryDatasetConfigurations` and will be removed in v2.24
 - ``CustomInferenceImage`` has been deprecated and will be removed in v2.24.
     :class:`datarobot.CustomModelVersion` with base_environment_id should be used in their place.
 - ``environment_id`` and ``environment_version_id`` are deprecated for :meth:`CustomModelTest.create<datarobot.CustomModelTest.create>`
 
-Documentation Changes
+Documentation changes
 *********************
 
 - `feature_lineage_id` is added as a new parameter in the response for retrieval of a :class:`datarobot.models.Feature` created by automated feature discovery or time series feature derivation.
   This id is required to retrieve a :class:`datarobot.models.FeatureLineage` instance.
 
 2.22.1
 ======
 
-New Features
+New features
 ************
 
 - Batch Prediction jobs now support :ref:`dataset <batch_predictions-intake-types-dataset>` as intake settings for
   :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 
 - Create a Dataset from DataSource:
 
@@ -1556,40 +1784,34 @@
 
 - Make trafaret validator for datasets use a syntax that works properly with a wider range of trafaret versions.
 
 - Handle extra keys in CustomModelTests and CustomModelVersions
 
 - ``ImageEmbedding`` and ``ImageActivationMap`` now supports regression projects.
 
-API Changes
+API changes
 ***********
 
 - The default value for the ``mode`` param in :meth:`Project.set_target
   <datarobot.models.Project.set_target>` has been changed from ``AUTOPILOT_MODE.FULL_AUTO``
   to ``AUTOPILOT_MODE.QUICK``
 
-Deprecation Summary
-*******************
-
-Configuration Changes
-*********************
-
-Documentation Changes
+Documentation changes
 *********************
 
 - Added links to classes with duration parameters such as `validation_duration` and `holdout_duration` to
   provide duration string examples to users.
 
 - The :ref:`models documentation <models>` has been revised to include section on how to train a new model and how to run cross-validation
   or backtesting for a model.
 
 2.21.0
 ======
 
-New Features
+New features
 ************
 
 - Added new arguments ``explanation_algorithm`` and ``max_explanations`` to method
   :meth:`Model.request_training_predictions <datarobot.models.Model.request_training_predictions>`.
   New fields ``explanation_algorithm``, ``max_explanations`` and ``shap_warnings`` have been added to class
   :class:`TrainingPredictions <datarobot.models.training_predictions.TrainingPredictions>`.
   New fields ``prediction_explanations`` and ``shap_metadata`` have been added to class
@@ -1728,35 +1950,35 @@
 ********
 
 - An issue with input validation of the Batch Prediction module
 - parent_model_id was not visible for all frozen models
 - Batch Prediction jobs that used other output types than `local_file` failed when using `.wait_for_completion()`
 - A race condition in the Batch Prediction file scoring logic
 
-API Changes
+API changes
 ***********
 
 - Three new fields were added to the :class:`Dataset<datarobot.models.Dataset>` object. This reflects the
   updated fields in the public API routes at `api/v2/datasets/`. The added fields are:
 
     - processing_state: Current ingestion process state of the dataset
     - row_count: The number of rows in the dataset.
     - size: The size of the dataset as a CSV in bytes.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``datarobot.enums.VARIABLE_TYPE_TRANSFORM.CATEGORICAL`` for is deprecated for the following and will be removed in  v2.22.
     - meth:`Project.batch_features_type_transform`
     - meth:`Project.create_type_transform_feature`
 
 2.20.0
 ======
 
-New Features
+New features
 ************
 
 - There is a new :class:`Dataset<datarobot.models.Dataset>` object that implements some of the
   public API routes at `api/v2/datasets/`. This also adds two new feature classes and a details
   class.
 
     - :class:`DatasetFeature<datarobot.models.DatasetFeature>`
@@ -1846,30 +2068,18 @@
 ********
 - An issue where uploaded CSV's would loose quotes during serialization causing issues when columns containing line terminators where loaded in a dataframe, has been fixed
 
 - :meth:`Project.get_association_featurelists <datarobot.models.Project.get_association_featurelists>` is now using the correct endpoint name, but the old one will continue to work
 
 - Python API :class:`PredictionServer<datarobot.PredictionServer>` supports now on-premise format of API response.
 
-API Changes
-***********
-
-Deprecation Summary
-*******************
-
-Configuration Changes
-*********************
-
-Documentation Changes
-*********************
-
 2.19.0
 ======
 
-New Features
+New features
 ************
 
 - Projects can be cloned using :meth:`Project.clone_project <datarobot.models.Project.clone_project>`
 - Calendars used in time series projects now support having series-specific events, for instance if a holiday only affects some stores. This can be controlled by using new argument of the :meth:`CalendarFile.create <datarobot.CalendarFile.create>` method.
   If multiseries id columns are not provided, calendar is considered to be single series and all events are applied to all series.
 - We have expanded prediction intervals availability to the following use-cases:
 
@@ -1929,30 +2139,30 @@
     - ``order_by``: An attribute by which to sort the results
 
 
 Bugfixes
 ********
 - An issue when using :meth:`Feature.get <datarobot.models.Feature.get>` and :meth:`ModelingFeature.get <datarobot.models.ModelingFeature.get>` to retrieve summarized categorical feature has been fixed.
 
-API Changes
+API changes
 ***********
 - The datarobot package is now no longer a
   `namespace package <https://packaging.python.org/guides/packaging-namespace-packages/>`_.
 - ``datarobot.enums.BLENDER_METHOD.FORECAST_DISTANCE`` is removed (deprecated in 2.18.0).
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Updated :ref:`Residuals charts <residuals_chart>` documentation to reflect that the data rows include row numbers from the source dataset for projects
   created in DataRobot 5.3 and newer.
 
 2.18.0
 ======
 
-New Features
+New features
 ************
 - :ref:`Residuals charts <residuals_chart>` can now be retrieved for non-time-aware regression models.
 
 - :ref:`Deployment monitoring <deployment_monitoring>` can now be used to retrieve service stats, service health, accuracy info, permissions, and feature lists for deployments.
 
 - :ref:`Time series <time_series>` projects now support the Average by Forecast Distance blender, configured with more than one Forecast Distance. The blender blends the selected models, selecting the best three models based on the backtesting score for each Forecast Distance and averaging their predictions. The new blender method ``FORECAST_DISTANCE_AVG`` has been added to ``datarobot.enums.BLENDER_METHOD``.
 
@@ -1978,31 +2188,31 @@
 
 - Calls to :py:meth:`Project.start <datarobot.models.Project.start>` and :py:meth:`Project.upload_dataset <datarobot.models.Project.upload_dataset>` now support uploading data via S3 URI and `pathlib.Path` objects.
 
 - Errors upon connecting to DataRobot are now clearer when an incorrect API Token is used.
 
 - The datarobot package is now a `namespace package <https://packaging.python.org/guides/packaging-namespace-packages/>`_.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``datarobot.enums.BLENDER_METHOD.FORECAST_DISTANCE`` is deprecated and will be removed in 2.19. Use ``FORECAST_DISTANCE_ENET`` instead.
 
-Documentation Changes
+Documentation changes
 *********************
 - Various typo and wording issues have been addressed.
 
 - A new notebook showing regression-specific features is now been added to the :ref:`examples<examples_index>`.
 
 - Documentation for :ref:`Access lists <sharing>` has been added.
 
 2.17.0
 ======
 
-New Features
+New features
 ************
 - :ref:`Deployments <deployments_overview>` can now be managed via the API by using the new :py:class:`Deployment <datarobot.models.Deployment>` class.
 
 - Users can now list available prediction servers using :meth:`PredictionServer.list <datarobot.PredictionServer.list>`.
 
 - When :class:`specifying datetime partitioning <datarobot.DatetimePartitioningSpecification>` settings , :ref:`time series <time_series>` projects can now mark individual features as excluded from feature derivation using the
   :py:class:`FeatureSettings.do_not_derive <datarobot.FeatureSettings>` attribute. Any features not specified will be assigned according to the :py:class:`DatetimePartitioningSpecification.default_to_do_not_derive <datarobot.DatetimePartitioning>` value.
@@ -2029,23 +2239,23 @@
 
 Bugfixes
 ********
 - An issue affecting time series project creation for irregularly spaced dates has been fixed.
 - :class:`ComplianceDocTemplate <datarobot.models.compliance_doc_template.ComplianceDocTemplate>` now supports empty text blocks in user sections.
 - An issue when using :meth:`Predictions.get <datarobot.models.Predictions.get>` to retrieve predictions metadata has been fixed.
 
-Documentation Changes
+Documentation changes
 *********************
 - An overview on working with class ``ComplianceDocumentation`` and :class:`ComplianceDocTemplate <datarobot.models.compliance_doc_template.ComplianceDocTemplate>` has been created. :ref:`See here <automated_documentation_overview>` for more details.
 
 
 2.16.0
 ======
 
-New Features
+New features
 ************
 - Three new methods for Series Accuracy have been added to the :class:`DatetimeModel <datarobot.models.DatetimeModel>` class.
 
     - Start a request to calculate Series Accuracy with
       :meth:`DatetimeModel.compute_series_accuracy <datarobot.models.DatetimeModel.compute_series_accuracy>`
     - Once computed, Series Accuracy can be retrieved as a pandas.DataFrame using
       :meth:`DatetimeModel.get_series_accuracy_as_dataframe <datarobot.models.DatetimeModel.get_series_accuracy_as_dataframe>`
@@ -2069,15 +2279,15 @@
     - ``effective_feature_derivation_window_end``
     - ``forecast_window_start``
     - ``forecast_window_end``
     - ``windows_basis_unit``
 
 - Prediction metadata is now included in the return of :meth:`Predictions.get <datarobot.models.Predictions.get>`
 
-Documentation Changes
+Documentation changes
 *********************
 - Various typo and wording issues have been addressed.
 - The example data that was meant to accompany the Time Series examples has been added to the
   zip file of the download in the :ref:`examples<examples_index>`.
 
 2.15.1
 ======
@@ -2092,15 +2302,15 @@
 - Previously, attempting to retrieve the ``calendar_id`` of a project without a set target would result in an error.
   This has been fixed to return ``None`` instead.
 
 
 2.15.0
 ======
 
-New Features
+New features
 ************
 - Previously available for only Eureqa models, Advanced Tuning methods and objects, including
   :meth:`Model.start_advanced_tuning_session <datarobot.models.Model.start_advanced_tuning_session>`,
   :meth:`Model.get_advanced_tuning_parameters <datarobot.models.Model.get_advanced_tuning_parameters>`,
   :meth:`Model.advanced_tune <datarobot.models.Model.advanced_tune>`, and
   :class:`AdvancedTuningSession <datarobot.models.advanced_tuning.AdvancedTuningSession>`,
   now support all models other than blender, open source, and user-created models.  Use of
@@ -2123,60 +2333,57 @@
 * Information retrieval for :py:class:`ROC Curve <datarobot.models.roc_curve.RocCurve>` has been extended to include ``fraction_predicted_as_positive``, ``fraction_predicted_as_negative``, ``lift_positive`` and ``lift_negative``
 
 Bugfixes
 ********
 * Fixes an issue where the client would not be usable if it could not be sure it was compatible with the configured
   server
 
-API Changes
+API changes
 ***********
 - Methods for creating :py:class:`datarobot.models.Project`: `create_from_mysql`, `create_from_oracle`, and `create_from_postgresql`, deprecated in 2.11, have now been removed.
   Use :py:meth:`datarobot.models.Project.create_from_data_source` instead.
 - :py:class:`datarobot.FeatureSettings <datarobot.FeatureSettings>` attribute `apriori`, deprecated in 2.11, has been removed.
   Use :py:class:`datarobot.FeatureSettings.known_in_advance <datarobot.FeatureSettings>` instead.
 - :py:class:`datarobot.DatetimePartitioning <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, deprecated in 2.11, has been removed. Use
   :py:class:`datarobot.DatetimePartitioning.known_in_advance <datarobot.DatetimePartitioning>` instead.
 - :py:class:`datarobot.DatetimePartitioningSpecification <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, deprecated in 2.11, has been removed.
   Use :py:class:`datarobot.DatetimePartitioningSpecification.known_in_advance <datarobot.DatetimePartitioning>`
   instead.
 
-Deprecation Summary
-*******************
-
-Configuration Changes
+Configuration changes
 *********************
 - Now requires dependency on package `requests <https://pypi.org/project/requests/>`_  to be at least version 2.21.
 - Now requires dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be at least version 1.24.
 
-Documentation Changes
+Documentation changes
 *********************
 - Advanced model insights notebook extended to contain information on visualization of cumulative gains and lift charts.
 
 2.14.2
 ======
 
 Bugfixes
 ********
 - Fixed an issue where searches of the HTML documentation would sometimes hang indefinitely
 
-Documentation Changes
+Documentation changes
 *********************
 - Python3 is now the primary interpreter used to build the docs (this does not affect the ability to use the
   package with Python2)
 
 2.14.1
 ======
 
-Documentation Changes
+Documentation changes
 *********************
  - Documentation for the Model Deployment interface has been removed after the corresponding interface was removed in 2.13.0.
 
 2.14.0
 ======
-New Features
+New features
 ************
 - The new method :meth:`Model.get_supported_capabilities <datarobot.models.Model.get_supported_capabilities>`
   retrieves a summary of the capabilities supported by a particular model,
   such as whether it is eligible for Prime and whether it has word cloud data available.
 - New class for working with model compliance documentation feature of DataRobot:
   class ``ComplianceDocumentation``
 - New class for working with compliance documentation templates:
@@ -2216,32 +2423,32 @@
 - Timeseries projects can now accept feature derivation intervals, forecast windows, forecast points and prediction start/end dates in milliseconds.
 - :class:`DataSources <datarobot.DataSource>` and :class:`DataStores <datarobot.DataStore>` can now
   be :ref:`shared <sharing>` with other users.
 - Training predictions for datetime partitioned projects now support the new data subset
   `dr.enums.DATA_SUBSET.ALL_BACKTESTS` for requesting the predictions for all backtest validation
   folds.
 
-API Changes
-*******************
+API changes
+***********
 - The model recommendation type "Recommended" (deprecated in version 2.13.0) has been removed.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Example notebooks have been updated:
     - Notebooks now work in Python 2 and Python 3
     - A notebook illustrating time series capability has been added
     - The financial data example has been replaced with an updated introductory example.
 - To supplement the embedded Python notebooks in both the PDF and HTML docs bundles, the notebook files and supporting data can now be downloaded from the HTML docs bundle.
 - Fixed a minor typo in the code sample for ``get_or_request_feature_impact``
 
 2.13.0
 ======
 
-New Features
+New features
 ************
 - The new method :meth:`Model.get_or_request_feature_impact <datarobot.models.Model.get_or_request_feature_impact>` functionality will attempt to request feature impact
   and return the newly created feature impact object or the existing object so two calls are no longer required.
 - New methods and objects, including
   :meth:`Model.start_advanced_tuning_session <datarobot.models.Model.start_advanced_tuning_session>`,
   :meth:`Model.get_advanced_tuning_parameters <datarobot.models.Model.get_advanced_tuning_parameters>`,
   :meth:`Model.advanced_tune <datarobot.models.Model.advanced_tune>`, and
@@ -2284,52 +2491,52 @@
 
 Bugfixes
 ********
 - The Model Deployment interface which was previously visible in the client has been removed to
   allow the interface to mature, although the raw API is available as a "beta" API without full
   backwards compatibility support.
 
-API Changes
+API changes
 ***********
 - Added support for retrieving the Pareto Front of a Eureqa model. See
   :py:class:`ParetoFront <datarobot.models.pareto_front.ParetoFront>`.
 - A new recommendation type "Recommended for Deployment" has been added to
   :py:class:`ModelRecommendation <datarobot.models.ModelRecommendation>` which is now returns as the
   default recommended model when available. See :ref:`model_recommendation`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - The feature previously referred to as "Reason Codes" has been renamed to "Prediction
   Explanations", to provide increased clarity and accessibility. The old
   ReasonCodes interface has been deprecated and replaced with
   :py:class:`PredictionExplanations <datarobot.PredictionExplanations>`.
 - The recommendation type "Recommended" is deprecated and  will no longer be returned
   in v2.14 of the API.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Added a new documentation section :ref:`model_recommendation`.
 - Time series projects support multiseries as well as single series data. They are now documented in
   the :ref:`Time Series Projects <time_series>` documentation.
 
 2.12.0
 ======
 
-New Features
+New features
 ************
 - Some models now have Missing Value reports allowing users with access to uncensored blueprints to
   retrieve a detailed breakdown of how numeric imputation and categorical converter tasks handled
   missing values. See the :ref:`documentation <missing_values_report>` for more information on the
   report.
 
 2.11.0
 ======
 
-New Features
+New features
 ************
 - The new ``ModelRecommendation`` class can be used to retrieve the recommended models for a
   project.
 - A new helper method cross_validate was added to class Model. This method can be used to request
   Model's Cross Validation score.
 - Training a model with monotonic constraints is now supported. Training with monotonic
   constraints allows users to force models to learn monotonic relationships with respect to some features and the target. This helps users create accurate models that comply with regulations (e.g. insurance, banking). Currently, only certain blueprints (e.g. xgboost) support this feature, and it is only supported for regression and binary classification projects.
@@ -2339,51 +2546,51 @@
   a list of databases with tested support for DataRobot is available in the user guide
   in the web application. See :ref:`Database Connectivity <database_connectivity_overview>`
   for details.
 - Added a new feature to retrieve feature logs for time series projects. Check
   :py:meth:`datarobot.DatetimePartitioning.feature_log_list` and
   :py:meth:`datarobot.DatetimePartitioning.feature_log_retrieve` for details.
 
-API Changes
+API changes
 ***********
 - New attributes supporting monotonic constraints have been added to the
   :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>`,
   :py:class:`Project <datarobot.models.Project>`,
   :py:class:`Model <datarobot.models.Model>`, and :py:class:`Blueprint <datarobot.models.Blueprint>`
   classes. See :ref:`monotonic constraints<monotonic_constraints>` for more information on how to
   configure monotonic constraints.
 - New parameters `predictions_start_date` and `predictions_end_date` added to
   :py:meth:`Project.upload_dataset <datarobot.models.Project.upload_dataset>` to support bulk
   predictions upload for time series projects.
 
-Deprecation Summary
+Deprecation summary
 *******************
 - Methods for creating :py:class:`datarobot.models.Project`: `create_from_mysql`, `create_from_oracle`, and `create_from_postgresql`, have been deprecated and will be removed in 2.14.
   Use :py:meth:`datarobot.models.Project.create_from_data_source` instead.
 - :py:class:`datarobot.FeatureSettings <datarobot.FeatureSettings>` attribute `apriori`, has been deprecated and will be removed in 2.14.
   Use :py:class:`datarobot.FeatureSettings.known_in_advance <datarobot.FeatureSettings>` instead.
 - :py:class:`datarobot.DatetimePartitioning <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, has been deprecated and will be removed in 2.14.
   :py:class:`datarobot.DatetimePartitioning.known_in_advance <datarobot.DatetimePartitioning>` instead.
 - :py:class:`datarobot.DatetimePartitioningSpecification <datarobot.DatetimePartitioning>` attribute `default_to_a_priori`, has been deprecated and will be removed in 2.14.
   Use :py:class:`datarobot.DatetimePartitioningSpecification.known_in_advance <datarobot.DatetimePartitioning>`
   instead.
 
-Configuration Changes
+Configuration changes
 *********************
 - Retry settings compatible with those offered by urllib3's `Retry <https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#urllib3.util.retry.Retry>`_
   interface can now be configured. By default, we will now retry connection errors that prevented requests from arriving at the server.
 
-Documentation Changes
+Documentation changes
 *********************
 - "Advanced Model Insights" example has been updated to properly handle bin weights when rebinning.
 
 2.9.0
 =====
 
-New Features
+New features
 ************
 - New ``ModelDeployment`` class can be used to track status and health of models deployed for
   predictions.
 
 Enhancements
 ************
 - DataRobot API now supports creating 3 new blender types - Random Forest, TensorFlow, LightGBM.
@@ -2408,15 +2615,15 @@
   :py:class:`datarobot.DatetimePartitioningSpecification` class to fine-tune how time-series projects
   derive modeling features. `treat_as_exponential` can control whether data is analyzed as
   an exponential trend and transformations like log-transform are applied.
   `differencing_method` can control which differencing method to use for stationary data.
   `periodicities` can be used to specify periodicities occurring within the data.
   All are optional and defaults will be chosen automatically if they are unspecified.
 
-API Changes
+API changes
 ***********
 - Now ``training_row_count`` is available on non-datetime models as well as "rowCount" based
   datetime models. It reports the number of rows used to train the model (equivalent to
   ``sample_pct``).
 - Features retrieved from ``Feature.get`` now include ``target_leakage``.
 
 2.8.1
@@ -2431,15 +2638,15 @@
 - Version of ``trafaret`` library this package depends on is now pinned to ``trafaret>=0.7,<1.1``
   since versions outside that range are known to be incompatible.
 
 
 2.8.0
 =====
 
-New Features
+New features
 ************
 - The DataRobot API supports the creation, training, and predicting of multiclass classification
   projects. DataRobot, by default, handles a dataset with a numeric target column as regression.
   If your data has a numeric cardinality of fewer than 11 classes, you can override this behavior to
   instead create a multiclass classification project from the data. To do so, use the set_target
   function, setting target_type='Multiclass'. If DataRobot recognizes your data as categorical, and
   it has fewer than 11 classes, using multiclass will create a project that classifies which label
@@ -2483,39 +2690,39 @@
   parameter 'events_count' as a part of the AdvancedOptions object to allow specifying the
   events count column. See the user guide documentation in the webapp for more information
   on events count.
 - PredictJob.get_predictions now returns predicted probability for each class in the dataframe.
 - PredictJob.get_predictions now accepts prefix parameter to prefix the classes name returned in the
   predictions dataframe.
 
-API Changes
+API changes
 ***********
 - Add `target_type` parameter to set_target() and start(), used to override the project default.
 
 2.7.2
 =====
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Updated link to the publicly hosted documentation.
 
 2.7.1
 =====
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Online documentation hosting has migrated from PythonHosted to Read The Docs. Minor code changes
   have been made to support this.
 
 2.7.0
 =====
 
-New Features
+New features
 ************
 - Lift chart data for models can be retrieved using the `Model.get_lift_chart` and
   `Model.get_all_lift_charts` methods.
 - ROC curve data for models in classification projects can be retrieved using the
   `Model.get_roc_curve` and `Model.get_all_roc_curves` methods.
 - Semi-automatic autopilot mode is removed.
 - Word cloud data for text processing models can be retrieved using `Model.get_word_cloud` method.
@@ -2529,38 +2736,38 @@
   showing the coefficients for individual stages of multistage models (e.g. Frequency-Severity
   models).
 - When training a `DatetimeModel` on a window of data, a `time_window_sample_pct` can be specified
   to take a uniform random sample of the training data instead of using all data within the window.
 - Installing of DataRobot package now has an "Extra Requirements" section that will install all of
   the dependencies needed to run the example notebooks.
 
-Documentation Changes
+Documentation changes
 *********************
 - A new example notebook describing how to visualize some of the newly available model insights
   including lift charts, ROC curves, and word clouds has been added to the examples section.
 - A new section for `Common Issues` has been added to `Getting Started` to help debug issues related to client installation and usage.
 
 
 2.6.1
 =====
 
 Bugfixes
 ********
 
 - Fixed a bug with `Model.get_parameters` raising an exception on some valid parameter values.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - Fixed sorting order in Feature Impact example code snippet.
 
 2.6.0
 =====
 
-New Features
+New features
 ************
 - A new partitioning method (datetime partitioning) has been added. The recommended workflow is to
   preview the partitioning by creating a `DatetimePartitioningSpecification` and passing it into
   `DatetimePartitioning.generate`, inspect the results and adjust as needed for the specific project
   dataset by adjusting the `DatetimePartitioningSpecification` and re-generating, and then set the
   target by passing the final `DatetimePartitioningSpecification` object to the partitioning_method
   parameter of `Project.set_target`.
@@ -2607,24 +2814,24 @@
 ********
 
 - Fixed a bug (affecting Python 2 only) with printing any model (including frozen and prime models)
   whose model_type is not ascii.
 - FrozenModels were unable to correctly use methods inherited from Model. This has been fixed.
 - When calling `get_result` for a Job, ModelJob, or PredictJob that has errored, `AsyncProcessUnsuccessfulError` will now be raised instead of `JobNotFinished`, consistently with the behavior of `get_result_when_complete`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - Support for the experimental Recommender Problems projects has been removed. Any code relying on
   `RecommenderSettings` or the `recommender_settings` argument of `Project.set_target` and
   `Project.start` will error.
 - ``Project.update``, deprecated in v2.2.32, has been removed in favor of specific updates:
   ``rename``, ``unlock_holdout``, ``set_worker_count``.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - The link to Configuration from the Quickstart page has been fixed.
 
 2.5.1
 =====
 
@@ -2636,15 +2843,15 @@
 - Fixed an issue where the weights column (for weighted projects) did not appear
   in the `advanced_options` of a `Project`.
 
 
 2.5.0
 =====
 
-New Features
+New features
 ************
 
 - Methods to work with blender models have been added. Use `Project.blend` method to create new blenders,
   `Project.get_blenders` to get the list of existing blenders and `BlenderModel.get` to retrieve a model
   with blender-specific information.
 - Projects created via the API can now use smart downsampling when setting the target by passing
   `smart_downsampled` and `majority_downsampling_rate` into the `AdvancedOptions` object used with
@@ -2663,15 +2870,15 @@
 - When specifying the API endpoint in the configuration, the client will now behave correctly for
   endpoints with and without trailing slashes.
 
 
 2.4.0
 =====
 
-New Features
+New features
 ************
 
 - The premium add-on product `DataRobot Prime` has been added. You can now approximate a model
   on the leaderboard and download executable code for it. See documentation for further details, or
   talk to your account representative if the feature is not available on your account.
 - (Only relevant for on-premise users with a Standalone Scoring cluster.) Methods
   (`request_transferable_export` and `download_export`) have been added to the `Model` class for exporting models (which will only work if model export is turned on). There is a new class `ImportedModel` for managing imported models on a Standalone
@@ -2692,50 +2899,50 @@
 
 Bugfixes
 ********
 
 - Fixed an issue where `Model.request_predictions` might raise an error when predictions finished
   very quickly instead of returning the job.
 
-API Changes
+API changes
 ***********
 
 - To set the target with quickrun autopilot, call `Project.set_target` with `mode=AUTOPILOT_MODE.QUICK` instead of
   specifying `quickrun=True`.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - Semi-automatic mode for autopilot has been deprecated and will be removed in 3.0.
   Use manual or fully automatic instead.
 - Use of the `quickrun` argument in `Project.set_target` has been deprecated and will be removed in
   3.0. Use `mode=AUTOPILOT_MODE.QUICK` instead.
 
-Configuration Changes
+Configuration changes
 *********************
 
 - It is now possible to control the SSL certificate verification by setting the parameter
   `ssl_verify` in the config file.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - The "Modeling Airline Delay" example notebook has been updated to work with the new 2.3
   enhancements.
 - Documentation for the generic `Job` class has been added.
 - Class attributes are now documented in the `API Reference` section of the documentation.
 - The changelog now appears in the documentation.
 - There is a new section dedicated to configuration, which lists all of the configuration
   options and their meanings.
 
 
 2.3.0
 =====
 
-New Features
+New features
 ************
 
 - The DataRobot API now includes Feature Impact, an approach to measuring the relevance of each feature
   that can be applied to any model. The `Model` class now includes methods `request_feature_impact`
   (which creates and returns a feature impact job) and `get_feature_impact` (which can retrieve completed feature impact results).
 - A new improved workflow for predictions now supports first uploading a dataset via `Project.upload_dataset`,
   then requesting predictions via `Model.request_predictions`. This allows us to better support predictions on
@@ -2788,27 +2995,27 @@
 
 Bugfixes
 ********
 
 - Fixed a bug (affecting Python 2 only) with printing features and featurelists whose names are
   not ascii.
 
-API Changes
+API changes
 ***********
 
 - Job class hierarchy is rearranged to better express the relationship between these objects. See
   documentation for `datarobot.models.job` for details.
 - `Featurelist` objects now have a `project_id` attribute to indicate which project they belong
   to. Directly accessing the `project` attribute of a `Featurelist` object is now deprecated
 - Support INI-style configuration, which was deprecated in v2.1, has been removed. yaml is the only supported
   configuration format.
 - The method `Project.get_jobs` method, which was deprecated in v2.1, has been removed. Users should use
   the `Project.get_model_jobs` method instead to get the list of model jobs.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - `PredictJob.create` has been deprecated in favor of the alternate workflow using `Model.request_predictions`.
 - Feature.converter (used internally for object construction) has been made private.
 - Model.fetch_resource_data has been deprecated and will be removed in 3.0. To fetch a model from
    its ID, use Model.get.
 - The ability to use Feature.get with feature IDs (rather than names) is deprecated and will
@@ -2820,15 +3027,15 @@
   attribute of a `Featurelist` to instantiate a `Project` instance using `Project.get`.
 - Use of the attributes `Model.project`, `Model.blueprint`, and `Model.featurelist` are all deprecated now
   to avoid use of partially instantiated objects. Please use the ids of these objects instead.
 - Using a `Project` instance as an argument in `Featurelist.get` is now deprecated.
   Please use a project_id instead. Similarly, using a `Project` instance in `Model.get` is also deprecated,
   and a project_id should be used in its place.
 
-Configuration Changes
+Configuration changes
 *********************
 
 - Previously it was possible (though unintended) that the client configuration could be mixed through
   environment variables, configuration files, and arguments to `datarobot.Client`. This logic is now
   simpler - please see the `Getting Started` section of the documentation for more information.
 
 
@@ -2848,15 +3055,15 @@
 - Fixed a bug (affecting Python 2 only) with printing projects, features, and featurelists whose names are
   not ascii.
 
 
 2.2.32
 ======
 
-New Features
+New features
 ************
 
 - ``Project.get_features`` and ``Feature.get`` methods have been added for feature retrieval.
 - A generic ``Job`` entity has been added for use in retrieving the entire queue at once. Calling
   ``Project.get_all_jobs`` will retrieve all (appropriately filtered) jobs from the queue. Those
   can be cancelled directly as generic jobs, or transformed into instances of the specific
   job class using ``ModelJob.from_job`` and ``PredictJob.from_job``, which allow all functionality
@@ -2881,15 +3088,15 @@
 ********
 
 - Fixed an issue where updating the global client would not affect existing objects with cached clients.
   Now the global client is used for every API call.
 - An issue where mistyping a filepath for use in a file upload has been resolved. Now an error will be
   raised if it looks like the raw string content for modeling or predictions is just one single line.
 
-API Changes
+API changes
 ***********
 
 - Use of username and password to authenticate is no longer supported - use an API token instead.
 - Usage of ``start_time`` and ``finish_time`` parameters in ``Project.get_models`` is not
   supported both in filtering and ordering of models
 - Default value of ``sample_pct`` parameter of ``Model.train`` method is now ``None`` instead of ``100``.
   If the default value is used, models will be trained with all of the available *training* data based on
@@ -2899,21 +3106,21 @@
 - ``recommendation_settings`` parameter of ``Project.start`` which was deprecated in v0.2 has been removed.
 - ``Project.status`` method which was deprecated in v0.2 has been removed.
 - ``Project.wait_for_aim_stage`` method which was deprecated in v0.2 has been removed.
 - ``Delay``, ``ConstantDelay``, ``NoDelay``, ``ExponentialBackoffDelay``, ``RetryManager``
   classes from ``retry`` module which were deprecated in v2.1 were removed.
 - Package renamed to ``datarobot``.
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``Project.update`` deprecated in favor of specific updates:
   ``rename``, ``unlock_holdout``, ``set_worker_count``.
 
-Documentation Changes
+Documentation changes
 *********************
 
 - A new use case involving financial data has been added to the ``examples`` directory.
 - Added documentation for the partition methods.
 
 2.1.31
 ======
@@ -2943,15 +3150,15 @@
 
 - Minimal used version of ``requests_toolbelt`` package changed from 0.4 to 0.6
 
 
 2.1.28
 ======
 
-New Features
+New features
 ************
 
 - Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
 - Allow `config_path` argument to client
 - ``wait_for_autopilot`` method added to Project. This method can be used to
   block execution until autopilot has finished running on the project.
 - Support for specifying which featurelist to use with initial autopilot in
@@ -2970,26 +3177,26 @@
   and decide if they would like to resume waiting for async process to resolve
 
 Enhancements
 ************
 
 - ``AUTOPILOT_MODE`` enum now uses string names for autopilot modes instead of numbers
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``ConstantDelay``, ``NoDelay``, ``ExponentialBackoffDelay``, and ``RetryManager`` utils are now deprecated
 - INI-style config files are now deprecated (in favor of YAML config files)
 - Several functions in the `utils` submodule are now deprecated (they are
   being moved elsewhere and are not considered part of the public interface)
 - ``Project.get_jobs`` has been renamed ``Project.get_model_jobs`` for clarity and deprecated
 - Support for the experimental date partitioning has been removed in DataRobot API,
   so it is being removed from the client immediately.
 
-API Changes
+API changes
 ***********
 
 - In several places where ``AppPlatformError`` was being raised, now ``TypeError``, ``ValueError`` or
   ``InputNotUnderstoodError`` are now used. With this change, one can now safely assume that when
   catching an ``AppPlatformError`` it is because of an unexpected response from the server.
 - ``AppPlatformError`` has gained a two new attributes, ``status_code`` which is the HTTP status code
   of the unexpected response from the server, and ``error_code`` which is a DataRobot-defined error
@@ -3004,21 +3211,21 @@
   have the status_code of the unexpected response from the server, and the location that was being
   polled to wait for the asynchronous process to resolve.
 
 
 2.0.27
 ======
 
-New Features
+New features
 ************
 
 - ``PredictJob`` class was added to work with prediction jobs
 - ``wait_for_async_predictions`` function added to `predict_job` module
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - The `order_by` parameter of the ``Project.list`` is now deprecated.
 
 
 0.2.26
 ======
@@ -3030,15 +3237,15 @@
   keeping the client side in sync with the state of the project on the
   server
 - ``Project.create_featurelist`` now throws ``DuplicateFeaturesError``
   exception if passed list of features contains duplicates
 - ``Project.get_models`` now supports snake_case arguments to its
   order_by keyword
 
-Deprecation Summary
+Deprecation summary
 *******************
 
 - ``Project.wait_for_aim_stage`` is now deprecated, as the REST Async
   flow is a more reliable method of determining that project creation has
   completed successfully
 - ``Project.status`` is deprecated in favor of ``Project.get_status``
 - ``recommendation_settings`` parameter of ``Project.start`` is
```

### Comparing `datarobot-3.3.2/LICENSE.txt` & `datarobot-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/README.md` & `datarobot-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/common_setup.py` & `datarobot-3.4.0/common_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,27 +125,30 @@
 )
 
 tests_require = [
     "mock==3.0.5",
     "pytest==7.1.2",
     "pytest-cov",
     "responses==0.21",
-    "pytest-asyncio",
+    "pytest-asyncio==0.21.1",
+    "pyarrow",
 ] + images_require
 
 dev_require = (
     tests_require
     + lint_require
     + images_require
     + [
         "sphinx_rtd_theme==1.0.0",
         "nbsphinx==0.8.9",
         "numpydoc==1.4.0",
         "jupyter_contrib_nbextensions",
         "sphinx-autodoc-typehints==1.17.1",
+        "sphinxcontrib-spelling==8.0.0",
+        "pyenchant==3.2.2",
     ]
 )
 
 example_require = [
     "jupyter<=5.0",
     "fredapi==0.4.0",
     "matplotlib>=2.1.0",
```

### Comparing `datarobot-3.3.2/datarobot/__init__.py` & `datarobot-3.4.0/datarobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # flake8: noqa
 from ._version import __version__
 from .client import Client
 from .context import Context
 from .enums import (
     AUTOPILOT_MODE,
+    KeyValueCategory,
+    KeyValueEntityType,
+    KeyValueType,
     NETWORK_EGRESS_POLICY,
     PredictionEnvironmentPlatform,
     QUEUE_STATUS,
     SCORING_TYPE,
     SNAPSHOT_POLICY,
     TARGET_TYPE,
     VERBOSITY_LEVEL,
@@ -66,17 +69,19 @@
     FeatureAssociationMatrix,
     FeatureAssociationMatrixDetails,
     FeatureHistogram,
     FeatureImpactJob,
     FeatureLineage,
     Featurelist,
     FrozenModel,
+    genai,
     ImportedModel,
     InteractionFeature,
     Job,
+    KeyValue,
     Model,
     ModelBlueprintChart,
     ModelingFeature,
     ModelingFeaturelist,
     ModelJob,
     ModelRecommendation,
     PayoffMatrix,
@@ -90,14 +95,15 @@
     PrimeFile,
     PrimeModel,
     Project,
     RatingTable,
     RatingTableModel,
     RegisteredModel,
     RegisteredModelVersion,
+    registry,
     RelationshipsConfiguration,
     Ruleset,
     SecondaryDatasetConfigurations,
     SegmentationTask,
     SegmentInfo,
     ShapImpact,
     ShapMatrix,
```

### Comparing `datarobot-3.3.2/datarobot/_compat.py` & `datarobot-3.4.0/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/analytics.py` & `datarobot-3.4.0/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/context.py` & `datarobot-3.4.0/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/enums.py` & `datarobot-3.4.0/datarobot/enums.py`

 * *Files 21% similar despite different names*

```diff
@@ -132,15 +132,16 @@
 class TARGET_TYPE:
     BINARY = "Binary"
     MULTICLASS = "Multiclass"
     MULTILABEL = "Multilabel"
     REGRESSION = "Regression"
     UNSTRUCTURED = "Unstructured"
     ANOMALY = "Anomaly"
-    ALL = [BINARY, MULTICLASS, MULTILABEL, REGRESSION, UNSTRUCTURED, ANOMALY]
+    TEXT_GENERATION = "TextGeneration"
+    ALL = [BINARY, MULTICLASS, MULTILABEL, REGRESSION, UNSTRUCTURED, ANOMALY, TEXT_GENERATION]
 
 
 JOB_TYPE = enum(
     BATCH_MONITORING="batchMonitoring",
     BATCH_PREDICTIONS="batchPredictions",
     BATCH_PREDICTION_JOB_DEFINITIONS="batchPredictionJobDefinitions",
     FEATURE_IMPACT="featureImpact",
@@ -544,22 +545,23 @@
 class _SHARED_TARGET_TYPE:
     """Enum of all target types shared by tasks and models"""
 
     BINARY = "Binary"
     ANOMALY = "Anomaly"
     REGRESSION = "Regression"
     MULTICLASS = "Multiclass"
-    ALL = [BINARY, ANOMALY, REGRESSION, MULTICLASS]
+    TEXT_GENERATION = "TextGeneration"
+    ALL = [BINARY, ANOMALY, REGRESSION, MULTICLASS, TEXT_GENERATION]
 
 
 class CUSTOM_MODEL_TARGET_TYPE(_SHARED_TARGET_TYPE):
     """Enum of valid custom model target types"""
 
     UNSTRUCTURED = "Unstructured"
-    REQUIRES_TARGET_NAME = ("Binary", "Multiclass", "Regression")
+    REQUIRES_TARGET_NAME = ("Binary", "Multiclass", "Regression", "TextGeneration")
 
     ALL = _SHARED_TARGET_TYPE.ALL + [UNSTRUCTURED]
 
 
 class CUSTOM_TASK_TARGET_TYPE(_SHARED_TARGET_TYPE):
     """Enum of valid custom task target types"""
 
@@ -710,15 +712,15 @@
     BOX = 4
     HAMMING = 5
 
 
 # Defaults used for image transformations preprocessing
 # Image resize defaults
 DEFAULT_VISUAL_AI_SHOULD_RESIZE = True
-DEFAULT_VISUAL_AI_FORCE_SIZE = False
+DEFAULT_VISUAL_AI_FORCE_SIZE = True
 DEFAULT_VISUAL_AI_IMAGE_SIZE = (224, 224)
 # Image format defaults
 DEFAULT_VISUAL_AI_IMAGE_FORMAT = None  # preserve original image format
 DEFAULT_VISUAL_AI_IMAGE_SUBSAMPLING = None  # uses Pillow library default
 DEFAULT_VISUAL_AI_IMAGE_QUALITY_KEEP_IF_POSSIBLE = True
 DEFAULT_VISUAL_AI_IMAGE_QUALITY = 75
 DEFAULT_VISUAL_AI_IMAGE_RESAMPLE_METHOD = ImageResampleMethod.LANCZOS
@@ -765,14 +767,18 @@
     BIAS_MITIGATION_TECHNIQUE = "bias_mitigation_technique"
     INCLUDE_BIAS_MITIGATION_FEATURE_AS_PREDICTOR_VARIABLE = (
         "include_bias_mitigation_feature_as_predictor_variable"
     )
     MODEL_GROUP_ID = "model_group_id"
     MODEL_REGIME_ID = "model_regime_id"
     MODEL_BASELINES = "model_baselines"
+    INCREMENTAL_LEARNING_ONLY_MODE = "incremental_learning_only_mode"
+    INCREMENTAL_LEARNING_ON_BEST_MODEL = "incremental_learning_on_best_model"
+    CHUNK_DEFINITION_ID = "chunk_definition_id"
+    INCREMENTAL_LEARNING_EARLY_STOPPING_ROUNDS = "incremental_learning_early_stopping_rounds"
     ALL = set(
         [
             WEIGHTS,
             RESPONSE_CAP,
             SEED,
             MAJORITY_DOWNSAMPLING_RATE,
             OFFSET,
@@ -797,14 +803,18 @@
             FAIRNESS_THRESHOLD,
             BIAS_MITIGATION_FEATURE_NAME,
             BIAS_MITIGATION_TECHNIQUE,
             INCLUDE_BIAS_MITIGATION_FEATURE_AS_PREDICTOR_VARIABLE,
             MODEL_GROUP_ID,
             MODEL_REGIME_ID,
             MODEL_BASELINES,
+            INCREMENTAL_LEARNING_ONLY_MODE,
+            INCREMENTAL_LEARNING_ON_BEST_MODEL,
+            CHUNK_DEFINITION_ID,
+            INCREMENTAL_LEARNING_EARLY_STOPPING_ROUNDS,
         ]
     )
 
 
 class PersistableProjectOptions:
     """
     All of the available properties that can be saved in the DR backend from a ProjectOptions object.
@@ -955,14 +965,61 @@
     CAN_VIEW = "CAN_VIEW"
 
 
 class CredentialTypes(StrEnum):
     BASIC = "basic"
     OAUTH = "oauth"
     S3 = "s3"
+    AZURE = "azure"
+    GCP = "gcp"
+    SNOWFLAKE_KEY_PAIR_AUTH = "snowflake_key_pair_user_account"
+    DATABRICKS_ACCESS_TOKEN = "databricks_access_token_account"
+    DATABRICKS_SERVICE_PRINCIPAL = "databricks_service_principal_account"
+
+
+class DriverTypes(StrEnum):
+    JDBC = "jdbc"
+    DR_DATABASE_V1 = "dr-database-v1"
+    DR_CONNECTOR_V1 = "dr-connector-v1"
+    ALL = "all"
+    DATABASES = "databases"
+
+
+class ConnectorDriverTypes(StrEnum):
+    DR_CONNECTOR_V1 = DriverTypes.DR_CONNECTOR_V1
+
+
+class DataDriverTypes(StrEnum):
+    DR_DATABASE_V1 = DriverTypes.DR_DATABASE_V1
+    JDBC = DriverTypes.JDBC
+
+
+class DataDriverListTypes(StrEnum):
+    DR_DATABASE_V1 = DriverTypes.DR_DATABASE_V1
+    JDBC = DriverTypes.JDBC
+    ALL = DriverTypes.ALL
+
+
+class DataStoreTypes(StrEnum):
+    DR_DATABASE_V1 = DriverTypes.DR_DATABASE_V1
+    JDBC = DriverTypes.JDBC
+    DR_CONNECTOR_V1 = DriverTypes.DR_CONNECTOR_V1
+
+
+class DataStoreListTypes(StrEnum):
+    DR_DATABASE_V1 = DriverTypes.DR_DATABASE_V1
+    JDBC = DriverTypes.JDBC
+    DR_CONNECTOR_V1 = DriverTypes.DR_CONNECTOR_V1
+    ALL = DriverTypes.ALL
+    DATABASES = DriverTypes.DATABASES
+
+
+class DrDatabaseV1Types(StrEnum):
+    BIGQUERY = "bigquery-v1"
+    DATABRICKS = "databricks-v1"
 
 
 class TrainingDataSubsets(StrEnum, metaclass=DRStrEnum):
     """Subsets of training data that can be scored via Batch Predictions."""
 
     HOLDOUT = "holdout"
     VALIDATION = "validation"
@@ -1001,27 +1058,39 @@
     """
 
     AWS = "aws"
     GCP = "gcp"
     AZURE = "azure"
     ON_PREMISE = "onPremise"
     DATAROBOT = "datarobot"
+    DATAROBOT_SERVERLESS = "datarobotServerless"
     OPEN_SHIFT = "openShift"
     OTHER = "other"
     SNOWFLAKE = "snowflake"
 
-    ALL = [AWS, GCP, AZURE, ON_PREMISE, DATAROBOT, OPEN_SHIFT, OTHER, SNOWFLAKE]
+    ALL = [
+        AWS,
+        GCP,
+        AZURE,
+        ON_PREMISE,
+        DATAROBOT,
+        DATAROBOT_SERVERLESS,
+        OPEN_SHIFT,
+        OTHER,
+        SNOWFLAKE,
+    ]
     EXTERNALS = [AWS, GCP, AZURE, ON_PREMISE, OPEN_SHIFT, OTHER, SNOWFLAKE]
 
     HUMAN_STRING = {
         AWS: "Amazon Web Services (AWS)",
         GCP: "Google Cloud Platform (GCP)",
         AZURE: "Azure",
         ON_PREMISE: "On-premise",
         DATAROBOT: "DataRobot",
+        DATAROBOT_SERVERLESS: "DataRobot Serverless",
         OPEN_SHIFT: "OpenShift",
         OTHER: "Other",
         SNOWFLAKE: "Snowflake",
     }
 
 
 class PredictionEnvironmentModelFormats:
@@ -1044,16 +1113,17 @@
     """
 
     PASSING = "passing"
     WARNING = "warning"
     FAILING = "failing"
     UNKNOWN = "unknown"
     UNAVAILABLE = "unavailable"
+    NOT_APPLICABLE = "notApplicable"
 
-    ALL = [PASSING, WARNING, FAILING, UNKNOWN, UNAVAILABLE]
+    ALL = [PASSING, WARNING, FAILING, UNKNOWN, UNAVAILABLE, NOT_APPLICABLE]
 
 
 class DocumentTextExtractionMethod:
     OCR = "TESSERACT_OCR"
     EMBEDDED = "DOCUMENT_TEXT_EXTRACTOR"
 
     ALL = [OCR, EMBEDDED]
@@ -1096,7 +1166,320 @@
     ) -> Optional["CustomTaskOutgoingNetworkPolicy"]:
         if input_string is None:
             return None
         for el in cls:
             if el.name == input_string:
                 return el
         raise ValueError(f"{input_string!r} does not match any of {[el.name for el in cls]}")
+
+
+class CustomMetricDirectionality:
+    HIGHER_IS_BETTER = "higherIsBetter"
+    LOWER_IS_BETTER = "lowerIsBetter"
+    ALL = [HIGHER_IS_BETTER, LOWER_IS_BETTER]
+
+
+class CustomMetricAggregationType:
+    SUM = "sum"
+    AVERAGE = "average"
+    GAUGE = "gauge"
+    ALL = [SUM, AVERAGE, GAUGE]
+
+
+class CustomMetricBucketTimeStep:
+    HOUR = "hour"
+    ALL = [HOUR]
+
+
+class KeyValueEntityType(Enum):
+    """Key-Value entity type"""
+
+    DEPLOYMENT = "deployment"
+    MODEL_PACKAGE = "modelPackage"
+    REGISTERED_MODEL = "registeredModel"
+    CUSTOM_JOB = "customJob"
+    CUSTOM_JOB_RUN = "customJobRun"
+
+
+class KeyValueType(Enum):
+    """Key-Value type"""
+
+    BINARY = "binary"
+    BOOLEAN = "boolean"
+    CREDENTIAL = "credential"
+    DEPLOYMENT_ID = "deploymentId"
+    DATASET = "dataset"
+    IMAGE = "image"
+    JSON = "json"
+    MODEL_VERSION = "modelVersion"
+    NUMERIC = "numeric"
+    PICKLE = "pickle"
+    STRING = "string"
+    URL = "url"
+    YAML = "yaml"
+
+
+class KeyValueCategory(Enum):
+    """Key-Value category"""
+
+    TRAINING_PARAMETER = "trainingParameter"
+    METRIC = "metric"
+    TAG = "tag"
+    ARTIFACT = "artifact"
+    RUNTIME_PARAMETER = "runtimeParameter"
+
+
+class ExportStatus:
+    """A prediction data export processing state."""
+
+    CREATED = "CREATED"
+    SCHEDULED = "SCHEDULED"
+    CANCELLED = "CANCELLED"
+    FAILED = "FAILED"
+    SUCCEEDED = "SUCCEEDED"
+
+    ALL = [CREATED, SCHEDULED, CANCELLED, FAILED, SUCCEEDED]
+
+
+class ListVectorDatabasesSortQueryParams(StrEnum):
+    """supported Sort query params for the Vectordatabase.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_USER_DATE_ASCENDING = "creationUserId"
+    CREATION_USER_DATE_DESCENDING = "-creationUserId"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+    EMBEDDING_MODEL_ASCENDING = "embeddingModel"
+    EMBEDDING_MODEL_DESCENDING = "-embeddingModel"
+    DATASET_ID_ASCENDING = "datasetId"
+    DATASET_ID_DESCENDING = "-datasetId"
+    CHUNKING_METHOD_ASCENDING = "chunkingMethod"
+    CHUNKING_METHOD_DESCENDING = "-chunkingMethod"
+    CHUNKS_COUNT_ASCENDING = "chunksCount"
+    CHUNKS_COUNT_DESCENDING = "-chunksCount"
+    SIZE_ASCENDING = "size"
+    SIZE_DESCENDING = "-size"
+    USER_NAME_ASCENDING = "userName"
+    USER_NAME_DESCENDING = "-userName"
+    DATASET_NAME_ASCENDING = "datasetName"
+    DATASET_NAME_DESCENDING = "-datasetName"
+    PLAYGROUNDS_COUNT_ASCENDING = "playgroundsCount"
+    PLAYGROUNDS_COUNT_DESCENDING = "-playgroundsCount"
+    SOURCE_ASCENDING = "source"
+    SOURCE_DESCENDING = "-source"
+
+
+class VectorDatabaseEmbeddingModel(StrEnum):
+    """Text embedding model names for VectorDatabases."""
+
+    E5_LARGE_V2 = "intfloat/e5-large-v2"
+    E5_BASE_V2 = "intfloat/e5-base-v2"
+    MULTILINGUAL_E5_BASE = "intfloat/multilingual-e5-base"
+    ALL_MINILM_L6_V2 = "sentence-transformers/all-MiniLM-L6-v2"
+    JINA_EMBEDDING_T_EN_V1 = "jinaai/jina-embedding-t-en-v1"
+    SUP_SIMCSE_JA_BASE = "cl-nagoya/sup-simcse-ja-base"
+
+
+class VectorDatabaseChunkingMethod(StrEnum):
+    """Text chunking method names for VectorDatabases."""
+
+    RECURSIVE = "recursive"
+
+
+class VectorDatabaseDatasetLanguages(StrEnum):
+    """Dataset languages supported by VectorDatabases."""
+
+    AFRIKAANS = "Afrikaans"
+    AMHARIC = "Amharic"
+    ARABIC = "Arabic"
+    ASSAMESE = "Assamese"
+    AZERBAIJANI = "Azerbaijani"
+    BELARUSIAN = "Belarusian"
+    BULGARIAN = "Bulgarian"
+    BENGALI = "Bengali"
+    BRETON = "Breton"
+    BOSNIAN = "Bosnian"
+    CATALAN = "Catalan"
+    CZECH = "Czech"
+    WELSH = "Welsh"
+    DANISH = "Danish"
+    GERMAN = "German"
+    GREEK = "Greek"
+    ENGLISH = "English"
+    ESPERANTO = "Esperanto"
+    SPANISH = "Spanish"
+    ESTONIAN = "Estonian"
+    BASQUE = "Basque"
+    PERSIAN = "Persian"
+    FINNISH = "Finnish"
+    FRENCH = "French"
+    WESTERN_FRISIAN = "Western Frisian"
+    IRISH = "Irish"
+    SCOTTISH_GAELIC = "Scottish Gaelic"
+    GALICIAN = "Galician"
+    GUJARATI = "Gujarati"
+    HAUSA = "Hausa"
+    HEBREW = "Hebrew"
+    HINDI = "Hindi"
+    CROATIAN = "Croatian"
+    HUNGARIAN = "Hungarian"
+    ARMENIAN = "Armenian"
+    INDONESIAN = "Indonesian"
+    ICELANDIC = "Icelandic"
+    ITALIAN = "Italian"
+    JAPANESE = "Japanese"
+    JAVANESE = "Javanese"
+    GEORGIAN = "Georgian"
+    KAZAKH = "Kazakh"
+    KHMER = "Khmer"
+    KANNADA = "Kannada"
+    KOREAN = "Korean"
+    KURDISH = "Kurdish"
+    KYRGYZ = "Kyrgyz"
+    LATIN = "Latin"
+    LAO = "Lao"
+    LITHUANIAN = "Lithuanian"
+    LATVIAN = "Latvian"
+    MALAGASY = "Malagasy"
+    MACEDONIAN = "Macedonian"
+    MALAYALAM = "Malayalam"
+    MONGOLIAN = "Mongolian"
+    MARATHI = "Marathi"
+    MALAY = "Malay"
+    BURMESE = "Burmese"
+    NEPALI = "Nepali"
+    DUTCH = "Dutch"
+    NORWEGIAN = "Norwegian"
+    OROMO = "Oromo"
+    ORIYA = "Oriya"
+    PANJABI = "Panjabi"
+    POLISH = "Polish"
+    PASHTO = "Pashto"
+    PORTUGUESE = "Portuguese"
+    ROMANIAN = "Romanian"
+    RUSSIAN = "Russian"
+    SANSKRIT = "Sanskrit"
+    SINDHI = "Sindhi"
+    SINHALA = "Sinhala"
+    SLOVAK = "Slovak"
+    SLOVENIAN = "Slovenian"
+    SOMALI = "Somali"
+    ALBANIAN = "Albanian"
+    SERBIAN = "Serbian"
+    SUNDANESE = "Sundanese"
+    SWEDISH = "Swedish"
+    SWAHILI = "Swahili"
+    TAMIL = "Tamil"
+    TELUGU = "Telugu"
+    THAI = "Thai"
+    TAGALOG = "Tagalog"
+    TURKISH = "Turkish"
+    UYGHUR = "Uyghur"
+    UKRAINIAN = "Ukrainian"
+    URDU = "Urdu"
+    UZBEK = "Uzbek"
+    VIETNAMESE = "Vietnamese"
+    XHOSA = "Xhosa"
+    YIDDISH = "Yiddish"
+    CHINESE = "Chinese"
+
+    @classmethod
+    def list_all_languages(cls):
+        return list(map(lambda c: c.value, cls))  # type: ignore [attr-defined]
+
+
+class VectorDatabaseChunkingParameterType(StrEnum):
+    """Chunking parameter types supported by VectorDatabases."""
+
+    INT = "int"
+    LIST_STR = "list[str]"
+
+
+class VectorDatabaseSource(StrEnum):
+    """Supported source for VectorDatabases."""
+
+    DATAROBOT = "DataRobot"
+    EXTERNAL = "External"
+
+
+class VectorDatabaseExecutionStatus(StrEnum):
+    """Execution Statuses VectorDatabases can be in."""
+
+    NEW = "NEW"
+    RUNNING = "RUNNING"
+    COMPLETED = "COMPLETED"
+    ERROR = "ERROR"
+
+
+class ListPlaygroundsSortQueryParams(StrEnum):
+    """supported Sort query params for the Playground.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DESCRIPTION_ASCENDING = "description"
+    DESCRIPTION_DESCENDING = "-description"
+    CREATION_USER_DATE_ASCENDING = "creationUserId"
+    CREATION_USER_DATE_DESCENDING = "-creationUserId"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+    LAST_UPDATE_USER_DATE_ASCENDING = "lastUpdateUserId"
+    LAST_UPDATE_USER_DATE_DESCENDING = "-lastUpdateUserId"
+    SAVED_LLM_BLUEPRINTS_COUNT_ASCENDING = "savedLLMBlueprintsCount"
+    SAVED_LLM_BLUEPRINTS_COUNT_DESCENDING = "-savedLLMBlueprintsCount"
+
+
+class ListChatsSortQueryParams(StrEnum):
+    """supported Sort query params for the Chat.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class ListComparisonChatsSortQueryParams(StrEnum):
+    """supported Sort query params for the ComparisonChat.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class ListLLMBlueprintsSortQueryParams(StrEnum):
+    """supported Sort query params for the LLMBlueprint.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DESCRIPTION_ASCENDING = "description"
+    DESCRIPTION_DESCENDING = "-description"
+    CREATION_USER_DATE_ASCENDING = "creationUserId"
+    CREATION_USER_DATE_DESCENDING = "-creationUserId"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+    LAST_UPDATE_USER_DATE_ASCENDING = "lastUpdateUserId"
+    LAST_UPDATE_USER_DATE_DESCENDING = "-lastUpdateUserId"
+    LAST_UPDATE_DATE_ASCENDING = "lastUpdateDate"
+    LAST_UPDATE_DATE_DESCENDING = "-lastUpdateDate"
+    LLM_ID_ASCENDING = "llmId"
+    LLM_ID_DESCENDING = "-llmId"
+    VECTOR_DATABASE_ID_ASCENDING = "vectorDatabaseId"
+    VECTOR_DATABASE_ID_DESCENDING = "-vectorDatabaseId"
+
+
+class ListCustomModelValidationsSortQueryParams(StrEnum):
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DEPLOYMENT_NAME_ASCENDING = "deploymentName"
+    DEPLOYMENT_NAME_DESCENDING = "-deploymentName"
+    USER_NAME_ASCENDING = "userName"
+    USER_NAME_DESCENDING = "-userName"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class PromptType(StrEnum):
+    """Supported LLM Blueprint prompting types."""
+
+    ONE_TIME_PROMPT = "ONE_TIME_PROMPT"
+    CHAT_HISTORY_AWARE = "CHAT_HISTORY_AWARE"
```

### Comparing `datarobot-3.3.2/datarobot/errors.py` & `datarobot-3.4.0/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/helpers/__init__.py` & `datarobot-3.4.0/datarobot/helpers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,27 +89,27 @@
         Please remove any usage of this parameter as it will be removed from the API soon.
     events_count : string, optional
         (New in version v2.8) the name of a column specifying events count.
     monotonic_increasing_featurelist_id : string, optional
         (new in version 2.11) the id of the featurelist that defines the set of features
         with a monotonically increasing relationship to the target. If None,
         no such constraints are enforced. When specified, this will set a default for the project
-        that can be overriden at model submission time if desired.
+        that can be overridden at model submission time if desired.
     monotonic_decreasing_featurelist_id : string, optional
         (new in version 2.11) the id of the featurelist that defines the set of features
         with a monotonically decreasing relationship to the target. If None,
         no such constraints are enforced. When specified, this will set a default for the project
-        that can be overriden at model submission time if desired.
+        that can be overridden at model submission time if desired.
     only_include_monotonic_blueprints : bool, optional
         (new in version 2.11) when true, only blueprints that support enforcing
         monotonic constraints will be available in the project or selected for the autopilot.
     allowed_pairwise_interaction_groups : list of tuple, optional
         (New in version v2.19) For GA2M models - specify groups of columns for which pairwise
         interactions will be allowed. E.g. if set to [(A, B, C), (C, D)] then GA2M models will
-        allow interactions between columns AxB, BxC, AxC, CxD. All others (AxD, BxD) will
+        allow interactions between columns A x B, B x C, A x C, C x D. All others (A x D, B x D) will
         not be considered.
     blend_best_models: bool, optional
         (New in version v2.19) blend best models during Autopilot run.
     scoring_code_only: bool, optional
         (New in version v2.19) Keep only models that can be converted to scorable java code
         during Autopilot run
     shap_only_mode: bool, optional
@@ -195,14 +195,22 @@
     model_group_id: Optional[str] = None,
         (New in version v3.3) The name of a column containing the model group ID for each row.
     model_regime_id: Optional[str] = None,
         (New in version v3.3) The name of a column containing the model regime ID for each row.
     model_baselines: Optional[List[str]] = None,
         (New in version v3.3) The list of the names of the columns containing the model baselines
         for each row.
+    incremental_learning_only_mode: Optional[bool] = None,
+        (New in version v3.4) Keep only models that support incremental learning during Autopilot run.
+    incremental_learning_on_best_model: Optional[bool] = None,
+        (New in version v3.4) Run incremental learning on the best model during Autopilot run.
+    chunk_definition_id : string, optional
+        (New in version v3.4) Unique definition for chunks needed to run automated incremental learning.
+    incremental_learning_early_stopping_rounds : Optional[int] = None
+        (New in version v3.4) Early stopping rounds used in the automated incremental learning service.
 
     Examples
     --------
     .. code-block:: python
 
         import datarobot as dr
         advanced_options = dr.AdvancedOptions(
@@ -256,14 +264,18 @@
         bias_mitigation_technique: Optional[str] = None,
         include_bias_mitigation_feature_as_predictor_variable: Optional[bool] = None,
         default_monotonic_increasing_featurelist_id: Optional[str] = None,
         default_monotonic_decreasing_featurelist_id: Optional[str] = None,
         model_group_id: Optional[str] = None,
         model_regime_id: Optional[str] = None,
         model_baselines: Optional[List[str]] = None,
+        incremental_learning_only_mode: Optional[bool] = None,
+        incremental_learning_on_best_model: Optional[bool] = None,
+        chunk_definition_id: Optional[str] = None,
+        incremental_learning_early_stopping_rounds: Optional[int] = None,
     ) -> None:
         if scaleout_modeling_mode:
             deprecation_warning(
                 subject="Parameter `scaleout_modeling_mode` in Advanced Options is deprecated",
                 deprecated_since_version="3.1",
                 will_remove_version="3.3",
                 message="DataRobot no longer supports scaleout models. "
@@ -314,14 +326,18 @@
         )
         self.default_monotonic_decreasing_featurelist_id = (
             default_monotonic_decreasing_featurelist_id
         )
         self.model_group_id = model_group_id
         self.model_regime_id = model_regime_id
         self.model_baselines = model_baselines
+        self.incremental_learning_only_mode = incremental_learning_only_mode
+        self.incremental_learning_on_best_model = incremental_learning_on_best_model
+        self.chunk_definition_id = chunk_definition_id
+        self.incremental_learning_early_stopping_rounds = incremental_learning_early_stopping_rounds
         attributes = {
             k: v
             for k, v in self.__dict__.items()
             if not k.startswith("__") and not callable(getattr(self, k))
         }
         super().__init__(**attributes)
 
@@ -439,14 +455,18 @@
                 self.include_bias_mitigation_feature_as_predictor_variable
             ),
             default_monotonic_increasing_featurelist_id=self.default_monotonic_increasing_featurelist_id,
             default_monotonic_decreasing_featurelist_id=self.default_monotonic_decreasing_featurelist_id,
             model_group_id=self.model_group_id,
             model_regime_id=self.model_regime_id,
             model_baselines=self.model_baselines,
+            incremental_learning_only_mode=self.incremental_learning_only_mode,
+            incremental_learning_on_best_model=self.incremental_learning_on_best_model,
+            chunk_definition_id=self.chunk_definition_id,
+            incremental_learning_early_stopping_rounds=self.incremental_learning_early_stopping_rounds,
         )
 
         payload.update({k: v for k, v in optional.items() if v is not None})
 
         return payload
```

### Comparing `datarobot-3.3.2/datarobot/helpers/binary_data_utils.py` & `datarobot-3.4.0/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/helpers/eligibility_result.py` & `datarobot-3.4.0/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/helpers/feature_discovery.py` & `datarobot-3.4.0/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/helpers/image_utils.py` & `datarobot-3.4.0/datarobot/helpers/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,23 +50,23 @@
         image. If False, the resize method modifies the image to contain a thumbnail version
         of itself, no larger than the given size, that preserves the image's aspect ratio.
     image_size: Tuple[int, int]
         New image size (width, height). Both values (width, height) should be specified and contain
         a positive value. Depending on the value of `force_size`, the image will be resized exactly
         to the given image size or will be resized into a thumbnail version of itself, no larger
         than the given size.
-    image_format: enums.ImageFormat | str
+    image_format: ImageFormat | str
         What image format will be used to save result image after transformations. For example
         (ImageFormat.JPEG, ImageFormat.PNG). Values supported are in line with values supported
         by DataRobot. If no format is specified by passing `None` value original image format
         will be preserved.
     image_quality: int or None
         The image quality used when saving image. When None is specified, a value will
         not be passed and Pillow library will use its default.
-    resample_method: enum.ImageResampleMethod
+    resample_method: ImageResampleMethod
         What resampling method should be used when resizing image.
     keep_quality: bool
         Whether the image quality is kept (when possible). If True, for JPEG images quality will
         be preserved. For other types, the value specified in `image_quality` will be used.
     """
 
     def __init__(
@@ -211,11 +211,13 @@
         else:
             image.thumbnail(size=image_options.image_size, resample=image_options.resample_method)
 
     if image.mode != "RGB":
         if image.mode == "I":
             image = _scale_image_to_8bit_range(image)
         image = image.convert("RGB")
-        image.format = image_format
+
+    # Some PIL operations loose the image_format information.
+    image.format = image_format
 
     # convert to target image format and return as image_bytes
     return get_bytes_from_image(image, image_options)
```

### Comparing `datarobot-3.3.2/datarobot/helpers/partitioning_methods.py` & `datarobot-3.4.0/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/mixins/browser_mixin.py` & `datarobot-3.4.0/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/mixins/update_attributes_mixin.py` & `datarobot-3.4.0/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/__init__.py` & `datarobot-3.4.0/datarobot/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
+import datarobot.models.genai
+import datarobot.models.registry
+
 from .application import Application
 from .automated_documentation import AutomatedDocument
 from .batch_monitoring_job import BatchMonitoringJob, BatchMonitoringJobDefinition
 from .batch_prediction_job import BatchPredictionJob, BatchPredictionJobDefinition
 from .blueprint import Blueprint, BlueprintChart, BlueprintTaskDocument, ModelBlueprintChart
 from .calendar_file import CalendarFile
 from .change_request import ChangeRequest, ChangeRequestReview
@@ -61,20 +64,22 @@
     FeatureEffectMetadataDatetimePerBacktest,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
 from .featurelist import DatasetFeaturelist, Featurelist, ModelingFeaturelist
 from .imported_model import ImportedModel
 from .job import FeatureImpactJob, Job, TrainingPredictionsJob
+from .key_values import KeyValue
 from .model import (
     BlenderModel,
     ClusteringModel,
     CombinedModel,
     DatetimeModel,
     FrozenModel,
+    GenericModel,
     Model,
     ModelParameters,
     PrimeModel,
     RatingTableModel,
 )
 from .model_registry import RegisteredModel, RegisteredModelVersion
 from .modeljob import ModelJob
```

### Comparing `datarobot-3.3.2/datarobot/models/advanced_tuning.py` & `datarobot-3.4.0/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/anomaly_assessment.py` & `datarobot-3.4.0/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/api_object.py` & `datarobot-3.4.0/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/application.py` & `datarobot-3.4.0/datarobot/models/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     deployment_id: str
     reference_name: str
 
 
 class ApplicationRelatedEntity(TypedDict):
     model_id: Optional[str]
     project_id: Optional[str]
+    is_from_use_case: Optional[bool]
     is_from_experiment_container: Optional[bool]
 
 
 class Application(APIObject):
     """
     An entity associated with a DataRobot Application.
 
@@ -115,14 +116,15 @@
             t.Key("has_custom_logo"): t.Bool,
             t.Key("org_id"): t.String,
             t.Key("pool_used"): t.Bool,
             t.Key("related_entities", optional=True): t.Dict(
                 {
                     t.Key("model_id", optional=True): t.String,
                     t.Key("project_id", optional=True): t.String,
+                    t.Key("is_from_use_case", optional=True): t.Bool,
                     t.Key("is_from_experiment_container", optional=True): t.Bool,
                 }
             ),
             t.Key("application_template_type", optional=True): t.String,
             t.Key("deactivation_status_id", optional=True): t.String,
             t.Key("created_first_name", optional=True): t.String,
             t.Key("creator_last_name", optional=True): t.String,
@@ -207,15 +209,15 @@
         offset : Optional[int]
             Optional. Retrieve applications in a list after this number.
         limit : Optional[int]
             Optional. Retrieve only this number of applications.
         use_cases: Optional[Union[UseCase, List[UseCase], str, List[str]]]
             Optional. Filter available Applications by a specific Use Case or Use Cases.
             Accepts either the entity or the ID.
-            If set to [None], the method filters the project's applications by those not linked to a UseCase.
+            If set to [None], the method filters the application's datasets by those not linked to a UseCase.
 
         Returns
         -------
         applications : List[Application]
             The requested list of user applications.
         """
         query = {"offset": offset, "limit": limit}
```

### Comparing `datarobot-3.3.2/datarobot/models/automated_documentation.py` & `datarobot-3.4.0/datarobot/models/automated_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         --------
         .. code-block:: python
 
             import datarobot as dr
 
             dr.Client(token=my_token, endpoint=endpoint)
 
-            # NOTE: entity_id is either a model id or a model package id
+            # NOTE: entity_id is either a model id or a model package (version) id
             doc = dr.AutomatedDocument(
                     document_type="MODEL_COMPLIANCE",
                     entity_id="6f50cdb77cc4f8d1560c3ed5",
                     output_format="docx",
                     locale="EN_US")
 
             doc.initialize_model_compliance()
```

### Comparing `datarobot-3.3.2/datarobot/models/batch_job.py` & `datarobot-3.4.0/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/batch_monitoring_job.py` & `datarobot-3.4.0/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/batch_prediction_job.py` & `datarobot-3.4.0/datarobot/models/batch_prediction_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,24 @@
     recognize_sourcedata,
     Schedule,
 )
 from datarobot.models.credential import Credential
 from datarobot.models.dataset import Dataset
 from datarobot.models.prediction_explanations import PredictionExplanationsMode
 from datarobot.models.project import Project
-from datarobot.utils import get_id_from_response, pagination, to_api
+from datarobot.utils import (
+    deprecation_warning,
+    get_id_from_response,
+    logger,
+    pagination,
+    parse_time,
+    to_api,
+)
 
 from ..enums import DEFAULT_TIMEOUT, IntakeAdapters, JOB_TYPE, OutputAdapters, QUEUE_STATUS
-from ..utils import logger, parse_time
 from .api_object import APIObject
 
 LOG = logger.get_logger(__name__)
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
@@ -61,14 +67,21 @@
     class PredictionInstance(TypedDict):
         hostName: str
         sslEnabled: Optional[bool]
         datarobotKey: Optional[str]
         apiKey: Optional[str]
 
 
+class MissingType:
+    pass
+
+
+MISSING = MissingType()
+
+
 class BatchPredictionJob(AbstractBatchJob):
     """
     A Batch Prediction Job is used to score large data sets on
     prediction servers using the Batch Prediction API.
 
     Attributes
     ----------
@@ -85,14 +98,16 @@
             t.Key("explanation_num_top_classes", optional=True): t.Int(),
             t.Key("deployment_id", optional=True): String(),
             t.Key("model_id", optional=True): String(),
             t.Key("passthrough_columns", optional=True): t.List(String(allow_blank=True)),
             t.Key("passthrough_columns_set", optional=True): String(),
             t.Key("max_explanations", optional=True): Int(),
             t.Key("max_ngram_explanations", optional=True): t.Int(gte=0) | t.Atom("all"),
+            t.Key("explanation_algorithm", optional=True): String(),
+            t.Key("prediction_threshold", optional=True): t.Float(gte=0.0, lte=1.0) | t.Null(),
             t.Key("prediction_warning_enabled", optional=True): t.Bool(),
             t.Key("intake_settings", optional=True): t.Dict().allow_extra("*"),
             t.Key("output_settings", optional=True): t.Dict().allow_extra("*"),
             t.Key("timeseries_settings", optional=True): t.Dict().allow_extra("*"),
         }
     ).allow_extra("*")
     _links = t.Dict(
@@ -189,16 +204,18 @@
         timeseries_settings: Optional[TimeSeriesSettings] = None,
         num_concurrent: Optional[int] = None,
         chunk_size: Optional[Union[int, str]] = None,
         passthrough_columns: Optional[List[str]] = None,
         passthrough_columns_set: Optional[str] = None,
         max_explanations: Optional[int] = None,
         max_ngram_explanations: Optional[Union[int, str]] = None,
+        explanation_algorithm: Optional[str] = None,
         threshold_high: Optional[float] = None,
         threshold_low: Optional[float] = None,
+        prediction_threshold: Optional[float] = None,
         prediction_warning_enabled: Optional[bool] = None,
         include_prediction_status: bool = False,
         skip_drift_tracking: bool = False,
         prediction_instance: Optional[PredictionInstance] = None,
         abort_on_error: bool = True,
         column_names_remapping: Optional[Dict[str, str]] = None,
         include_probabilities: bool = True,
@@ -223,20 +240,26 @@
 
         if max_explanations is not None:
             job_data["maxExplanations"] = int(max_explanations)
 
         if max_ngram_explanations is not None:
             job_data["maxNgramExplanations"] = max_ngram_explanations
 
+        if explanation_algorithm is not None:
+            job_data["explanationAlgorithm"] = explanation_algorithm
+
         if threshold_high is not None:
             job_data["thresholdHigh"] = float(threshold_high)
 
         if threshold_low is not None:
             job_data["thresholdLow"] = float(threshold_low)
 
+        if prediction_threshold is not None:
+            job_data["predictionThreshold"] = float(prediction_threshold)
+
         if explanations_mode is not None:
             job_data.update(explanations_mode.get_api_parameters(batch_route=True))
 
         if include_prediction_status:
             job_data["includePredictionStatus"] = bool(include_prediction_status)
 
         if skip_drift_tracking:
@@ -370,16 +393,18 @@
         timeseries_settings: Optional[TimeSeriesSettings] = None,
         num_concurrent: Optional[int] = None,
         chunk_size: Optional[Union[int, str]] = None,
         passthrough_columns: Optional[List[str]] = None,
         passthrough_columns_set: Optional[str] = None,
         max_explanations: Optional[int] = None,
         max_ngram_explanations: Optional[Union[int, str]] = None,
+        explanation_algorithm: Optional[str] = None,
         threshold_high: Optional[float] = None,
         threshold_low: Optional[float] = None,
+        prediction_threshold: Optional[float] = None,
         prediction_warning_enabled: Optional[bool] = None,
         include_prediction_status: bool = False,
         skip_drift_tracking: bool = False,
         prediction_instance: Optional[PredictionInstance] = None,
         abort_on_error: bool = True,
         column_names_remapping: Optional[Dict[str, str]] = None,
         include_probabilities: bool = True,
@@ -637,14 +662,23 @@
 
         upload_read_timeout: int (optional, default 600)
             .. versionadded:: 2.28
 
             If using localFile intake, wait this many seconds for the server to respond
             after whole dataset upload.
 
+        prediction_threshold: float (optional)
+            .. versionadded:: 3.4.0
+
+            Threshold is the point that sets the class boundary for a predicted value. The model
+            classifies an observation below the threshold as FALSE, and an observation above the
+            threshold as TRUE. In other words, DataRobot automatically assigns the positive class
+            label to any prediction exceeding the threshold.
+            This value can be set between 0.0 and 1.0.
+
         Returns
         -------
         BatchPredictionJob
             Instance of BatchPredictionJob
         """
         try:
             dep_id = cast("Deployment", deployment).id
@@ -659,16 +693,18 @@
             timeseries_settings=timeseries_settings,
             num_concurrent=num_concurrent,
             chunk_size=chunk_size,
             passthrough_columns=passthrough_columns,
             passthrough_columns_set=passthrough_columns_set,
             max_explanations=max_explanations,
             max_ngram_explanations=max_ngram_explanations,
+            explanation_algorithm=explanation_algorithm,
             threshold_high=threshold_high,
             threshold_low=threshold_low,
+            prediction_threshold=prediction_threshold,
             prediction_warning_enabled=prediction_warning_enabled,
             include_prediction_status=include_prediction_status,
             skip_drift_tracking=skip_drift_tracking,
             prediction_instance=prediction_instance,
             abort_on_error=abort_on_error,
             column_names_remapping=column_names_remapping,
             include_probabilities=include_probabilities,
@@ -1267,16 +1303,18 @@
         output_settings: Optional[OutputSettings] = None,
         csv_settings: Optional[CsvSettings] = None,
         timeseries_settings: Optional[TimeSeriesSettings] = None,
         passthrough_columns: Optional[List[str]] = None,
         passthrough_columns_set: Optional[str] = None,
         max_explanations: Optional[int] = None,
         max_ngram_explanations: Optional[Union[int, str]] = None,
+        explanation_algorithm: Optional[str] = None,
         threshold_high: Optional[float] = None,
         threshold_low: Optional[float] = None,
+        prediction_threshold: Optional[float] = None,
         prediction_warning_enabled: Optional[bool] = None,
         include_prediction_status: bool = False,
         abort_on_error: bool = True,
         column_names_remapping: Optional[Dict[str, str]] = None,
         include_probabilities: bool = True,
         include_probabilities_classes: Optional[List[str]] = None,
         download_timeout: Optional[int] = 120,
@@ -1445,14 +1483,23 @@
 
         upload_read_timeout: int (optional, default 600)
             .. versionadded:: 2.28
 
             If using localFile intake, wait this many seconds for the server to respond
             after whole dataset upload.
 
+        prediction_threshold: float (optional)
+            .. versionadded:: 3.4.0
+
+            Threshold is the point that sets the class boundary for a predicted value. The model
+            classifies an observation below the threshold as FALSE, and an observation above the
+            threshold as TRUE. In other words, DataRobot automatically assigns the positive class
+            label to any prediction exceeding the threshold.
+            This value can be set between 0.0 and 1.0.
+
         Returns
         -------
         BatchPredictionJob
             Instance of BatchPredictionJob
         """
         try:
             model_id = cast("Model", model).id
@@ -1487,16 +1534,18 @@
             output_settings=output_settings,
             csv_settings=csv_settings,
             timeseries_settings=timeseries_settings,
             passthrough_columns=passthrough_columns,
             passthrough_columns_set=passthrough_columns_set,
             max_explanations=max_explanations,
             max_ngram_explanations=max_ngram_explanations,
+            explanation_algorithm=explanation_algorithm,
             threshold_high=threshold_high,
             threshold_low=threshold_low,
+            prediction_threshold=prediction_threshold,
             prediction_warning_enabled=prediction_warning_enabled,
             include_prediction_status=include_prediction_status,
             abort_on_error=abort_on_error,
             column_names_remapping=column_names_remapping,
             include_probabilities=include_probabilities,
             include_probabilities_classes=include_probabilities_classes,
             download_timeout=download_timeout,
@@ -1720,18 +1769,37 @@
             >>> definition
             BatchPredictionJobDefinition(60912e09fd1f04e832a575c1)
         """
 
         return cls.from_location(f"{cls._path}{batch_prediction_job_definition_id}/")
 
     @classmethod
-    def list(cls) -> List[BatchPredictionJobDefinition]:
+    def list(
+        cls,
+        search_name: Optional[str] = None,
+        deployment_id: Optional[str] = None,
+        limit: Union[int, MissingType] = MISSING,
+        offset: int = 0,
+    ) -> List[BatchPredictionJobDefinition]:
         """
         Get job all definitions
 
+        Parameters
+        ----------
+        search_name : str, optional
+            String for filtering job definitions
+            Job definitions that contain the string in name will be returned.
+            If not specified, all available job definitions will be returned.
+        deployment_id: str
+            The ID of the deployment record belongs to.
+        limit: int, optional
+            0 by default. At most this many results are returned.
+        offset: int, optional
+            This many results will be skipped.
+
         Returns
         -------
         List[BatchPredictionJobDefinition]
             List of job definitions the user has access to see
 
         Examples
         --------
@@ -1741,18 +1809,43 @@
             >>> definition = dr.BatchPredictionJobDefinition.list()
             >>> definition
             [
                 BatchPredictionJobDefinition(60912e09fd1f04e832a575c1),
                 BatchPredictionJobDefinition(6086ba053f3ef731e81af3ca)
             ]
         """
+        if limit is MISSING:
+            deprecation_warning(
+                "BatchPredictionJobDefinition.list",
+                deprecated_since_version="v3.4",
+                will_remove_version="v3.6",
+                message="BatchPredictionJobDefinition.list will no longer return all job definitions "
+                "after version 3.6 is released. To preserve current behavior please pass limit=0.",
+            )
+
+            limit = 0  # deprecated behaviour: return everything
+
+        params = {}
+        if search_name:
+            params["searchName"] = search_name
+        if deployment_id:
+            params["deploymentId"] = deployment_id
+
+        if limit == 0:  # unlimited results
+            r_data = pagination.unpaginate(cls._path, params, cls._client)
+        else:
+            params["offset"] = offset
+            params["limit"] = limit
+            response = cls._client.get(cls._path, params=params).json()
+            r_data = response["data"]
 
-        return list(
-            cls.from_server_data(item) for item in pagination.unpaginate(cls._path, {}, cls._client)
+        records = cast(
+            List["BatchPredictionJobDefinition"], [cls.from_server_data(item) for item in r_data]
         )
+        return records
 
     @classmethod
     def create(
         cls,
         enabled: bool,
         batch_prediction_job,
         name: Optional[str] = None,
```

### Comparing `datarobot-3.3.2/datarobot/models/blueprint.py` & `datarobot-3.4.0/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/calendar_file.py` & `datarobot-3.4.0/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/change_request.py` & `datarobot-3.4.0/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/cluster.py` & `datarobot-3.4.0/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/cluster_insight.py` & `datarobot-3.4.0/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/compliance_doc_template.py` & `datarobot-3.4.0/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/confusion_chart.py` & `datarobot-3.4.0/datarobot/models/confusion_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     Attributes
     ----------
     source : str
         Confusion Chart data source. Can be 'validation', 'crossValidation' or 'holdout'.
     raw_data : dict
         All of the raw data for the Confusion Chart
     confusion_matrix : list of list
-        The NxN confusion matrix
+        The N x N confusion matrix
     classes : list
         The names of each of the classes
     class_metrics : list of dicts
         List of dicts with schema described as ``ClassMetrics`` above.
     source_model_id : str
         ID of the model this Confusion chart represents; in some cases,
         insights from the parent of a frozen model may be used
```

### Comparing `datarobot-3.3.2/datarobot/models/connector.py` & `datarobot-3.4.0/datarobot/models/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,32 +44,35 @@
     _path = "externalConnectors/"
     _file_upload_path = "externalDataDriverFile/"
     _converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("creator_id"): String(),
             t.Key("configuration_id"): String(),
-            t.Key("base_name"): String(),
+            t.Key("base_name", optional=True): t.Or(String, t.Null),
             t.Key("canonical_name"): String(),
+            t.Key("connector_type", optional=True): t.Or(String, t.Null),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id: Optional[str] = None,
         creator_id: Optional[str] = None,
         configuration_id: Optional[str] = None,
         base_name: Optional[str] = None,
         canonical_name: Optional[str] = None,
+        connector_type: Optional[str] = None,
     ):
         self._id = id
         self._creator_id = creator_id
         self._configuration_id = configuration_id
         self._base_name = base_name
         self._canonical_name = canonical_name
+        self._connector_type = connector_type
 
     @classmethod
     def list(cls) -> List[Connector]:
         """
         Returns list of available connectors.
 
         Returns
@@ -234,9 +237,13 @@
     def base_name(self) -> Optional[str]:
         return self._base_name
 
     @property
     def canonical_name(self) -> Optional[str]:
         return self._canonical_name
 
+    @property
+    def connector_type(self) -> Optional[str]:
+        return self._connector_type
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}('{self.canonical_name or self.id}')"
```

### Comparing `datarobot-3.3.2/datarobot/models/credential.py` & `datarobot-3.4.0/datarobot/models/key_values.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,444 +1,424 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2024 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from datetime import datetime
-import json
-from typing import Any, Dict, List, Optional, Union
+from typing import List, Optional, Set, Union
 
 import trafaret as t
-from trafaret.contrib.rfc_3339 import DateTime
 
 from datarobot._compat import String
+from datarobot.enums import KeyValueCategory, KeyValueEntityType, KeyValueType
 from datarobot.models.api_object import APIObject
-from datarobot.utils import pagination, rawdict
+from datarobot.utils.pagination import unpaginate
 
 
-class Credential(APIObject):  # pylint: disable=missing-class-docstring
-    _path = "credentials/"
+class KeyValue(APIObject):
+    """A DataRobot Key-Value.
+
+    .. versionadded:: v3.4
+
+    Attributes
+    ----------
+    id: str
+        ID of the Key-Value
+    created_at: str
+        creation time of the Key-Value
+    entity_id: str
+        ID of the related Entity
+    entity_type: KeyValueEntityType
+        type of the related Entity
+    name: str
+        Key-Value name
+    value: str
+        Key-Value value
+    numeric_value: float
+        Key-Value numeric value
+    boolean_value: bool
+        Key-Value boolean value
+    value_type: KeyValueType
+        Key-Value type
+    description: str
+        Key-Value description
+    creator_id: str
+        ID of the user who created the Key-Value
+    creator_name: str
+        ID of the user who created the Key-Value
+    category: KeyValueCategory
+        Key-Value category
+    artifact_size: int
+        size in bytes of associated image, if applicable
+    original_file_name: str
+        name of uploaded original image or dataset file
+    is_editable: bool
+        true if a user with permissions can edit or delete
+    is_dataset_missing: bool
+        true if the key-value type is "dataset" and its dataset is not visible to the user
+    error_message: str
+        additional information if "isDataSetMissing" is true. Blank if there are no errors
+    """
+
+    _path = "keyValues/"
+
     _converter = t.Dict(
         {
+            t.Key("id"): String(),
+            t.Key("created_at"): String(),
+            t.Key("entity_id"): String(),
+            t.Key("entity_type"): t.Enum(*[e.value for e in KeyValueEntityType]),
             t.Key("name"): String(),
-            t.Key("credential_id"): String(),
-            t.Key("creation_date"): DateTime(),
-            t.Key("credential_type"): String(),
+            t.Key("value"): String(),
+            t.Key("numeric_value"): t.Float(),
+            t.Key("boolean_value", optional=True, default=False): t.Bool(),
+            t.Key("value_type"): t.Enum(*[e.value for e in KeyValueType]),
             t.Key("description"): String(allow_blank=True),
+            t.Key("creator_id"): String(),
+            t.Key("creator_name"): String(),
+            t.Key("category"): t.Enum(*[e.value for e in KeyValueCategory]),
+            t.Key("artifact_size"): t.Int(),
+            t.Key("original_file_name"): String(allow_blank=True),
+            t.Key("is_editable"): t.Bool(),
+            t.Key("is_dataset_missing"): t.Bool(),
+            t.Key("error_message"): String(allow_blank=True),
         }
-    ).allow_extra("*")
+    ).ignore_extra("*")
+
+    schema = _converter
 
     def __init__(
         self,
-        credential_id: Optional[str] = None,
-        name: Optional[str] = None,
-        credential_type: Optional[str] = None,
-        creation_date: Optional[datetime] = None,
-        description: Optional[str] = None,
+        id: str,
+        created_at: str,
+        entity_id: str,
+        entity_type: KeyValueEntityType,
+        name: str,
+        value: str,
+        numeric_value: float,
+        boolean_value: bool,
+        value_type: KeyValueType,
+        description: str,
+        creator_id: str,
+        creator_name: str,
+        category: KeyValueCategory,
+        artifact_size: int,
+        original_file_name: str,
+        is_editable: bool,
+        is_dataset_missing: bool,
+        error_message: str,
     ) -> None:
-        self.credential_id = credential_id
+        self.id = id
+        self.created_at = created_at
+        self.entity_id = entity_id
+        self.entity_type = KeyValueEntityType(entity_type)
         self.name = name
-        self.credential_type = credential_type
-        self.creation_date = creation_date
+        self.value = value
+        self.numeric_value = numeric_value
+        self.boolean_value = boolean_value
+        self.value_type = KeyValueType(value_type)
         self.description = description
+        self.creator_id = creator_id
+        self.creator_name = creator_name
+        self.category = KeyValueCategory(category)
+        self.artifact_size = artifact_size
+        self.original_file_name = original_file_name
+        self.is_editable = is_editable
+        self.is_dataset_missing = is_dataset_missing
+        self.error_message = error_message
 
-    @classmethod
-    def list(cls) -> List[Credential]:
-        """
-        Returns list of available credentials.
-
-        Returns
-        -------
-        credentials : list of Credential instances
-            contains a list of available credentials.
-
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> data_sources = dr.Credential.list()
-            >>> data_sources
-            [
-                Credential('5e429d6ecf8a5f36c5693e03', 'my_s3_cred', 's3'),
-                Credential('5e42cc4dcf8a5f3256865840', 'my_jdbc_cred', 'jdbc'),
-            ]
-        """
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.name or self.id!r})"
 
-        return [
-            cls.from_server_data(item) for item in pagination.unpaginate(cls._path, {}, cls._client)
-        ]
+    def _update_values(self, new_response: KeyValue) -> None:
+        fields: Set[str] = self._fields()  # type: ignore[no-untyped-call]
+        for attr in fields:
+            new_value = getattr(new_response, attr)
+            setattr(self, attr, new_value)
 
     @classmethod
-    def get(cls, credential_id: str) -> Credential:
-        """
-        Gets the Credential.
-
-        Parameters
-        ----------
-        credential_id : str
-            the identifier of the credential.
-
-        Returns
-        -------
-        credential : Credential
-            the requested credential.
+    def _key_value_path(cls, key_value_id: str) -> str:
+        return f"{cls._path}{key_value_id}/"
 
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.get('5a8ac9ab07a57a0001be501f')
-            >>> cred
-            Credential('5e429d6ecf8a5f36c5693e03', 'my_s3_cred', 's3'),
-        """
-        return cls.from_location(f"{cls._path}{credential_id}/")
+    @classmethod
+    def get(cls, key_value_id: str) -> KeyValue:
+        """Get Key-Value by id.
 
-    def delete(self) -> None:
-        """
-        Deletes the Credential the store.
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        credential_id : str
-            the identifier of the credential.
+        key_value_id: str
+            ID of the Key-Value
 
         Returns
         -------
-        credential : Credential
-            the requested credential.
+        KeyValue
+            retrieved Key-Value
 
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.get('5a8ac9ab07a57a0001be501f')
-            >>> cred.delete()
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status.
+        datarobot.errors.ServerError
+            if the server responded with 5xx status.
         """
-        self._client.delete(f"{self._path}{self.credential_id}/")
+        path = cls._key_value_path(key_value_id)
+        return cls.from_location(path)
 
     @classmethod
-    def create_basic(
-        cls,
-        name: str,
-        user: str,
-        password: str,
-        description: Optional[str] = None,
-    ) -> Credential:
-        """
-        Creates the credentials.
+    def list(cls, entity_id: str, entity_type: KeyValueEntityType) -> List[KeyValue]:
+        """List Key-Values.
+
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        name : str
-            the name to use for this set of credentials.
-        user : str
-            the username to store for this set of credentials.
-        password : str
-            the password to store for this set of credentials.
-        description : str, optional
-            the description to use for this set of credentials.
+        entity_id: str
+            ID of the related Entity
+        entity_type: KeyValueEntityType
+            type of the related Entity
 
         Returns
         -------
-        credential : Credential
-            the created credential.
+        List[KeyValue]
+            a list of Key-Values
 
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.create_basic(
-            ...     name='my_basic_cred',
-            ...     user='username',
-            ...     password='password',
-            ... )
-            >>> cred
-            Credential('5e429d6ecf8a5f36c5693e03', 'my_basic_cred', 'basic'),
-        """
-        payload = {
-            "name": name,
-            "credentialType": "basic",
-            "user": user,
-            "password": password,
-            "description": description,
-        }
-        return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status
+        datarobot.errors.ServerError
+            if the server responded with 5xx status
+        """
+        data = unpaginate(
+            cls._path,
+            {"entityId": entity_id, "entityType": entity_type.value},
+            cls._client,
+        )
+        return [cls.from_server_data(item) for item in data]
 
     @classmethod
-    def create_oauth(
-        cls,
-        name: str,
-        token: str,
-        refresh_token: str,
-        description: Optional[str] = None,
-    ) -> Credential:
-        """
-        Creates the OAUTH credentials.
+    def find(cls, entity_id: str, entity_type: KeyValueEntityType, name: str) -> Optional[KeyValue]:
+        """Find Key-Value by name.
+
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        name : str
-            the name to use for this set of credentials.
-        token: str
-            the OAUTH token
-        refresh_token: str
-            The OAUTH token
-        description : str, optional
-            the description to use for this set of credentials.
+        entity_id: str
+            ID of the related Entity
+        entity_type: KeyValueEntityType
+            type of the related Entity
+        name: str
+            name of the Key-Value
 
         Returns
         -------
-        credential : Credential
-            the created credential.
+        List[KeyValue]
+            a list of Key-Values
 
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.create_oauth(
-            ...     name='my_oauth_cred',
-            ...     token='XXX',
-            ...     refresh_token='YYY',
-            ... )
-            >>> cred
-            Credential('5e429d6ecf8a5f36c5693e03', 'my_oauth_cred', 'oauth'),
-        """
-        payload = {
-            "name": name,
-            "credentialType": "oauth",
-            "token": token,
-            "refreshToken": refresh_token,
-            "description": description,
-        }
-        return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status
+        datarobot.errors.ServerError
+            if the server responded with 5xx status
+        """
+        data = unpaginate(
+            cls._path,
+            {"entityId": entity_id, "entityType": entity_type.value, "name": name},
+            cls._client,
+        )
+        kv_data = next(data, None)
+        if not kv_data:
+            return None
+        return cls.from_server_data(kv_data)
 
     @classmethod
-    def create_s3(
+    def create(
         cls,
+        entity_id: str,
+        entity_type: KeyValueEntityType,
         name: str,
-        aws_access_key_id: Optional[str] = None,
-        aws_secret_access_key: Optional[str] = None,
-        aws_session_token: Optional[str] = None,
+        category: KeyValueCategory,
+        value_type: KeyValueType,
+        value: Optional[Union[str, float, bool]] = None,
         description: Optional[str] = None,
-    ) -> Credential:
-        """
-        Creates the S3 credentials.
+    ) -> KeyValue:
+        """Create a Key-Value.
+
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        name : str
-            the name to use for this set of credentials.
-        aws_access_key_id : str, optional
-            the AWS access key id.
-        aws_secret_access_key : str, optional
-            the AWS secret access key.
-        aws_session_token : str, optional
-            the AWS session token.
-        description : str, optional
-            the description to use for this set of credentials.
+        entity_id: str
+            ID of the associated resource
+        entity_type: KeyValueEntityType
+            type of the associated resource
+        name: str
+            name of the Key-Value. Cannot contain: { } ; |
+        category: KeyValueCategory
+            category of the Key-Value
+        value_type: KeyValueType
+            type of the Key-Value value
+        value: Optional[Union[str, float, bool]]
+            value of Key-Value
+        description: Optional[str]
+            description of the Key-Value
 
         Returns
         -------
-        credential : Credential
-            the created credential.
+        KeyValue
+            created Key-Value
 
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.create_s3(
-            ...     name='my_s3_cred',
-            ...     aws_access_key_id='XXX',
-            ...     aws_secret_access_key='YYY',
-            ...     aws_session_token='ZZZ',
-            ... )
-            >>> cred
-            Credential('5e429d6ecf8a5f36c5693e03', 'my_s3_cred', 's3'),
-        """
-        payload = {
-            "name": name,
-            "credentialType": "s3",
-            "awsAccessKeyId": aws_access_key_id,
-            "awsSecretAccessKey": aws_secret_access_key,
-            "awsSessionToken": aws_session_token,
-            "description": description,
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status.
+        datarobot.errors.ServerError
+            if the server responded with 5xx status.
+        """
+        value_keys = {
+            KeyValueType.NUMERIC: "numericValue",
+            KeyValueType.BOOLEAN: "booleanValue",
         }
-        return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
+        value_key = value_keys.get(value_type, "value")
 
-    @classmethod
-    def create_azure(
-        cls,
-        name: str,
-        azure_connection_string: str,
+        response = cls._client.post(
+            cls._path,
+            data={
+                "entityId": entity_id,
+                "entityType": entity_type.value,
+                "name": name,
+                "category": category.value,
+                "value_type": value_type.value,
+                value_key: value,
+                "description": description,
+            },
+        )
+
+        return cls.get(response.json()["id"])
+
+    def update(
+        self,
+        entity_id: Optional[str] = None,
+        entity_type: Optional[KeyValueEntityType] = None,
+        name: Optional[str] = None,
+        category: Optional[KeyValueCategory] = None,
+        value_type: Optional[KeyValueType] = None,
+        value: Optional[Union[str, float, bool]] = None,
         description: Optional[str] = None,
-    ) -> Credential:
-        """
-        Creates the Azure storage credentials.
+        comment: Optional[str] = None,
+    ) -> None:
+        """Update Key-Value.
+
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        name : str
-            the name to use for this set of credentials.
-        azure_connection_string : str
-            the Azure connection string.
-        description : str, optional
-            the description to use for this set of credentials.
-
-        Returns
-        -------
-        credential : Credential
-            the created credential.
-
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.create_azure(
-            ...     name='my_azure_cred',
-            ...     azure_connection_string='XXX',
-            ... )
-            >>> cred
-            Credential('5e429d6ecf8a5f36c5693e03', 'my_azure_cred', 'azure'),
+        entity_id: Optional[str]
+            ID of the associated resource
+        entity_type: Optional[KeyValueEntityType]
+            type of the associated resource
+        name: Optional[str]
+            name of the Key-Value. Cannot contain: { } ; |
+        category: Optional[KeyValueCategory]
+            category of the Key-Value
+        value_type: Optional[KeyValueType]
+            type of the Key-Value value
+        value: Optional[[Union[str, float, bool]]
+            value of Key-Value
+        description: Optional[str]
+            description of the Key-Value
+        comment: Optional[str]
+            user comment explaining the change
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status.
+        datarobot.errors.ServerError
+            if the server responded with 5xx status.
         """
         payload = {
-            "name": name,
-            "credentialType": "azure",
-            "azureConnectionString": azure_connection_string,
-            "description": description,
+            "entityId": entity_id if entity_id is not None else self.entity_id,
+            "entityType": entity_type.value if entity_type is not None else self.entity_type.value,
+            "name": name if name is not None else self.name,
+            "category": category.value if category is not None else self.category.value,
+            "valueType": value_type.value if value_type is not None else self.value_type.value,
+            "value": self.value
+            if value is None
+            else None,  # backend expects `value` to be always provided
         }
-        return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
+        if value is not None:
+            value_keys = {
+                KeyValueType.NUMERIC: "numericValue",
+                KeyValueType.BOOLEAN: "booleanValue",
+            }
+            value_key = value_keys.get(value_type if value_type else self.value_type, "value")
+            payload[value_key] = value  # type: ignore[assignment]
+        if description is not None:
+            payload["description"] = description
+        if comment is not None:
+            payload["comment"] = comment
 
-    def __repr__(self) -> str:
-        return "{}('{}', '{}', '{}')".format(
-            self.__class__.__name__,
-            self.credential_id,
-            self.name,
-            self.credential_type,
-        )
+        response = self._client.patch(self._key_value_path(self.id), data=payload)
 
-    @classmethod
-    def create_gcp(
-        cls,
-        name: str,
-        gcp_key: Optional[Union[str, Dict[str, str]]] = None,
-        description: Optional[str] = None,
-    ) -> Credential:
-        """
-        Creates the GCP credentials.
+        data = response.json()
+        new_version = self.from_server_data(data)
+        self._update_values(new_version)
 
-        Parameters
-        ----------
-        name : str
-            the name to use for this set of credentials.
-        gcp_key : str | dict
-            the GCP key in json format or parsed as dict.
-        description : str, optional
-            the description to use for this set of credentials.
+    def refresh(self) -> None:
+        """Update Key-Value with the latest data from server.
 
-        Returns
-        -------
-        credential : Credential
-            the created credential.
+        .. versionadded:: v3.4
 
-        Examples
-        --------
-        .. code-block:: python
-
-            >>> import datarobot as dr
-            >>> cred = dr.Credential.create_gcp(
-            ...     name='my_gcp_cred',
-            ...     gcp_key='XXX',
-            ... )
-            >>> cred
-            Credential('5e429d6ecf8a5f36c5693e03', 'my_gcp_cred', 'gcp'),
+        Raises
+        ------
+        datarobot.errors.ClientError
+            if the server responded with 4xx status
+        datarobot.errors.ServerError
+            if the server responded with 5xx status
         """
 
-        if isinstance(gcp_key, str):
-            try:
-                gcp_key = json.loads(gcp_key)
-            except ValueError as e:
-                raise ValueError(f"Could not parse gcp_key: {e}")
-
-        payload = {
-            "name": name,
-            "credentialType": "gcp",
-            "gcpKey": rawdict(gcp_key),  # type: ignore[arg-type]
-            "description": description,
-        }
-        return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
+        new_object = self.get(self.id)
+        self._update_values(new_object)
 
-    def update(
-        self, name: Optional[str] = None, description: Optional[str] = None, **kwargs: Any
-    ) -> None:
-        """Update the credential values of an existing credential. Updates this object in place.
+    def delete(self) -> None:
+        """Delete Key-Value.
 
-        .. versionadded:: v3.2
+        .. versionadded:: v3.4
 
-        Parameters
-        ----------
-        name : str
-            The name to use for this set of credentials.
-        description : str, optional
-            The description to use for this set of credentials; if omitted, and name is not
-            omitted, then it clears any previous description for that name.
-        kwargs : Keyword arguments specific to the given credential_type that should be updated.
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
         """
-        if name is not None:
-            kwargs["name"] = name
-        if description is not None:
-            kwargs["description"] = description
+        path = self._key_value_path(self.id)
+        self._client.delete(path)
 
-        self._client.patch(f"{self._path}{self.credential_id}/", data=kwargs)
-
-        if name is not None:
-            self.name = name
-        if description is not None:
-            self.description = description
+    def get_value(self) -> Union[str, float, bool]:
+        """Get a value of Key-Value.
 
+        .. versionadded:: v3.4
 
-BasicCredentialsSchema = t.Dict(
-    {
-        t.Key("credentialType"): t.Atom("basic"),
-        t.Key("user"): String(),
-        t.Key("password"): String(),
-    }
-).allow_extra("*")
-
-S3CredentialsSchema = t.Dict(
-    {
-        t.Key("credentialType"): t.Atom("s3"),
-        t.Key("awsAccessKeyId", optional=True): String(),
-        t.Key("awsSecretAccessKey", optional=True): String(),
-        t.Key("awsSessionToken", optional=True): String(),
-    }
-).allow_extra("*")
-
-OauthCredentialsSchema = t.Dict(
-    {
-        t.Key("credentialType"): t.Atom("oauth"),
-        t.Key("oauthRefreshToken"): String(),
-        t.Key("oauthClientId", optional=True): String(),
-        t.Key("oauthClientSecret", optional=True): String(),
-        t.Key("oauthAccessToken", optional=True): String(),
-    }
-).allow_extra("*")
-
-AnyCredentialsSchema = t.Dict({t.Key("credentialType"): String()}).allow_extra("*")
-
-CredentialDataSchema = t.Or(
-    BasicCredentialsSchema, S3CredentialsSchema, OauthCredentialsSchema, AnyCredentialsSchema
-)
+        Returns
+        -------
+        Union[str, float, boolean]
+            value depending on the value type
+        """
+        if self.value_type == KeyValueType.NUMERIC:
+            return self.numeric_value
+        elif self.value_type == KeyValueType.BOOLEAN:
+            return self.boolean_value
+        else:
+            return self.value
```

### Comparing `datarobot-3.3.2/datarobot/models/custom_model.py` & `datarobot-3.4.0/datarobot/models/custom_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     _converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("name"): String(),
             t.Key("description"): String(allow_blank=True),
             t.Key("supports_binary_classification", optional=True, default=False): t.Bool(),
             t.Key("supports_regression", optional=True, default=False): t.Bool(),
+            t.Key("supports_textgeneration", optional=True, default=False): t.Bool(),
             t.Key("latest_version", optional=True, default=None): t.Or(
                 CustomModelVersion.schema, t.Null()
             ),
             t.Key("deployments_count", optional=True, default=None): Int(),
             t.Key("created_by"): String(),
             t.Key("updated") >> "updated_at": String(),
             t.Key("created") >> "created_at": String(),
@@ -62,47 +63,57 @@
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
         id: str,
         name: str,
         description: str,
         supports_binary_classification: bool,
         supports_regression: bool,
+        supports_textgeneration: bool,
         latest_version: CustomModelVersion,
         deployments_count: int,
         created_by: str,
         updated_at: str,
         created_at: str,
         target_type: str,
     ) -> None:
         self.id = id
         self.name = name
         self.description = description
 
         self.target_type = target_type
-        if supports_binary_classification and supports_regression:
+        if supports_binary_classification + supports_regression + supports_textgeneration > 1:
             raise ValueError("Model should support only 1 target type")
 
         if not target_type:
             if supports_binary_classification:
                 self.target_type = CUSTOM_MODEL_TARGET_TYPE.BINARY
             elif supports_regression:
                 self.target_type = CUSTOM_MODEL_TARGET_TYPE.REGRESSION
+            elif supports_textgeneration:
+                self.target_type = CUSTOM_MODEL_TARGET_TYPE.TEXT_GENERATION
             else:
                 raise ValueError("Target type must be provided")
         else:
             if target_type != CUSTOM_MODEL_TARGET_TYPE.BINARY and supports_binary_classification:
                 raise ValueError(
                     "Cannot specify both target_type {} and "
                     "supports_binary_classification.".format(target_type)
                 )
             elif target_type != CUSTOM_MODEL_TARGET_TYPE.REGRESSION and supports_regression:
                 raise ValueError(
                     "Cannot specify both target_type {} and "
                     "supports_regression.".format(target_type)
                 )
+            elif (
+                target_type != CUSTOM_MODEL_TARGET_TYPE.TEXT_GENERATION and supports_textgeneration
+            ):
+                raise ValueError(
+                    "Cannot specify both target_type {} and "
+                    "supports_text_generation.".format(target_type)
+                )
 
         self.latest_version = CustomModelVersion(**latest_version) if latest_version else None  # type: ignore[arg-type]
         self.deployments_count = deployments_count
         self.created_by = created_by
         self.updated_at = updated_at
         self.created_at = created_at
 
@@ -384,15 +395,15 @@
         Can be "python", "r", "java" or "other".
     description: str
         The description of the custom inference model.
     target_type: datarobot.TARGET_TYPE
         Target type of the custom inference model.
         Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
         `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`,
-        `datarobot.TARGET_TYPE.ANOMALY`]
+        `datarobot.TARGET_TYPE.ANOMALY`, `datarobot.TARGET_TYPE.TEXT_GENERATION`]
     target_name: str, optional
         Target feature name.
         It is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED`
         or `datarobot.TARGET_TYPE.ANOMALY` target type.
     latest_version: datarobot.CustomModelVersion or None
         The latest version of the custom model if the model has a latest version.
     deployments_count: int
@@ -614,15 +625,16 @@
         Parameters
         ----------
         name: str
             Name of the custom inference model.
         target_type: datarobot.TARGET_TYPE
             Target type of the custom inference model.
             Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
-            `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`]
+            `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`,
+            `datarobot.TARGET_TYPE.TEXT_GENERATION`]
         target_name: str, optional
             Target feature name.
             It is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED` target type.
         language: str, optional
             Programming language of the custom learning model.
         description: str, optional
             Description of the custom learning model.
@@ -817,15 +829,15 @@
         datarobot.errors.ServerError
             If the server responded with 5xx status.
         """
         super().delete()
 
     @deprecated(
         deprecated_since_version="v3.2",
-        will_remove_version="v3.4",
+        will_remove_version="v3.5",
         message="Please use training data assignment on the model version level: "
         "CustomModelVersion.create_from_previous or CustomModelVersion.create_clean",
     )
     def assign_training_data(
         self,
         dataset_id: str,
         partition_column: Optional[str] = None,
@@ -834,20 +846,20 @@
         """Assign training data to the custom inference model.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         dataset_id: str
-            The id of the training dataset to be assigned.
+            The ID of the training dataset to be assigned.
         partition_column: str, optional
-            Name of a partition column in the training dataset.
+            The name of a partition column in the training dataset.
         max_wait: int, optional
-            Max time to wait for a training data assignment.
-            If set to None - method will return without waiting.
+            The max time to wait for a training data assignment.
+            If set to None, then method will return without waiting.
             Defaults to 10 min.
 
         Raises
         ------
         datarobot.errors.ClientError
             If the server responded with 4xx status
         datarobot.errors.ServerError
```

### Comparing `datarobot-3.3.2/datarobot/models/custom_model_test.py` & `datarobot-3.4.0/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/custom_model_version.py` & `datarobot-3.4.0/datarobot/models/custom_model_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
 from datarobot.errors import InvalidUsageError, TrainingDataAssignmentError
 from datarobot.models.api_object import APIObject, ServerDataType
 from datarobot.models.job import filter_feature_impact_result
+from datarobot.models.runtime_parameters import RuntimeParameter, RuntimeParameterValue
 from datarobot.models.validators import custom_model_feature_impact_trafaret
 from datarobot.utils import camelize
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution, wait_for_custom_resolution
 
 
 class RequiredMetadataValue(APIObject):
@@ -566,14 +567,15 @@
             t.Key("dependencies", optional=True): t.List(CustomDependency.schema),
             t.Key("network_egress_policy", optional=True): t.Enum(*NETWORK_EGRESS_POLICY.ALL),
             t.Key("maximum_memory", optional=True): Int(),
             t.Key("replicas", optional=True): Int(),
             t.Key("required_metadata_values", optional=True): t.List(RequiredMetadataValue.schema),
             t.Key("training_data", optional=True): t.Or(TrainingData.schema, t.Null()),
             t.Key("holdout_data", optional=True): t.Or(HoldoutData.schema, t.Null()),
+            t.Key("runtime_parameters", optional=True): t.List(RuntimeParameter.schema),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
     def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
@@ -597,14 +599,15 @@
         dependencies: Optional[List[CustomDependency]] = None,
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
         maximum_memory: Optional[int] = None,
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_data: Optional[Mapping[str, Any]] = None,
         holdout_data: Optional[Mapping[str, Any]] = None,
+        runtime_parameters: Optional[List[RuntimeParameter]] = None,
     ) -> None:
         self.id = id
         self.custom_model_id = custom_model_id
         self.version_minor = version_minor
         self.version_major = version_major
         self.is_frozen = is_frozen
         self.items = [CustomModelFileItem(**item) for item in items]  # type: ignore[arg-type]
@@ -620,14 +623,19 @@
         self.required_metadata_values = (
             [RequiredMetadataValue.from_server_data(val) for val in required_metadata_values]  # type: ignore[arg-type]
             if required_metadata_values
             else None
         )
         self.training_data = TrainingData(**training_data) if training_data else None
         self.holdout_data = HoldoutData(**holdout_data) if holdout_data else None
+        self.runtime_parameters = (
+            [RuntimeParameter(**param) for param in runtime_parameters]  # type: ignore[arg-type]
+            if runtime_parameters
+            else None
+        )
 
     @classmethod
     def from_server_data(
         cls, data: ServerDataType, keep_attrs: Optional[Iterable[str]] = None
     ) -> CustomModelVersion:
         initial = super().from_server_data(data, keep_attrs)
         # from_server_data will make the keys in requiredMetadata lowercase,
@@ -635,50 +643,61 @@
         initial.required_metadata = data.get("requiredMetadata")  # type: ignore[union-attr]
         return initial
 
     @classmethod
     def create_clean(
         cls,
         custom_model_id: str,
-        base_environment_id: str,
-        is_major_update: bool = True,
+        base_environment_id: Optional[str] = None,
+        is_major_update: Optional[bool] = True,
         folder_path: Optional[str] = None,
         files: Optional[List[Tuple[str, str]]] = None,
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
         maximum_memory: Optional[int] = None,
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_dataset_id: Optional[str] = None,
         partition_column: Optional[str] = None,
         holdout_dataset_id: Optional[str] = None,
         keep_training_holdout_data: Optional[bool] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
+        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
+        base_environment_version_id: Optional[str] = None,
     ) -> CustomModelVersion:
         """Create a custom model version without files from previous versions.
 
            Create a version with training or holdout data:
            If training/holdout data related parameters are provided,
            the training data is assigned asynchronously.
            In this case:
            * if max_wait is not None, the function returns once the job is finished.
            * if max_wait is None, the function returns immediately. Progress can be polled by the user (see examples).
 
            If training data assignment fails, new version is still created,
-           but it is not allowed to create a model package for the model version and to deploy it.
+           but it is not allowed to create a model package (version) for the model version and to deploy it.
            To check for training data assignment error, check version.training_data.assignment_error["message"].
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
             The ID of the custom model.
         base_environment_id: str
-            The ID of the base environment to use with the custom model version.
-        is_major_update: bool
+            The base environment to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+        base_environment_version_id: str
+            The base environment version ID to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+            If not specified: in case previous model versions exist, the value from the latest model
+            version is inherited, otherwise, latest successfully built version of the environment
+            specified in "base_environment_id" is used.
+        is_major_update: bool, optional
             The flag defining if a custom model version will be a minor or a major version.
             Default to `True`
         folder_path: str, optional
             The path to a folder containing files to be uploaded.
             Each file in the folder is uploaded under path relative to a folder path.
         files: list, optional
             The list of tuples, where values in each tuple are the local filesystem path and
@@ -717,14 +736,18 @@
             Defaults to True.
             This field is only applicable if the model has training data for versions enabled,
             otherwise the field value will be ignored.
         max_wait: int, optional
             Max time to wait for training data assignment.
             If set to None - method will return without waiting.
             Defaults to 10 minutes.
+        runtime_parameter_values: List[RuntimeParameterValue]
+            Additional parameters to be injected into a model at runtime. The fieldName
+            must match a fieldName that is listed in the runtimeParameterDefinitions section
+            of the model-metadata.yaml file.
 
         Returns
         -------
         CustomModelVersion
             Created custom model version.
 
         Raises
@@ -782,69 +805,82 @@
         if files and not isinstance(files[0], tuple) and isinstance(files[0], str):  # type: ignore[unreachable]
             files = [(filename, os.path.basename(filename)) for filename in files]  # type: ignore[unreachable]
         return cls._create(
             "post",
             custom_model_id,
             is_major_update,
             base_environment_id,
+            base_environment_version_id,
             folder_path,
             files,
             extra_upload_data=None,
             network_egress_policy=network_egress_policy,
             maximum_memory=maximum_memory,
             replicas=replicas,
             required_metadata_values=required_metadata_values,
             training_dataset_id=training_dataset_id,
             partition_column=partition_column,
             holdout_dataset_id=holdout_dataset_id,
             keep_training_holdout_data=keep_training_holdout_data,
             max_wait=max_wait,
+            runtime_parameter_values=runtime_parameter_values,
         )
 
     @classmethod
     def create_from_previous(
         cls,
         custom_model_id: str,
-        base_environment_id: str,
-        is_major_update: bool = True,
+        base_environment_id: Optional[str] = None,
+        is_major_update: Optional[bool] = True,
         folder_path: Optional[str] = None,
         files: Optional[List[Tuple[str, str]]] = None,
         files_to_delete: Optional[List[str]] = None,
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
         maximum_memory: Optional[int] = None,
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_dataset_id: Optional[str] = None,
         partition_column: Optional[str] = None,
         holdout_dataset_id: Optional[str] = None,
         keep_training_holdout_data: Optional[bool] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
+        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
+        base_environment_version_id: Optional[str] = None,
     ) -> CustomModelVersion:
         """Create a custom model version containing files from a previous version.
 
            Create a version with training/holdout data:
            If training/holdout data related parameters are provided,
            the training data is assigned asynchronously.
            In this case:
            * if max_wait is not None, function returns once job is finished.
            * if max_wait is None, function returns immediately, progress can be polled by the user, see examples.
 
            If training data assignment fails, new version is still created,
-           but it is not allowed to create a model package for the model version and to deploy it.
+           but it is not allowed to create a model package (version) for the model version and to deploy it.
            To check for training data assignment error, check version.training_data.assignment_error["message"].
 
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
             The ID of the custom model.
         base_environment_id: str
-            The ID of the base environment to use with the custom model version.
+            The base environment to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+        base_environment_version_id: str
+            The base environment version ID to use with this model version.
+            At least one of "base_environment_id" and "base_environment_version_id" must be provided.
+            If both are specified, the version must belong to the environment.
+            If not specified: in case previous model versions exist, the value from the latest model
+            version is inherited, otherwise, latest successfully built version of the environment
+            specified in "base_environment_id" is used.
         is_major_update: bool, optional
             The flag defining if a custom model version will be a minor or a major version.
             Defaults to `True`.
         folder_path: str, optional
             The path to a folder containing files to be uploaded.
             Each file in the folder is uploaded under path relative to a folder path.
         files: list, optional
@@ -887,14 +923,20 @@
             Defaults to True.
             This field is only applicable if the model has training data for versions enabled,
             otherwise the field value will be ignored.
         max_wait: int, optional
             Max time to wait for training data assignment.
             If set to None - method will return without waiting.
             Defaults to 10 minutes.
+        runtime_parameter_values: List[RuntimeParameterValue]
+            Additional parameters to be injected into the model at runtime. The fieldName
+            must match a fieldName that is listed in the runtimeParameterDefinitions section
+            of the model-metadata.yaml file. This list will be merged with any existing
+            runtime values set from the prior version, so it is possible to specify a `null` value
+            to unset specific parameters and fall back to the defaultValue from the definition.
 
         Returns
         -------
         CustomModelVersion
             created custom model version
 
         Raises
@@ -957,47 +999,51 @@
         else:
             upload_data = None
         return cls._create(
             "patch",
             custom_model_id,
             is_major_update,
             base_environment_id,
+            base_environment_version_id,
             folder_path,
             files,
             upload_data,
             network_egress_policy,
             maximum_memory,
             replicas,
             required_metadata_values=required_metadata_values,
             training_dataset_id=training_dataset_id,
             partition_column=partition_column,
             holdout_dataset_id=holdout_dataset_id,
             keep_training_holdout_data=keep_training_holdout_data,
             max_wait=max_wait,
+            runtime_parameter_values=runtime_parameter_values,
         )
 
     @classmethod
     def _create(
         cls,
         method: str,
         custom_model_id: str,
-        is_major_update: bool,
-        base_environment_id: str,
+        is_major_update: Optional[bool],
+        base_environment_id: Optional[str],
+        base_environment_version_id: Optional[str],
         folder_path: Optional[str],
         files: Optional[List[Tuple[str, str]]],
         extra_upload_data: Optional[List[Tuple[str, Any]]],
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY],
         maximum_memory: Optional[int],
         replicas: Optional[int],
         required_metadata_values: Optional[List[RequiredMetadataValue]],
         training_dataset_id: Optional[str],
         partition_column: Optional[str],
         holdout_dataset_id: Optional[str],
         keep_training_holdout_data: Optional[bool],
         max_wait: Optional[int],
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
     ) -> CustomModelVersion:
         # TODO: pass model object
         """Create a custom model version"""
 
         def _wait_for_training_data_assignment(version: CustomModelVersion) -> None:
             # This check is needed to make sure user explicitly passes new training data.
             # Checking only for `version.training_data.assignment_in_progress` is not enough as it is not known
@@ -1041,16 +1087,20 @@
             if keep_training_holdout_data and (training_dataset_id or holdout_dataset_id):
                 raise InvalidUsageError(
                     "It is not allowed to keep existing training/holdout data and to provide a new ones."
                 )
 
             upload_data: List[Tuple[str, Any]] = [
                 ("isMajorUpdate", str(is_major_update)),
-                ("baseEnvironmentId", base_environment_id),
             ]
+            if base_environment_id:
+                upload_data.append(("baseEnvironmentId", base_environment_id))
+
+            if base_environment_version_id:
+                upload_data.append(("baseEnvironmentVersionId", base_environment_version_id))
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
                     for path in file_paths:
                         file_path = os.path.join(root_path, path)
                         file = stack.enter_context(open(file_path, "rb"))
 
@@ -1106,14 +1156,27 @@
                     hd_payload["partitionColumn"] = partition_column
 
                 if len(hd_payload):
                     upload_data.append(("holdoutData", json.dumps(hd_payload)))
             if keep_training_holdout_data is not None:
                 upload_data.append(("keepTrainingHoldoutData", str(keep_training_holdout_data)))
 
+            if runtime_parameter_values is not None:
+                upload_data.append(
+                    (
+                        "runtimeParameterValues",
+                        json.dumps(
+                            [
+                                {camelize(k): v for k, v in param.to_dict().items()}
+                                for param in runtime_parameter_values
+                            ]
+                        ),
+                    )
+                )
+
             encoder = MultipartEncoder(fields=upload_data)
             headers = {"Content-Type": encoder.content_type}
             response = cls._client.request(method, url, data=encoder, headers=headers)
             new_version = cls.from_server_data(response.json())
 
             _wait_for_training_data_assignment(new_version)
 
@@ -1455,15 +1518,15 @@
         Parameters
         ----------
         custom_model_id : str
             The ID of the associated custom model.
         custom_model_version_id : str
             The ID of the associated custom model version.
         conversion_id :
-            THe ID of a conversion that is in-progress.
+            The ID of a conversion that is in-progress.
 
         Raises
         ------
         datarobot.errors.ClientError
             If the server responded with 4xx status.
         datarobot.errors.ServerError
             If the server responded with 5xx status.
```

### Comparing `datarobot-3.3.2/datarobot/models/custom_task.py` & `datarobot-3.4.0/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/custom_task_version.py` & `datarobot-3.4.0/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/custom_task_version_dependency_build.py` & `datarobot-3.4.0/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/data_engine_query_generator.py` & `datarobot-3.4.0/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/data_slice.py` & `datarobot-3.4.0/datarobot/models/data_slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 
 class DataSlicesOperators(str, enum.Enum):
     EQUAL = "eq"
     CONTAINS = "in"
     LESS_THAN = "<"
     GREATER_THAN = ">"
+    BETWEEN = "between"
+    NOT_BETWEEN = "notBetween"
 
 
 class DataSliceSizeInfo(APIObject):
     """
     Definition of a data slice applied to a source
 
     Attributes
```

### Comparing `datarobot-3.3.2/datarobot/models/data_source.py` & `datarobot-3.4.0/datarobot/models/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,46 +8,49 @@
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
-from typing import cast, Iterable, List, Optional, Type, TYPE_CHECKING, TypeVar
+from typing import cast, Iterable, List, Optional, Type, TYPE_CHECKING, TypeVar, Union
 
 import trafaret as t
 
 from datarobot._compat import Int, String
+from datarobot.enums import DataStoreListTypes, DataStoreTypes
 from datarobot.models.api_object import APIObject
 from datarobot.models.dataset import Dataset
 from datarobot.models.sharing import SharingAccess
 from datarobot.utils.pagination import unpaginate
 
 from ..utils import from_api, parse_time
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.api_object import ServerDataType
 
     class DataSourceParametersPayload(TypedDict, total=False):
         data_store_id: Optional[str]
+        catalog: Optional[str]
         table: Optional[str]
         schema: Optional[str]
         partition_column: Optional[str]
         query: Optional[str]
         fetch_size: Optional[int]
 
 
 TDataSource = TypeVar("TDataSource", bound="DataSource")
 TDataSourceParameters = TypeVar("TDataSourceParameters", bound="DataSourceParameters")
 
 _data_source_params_converter = t.Dict(
     {
         t.Key("data_store_id"): t.Or(String(), t.Null),
+        t.Key("catalog", optional=True): t.Or(String(), t.Null),
         t.Key("table", optional=True): t.Or(String(), t.Null),
         t.Key("schema", optional=True): t.Or(String(), t.Null),
         t.Key("partition_column", optional=True): t.Or(String(), t.Null),
         t.Key("query", optional=True): t.Or(String(), t.Null),
         t.Key("fetch_size", optional=True): t.Or(Int(), t.Null),
     }
 ).ignore_extra("*")
@@ -72,40 +75,44 @@
         optional, a user specified fetch size in the range [1, 20000].
         By default a fetchSize will be assigned to balance throughput and memory usage
     """
 
     def __init__(
         self,
         data_store_id: Optional[str] = None,
+        catalog: Optional[str] = None,
         table: Optional[str] = None,
         schema: Optional[str] = None,
         partition_column: Optional[str] = None,
         query: Optional[str] = None,
         fetch_size: Optional[int] = None,
     ) -> None:
         _data_source_params_converter.check(
             {
                 "data_store_id": data_store_id,
+                "catalog": catalog,
                 "table": table,
                 "schema": schema,
                 "partition_column": partition_column,
                 "query": query,
                 "fetch_size": fetch_size,
             }
         )
         self.data_store_id = data_store_id
+        self.catalog = catalog
         self.table = table
         self.schema = schema
         self.partition_column = partition_column
         self.query = query
         self.fetch_size = fetch_size
 
     def collect_payload(self) -> DataSourceParametersPayload:
         return {
             "data_store_id": self.data_store_id,
+            "catalog": self.catalog,
             "table": self.table,
             "schema": self.schema,
             "partition_column": self.partition_column,
             "query": self.query,
             "fetch_size": self.fetch_size,
         }
 
@@ -174,33 +181,41 @@
         self.canonical_name = canonical_name
         self._creator = creator
         self._updated = updated
         self.params = params
         self.role = role
 
     @classmethod
-    def list(cls) -> List[DataSource]:
+    def list(cls, typ: Optional[DataStoreListTypes] = None) -> List[DataSource]:
         """
         Returns list of available data sources.
 
+        Parameters
+        ----------
+        typ : DataStoreListTypes
+            If specified, filters by specified datasource type.
+
         Returns
         -------
         data_sources : list of DataSource instances
             contains a list of available data sources.
 
         Examples
         --------
         .. code-block:: python
 
             >>> import datarobot as dr
             >>> data_sources = dr.DataSource.list()
             >>> data_sources
             [DataSource('Diagnostics'), DataSource('Airlines 100mb'), DataSource('Airlines 10mb')]
         """
-        r_data = cls._client.get(cls._path).json()
+        if typ is not None:
+            r_data = cls._client.get(cls._path, params={"type": str(typ)}).json()
+        else:
+            r_data = cls._client.get(cls._path).json()
         return [cls.from_server_data(item) for item in r_data["data"]]
 
     @classmethod
     def get(cls: Type[TDataSource], data_source_id: str) -> TDataSource:
         """
         Gets the data source.
 
@@ -224,24 +239,24 @@
             DataSource('Diagnostics')
         """
         return cls.from_location(f"{cls._path}{data_source_id}/")
 
     @classmethod
     def create(
         cls: Type[TDataSource],
-        data_source_type: str,
+        data_source_type: Union[str, DataStoreTypes],
         canonical_name: str,
         params: DataSourceParameters,
     ) -> TDataSource:
         """
         Creates the data source.
 
         Parameters
         ----------
-        data_source_type : str
+        data_source_type : str or DataStoreTypes
             the type of data source.
         canonical_name : str
             the user-friendly name of the data source.
         params : DataSourceParameters
             a list specifying data source parameters.
 
         Returns
@@ -263,15 +278,15 @@
             ...     canonical_name='airlines stats after 1995',
             ...     params=params
             ... )
             >>> data_source
             DataSource('airlines stats after 1995')
         """
         payload = {
-            "type": data_source_type,
+            "type": str(data_source_type),
             "canonicalName": canonical_name,
             "params": params.collect_payload(),
         }
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
     def update(
         self, canonical_name: Optional[str] = None, params: Optional[DataSourceParameters] = None
```

### Comparing `datarobot-3.3.2/datarobot/models/data_store.py` & `datarobot-3.4.0/datarobot/models/data_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 import trafaret as t
 
 from datarobot._compat import String
-from datarobot.enums import DATA_STORE_TABLE_TYPE
+from datarobot.enums import DATA_STORE_TABLE_TYPE, DataStoreListTypes, DataStoreTypes
 from datarobot.models.api_object import APIObject, ServerDataType
 from datarobot.models.credential import CredentialDataSchema
 from datarobot.models.sharing import SharingAccess, SharingRole
 from datarobot.utils import deprecated, deprecation_warning, from_api, parse_time, to_api
 from datarobot.utils.pagination import unpaginate
 
 field_converter = t.Dict(
@@ -138,15 +138,15 @@
         self.canonical_name = canonical_name
         self._creator = creator
         self._updated = updated
         self.params = params
         self.role = role
 
     @classmethod
-    def list(cls, typ: Optional[str] = None) -> List[DataStore]:
+    def list(cls, typ: Optional[Union[str, DataStoreListTypes]] = None) -> List[DataStore]:
         """
         Returns list of available data stores.
 
         Parameters
         ----------
         typ : str
             If specified, filters by specified data store type.
@@ -162,15 +162,15 @@
 
             >>> import datarobot as dr
             >>> data_stores = dr.DataStore.list()
             >>> data_stores
             [DataStore('Demo'), DataStore('Airlines')]
         """
         if typ is not None:
-            r_data = cls._client.get(cls._path, params={"type": typ}).json()
+            r_data = cls._client.get(cls._path, params={"type": str(typ)}).json()
         else:
             r_data = cls._client.get(cls._path).json()
         return [cls.from_server_data(item) for item in r_data["data"]]
 
     @classmethod
     def get(cls, data_store_id: str) -> DataStore:
         """
@@ -196,26 +196,26 @@
             DataStore('Demo')
         """
         return cls.from_location(f"{cls._path}{data_store_id}/")
 
     @classmethod
     def create(
         cls,
-        data_store_type: str,
+        data_store_type: Union[str, DataStoreTypes],
         canonical_name: str,
         driver_id: str,
         jdbc_url: Optional[str] = None,
         fields: Optional[List[Dict[str, str]]] = None,
     ) -> DataStore:
         """
         Creates the data store.
 
         Parameters
         ----------
-        data_store_type : str
+        data_store_type : str or DataStoreTypes
             the type of data store.
         canonical_name : str
             the user-friendly name of the data store.
         driver_id : str
             the identifier of the DataDriver.
         jdbc_url : str
             Optional. The full JDBC URL (for example: `jdbc:postgresql://my.dbaddress.org:5432/my_db`).
@@ -238,15 +238,15 @@
             ...     driver_id='5a6af02eb15372000117c040',
             ...     jdbc_url='jdbc:postgresql://my.db.address.org:5432/perftest'
             ... )
             >>> data_store
             DataStore('Demo DB')
         """
         payload = {
-            "type": data_store_type,
+            "type": str(data_store_type),
             "canonicalName": canonical_name,
             "params": DataStoreParameters(
                 driver_id=driver_id, jdbc_url=jdbc_url, fields=fields
             ).collect_payload(),
         }
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
```

### Comparing `datarobot-3.3.2/datarobot/models/dataset.py` & `datarobot-3.4.0/datarobot/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         t.Key("created_by", optional=True): t.Or(String, t.Null),
         t.Key("data_persisted", optional=True): t.Bool,
         t.Key("is_data_engine_eligible"): t.Bool,
         t.Key("is_latest_version"): t.Bool,
         t.Key("is_snapshot"): t.Bool,
         t.Key("dataset_size", optional=True) >> "size": Int,
         t.Key("row_count", optional=True): Int,
+        t.Key("sample_size", optional=True): t.Or(
+            t.Dict({t.Key("type"): String, t.Key("value"): Int}), t.Null
+        ),
         t.Key("processing_state"): String,
     }
 )
 
 
 class Dataset(APIObject, BrowserMixin):
     """Represents a Dataset returned from the api/v2/datasets/ endpoints.
@@ -105,14 +108,18 @@
     processing_state: string
         Current ingestion process state of
         the dataset
     row_count: int, optional
         The number of rows in the dataset.
     size: int, optional
         The size of the dataset as a CSV in bytes.
+    sample_size: dict, optional
+        The size of data fetched during dataset registration. For example, to fetch the first 95
+        rows,  the sample_size value is {'type': 'rows', 'value': 95}.
+        Currently only 'rows' type is supported.
     """
 
     _converter = _base_dataset_schema.allow_extra("*")
     _path = "datasets/"
 
     def __init__(
         self,
@@ -126,14 +133,15 @@
         is_snapshot: bool,
         processing_state: str,
         created_by: Optional[str] = None,
         data_persisted: Optional[bool] = None,
         size: Optional[int] = None,
         row_count: Optional[int] = None,
         recipe_id: Optional[str] = None,
+        sample_size: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.id = dataset_id
         self.version_id = version_id
         self.name = name
         self.data_persisted = data_persisted
         self.categories = categories[:]
         self.created_at = created_at
@@ -141,14 +149,15 @@
         self.is_data_engine_eligible = is_data_engine_eligible
         self.is_latest_version = is_latest_version
         self.is_snapshot = is_snapshot
         self.size = size
         self.row_count = row_count
         self.processing_state = processing_state
         self.recipe_id = recipe_id
+        self.sample_size = sample_size
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name={self.name!r}, id={self.id!r})"
 
     def get_uri(self) -> str:
         """
         Returns
@@ -351,14 +360,15 @@
     @add_to_use_case(allow_multiple=True)
     def create_from_url(
         cls: Type[TDataset],
         url: str,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
         categories: Optional[List[str]] = None,
+        sample_size: Optional[Dict[str, Any]] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TDataset:
         """
         A blocking call that creates a new Dataset from data stored at a url.
         Returns when the dataset has been successfully uploaded and processed.
 
         Parameters
@@ -377,14 +387,19 @@
             (which includes data statistics like min/max/median/mean, histogram, etc.). If false,
             will not enforce saving data. The data schema (feature names and types) still will be
             available. Specifying this parameter to false and `doSnapshot` to true will result in
             an error.
         categories: list[string], optional
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
+        sample_size: dict, optional
+            The size of data fetched during dataset registration.
+            For example, to fetch the first 95 rows,  the sample_size value would be:
+            {'type': 'rows', 'value': 95}.
+            Currently only 'rows' type is supported.
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful.
         use_cases: list[UseCase] | UseCase | list[string] | string, optional
             A list of UseCase objects, UseCase object,
             list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
@@ -393,14 +408,15 @@
             The Dataset created from the uploaded data
         """
         base_data = {
             "url": url,
             "do_snapshot": do_snapshot,
             "persist_data_after_ingestion": persist_data_after_ingestion,
             "categories": categories,
+            "sample_size": sample_size,
         }
         data = _remove_empty_params(base_data)
         upload_url = f"{cls._path}fromURL/"
         response = cls._client.post(upload_url, data=data)
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
@@ -456,14 +472,15 @@
         password: Optional[str] = None,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
         categories: Optional[List[str]] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
         credential_data: Optional[Dict[str, str]] = None,
+        sample_size: Optional[Dict[str, Any]] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TDataset:
         """
         A blocking call that creates a new Dataset from data stored at a DataSource.
         Returns when the dataset has been successfully uploaded and processed.
 
         .. versionadded:: v2.22
@@ -499,14 +516,19 @@
             will become optional.
         use_kerberos: bool, optional
             If unset, uses the server default: False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
+        sample_size: dict, optional
+            The size of data fetched during dataset registration.
+            For example, to fetch the first 95 rows,  the sample_size value would be:
+            {'type': 'rows', 'value': 95}.
+            Currently only 'rows' type is supported.
         max_wait: int, optional
             Time in seconds after which project creation is considered unsuccessful.
         use_cases: list[UseCase] | UseCase | list[string] | string, optional
             A list of UseCase objects, UseCase object,
             list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
@@ -520,14 +542,15 @@
             "password": password,
             "do_snapshot": do_snapshot,
             "persist_data_after_ingestion": persist_data_after_ingestion,
             "categories": categories,
             "credential_id": credential_id,
             "use_kerberos": use_kerberos,
             "credential_data": credential_data,
+            "sample_size": sample_size,
         }
         data = _remove_empty_params(base_data)
 
         if "credential_data" in data:
             data["credential_data"] = CredentialDataSchema(data["credential_data"])
 
         upload_url = f"{cls._path}fromDataSource/"
@@ -1042,18 +1065,29 @@
         """
         if low_memory:
             with tempfile.NamedTemporaryFile(suffix=".csv") as csv_file:
                 iter = self._client.get(f"{self._path}{self.id}/file/", stream=True)
                 with open(csv_file.name, "wb") as out:
                     for chunk in iter.iter_content(1000):
                         out.write(chunk)
-                return pd.read_csv(csv_file.name)
+                try:
+                    return pd.read_csv(csv_file.name)
+                except Exception:
+                    # different versions of python and pandas
+                    # raise different exceptions
+                    with open(csv_file.name, "rb") as inp:
+                        dat = inp.read(4)
+                    if dat == b"PAR1":
+                        return pd.read_parquet(csv_file.name)
+                    raise
         else:
             raw_bytes = BytesIO()
             self.get_file(filelike=raw_bytes)
+            if raw_bytes.getvalue().startswith(b"PAR1"):
+                return pd.read_parquet(raw_bytes)
             data = StringIO(raw_bytes.getvalue().decode())
             return pd.read_csv(data)
 
     def get_projects(self) -> List[ProjectLocation]:
         """
         Retrieves the Dataset's projects as ProjectLocation named tuples.
 
@@ -1513,14 +1547,18 @@
     uri: string
         the uri to datasource like:
         - 'file_name.csv'
         - 'jdbc:DATA_SOURCE_GIVEN_NAME/SCHEMA.TABLE_NAME'
         - 'jdbc:DATA_SOURCE_GIVEN_NAME/<query>' - for `query` based datasources
         - 'https://s3.amazonaws.com/datarobot_test/kickcars-sample-200.csv'
         - etc.
+    sample_size: dict, optional
+        The size of data fetched during dataset registration. For example, to fetch the first 95
+        rows,  the sample_size value is {'type': 'rows', 'value': 95}.
+        Currently only 'rows' type is supported.
     """
 
     _extra_fields = t.Dict(
         {
             t.Key("data_engine_query_id", optional=True): String,
             t.Key("data_source_id", optional=True): String,
             t.Key("data_source_type"): String(allow_blank=True),
@@ -1571,14 +1609,15 @@
         feature_count: Optional[int] = None,
         feature_count_by_type: Optional[List[FeatureTypeCount]] = None,
         row_count: Optional[int] = None,
         size: Optional[int] = None,
         tags: Optional[List[str]] = None,
         recipe_id: Optional[str] = None,
         is_wrangling_eligible: Optional[bool] = None,
+        sample_size: Optional[Dict[str, Any]] = None,
     ):
         self.dataset_id = dataset_id
         self.version_id = version_id
         self.categories = categories
         self.created_by = created_by
         self.created_at = created_at
         self.data_source_type = data_source_type
@@ -1600,14 +1639,15 @@
         self.feature_count_by_type = feature_count_by_type
         self.processing_state = processing_state
         self.row_count = row_count
         self.size = size
         self.tags = tags
         self.recipe_id = recipe_id
         self.is_wrangling_eligible = is_wrangling_eligible
+        self.sample_size = sample_size
 
     @classmethod
     def get(cls: Type[TDatasetDetails], dataset_id: str) -> TDatasetDetails:
         """
         Get details for a Dataset from the server
 
         Parameters
```

### Comparing `datarobot-3.3.2/datarobot/models/datetime_trend_plots.py` & `datarobot-3.4.0/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/deployment/accuracy.py` & `datarobot-3.4.0/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/deployment/bias_and_fairness.py` & `datarobot-3.4.0/datarobot/models/deployment/bias_and_fairness.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     protected_feature : str
         name of protected feature
     fairnessThreshold : float
         threshold used to compute fairness results
     modelId : str
         model id for which fairness is computed
     modelPackageId : str
-        model package id for which fairness is computed
+        model package (version) id for which fairness is computed
     favorableTargetOutcome : bool
         preferable class of the target
     """
 
     _path = "deployments/{}/fairnessScoresOverTime/"
     _period = t.Dict(
         {
```

### Comparing `datarobot-3.3.2/datarobot/models/deployment/data_drift.py` & `datarobot-3.4.0/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/deployment/deployment.py` & `datarobot-3.4.0/datarobot/models/deployment/deployment.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,49 +12,59 @@
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 from collections import defaultdict
 from datetime import datetime
 from io import IOBase
 from typing import Any, cast, Dict, List, Optional, Tuple, Type, TYPE_CHECKING, TypeVar, Union
+import warnings
 
 import dateutil
 import pandas as pd
 import pytz
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.enums import (
     ACCURACY_METRIC,
     BUCKET_SIZE,
     DEFAULT_MAX_WAIT,
+    ExportStatus,
     FileLocationType,
     LocalSourceType,
 )
-from datarobot.errors import InvalidUsageError
+from datarobot.errors import ClientError, InvalidUsageError
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
 from datarobot.models.custom_model_version import CustomModelVersion
 from datarobot.models.deployment.accuracy import (
     Accuracy,
     AccuracyOverTime,
     PredictionsVsActualsOverTime,
 )
 from datarobot.models.deployment.bias_and_fairness import FairnessScoresOverTime
+from datarobot.models.deployment.challenger import Challenger
+from datarobot.models.deployment.champion_model_package import ChampionModelPackage
 from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
+from datarobot.models.deployment.data_exports import (
+    ActualsDataExport,
+    PredictionDataExport,
+    TrainingDataExport,
+)
 from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
 from datarobot.models.status_check_job import StatusCheckJob
-from datarobot.utils import deprecated, from_api, get_id_from_location
+from datarobot.models.types import Schedule
+from datarobot.utils import deprecated, deprecation_warning, from_api, get_id_from_location, to_api
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.waiters import wait_for_async_resolution
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
@@ -80,14 +90,19 @@
 
     class ModelDict(TypedDict):
         id: Optional[str]
         type: Optional[str]
         target_name: Optional[str]
         project_id: Optional[str]
 
+    class ModelPackageDict(TypedDict):
+        id: Optional[str]
+        name: Optional[str]
+        registered_model_id: Optional[str]
+
     class PredictionUsage(TypedDict):
         daily_rates: Optional[List[float]]
         last_timestamp: Optional[str]
 
     class Health(TypedDict, total=False):
         status: Optional[str]
         message: Optional[str]
@@ -119,14 +134,26 @@
 
     class BiasAndFairnessSettings(TypedDict):
         protected_features: List[str]
         preferable_target_value: bool
         fairness_metric_set: str
         fairness_threshold: float
 
+    class ChallengerReplaySettings(Settings):
+        schedule: Schedule
+
+    class HealthSettings(TypedDict):
+        service: Dict[str, Any]
+        data_drift: Dict[str, Any]
+        accuracy: Dict[str, Any]
+        fairness: Dict[str, Any]
+        custom_metrics: Dict[str, Any]
+        predictions_timeliness: Dict[str, Any]
+        actuals_timeliness: Dict[str, Any]
+
     class Actual(TypedDict):
         association_id: str
         actual_value: Union[str, int, float]
         was_acted_on: Optional[bool]
         timestamp: Union[datetime, str]
 
 
@@ -167,14 +194,16 @@
         * datarobot-key: str. Corresponds the to the ``PredictionServer``'s "snake_cased"
           ``datarobot_key`` parameter that allows you to verify and access the prediction server.
 
     importance : str, optional
         deployment importance
     model : dict
         information on the model of the deployment
+    model_package : dict
+        (New in version v3.4) information on the model package of the deployment
     capabilities : dict
         information on the capabilities of the deployment
     prediction_usage : dict
         information on the prediction usage of the deployment
     permissions : list
         (New in version v2.18) user's permissions on the deployment
     service_health : dict
@@ -205,14 +234,21 @@
         {
             t.Key("id", optional=True): String(),
             t.Key("type", optional=True): String(allow_blank=True),
             t.Key("target_name", optional=True): String(allow_blank=True),
             t.Key("project_id", optional=True): String(allow_blank=True),
         }
     ).allow_extra("*")
+    _model_package_converter = t.Dict(
+        {
+            t.Key("id", optional=True): String(),
+            t.Key("name", optional=True): String(allow_blank=True),
+            t.Key("registered_model_id", optional=True): String(allow_blank=True),
+        }
+    ).allow_extra("*")
     _prediction_usage = t.Dict(
         {
             t.Key("daily_rates", optional=True): t.List(t.Float()),
             t.Key("last_timestamp", optional=True): String >> dateutil.parser.parse,
         }
     ).allow_extra("*")
     _health = t.Dict(
@@ -228,14 +264,15 @@
             t.Key("id"): String(),
             t.Key("label", optional=True): String(allow_blank=True),
             t.Key("description", optional=True): t.Or(String(allow_blank=True), t.Null()),
             t.Key("status", optional=True): t.Or(String(), t.Null()),
             t.Key("default_prediction_server", optional=True): _default_prediction_server_converter,
             t.Key("importance", optional=True): t.Or(String(), t.Null()),
             t.Key("model", optional=True): _model_converter,
+            t.Key("model_package", optional=True): _model_package_converter,
             t.Key("capabilities", optional=True): t.Dict().allow_extra("*"),
             t.Key("prediction_usage", optional=True): _prediction_usage,
             t.Key("permissions", optional=True): t.List(String),
             t.Key("service_health", optional=True): _health,
             t.Key("model_health", optional=True): _health,
             t.Key("accuracy_health", optional=True): _health,
             t.Key("fairness_health", optional=True): _health,
@@ -249,14 +286,15 @@
         self,
         id: str,
         label: Optional[str] = None,
         description: Optional[str] = None,
         status: Optional[str] = None,
         default_prediction_server: Optional[PredictionServer] = None,
         model: Optional[ModelDict] = None,
+        model_package: Optional[ModelPackageDict] = None,
         capabilities: Optional[Dict[str, Any]] = None,
         prediction_usage: Optional[PredictionUsage] = None,
         permissions: Optional[List[str]] = None,
         service_health: Optional[Health] = None,
         model_health: Optional[Health] = None,
         accuracy_health: Optional[Health] = None,
         importance: Optional[str] = None,
@@ -267,14 +305,15 @@
     ) -> None:
         self.id = id
         self.label = label
         self.status = status
         self.description = description
         self.default_prediction_server = default_prediction_server
         self.model = model
+        self.model_package = model_package
         self._capabilities = capabilities
         self.prediction_usage = prediction_usage
         self.permissions = permissions
         self.service_health = service_health
         self.model_health = model_health
         self.accuracy_health = accuracy_health
         self.importance = importance
@@ -554,20 +593,20 @@
         default_prediction_server_id: Optional[str] = None,
         prediction_environment_id: Optional[str] = None,
         importance: Optional[str] = None,
         user_provided_id: Optional[str] = None,
         additional_metadata: Optional[Dict[str, str]] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TDeployment:
-        """Create a deployment from a DataRobot model package.
+        """Create a deployment from a DataRobot model package (version).
 
         Parameters
         ----------
         model_package_id : str
-            The ID of the DataRobot model package to deploy.
+            The ID of the DataRobot model package (version) to deploy.
         label : str
             A human readable label of the deployment.
         description : str, optional
             A human readable description of the deployment.
         default_prediction_server_id : str, optional
             an identifier of a prediction server to be used as the default prediction server
             When working with prediction environments, default prediction server Id should not be provided
@@ -884,15 +923,26 @@
             self._client, response.headers["Location"], max_wait=max_wait
         )
 
         deployment_id = get_id_from_location(deployment_loc)
         deployment = Deployment.get(deployment_id)
         self.status = deployment.status
 
-    def replace_model(self, new_model_id: str, reason: str, max_wait: int = 600) -> None:
+    @deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This method is deprecated, please use 'perform_model_replace' instead.",
+    )
+    def replace_model(
+        self,
+        new_model_id: Optional[str],
+        reason: str,
+        max_wait: int = 600,
+        new_registered_model_version_id: Optional[str] = None,
+    ) -> None:
         """Replace the model used in this deployment. To confirm model replacement eligibility, use
          :meth:`~datarobot.models.Deployment.validate_replacement_model` beforehand.
 
         .. versionadded:: v2.17
 
         Model replacement is an asynchronous process, which means some preparatory work may
         be performed after the initial request is completed. This function will not return until all
@@ -900,24 +950,28 @@
 
         Predictions made against this deployment will start using the new model as soon as the
         request is completed. There will be no interruption for predictions throughout
         the process.
 
         Parameters
         ----------
-        new_model_id : str
+        new_model_id : Optional[str]
             The id of the new model to use. If replacing the deployment's model with a
             CustomInferenceModel, a specific CustomModelVersion ID must be used.
+            If None, new_registered_model_version_id must be specified.
         reason : MODEL_REPLACEMENT_REASON
             The reason for the model replacement. Must be one of 'ACCURACY', 'DATA_DRIFT', 'ERRORS',
             'SCHEDULED_REFRESH', 'SCORING_SPEED', or 'OTHER'. This value will be stored in the model
             history to keep track of why a model was replaced
         max_wait : int, optional
             (new in version 2.22) The maximum time to wait for
             model replacement job to complete before erroring
+        new_registered_model_version_id : Optional[str]
+            (new in version 3.4) The registered model version (model package) ID of the new model to use. Must be
+            passed if new_model_id is None.
 
         Examples
         --------
         .. code-block:: python
 
             from datarobot import Deployment
             from datarobot.enums import MODEL_REPLACEMENT_REASON
@@ -926,23 +980,36 @@
             >>>('5c0a979859b00004ba52e431', 'Decision Tree Classifier (Gini)')
 
             deployment.replace_model('5c0a969859b00004ba52e41b', MODEL_REPLACEMENT_REASON.ACCURACY)
             deployment.model['id'], deployment.model['type']
             >>>('5c0a969859b00004ba52e41b', 'Support Vector Classifier (Linear Kernel)')
         """
 
+        if new_model_id is None and new_registered_model_version_id is None:
+            raise ValueError("Must specify either new_model_id or new_registered_model_version_id.")
+        if new_model_id is not None and new_registered_model_version_id is not None:
+            raise ValueError(
+                "Cannot specify both new_model_id and new_registered_model_version_id."
+            )
+
+        payload = {"reason": reason}
+        if new_model_id is not None:
+            payload["modelId"] = new_model_id
+        if new_registered_model_version_id is not None:
+            payload["modelPackageId"] = new_registered_model_version_id
+
         url = f"{self._path}{self.id}/model/"
-        payload = {"modelId": new_model_id, "reason": reason}
         response = self._client.patch(url, data=payload)
         deployment_loc = wait_for_async_resolution(
             self._client, response.headers["Location"], max_wait=max_wait
         )
         deployment_id = get_id_from_location(deployment_loc)
         deployment = Deployment.get(deployment_id)
         self.model = deployment.model
+        self.model_package = deployment.model_package
 
         # Update prediction intervals settings and check if the new model can support them
         old_pred_int_settings = self.get_prediction_intervals_settings()
         try:
             if old_pred_int_settings["percentiles"]:
                 self.update_prediction_intervals_settings(
                     percentiles=old_pred_int_settings["percentiles"],
@@ -950,39 +1017,144 @@
                 )
         except Exception:
             # Doing a catch-all here because any errors from prediction intervals should not affect
             # the rest of model replacement. If there are errors, then update deployment to use
             # default prediction intervals settings.
             self.update_prediction_intervals_settings(percentiles=[], enabled=False)
 
-    def validate_replacement_model(self, new_model_id: str) -> Tuple[str, str, Dict[str, Any]]:
+    def perform_model_replace(
+        self,
+        new_registered_model_version_id: str,
+        reason: str,
+        max_wait: int = 600,
+    ) -> None:
+        """Replace the model used in this deployment. To confirm model replacement eligibility, use
+         :meth:`~datarobot.models.Deployment.validate_replacement_model` beforehand.
+
+        .. versionadded:: v3.4
+
+        Model replacement is an asynchronous process, which means some preparatory work may
+        be performed after the initial request is completed. This function will not return until all
+        preparatory work is fully finished.
+
+        Predictions made against this deployment will start using the new model as soon as the
+        request is completed. There will be no interruption for predictions throughout
+        the process.
+
+        Parameters
+        ----------
+        new_registered_model_version_id : str
+            The registered model version (model package) ID of the new model to use.
+        reason : MODEL_REPLACEMENT_REASON
+            The reason for the model replacement. Must be one of 'ACCURACY', 'DATA_DRIFT', 'ERRORS',
+            'SCHEDULED_REFRESH', 'SCORING_SPEED', or 'OTHER'. This value will be stored in the model
+            history to keep track of why a model was replaced
+        max_wait : int, optional
+            The maximum time to wait for
+            model replacement job to complete before erroring
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from datarobot import Deployment
+            from datarobot.enums import MODEL_REPLACEMENT_REASON
+            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
+            deployment.model_package['id']
+            >>>'5c0a979859b00004ba52e431'
+
+            deployment.perform_model_replace('5c0a969859b00004ba52e41b', MODEL_REPLACEMENT_REASON.ACCURACY)
+            deployment.model_package['id']
+            >>>'5c0a969859b00004ba52e41b'
+        """
+
+        payload = {"modelPackageId": new_registered_model_version_id, "reason": reason}
+
+        url = f"{self._path}{self.id}/model/"
+        response = self._client.patch(url, data=payload)
+        deployment_loc = wait_for_async_resolution(
+            self._client, response.headers["Location"], max_wait=max_wait
+        )
+        deployment_id = get_id_from_location(deployment_loc)
+        deployment = Deployment.get(deployment_id)
+        self.model = deployment.model
+        self.model_package = deployment.model_package
+
+        # Update prediction intervals settings and check if the new model can support them
+        old_pred_int_settings = self.get_prediction_intervals_settings()
+        try:
+            if old_pred_int_settings["percentiles"]:
+                self.update_prediction_intervals_settings(
+                    percentiles=old_pred_int_settings["percentiles"],
+                    enabled=old_pred_int_settings["enabled"],
+                )
+        except ClientError:
+            warnings.warn(
+                "Deployment.perform_model_replace: "
+                "Failed to update prediction intervals settings to match previous "
+                "- falling back to the defaults."
+            )
+            # Doing a catch-all here because any errors from prediction intervals should not affect
+            # the rest of model replacement. If there are errors, then update deployment to use
+            # default prediction intervals settings.
+            self.update_prediction_intervals_settings(percentiles=[], enabled=False)
+
+    def validate_replacement_model(
+        self,
+        new_model_id: Optional[str] = None,
+        new_registered_model_version_id: Optional[str] = None,
+    ) -> Tuple[str, str, Dict[str, Any]]:
         """Validate a model can be used as the replacement model of the deployment.
 
         .. versionadded:: v2.17
 
         Parameters
         ----------
-        new_model_id : str
+        new_model_id : Optional[str]
             the id of the new model to validate
+        new_registered_model_version_id : Optional[str]
+            (new in version 3.4) The registered model version (model package) ID of the new model to use.
 
         Returns
         -------
         status : str
             status of the validation, will be one of 'passing', 'warning' or 'failing'.
             If the status is passing or warning, use :meth:`~datarobot.models.Deployment.replace_model` to
             perform a model replacement. If the status is failing, refer to ``checks`` for more
             detail on why the new model cannot be used as a replacement.
         message : str
             message for the validation result
         checks : dict
             explain why the new model can or cannot replace the deployment's current model
         """
 
+        if new_model_id is None and new_registered_model_version_id is None:
+            raise ValueError("Must specify either new_model_id or new_registered_model_version_id.")
+        if new_model_id is not None and new_registered_model_version_id is not None:
+            raise ValueError(
+                "Cannot specify both new_model_id and new_registered_model_version_id."
+            )
+
         url = f"{self._path}{self.id}/model/validation/"
-        payload = {"modelId": new_model_id}
+        payload = {}
+        if new_model_id is not None:
+            deprecation_warning(
+                subject="Deployment.validate_replacement_model",
+                deprecated_since_version="3.4",
+                will_remove_version="3.6",
+                message=(
+                    "`Deployment.validate_replacement_model` will no longer support "
+                    "`new_model_id` parameter after version 3.6 released. "
+                    "Please use `new_registered_model_version_id` instead."
+                ),
+            )
+            payload["modelId"] = new_model_id
+        if new_registered_model_version_id is not None:
+            payload["modelPackageId"] = new_registered_model_version_id
+
         data = cast(ServerDataDictType, from_api(self._client.post(url, data=payload).json()))
         return (
             cast(str, data.get("status")),
             cast(str, data.get("message")),
             cast(Dict[str, Any], data.get("checks")),
         )
 
@@ -1453,14 +1625,55 @@
                 "fairnessThreshold": fairness_threshold,
                 "preferableTargetValue": preferable_target_value,
             }
         }
         response = self._client.patch(url, json=payload)
         wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
 
+    def get_challenger_replay_settings(self) -> ChallengerReplaySettings:
+        """Retrieve challenger replay settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Returns
+        -------
+        settings : dict in the following format:
+            enabled : bool
+                If challenger replay is enabled. To update
+                existing ''challenger_replay'' settings, see
+                :meth:`~datarobot.models.Deployment.update_challenger_replay_settings`
+            schedule : Schedule
+                The recurring schedule for the challenger replay job.
+        """
+
+        url = f"{self._path}{self.id}/challengerReplaySettings/"
+        response_json = cast(ServerDataDictType, from_api(self._client.get(url).json()))
+        return cast("ChallengerReplaySettings", response_json)
+
+    def update_challenger_replay_settings(
+        self, enabled: bool, schedule: Optional[Schedule] = None
+    ) -> None:
+        """Update challenger replay settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Parameters
+        ----------
+        enabled : bool
+             If challenger replay is enabled.
+        schedule : Optional[Schedule]
+            The recurring schedule for the challenger replay job.
+        """
+        url = f"{self._path}{self.id}/challengerReplaySettings/"
+        payload = {
+            "enabled": enabled,
+            "schedule": schedule,
+        }
+        self._client.patch(url, json=to_api(payload))
+
     def get_drift_tracking_settings(self) -> DriftTrackingSettings:
         """Retrieve drift tracking settings of this deployment.
 
         .. versionadded:: v2.17
 
         Returns
         -------
@@ -1778,14 +1991,118 @@
 
         # Now update deployment with new prediction intervals settings
         payload = {"predictionIntervals": {"enabled": enabled, "percentiles": percentiles or []}}
         url = f"{self._path}{self.id}/settings/"
         response = self._client.patch(url, data=payload)
         wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
 
+    def get_health_settings(self) -> HealthSettings:
+        """Retrieve health settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Returns
+        -------
+        settings : dict in the following format:
+            service : dict
+                Service health settings.
+            data_drift : dict
+                Data drift health settings.
+            accuracy : dict
+                Accuracy health settings.
+            fairness : dict
+                Fairness health settings.
+            custom_metrics : dict
+                Custom metrics health settings.
+            predictions_timeliness : dict
+                Predictions timeliness health settings.
+            actuals_timeliness : dict
+                Actuals timeliness health settings.
+        """
+
+        url = f"{self._path}{self.id}/healthSettings/"
+        response_json = cast(ServerDataDictType, from_api(self._client.get(url).json()))
+        return cast("HealthSettings", response_json)
+
+    def update_health_settings(
+        self,
+        service: Optional[Dict[str, Any]] = None,
+        data_drift: Optional[Dict[str, Any]] = None,
+        accuracy: Optional[Dict[str, Any]] = None,
+        fairness: Optional[Dict[str, Any]] = None,
+        custom_metrics: Optional[Dict[str, Any]] = None,
+        predictions_timeliness: Optional[Dict[str, Any]] = None,
+        actuals_timeliness: Optional[Dict[str, Any]] = None,
+    ) -> HealthSettings:
+        """Update health settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Parameters
+        ----------
+        service : dict
+            Service health settings.
+        data_drift : dict
+            Data drift health settings.
+        accuracy : dict
+            Accuracy health settings.
+        fairness : dict
+            Fairness health settings.
+        custom_metrics : dict
+            Custom metrics health settings.
+        predictions_timeliness : dict
+            Predictions timeliness health settings.
+        actuals_timeliness : dict
+            Actuals timeliness health settings.
+        """
+
+        url = f"{self._path}{self.id}/healthSettings/"
+        payload = {
+            "service": service,
+            "data_drift": data_drift,
+            "accuracy": accuracy,
+            "fairness": fairness,
+            "custom_metrics": custom_metrics,
+            "predictions_timeliness": predictions_timeliness,
+            "actuals_timeliness": actuals_timeliness,
+        }
+        payload = {key: value for key, value in payload.items() if value is not None}
+        if not payload:
+            raise ValueError("Must provide at least one health settings object.")
+        response = self._client.patch(url, data=to_api(payload))
+        return cast("HealthSettings", from_api(response.json()))
+
+    def get_default_health_settings(self) -> HealthSettings:
+        """Retrieve default health settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Returns
+        -------
+        settings : dict in the following format:
+            service : dict
+                Service health settings.
+            data_drift : dict
+                Data drift health settings.
+            accuracy : dict
+                Accuracy health settings.
+            fairness : dict
+                Fairness health settings.
+            custom_metrics : dict
+                Custom metrics health settings.
+            predictions_timeliness : dict
+                Predictions timeliness health settings.
+            actuals_timeliness : dict
+                Actuals timeliness health settings.
+        """
+
+        url = f"{self._path}{self.id}/healthSettings/defaults/"
+        response_json = cast(ServerDataDictType, from_api(self._client.get(url).json()))
+        return cast("HealthSettings", response_json)
+
     def get_service_stats(
         self,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         execution_time_quantile: Optional[float] = None,
         response_time_quantile: Optional[float] = None,
@@ -2379,14 +2696,15 @@
     def download_scoring_code(
         self,
         filepath: str,
         source_code: bool = False,
         include_agent: bool = False,
         include_prediction_explanations: bool = False,
         include_prediction_intervals: bool = False,
+        max_wait: int = DEFAULT_MAX_WAIT,
     ) -> None:
         """Retrieve scoring code of the current deployed model.
 
         .. versionadded:: v2.24
 
         Notes
         -----
@@ -2402,14 +2720,18 @@
             whether source code or binary of the scoring code will be retrieved
         include_agent : bool
             whether the scoring code retrieved will include tracking agent
         include_prediction_explanations : bool
             whether the scoring code retrieved will include prediction explanations
         include_prediction_intervals : bool
             whether the scoring code retrieved will support prediction intervals
+        max_wait: int, optional
+            Seconds to wait for successful resolution of a deployment creation job.
+            Deployment supports making predictions only after a deployment creating job
+            has successfully finished
 
         Examples
         --------
         .. code-block:: python
 
             from datarobot import Deployment
             deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
@@ -2423,15 +2745,17 @@
                 build_url,
                 data={
                     "includeAgent": include_agent,
                     "includePredictionExplanations": include_prediction_explanations,
                     "includePredictionIntervals": include_prediction_intervals,
                 },
             )
-            retrieve_url = wait_for_async_resolution(self._client, response.headers["Location"])
+            retrieve_url = wait_for_async_resolution(
+                self._client, response.headers["Location"], max_wait=max_wait
+            )
             response = self._client.get(retrieve_url)
         else:
             retrieve_url = f"{self._path}{self.id}/scoringCode/"
             params = {
                 "sourceCode": source_code,
                 "includeAgent": include_agent,
                 "includePredictionExplanations": include_prediction_explanations,
@@ -2538,15 +2862,15 @@
         limit: int (Default=0)
             At most this many results are returned.
         offset: int (Default=0)
             This many results will be skipped.
 
         Returns
         -------
-        list(DeploymentSharedRole)
+        List[DeploymentSharedRole]
         """
         path = f"{self._path}{self.id}/sharedRoles/"
         params = dict(
             name=name,
             id=id,
             share_recipient_type=share_recipient_type,
             limit=limit,
@@ -2584,14 +2908,129 @@
                     "'roles' must be a list of one of: dict, "
                     "DeploymentGrantSharedRoleWithUsername, DeploymentGrantSharedRoleWithId"
                 )
             roles_json.append(role if isinstance(role, dict) else role.to_dict())
 
         self._client.patch(path, data=dict(operation="updateRoles", roles=roles_json))
 
+    def list_challengers(self) -> List[Challenger]:
+        """Get a list of challengers for this deployment.
+
+        .. versionadded:: v3.4
+
+        Returns
+        -------
+        list(Challenger)
+        """
+        return Challenger.list(self.id)
+
+    def get_champion_model_package(self) -> ChampionModelPackage:
+        """
+        Get a champion model package for this deployment.
+
+        Returns
+        -------
+        champion_model_package : ChampionModelPackage
+            A champion model package object.
+
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from datarobot import Deployment
+            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
+            champion_model_package = deployment.get_champion_model_package()
+        """
+        path = f"{self._path}{self.id}/championModelPackage/"
+        response = self._client.get(path)
+        champion_model_package = ChampionModelPackage.from_data(data=from_api(response.json()))
+        return champion_model_package
+
+    def list_prediction_data_exports(
+        self,
+        model_id: Optional[str] = None,
+        status: Optional[ExportStatus] = None,
+        batch: Optional[bool] = None,
+        offset: Optional[int] = 0,
+        limit: Optional[int] = 100,
+    ) -> List[PredictionDataExport]:
+        """
+        Retrieve a list of asynchronous prediction data exports.
+
+        Parameters
+        ----------
+        model_id: Optional[str]
+            The ID of the model used for prediction data export.
+        status: Optional[str]
+            A prediction data export processing state.
+        batch: Optional[bool]
+            If true, only return batch exports.
+            If false, only return real-time exports.
+            If not provided, return both real-time and batch exports.
+        limit: Optional[int]
+            The maximum number of objects to return. The default is 100 (0 means no limit).
+        offset: Optional[int]
+            The starting offset of the results. The default is 0.
+
+        Returns
+        -------
+        prediction_data_exports: List[PredictionDataExport]
+            A list of prediction data exports.
+        """
+        return PredictionDataExport.list(
+            deployment_id=self.id,
+            model_id=model_id,
+            status=status,
+            batch=batch,
+            offset=offset,
+            limit=limit,
+        )
+
+    def list_actuals_data_exports(
+        self,
+        status: Optional[ExportStatus] = None,
+        offset: Optional[int] = 0,
+        limit: Optional[int] = 100,
+    ) -> List[ActualsDataExport]:
+        """
+        Retrieve a list of asynchronous actuals data exports.
+
+        Parameters
+        ----------
+        status: Optional[str]
+            Actuals data export processing state.
+        limit: Optional[int]
+            The maximum number of objects to return. The default is 100 (0 means no limit).
+        offset: Optional[int]
+            The starting offset of the results. The default is 0.
+
+        Returns
+        -------
+        actuals_data_exports: List[ActualsDataExport]
+            A list of actuals data exports.
+        """
+        return ActualsDataExport.list(
+            deployment_id=self.id,
+            status=status,
+            offset=offset,
+            limit=limit,
+        )
+
+    def list_training_data_exports(self) -> List[TrainingDataExport]:
+        """
+        Retrieve a list of successful training data exports.
+
+        Returns
+        -------
+        training_data_export: List[TrainingDataExport]
+            A list of training data exports.
+        """
+        return TrainingDataExport.list(deployment_id=self.id)
+
 
 class DeploymentListFilters:  # pylint: disable=missing-class-docstring
     def __init__(
         self,
         role: Optional[str] = None,
         service_health: Optional[List[str]] = None,
         model_health: Optional[List[str]] = None,
```

### Comparing `datarobot-3.3.2/datarobot/models/deployment/mixins.py` & `datarobot-3.4.0/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/deployment/service_stats.py` & `datarobot-3.4.0/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/deployment/sharing.py` & `datarobot-3.4.0/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/documentai/document.py` & `datarobot-3.4.0/datarobot/models/documentai/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """Page of a document as an image file.
 
     Attributes
     ----------
     project_id : str
         The identifier of the project which the document page belongs to.
     document_page_id : str
-        The unqique identifer for the document page.
+        The unique identifier for the document page.
     height : int
          The height of the document thumbnail in pixels.
     width : int
          The width of the document thumbnail in pixels.
     thumbnail_bytes : bytes
         The number of bytes of the document thumbnail image. Accessing this may
         require a server request and an associated delay in fetching the resource.
```

### Comparing `datarobot-3.3.2/datarobot/models/execution_environment.py` & `datarobot-3.4.0/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/execution_environment_version.py` & `datarobot-3.4.0/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/external_baseline_validation.py` & `datarobot-3.4.0/datarobot/models/external_baseline_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         a list of the names of multiseries id columns to define series
         within the training data.  Currently only one multiseries id column is supported.
     holdout_start_date : str or None
         the start date of holdout scoring data
     holdout_end_date : str or None
         the end date of holdout scoring data
     backtests : list of dicts containing validation_start_date and validation_end_date or None
-        the configurd backtets of the time series project
+        the configured backtests of the time series project
     forecast_window_start : int
         offset into the future to define how far forward relative to the forecast point the
         forecast window should start.
     forecast_window_end : int
         offset into the future to define how far forward relative to the forecast point the
         forecast window should end.
     message : str or None
```

### Comparing `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot-3.4.0/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/feature.py` & `datarobot-3.4.0/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot-3.4.0/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot-3.4.0/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import List, Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import FEATURE_ASSOCIATION_METRIC, FEATURE_ASSOCIATION_TYPE
 from datarobot.models.api_object import APIObject
+from datarobot.models.status_check_job import StatusCheckJob
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Strength(TypedDict):
         feature1: str
         feature2: str
@@ -174,9 +175,31 @@
         url = cls._path.format(project_id)
         response = cls._client.get(url, params=params)
         feature_association_matrix = cls.from_server_data(response.json())
         # FAM public API doesn't include project_id so lets populate it
         feature_association_matrix.project_id = project_id
         return feature_association_matrix
 
+    @classmethod
+    def create(cls, project_id: str, featurelist_id: str) -> StatusCheckJob:
+        """Compute the Feature Association Matrix for a Feature List
+
+        Parameters
+        ----------
+        project_id : str
+            The ID of the project that the feature list belongs to.
+        featurelist_id : str
+            The ID of the feature list for which insights are requested.
+
+        Returns
+        -------
+        status_check_job : StatusCheckJob
+            Object contains all needed logic for a periodical status check of an async job.
+        """
+
+        url = cls._path.format(project_id)
+        payload = {"featurelistId": featurelist_id}
+        resp = cls._client.post(url, data=payload)
+        return StatusCheckJob.from_response(resp, response_type=FeatureAssociationMatrix)
+
     def to_dict(self) -> FeatureAssociationMatrixDict:
         return {"strengths": self.strengths, "features": self.features}
```

### Comparing `datarobot-3.3.2/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot-3.4.0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/feature_effect.py` & `datarobot-3.4.0/datarobot/models/feature_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,14 +331,17 @@
         repacked_server_data = {
             "projectId": this_item["projectId"],
             "modelId": this_item["entityId"],
             "source": this_item["source"],
             insight_name: this_item["data"][insight_name],
             "dataSliceId": this_item["dataSliceId"],
         }
+        if "backtestIndex" in this_item:
+            repacked_server_data["backtestIndex"] = this_item.get("backtestIndex")
+
         return repacked_server_data
 
     @classmethod
     def from_server_data(cls, data, *args, use_insights_format=False, **kwargs):
         """
         Instantiate an object of this class using the data directly from the server,
         meaning that the keys may have the wrong camel casing.
```

### Comparing `datarobot-3.3.2/datarobot/models/feature_impact.py` & `datarobot-3.4.0/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/featurelist.py` & `datarobot-3.4.0/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/imported_model.py` & `datarobot-3.4.0/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/job.py` & `datarobot-3.4.0/datarobot/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from .. import errors
 from ..client import get_client, staticproperty
 from ..enums import DEFAULT_MAX_WAIT, JOB_TYPE, PREDICTION_PREFIX, QUEUE_STATUS
 from ..utils import from_api, raw_prediction_response_to_dataframe
 from .feature_effect import FeatureEffects, FeatureEffectsMulticlass
-from .model import Model, PrimeModel
+from .model import DatetimeModel, Model, PrimeModel
 from .prediction_explanations import PredictionExplanations, PredictionExplanationsInitialization
 from .prime_file import PrimeFile
 from .rating_table import RatingTable
 from .ruleset import Ruleset
 from .training_predictions import TrainingPredictions
 
 TAbstractSpecificJob = TypeVar("TAbstractSpecificJob", bound="AbstractSpecificJob")
@@ -178,14 +178,16 @@
         if not self._completed_resource_url:
             raise errors.JobNotFinished
         completed_resource_path = self._client.strip_endpoint(self._completed_resource_url)
         return self._make_result_from_location(completed_resource_path, params)
 
     def _make_result_from_json(self, server_data):  # pylint: disable=missing-function-docstring
         if self.job_type == JOB_TYPE.MODEL:
+            if "/datetimeModels" in self._completed_resource_url:
+                return DatetimeModel.from_server_data(server_data)
             return Model.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PREDICT:
             return raw_prediction_response_to_dataframe(server_data, PREDICTION_PREFIX.DEFAULT)
         elif self.job_type == JOB_TYPE.FEATURE_IMPACT:
             # Note: a custom FeatureImpactJob class is used for high level API now.
             return server_data["featureImpacts"]
         elif self.job_type == JOB_TYPE.FEATURE_EFFECTS:
@@ -469,15 +471,15 @@
     In general, we aim to keep the number of Job classes low by just utilizing the `job_type`
     attribute to control any specific formatting; however in this case when we needed to support
     a new representation with the _same_ job_type, customizing the behavior of
     `_make_result_from_location` allowed us to achieve our ends without complicating the
     `_make_result_from_json` method.
     """
 
-    # This is a default value used by a new instantiated job. This can be overriden in `__init__()`
+    # This is a default value used by a new instantiated job. This can be overridden in `__init__()`
     # but for existing instances it will not change on subsequent `__init__()` calls without
     # explicit `with_metadata` parameter (which `refresh()` does).
     _with_metadata = False
 
     def __init__(self, data, completed_resource_url=None, with_metadata=False):
         super().__init__(data, completed_resource_url=completed_resource_url)
         # We might be in existing instance with .refresh() called, that does not know about
```

### Comparing `datarobot-3.3.2/datarobot/models/lift_chart.py` & `datarobot-3.4.0/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/missing_report.py` & `datarobot-3.4.0/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/model.py` & `datarobot-3.4.0/datarobot/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 from datetime import datetime
 from io import IOBase, StringIO
 from typing import Any, cast, Dict, List, NoReturn, Optional, Set, Tuple, TYPE_CHECKING, Union
-from urllib.parse import urljoin
 import warnings
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.errors import (
@@ -59,33 +58,34 @@
 from datarobot.models.pareto_front import ParetoFront
 from datarobot.models.residuals import ResidualsChart, SlicedResidualsChart
 from datarobot.models.roc_curve import LabelwiseRocCurve, RocCurve, SlicedRocCurve
 from datarobot.models.ruleset import Ruleset
 from datarobot.models.segmentation import SegmentInfo
 from datarobot.models.status_check_job import StatusCheckJob
 from datarobot.models.training_predictions import TrainingPredictions
-from datarobot.models.validators import feature_impact_trafaret, multiclass_feature_impact_trafaret
+from datarobot.models.validators import multiclass_feature_impact_trafaret
 from datarobot.models.word_cloud import WordCloud
-from datarobot.utils import assert_single_parameter, datetime_to_string, to_api
+from datarobot.utils import assert_single_parameter, datetime_to_string, deprecated, to_api
 from datarobot.utils.pagination import unpaginate
 
 from ..enums import (
     CHART_DATA_SOURCE,
     DATETIME_TREND_PLOTS_STATUS,
     DEFAULT_MAX_WAIT,
+    INSIGHTS_SOURCES,
     MONOTONICITY_FEATURELIST_DEFAULT,
     SOURCE_TYPE,
-    TARGET_TYPE,
 )
 from ..utils import from_api, get_id_from_response, parse_time
 from ..utils.waiters import wait_for_async_resolution
 from .advanced_tuning import AdvancedTuningSession
 from .api_object import APIObject
 from .feature_impact import FeatureImpact
 
+MODEL_RECORDS_CHUNK_SIZE = 250
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.blueprint import BlueprintJson
     from datarobot.models.dataset import Dataset
     from datarobot.models.job import Job
     from datarobot.models.modeljob import ModelJob
@@ -158,137 +158,49 @@
     see get_roc_curve for more info
     """
 
 
 DATA_SLICE_WITH_ID_NONE = Sentinel()
 
 
-class Model(APIObject, BrowserMixin):
-    """A model trained on a project's dataset capable of making predictions
-
-    All durations are specified with a duration string such as those returned
-    by the :meth:`partitioning_methods.construct_duration_string
-    <datarobot.helpers.partitioning_methods.construct_duration_string>` helper method.
-    Please see :ref:`datetime partitioned project documentation <date_dur_spec>`
-    for more information on duration strings.
-
-    Attributes
-    ----------
-    id : str
-        the id of the model
-    project_id : str
-        the id of the project the model belongs to
-    processes : list of str
-        the processes used by the model
-    featurelist_name : str
-        the name of the featurelist used by the model
-    featurelist_id : str
-        the id of the featurelist used by the model
-    sample_pct : float or None
-        the percentage of the project dataset used in training the model.  If the project uses
-        datetime partitioning, the sample_pct will be None.  See `training_row_count`,
-        `training_duration`, and `training_start_date` and `training_end_date` instead.
-    training_row_count : int or None
-        the number of rows of the project dataset used in training the model.  In a datetime
-        partitioned project, if specified, defines the number of rows used to train the model and
-        evaluate backtest scores; if unspecified, either `training_duration` or
-        `training_start_date` and `training_end_date` was used to determine that instead.
-    training_duration : str or None
-        only present for models in datetime partitioned projects.  If specified, a duration string
-        specifying the duration spanned by the data used to train the model and evaluate backtest
-        scores.
-    training_start_date : datetime or None
-        only present for frozen models in datetime partitioned projects.  If specified, the start
-        date of the data used to train the model.
-    training_end_date : datetime or None
-        only present for frozen models in datetime partitioned projects.  If specified, the end
-        date of the data used to train the model.
-    model_type : str
-        what model this is, e.g. 'Nystroem Kernel SVM Regressor'
-    model_category : str
-        what kind of model this is - 'prime' for DataRobot Prime models, 'blend' for blender models,
-        and 'model' for other models
-    is_frozen : bool
-        whether this model is a frozen model
-    is_n_clusters_dynamically_determined : bool
-        (New in version v2.27) optional, if this model determines number of clusters dynamically
-    blueprint_id : str
-        the id of the blueprint used in this model
-    metrics : dict
-        a mapping from each metric to the model's scores for that metric
-    monotonic_increasing_featurelist_id : str
-        optional, the id of the featurelist that defines the set of features with
-        a monotonically increasing relationship to the target.
-        If None, no such constraints are enforced.
-    monotonic_decreasing_featurelist_id : str
-        optional, the id of the featurelist that defines the set of features with
-        a monotonically decreasing relationship to the target.
-        If None, no such constraints are enforced.
-    n_clusters : int
-        (New in version v2.27) optional, number of data clusters discovered by model
-    has_empty_clusters: bool
-        (New in version v2.27) optional, whether clustering models produces empty clusters.
-    supports_monotonic_constraints : bool
-        optional, whether this model supports enforcing monotonic constraints
-    is_starred : bool
-        whether this model marked as starred
-    prediction_threshold : float
-        for binary classification projects, the threshold used for predictions
-    prediction_threshold_read_only : bool
-        indicated whether modification of the prediction threshold is forbidden. Threshold
-        modification is forbidden once a model has had a deployment created or predictions made via
-        the dedicated prediction API.
-    model_number : integer
-        model number assigned to a model
-    parent_model_id : str or None
-        (New in version v2.20) the id of the model that tuning parameters are derived from
-    use_project_settings : bool or None
-        (New in version v2.20) Only present for models in datetime-partitioned projects. If
-        ``True``, indicates that the custom backtest partitioning settings specified by the user
-        were used to train the model and evaluate backtest scores.
-    supports_composable_ml : bool or None
-        (New in version v2.26)
-        whether this model is supported in the Composable ML.
+class GenericModel(APIObject, BrowserMixin):
+    """
+    GenericModel [ModelRecord] is the object which is returned from /modelRecords list route.
+    Contains most generic model information.
     """
 
     _base_model_path_template = "projects/{}/models/"
-    _base_insights_template = "insights/{}/"
 
     _converter = t.Dict(
         {
-            t.Key("id", optional=True): String,
+            t.Key("id"): String,
             t.Key("processes", optional=True): t.List(String),
             t.Key("featurelist_name", optional=True): String,
             t.Key("featurelist_id", optional=True): String,
-            t.Key("project_id", optional=True): String,
+            t.Key("project_id"): String,
             t.Key("sample_pct", optional=True): t.Float,
-            t.Key("training_row_count", optional=True): Int,
+            t.Key("model_type"): String,
+            t.Key("model_category"): String,
+            t.Key("model_number"): Int,
+            t.Key("model_family"): String,
+            t.Key("blueprint_id"): String,
+            t.Key("metrics"): t.Dict().allow_extra("*"),
+            t.Key("is_frozen"): t.Bool,
+            t.Key("is_starred"): t.Bool,
+            t.Key("parent_model_id", optional=True): String,
+            t.Key("is_trained_into_validation"): t.Bool,
+            t.Key("is_trained_into_holdout"): t.Bool,
+            # datetime models only
+            t.Key("training_row_count", optional=True): t.Int,
             t.Key("training_duration", optional=True): String,
             t.Key("training_start_date", optional=True): parse_time,
             t.Key("training_end_date", optional=True): parse_time,
-            t.Key("model_type", optional=True): String,
-            t.Key("model_category", optional=True): String,
-            t.Key("is_frozen", optional=True): t.Bool,
-            t.Key("is_n_clusters_dynamically_determined", optional=True): t.Bool,
-            t.Key("blueprint_id", optional=True): String,
-            t.Key("metrics", optional=True): t.Dict().allow_extra("*"),
-            t.Key("monotonic_increasing_featurelist_id", optional=True): t.Or(String(), t.Null()),
-            t.Key("monotonic_decreasing_featurelist_id", optional=True): t.Or(String(), t.Null()),
-            t.Key("n_clusters", optional=True): Int,
-            t.Key("has_empty_clusters", optional=True): t.Bool(),
-            t.Key("supports_monotonic_constraints", optional=True): t.Bool(),
-            t.Key("is_starred", optional=True): t.Bool(),
-            t.Key("prediction_threshold", optional=True): t.Float,
-            t.Key("prediction_threshold_read_only", optional=True): t.Bool,
-            t.Key("model_number", optional=True): Int,
-            t.Key("parent_model_id", optional=True): t.Or(String(), t.Null),
-            t.Key("useProjectSettings", optional=True): t.Bool,
-            t.Key("supports_composable_ml", optional=True): t.Bool,
-            t.Key("n_clusters", optional=True): t.Int,
-            t.Key("is_n_clusters_dynamically_determined", optional=True): t.Bool,
+            t.Key("data_selection_method", optional=True): String,
+            t.Key("time_window_sample_pct", optional=True): Int,
+            t.Key("sampling_method", optional=True): String,
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id=None,
         processes=None,
@@ -299,118 +211,155 @@
         training_row_count=None,
         training_duration=None,
         training_start_date=None,
         training_end_date=None,
         model_type=None,
         model_category=None,
         is_frozen=None,
-        is_n_clusters_dynamically_determined=None,
         blueprint_id=None,
         metrics=None,
-        project=None,
-        monotonic_increasing_featurelist_id=None,
-        monotonic_decreasing_featurelist_id=None,
-        n_clusters=None,
-        has_empty_clusters=None,
-        supports_monotonic_constraints=None,
         is_starred=None,
-        prediction_threshold=None,
-        prediction_threshold_read_only=None,
+        model_family=None,
         model_number=None,
         parent_model_id=None,
-        use_project_settings=None,
-        supports_composable_ml=None,
+        data_selection_method=None,
+        time_window_sample_pct=None,
+        sampling_method=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
     ) -> None:
-        # Public attributes
         self.id = id
         self.processes = processes
         self.featurelist_name = featurelist_name
         self.featurelist_id = featurelist_id
         self.project_id = project_id
         self.sample_pct = sample_pct
-        self.training_row_count = training_row_count
-        self.training_duration = training_duration
-        self.training_start_date = training_start_date
-        self.training_end_date = training_end_date
+
+        self.model_number = model_number
         self.model_type = model_type
         self.model_category = model_category
-        self.is_frozen = is_frozen
-        self.is_n_clusters_dynamically_determined = is_n_clusters_dynamically_determined
+        self.model_family = model_family
+
         self.blueprint_id = blueprint_id
         self.metrics = metrics
-        self.monotonic_increasing_featurelist_id = monotonic_increasing_featurelist_id
-        self.monotonic_decreasing_featurelist_id = monotonic_decreasing_featurelist_id
-        self.n_clusters = n_clusters
-        self.has_empty_clusters = has_empty_clusters
-        self.supports_monotonic_constraints = supports_monotonic_constraints
         self.is_starred = is_starred
-        self.prediction_threshold = prediction_threshold
-        self.prediction_threshold_read_only = prediction_threshold_read_only
-        self.model_number = model_number
-        self.parent_model_id = parent_model_id
-        self.use_project_settings = use_project_settings
-        self.supports_composable_ml = supports_composable_ml
+        self.is_trained_into_validation = is_trained_into_validation
+        self.is_trained_into_holdout = is_trained_into_holdout
 
-        # Private attributes
-        self._base_model_path = self._base_model_path_template.format(self.project_id)
+        self.is_frozen = is_frozen
+        self.parent_model_id = parent_model_id
 
-        # Deprecated attributes
-        self._project = project
-        self._featurelist = None
-        self._blueprint = None
+        self.training_row_count = training_row_count
+        # makes sense only for datetime models
+        self.training_duration = training_duration
+        self.training_start_date = training_start_date
+        self.training_end_date = training_end_date
+        self.data_selection_method = data_selection_method
+        self.time_window_sample_pct = time_window_sample_pct
+        self.sampling_method = sampling_method
 
-        self._make_objects()
+        self._base_model_path = self._base_model_path_template.format(self.project_id)
 
     def __repr__(self) -> str:
-        return f"Model({self.model_type or self.id!r})"
-
-    @property
-    def project(self):
-        return self._project
-
-    @property
-    def blueprint(self):
-        return self._blueprint
-
-    @property
-    def featurelist(self):
-        return self._featurelist
-
-    def _make_objects(self) -> None:
-        """Create Project, Blueprint and Featurelist objects"""
-        from . import (  # pylint: disable=import-outside-toplevel,cyclic-import
-            Blueprint,
-            Featurelist,
-            Project,
-        )
-
-        def _nonefree(d):
-            return {k: v for k, v in d.items() if v is not None}
+        return f"GenericModel({self.model_type or self.id!r})"
 
-        # Construct Project
-        if not self._project:
-            self._project = Project(id=self.project_id)
-
-        # Construct Blueprint
-        bp_data = {
-            "id": self.blueprint_id,
-            "processes": self.processes,
-            "model_type": self.model_type,
-            "project_id": self.project_id,
-            "supports_composable_ml": self.supports_composable_ml,
-        }
-        self._blueprint = Blueprint.from_data(_nonefree(bp_data))
+    @classmethod
+    def list(
+        cls,
+        project_id: str,
+        # sorting
+        sort_by_partition: Optional[str] = "validation",
+        sort_by_metric: Optional[str] = None,
+        # if result should contain specific metric, not all of them
+        with_metric: Optional[str] = None,
+        # search in model name or processes,
+        search_term: Optional[str] = None,
+        # filtering options
+        featurelists: Optional[List[str]] = None,
+        families: Optional[List[str]] = None,
+        blueprints: Optional[List[str]] = None,
+        labels: Optional[List[str]] = None,
+        characteristics: Optional[List[str]] = None,
+        training_filters: Optional[List[Any]] = None,
+        # pagination
+        limit: int = 100,
+        offset: int = 0,
+    ) -> List[GenericModel]:
+        """
+        Retrieve paginated model records, sorted by scores, with optional filtering.
 
-        # Construct Featurelist
-        ft_list_data = {
-            "id": self.featurelist_id,
-            "project_id": self.project_id,
-            "name": self.featurelist_name,
-        }
-        self._featurelist = Featurelist.from_data(_nonefree(ft_list_data))
+        Parameters
+        ----------
+        sort_by_partition: str, one of `validation`, `backtesting`, `crossValidation` or `holdout`
+            Set the partition to use for sorted (by score) list of models. `validation` is the default.
+        sort_by_metric: str
+            Set the project metric to use for model sorting. DataRobot-selected project optimization metric
+            is the default.
+        with_metric: str
+            For a single-metric list of results, specify that project metric.
+        search_term: str
+            If specified, only models containing the term in their name or processes are returned.
+        featurelists: list of str
+           If specified, only models trained on selected featurelists are returned.
+        families: list of str
+            If specified, only models belonging to selected families are returned.
+        blueprints: list of str
+             If specified, only models trained on specified blueprint IDs are returned.
+        labels: list of str, `starred` or `prepared for deployment`
+            If specified, only models tagged with all listed labels are returned.
+        characteristics: list of str
+            If specified, only models matching all listed characteristics are returned.
+        training_filters: list of str
+            If specified, only models matching at least one of the listed training conditions are returned.
+            The following formats are supported for autoML and datetime partitioned projects:
+            - number of rows in training subset
+            For datetime partitioned projects:
+            - <training duration>, example `P6Y0M0D`
+            - <training_duration>-<time_window_sample_percent>-<sampling_method> Example: `P6Y0M0D-78-Random`,
+            (returns models trained on 6 years of data, sampling rate 78%, random sampling).
+            - `Start/end date`
+            - `Project settings`
+        limit: int
+        offset: int
+
+        Returns
+        -------
+        generic_models: list of GenericModel
+        """
+
+        query_params = {"limit": limit, "offset": offset}
+        if sort_by_partition:
+            query_params["sort_by_partition"] = sort_by_partition
+        if sort_by_metric:
+            query_params["sort_by_metric"] = sort_by_metric
+        if with_metric:
+            query_params["with_metric"] = with_metric
+        if search_term:
+            query_params["search_term"] = search_term
+        # filtering
+        if blueprints:
+            query_params["blueprints"] = ",".join(blueprints)
+        if featurelists:
+            query_params["featurelists"] = ",".join(featurelists)
+        if families:
+            query_params["families"] = ",".join(families)
+        if labels:
+            query_params["labels"] = ",".join(labels)
+        if characteristics:
+            query_params["characteristics"] = ",".join(characteristics)
+        if training_filters:
+            query_params["training_filters"] = ",".join(training_filters)
+        url = f"projects/{project_id}/modelRecords/"
+        if limit == 0:  # unlimited results
+            query_params["limit"] = MODEL_RECORDS_CHUNK_SIZE
+            return [
+                cls.from_server_data(entry) for entry in unpaginate(url, query_params, cls._client)
+            ]
+        resp_data = cls._client.get(url, params=query_params).json()
+        return [cls.from_server_data(item) for item in resp_data["data"]]
 
     @classmethod
     def from_server_data(cls, data, keep_attrs=None):
         """
         Overrides the inherited method since the model must _not_ recursively change casing
 
         Parameters
@@ -421,55 +370,14 @@
         keep_attrs : list
             List of attribute namespaces like: `['top.middle.bottom']`, that should be kept
             even if their values are `None`
         """
         case_converted = from_api(data, do_recursive=False, keep_attrs=keep_attrs)
         return cls.from_data(case_converted)
 
-    @classmethod
-    def get(cls, project: str, model_id: str) -> Model:
-        """
-        Retrieve a specific model.
-
-        Parameters
-        ----------
-        project : str
-            The project's id.
-        model_id : str
-            The ``model_id`` of the leaderboard item to retrieve.
-
-        Returns
-        -------
-        model : Model
-            The queried instance.
-
-        Raises
-        ------
-        ValueError
-            passed ``project`` parameter value is of not supported type
-        """
-        from . import Project  # pylint: disable=import-outside-toplevel,cyclic-import
-
-        if isinstance(project, Project):
-            project_id = project.id
-            project_instance = project
-        elif isinstance(project, str):
-            project_id = project
-            project_instance = Project.get(project_id)
-        else:
-            raise ValueError("Project arg can be Project instance or str")
-
-        if project_instance.is_datetime_partitioned:
-            return DatetimeModel.get(project=project_id, model_id=model_id)
-        else:
-            url = cls._base_model_path_template.format(project_id) + model_id + "/"
-            resp_data = cls._server_data(url)
-            safe_data = cls._safe_data(resp_data)
-            return cls(**dict(safe_data, project=project_instance))
-
     def get_features_used(self) -> List[str]:
         """Query the server to determine which features were used.
 
         Note that the data returned by this method is possibly different
         than the names of the features in the featurelist used by this model.
         This method will return the raw features that must be supplied in order
         for predictions to be generated on a new set of data. The featurelist,
@@ -541,24 +449,24 @@
         response = self._client.get(url)
         return response.json()
 
     def delete(self) -> None:
         """
         Delete a model from the project's leaderboard.
         """
-        self._client.delete(self._get_model_url())
+        self._client.delete(f"{self._base_model_path}{self.id}/")
 
     def get_uri(self) -> str:
         """
         Returns
         -------
         url : str
             Permanent static hyperlink to this model at leaderboard.
         """
-        return f"{self._client.domain}/{self._base_model_path}{self.id}"
+        return f"{self._client.domain}/projects/{self.project_id}/models/{self.id}"
 
     def train(
         self,
         sample_pct: Optional[float] = None,
         featurelist_id: Optional[str] = None,
         scoring_type: Optional[str] = None,
         training_row_count: Optional[int] = None,
@@ -806,32 +714,43 @@
             "trainingRowCount": training_row_count,
         }
         if n_clusters:
             payload["nClusters"] = n_clusters
         response = self._client.post(url, data=payload)
         return ModelJob.from_id(self.project_id, get_id_from_response(response))
 
-    def incremental_train(
+    def train_incremental(
         self,
         data_stage_id: str,
         training_data_name: Optional[str] = None,
-    ) -> ModelJob:
+        data_stage_encoding: Optional[str] = None,
+        data_stage_delimiter: Optional[str] = None,
+        data_stage_compression: Optional[str] = None,
+    ):
         """Submit a job to the queue to perform incremental training on an existing model using
         additional data. The id of the additional data to use for training is specified with the data_stage_id.
         Optionally a name for the iteration can be supplied by the user to help identify the contents of data in
         the iteration.
 
         This functionality requires the INCREMENTAL_LEARNING feature flag to be enabled.
 
         Parameters
         ----------
         data_stage_id: str
             The id of the data stage to use for training.
         training_data_name : str, optional
             The name of the iteration or data stage to indicate what the incremental learning was performed on.
+        data_stage_encoding : str, optional
+            The encoding type of the data in the data stage (default: UTF-8).
+            Supported formats: UTF-8, ASCII, WINDOWS1252
+        data_stage_encoding : str, optional
+            The delimiter used by the data in the data stage (default: ',').
+        data_stage_compression : str, optional
+            The compression type of the data stage file, e.g. 'zip' (default: None).
+            Supported formats: zip
 
         Returns
         -------
         job : ModelJob
             The created job that is retraining the model
         """
         from .modeljob import ModelJob  # pylint: disable=import-outside-toplevel,cyclic-import
@@ -841,24 +760,39 @@
 
         url = f"projects/{self.project_id}/incrementalLearningModels/fromModel/"
         payload = {
             "modelId": self.id,
             "dataStageId": data_stage_id,
             "trainingDataName": training_data_name,
         }
+        # When defined add provided data stage options to the request.
+        # To use defaults the arguments should not be passed to the endpoint.
+        if data_stage_encoding:
+            payload.update({"dataStageEncoding": data_stage_encoding})
+        if data_stage_delimiter:
+            payload.update({"dataStageDelimiter": data_stage_delimiter})
+        if data_stage_compression:
+            payload.update({"dataStageCompression": data_stage_compression})
         response = self._client.post(url, data=payload)
         return ModelJob.from_id(self.project_id, get_id_from_response(response))
 
-    def _get_model_url(self) -> str:
-        if self.id is None:
-            # This check is why this is a method instead of an attribute. Once we stop creating
-            # models without model id's in the tests, we can make this an attribute we set in the
-            # constructor.
-            raise ValueError("Sorry, id attribute is None so I can't make the url to this model.")
-        return f"{self._base_model_path}{self.id}/"
+    @deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This method is deprecated, please use 'train_incremental' instead.",
+    )
+    def incremental_train(
+        self,
+        data_stage_id: str,
+        training_data_name: Optional[str] = None,
+    ) -> ModelJob:
+        """Submit a job to the queue to perform incremental training on an existing model.
+        See train_incremental documentation.
+        """
+        return self.train_incremental(data_stage_id, training_data_name)
 
     def request_predictions(
         self,
         dataset_id: Optional[str] = None,
         dataset: Optional[Dataset] = None,
         dataframe: Optional[pd.DataFrame] = None,
         file_path: Optional[str] = None,
@@ -1023,25 +957,18 @@
         if (e.status_code not in [403, 422]) and not (
             e.json.get("message") == {"unslicedOnly": "unslicedOnly is not allowed key"}
         ):
             raise e
 
     def _post_insights_url(self, insight_name: str) -> str:
         """Build URL for requests to POST /insights/.../ endpoints, used with sliced insights."""
-        return self._base_insights_template.format(insight_name)
+        return f"insights/{insight_name}/"
 
     def _get_insights_url(self, insight_name: str) -> str:
         """Build URL for requests to GET /insights/.../ endpoints, used with sliced insights."""
-        # set default value for model_id
-        # verify that we got either self.id or model_id set
-        if self.id is None:
-            # This check is why this is a method instead of an attribute. Once we stop creating
-            # models without model id's in the tests, we can make this an attribute we set in the
-            # constructor.
-            raise ValueError("Sorry, id attribute is None so I can't make the url to this model.")
         return f"insights/{insight_name}/models/{self.id}"
 
     def _data_slice_to_query_params(self, data_slice_filter: DataSlice = None) -> Dict[str, str]:
         """Convert a DataSlice object to the query params needed to request insights with a matching
         DataSlice.  Passing in data_slice_filter = None will set params to return all insights"""
         params = {}
         if data_slice_filter:
@@ -1064,16 +991,15 @@
         this potentially will return a list of charts. The methods listed above expect to return
         only a single chart sliced or unsliced insight.
         """
         if data_slice_filter is None:
             raise ValueError("Invalid data_slice_filter value. Please specify `DataSlice` filter")
 
     def _get_feature_impact_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureImpact/"
+        return f"{self._base_model_path}{self.id}/featureImpact/"
 
     def get_feature_impact(
         self,
         with_metadata: bool = False,
         data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
     ):
         """
@@ -1138,17 +1064,20 @@
         """
 
         self._validate_data_slice_filter(data_slice_filter)
 
         if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
             data_slice_filter = DataSlice(id=None)
 
-        insight_name = "featureImpact"
         params = self._data_slice_to_query_params(data_slice_filter)
+        return self._make_get_insights_feature_impact_request(params, with_metadata)
 
+    def _make_get_insights_feature_impact_request(self, params, with_metadata):
+        """Make GET request to Feature Impact insights API"""
+        insight_name = "featureImpact"
         try:
             insights_fi_url = self._get_insights_url(insight_name)
             paginated_response = self._client.get(insights_fi_url, params=params).json()
             # if the insights API returns an empty response, raise 404
             # to maintain backwards-compatibility of this function
             if not paginated_response["data"]:
                 error_msg = f"No feature impact data found for model {self.id}."
@@ -1252,19 +1181,34 @@
            'impactNormalized', and 'impactUnnormalized', and 'redundantWith'.
 
         Raises
         ------
         ClientError (404)
             If the multiclass feature impacts have not been computed.
         """
-        url = self._get_model_url() + "multiclassFeatureImpact/"
+        url = f"{self._base_model_path}{self.id}/multiclassFeatureImpact/"
         data = self._client.get(url).json()
         data = multiclass_feature_impact_trafaret.check(data)
         return data["classFeatureImpacts"]
 
+    def _make_post_insights_feature_impact_request(self, source, data_slice_id, row_count):
+        """Make POST request to Feature Impact insights API"""
+        route = self._post_insights_url("featureImpact")
+        payload = {
+            "source": source,
+            "dataSliceId": data_slice_id,
+            "entityType": "datarobotModel",
+            "entityId": self.id,
+            "rowCount": row_count,
+        }
+        response = self._client.post(route, data=payload)
+        # `/insights/featureImpact/` returns `status_id`, so there is no `job_id`
+        # to build a FeatureImpactJob object
+        return StatusCheckJob.from_response(response, FeatureImpact)
+
     def request_feature_impact(
         self,
         row_count: Optional[int] = None,
         with_metadata: bool = False,
         data_slice_id: Optional[str] = None,
     ):
         """
@@ -1295,26 +1239,17 @@
         ------
         JobAlreadyRequested (422)
             If the feature impacts have already been requested.
         """
         from .job import FeatureImpactJob  # pylint: disable=import-outside-toplevel,cyclic-import
 
         if data_slice_id:
-            route = self._post_insights_url("featureImpact")
-            payload = {
-                "source": "training",
-                "dataSliceId": data_slice_id,
-                "entityType": "datarobotModel",
-                "entityId": self.id,
-                "rowCount": row_count,
-            }
-            response = self._client.post(route, data=payload)
-            # `/insights/featureImpact/` returns `status_id`, so there is no `job_id`
-            # to build a FeatureImpactJob object
-            return StatusCheckJob.from_response(response, FeatureImpact)
+            return self._make_post_insights_feature_impact_request(
+                source="training", data_slice_id=data_slice_id, row_count=row_count
+            )
 
         route = self._get_feature_impact_url()
         payload = {"row_count": row_count} if row_count is not None else {}
         response = self._client.post(route, data=payload)
         job_id = get_id_from_response(response)
         return FeatureImpactJob.get(self.project_id, job_id, with_metadata=with_metadata)
 
@@ -1373,24 +1308,25 @@
             )
 
             with_metadata = kwargs.get("with_metadata", False)
             feature_impact_response = FeatureImpactJob.get(
                 self.project_id, qid, with_metadata=with_metadata
             )
         if kwargs.get("data_slice_id"):
-            wait_for_async_resolution(self._client, f"status/{feature_impact_response}/", max_wait)
+            wait_for_async_resolution(
+                self._client, f"status/{feature_impact_response.job_id}/", max_wait
+            )
             data_slice = DataSlice(id=kwargs["data_slice_id"])
 
             return self.get_feature_impact(data_slice_filter=data_slice, with_metadata=True)
 
         return feature_impact_response.get_result_when_complete(max_wait=max_wait)
 
     def _get_feature_effect_metadata_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureEffectsMetadata/"
+        return f"{self._base_model_path}{self.id}/featureEffectsMetadata/"
 
     def get_feature_effect_metadata(self):
         """
         Retrieve Feature Effects metadata. Response contains status and available model sources.
 
         * Feature Effect for the `training` partition is always available, with the exception of older
           projects that only supported Feature Effect for `validation`.
@@ -1410,16 +1346,15 @@
 
         """
         fe_metadata_url = self._get_feature_effect_metadata_url()
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadata.from_server_data(server_data)
 
     def _get_feature_effect_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureEffects/"
+        return f"{self._base_model_path}{self.id}/featureEffects/"
 
     def request_feature_effect(
         self, row_count: Optional[int] = None, data_slice_id: Optional[str] = None
     ):
         """
         Submit request to compute Feature Effects for the model.
 
@@ -2095,15 +2030,14 @@
         Raises
         ------
         ClientError (404)
             If the insight is not available for this model
         """
 
         if self.is_frozen and fallback_to_parent_insights:
-
             response_items: Set[Tuple[str, str]] = {
                 (item["source"], item["dataSliceId"]) for item in response_data["data"]
             }
 
             source_types = [
                 CHART_DATA_SOURCE.VALIDATION,
                 CHART_DATA_SOURCE.CROSSVALIDATION,
@@ -2717,14 +2651,16 @@
     def get_roc_curve(
         self,
         source: str,
         fallback_to_parent_insights: bool = False,
         data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
     ):
         """Retrieve the ROC curve for a binary model for the specified source.
+        This method is valid only for binary projects. For multilabel projects, use
+        Model.get_labelwise_roc_curves.
 
         Parameters
         ----------
         source : str
             ROC curve data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
             (New in version v2.23) For time series and OTV models, also accepts values `backtest_2`,
             `backtest_3`, ..., up to the number of backtests in the model.
@@ -2748,21 +2684,14 @@
         ClientError
             If the insight is not available for this model
         (New in version v3.0) TypeError
             If the underlying project type is multilabel
         ValueError
             If data_slice_filter passed as None
         """
-        if self.project.target_type == TARGET_TYPE.MULTILABEL:
-            error_message = (
-                "Model.get_roc_curve should be used for binary projects. "
-                "Please use Model.get_labelwise_roc_curves API for multilabel models."
-            )
-            raise TypeError(error_message)
-
         self._validate_data_slice_filter(data_slice_filter)
 
         if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
             data_slice_filter = DataSlice(id=None)
 
         insight_name = "rocCurve"
         params = self._data_slice_to_query_params(data_slice_filter)
@@ -2854,15 +2783,17 @@
             use_insights_format = False
         return [
             RocCurve.from_server_data(data=lc_data, use_insights_format=use_insights_format)
             for lc_data in response_data
         ]
 
     def get_labelwise_roc_curves(self, source, fallback_to_parent_insights=False):
-        """Retrieve a list of LabelwiseRocCurve instances for a multilabel model the given source and all labels.
+        """
+        Retrieve a list of LabelwiseRocCurve instances for a multilabel model for the given source and all labels.
+        This method is valid only for multilabel projects. For binary projects, use Model.get_roc_curve API .
 
         .. versionadded:: v2.24
 
         Parameters
         ----------
         source : str
             ROC curve data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
@@ -2877,25 +2808,15 @@
         list of :class:`LabelwiseRocCurve <datarobot.models.roc_curve.LabelwiseRocCurve>`
             Labelwise ROC Curve instances for ``source`` and all labels
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
-        (New in version v3.0) TypeError
-            If the underlying project type is binary
         """
-        if self.project.target_type == TARGET_TYPE.BINARY:
-            error_message = (
-                "Model.get_labelwise_roc_curves should be used "
-                "for multilabel projects. Please use Model.get_roc_curve API "
-                "for binary models."
-            )
-            raise TypeError(error_message)
-
         url_template = "projects/{}/models/{}/labelwiseRocCurves/{}/"
         response_data = self._get_insight(
             url_template,
             source,
             "Labelwise ROC Curve",
             fallback_to_parent_insights=fallback_to_parent_insights,
         )
@@ -2922,15 +2843,15 @@
         """
         url = "projects/{}/models/{}/wordCloud/?excludeStopWords={}".format(
             self.project_id, self.id, "true" if exclude_stop_words else "false"
         )
         response_data = self._client.get(url).json()
         return WordCloud.from_server_data(response_data)
 
-    def download_scoring_code(self, file_name, source_code=False):
+    def download_scoring_code(self, file_name: str, source_code: bool = False) -> None:
         """Download the Scoring Code JAR.
 
         Parameters
         ----------
         file_name : str
             File path where scoring code will be saved.
         source_code : bool, optional
@@ -2949,15 +2870,17 @@
         """Get the blueprint json representation used by this model.
 
         Returns
         -------
         BlueprintJson
             Json representation of the blueprint stages.
         """
-        return self.blueprint.get_json()
+        from . import Blueprint  # pylint: disable=import-outside-toplevel
+
+        return Blueprint(id=self.blueprint_id, project_id=self.project_id).get_json()
 
     def get_model_blueprint_documents(self):
         """Get documentation for tasks used in this model.
 
         Returns
         -------
         list of BlueprintTaskDocument
@@ -3403,15 +3326,15 @@
         threshold : float
            only used for binary classification projects. The threshold to when deciding between
            the positive and negative classes when making predictions.  Should be between 0.0 and
            1.0 (inclusive).
         """
         url = f"projects/{self.project_id}/models/{self.id}/"
         self._client.patch(url, data={"prediction_threshold": threshold})
-        self.prediction_threshold = threshold
+        self.prediction_threshold = threshold  # pylint: disable=attribute-defined-outside-init
 
     def download_training_artifact(self, file_name):
         """Retrieve trained artifact(s) from a model containing one or more custom tasks.
 
         Artifact(s) will be downloaded to the specified local filepath.
 
         Parameters
@@ -3436,15 +3359,15 @@
             The fairness metric used to calculate the fairness scores.
 
         Returns
         -------
         status_id : str
             A statusId of computation request.
         """
-        route = urljoin(self._get_model_url(), "fairnessInsights/")
+        route = f"{self._base_model_path}{self.id}/fairnessInsights/"
         data = {"fairness_metrics_set": fairness_metrics_set} if fairness_metrics_set else {}
         response = self._client.post(route, data)
         status_id = get_id_from_response(response)
 
         return status_id
 
     def get_fairness_insights(self, fairness_metrics_set=None, offset=0, limit=100):
@@ -3464,16 +3387,15 @@
         Returns
         -------
         json
         """
         query_params = f"?offset={offset}&limit={limit}"
         if fairness_metrics_set:
             query_params += f"&fairnessMetricsSet={fairness_metrics_set}"
-        route = urljoin(self._get_model_url(), f"fairnessInsights/{query_params}")
-
+        route = f"{self._base_model_path}{self.id}/fairnessInsights/{query_params}"
         return self._client.get(route).json()
 
     def request_data_disparity_insights(self, feature, compared_class_names):
         """
         Request data disparity insights to be computed for the model.
 
         Parameters
@@ -3484,15 +3406,15 @@
             List of two classes to compare
 
         Returns
         -------
         status_id : str
             A statusId of computation request.
         """
-        route = f"{self._get_model_url()}dataDisparityInsights/"
+        route = f"{self._base_model_path}{self.id}/dataDisparityInsights/"
         response = self._client.post(
             route,
             data={"feature": feature, "compared_class_names": compared_class_names},
         )
         status_id = get_id_from_response(response)
 
         return status_id
@@ -3510,47 +3432,289 @@
         class_name2 : str
             Another compared class
 
         Returns
         -------
         json
         """
-        route = "{}dataDisparityInsights/?feature={}&className1={}&className2={}".format(
-            self._get_model_url(), feature, class_name1, class_name2
+        route = (
+            f"{self._base_model_path}{self.id}/dataDisparityInsights/?"
+            f"feature={feature}&className1={class_name1}&className2={class_name2}"
         )
         return self._client.get(route).json()
 
     def request_cross_class_accuracy_scores(self):
         """
         Request data disparity insights to be computed for the model.
 
         Returns
         -------
         status_id : str
             A statusId of computation request.
         """
-        route = f"{self._get_model_url()}crossClassAccuracyScores/"
+        route = f"{self._base_model_path}{self.id}/crossClassAccuracyScores/"
         response = self._client.post(route)
         status_id = get_id_from_response(response)
 
         return status_id
 
     def get_cross_class_accuracy_scores(self):
         """
         Retrieves a list of Cross Class Accuracy scores for the model.
 
         Returns
         -------
         json
         """
-        route = f"{self._get_model_url()}crossClassAccuracyScores/"
-
+        route = f"{self._base_model_path}{self.id}/crossClassAccuracyScores/"
         return self._client.get(route).json()
 
 
+class Model(GenericModel):
+    """A model trained on a project's dataset capable of making predictions.
+
+    All durations are specified with a duration string such as those returned
+    by the :meth:`partitioning_methods.construct_duration_string
+    <datarobot.helpers.partitioning_methods.construct_duration_string>` helper method.
+    See :ref:`datetime partitioned project documentation <date_dur_spec>`
+    for more information on duration strings.
+
+    Attributes
+    ----------
+    id : str
+        ID of the model.
+    project_id : str
+        ID of the project the model belongs to.
+    processes : list of str
+        Processes used by the model.
+    featurelist_name : str
+        Name of the featurelist used by the model.
+    featurelist_id : str
+        ID of the featurelist used by the model.
+    sample_pct : float or None
+        Percentage of the project dataset used in model training. If the project uses
+        datetime partitioning, the sample_pct will be None.  See `training_row_count`,
+        `training_duration`, and `training_start_date` / `training_end_date` instead.
+    training_row_count : int or None
+        Number of rows of the project dataset used in model training.  In a datetime
+        partitioned project, if specified, defines the number of rows used to train the model and
+        evaluate backtest scores; if unspecified, either `training_duration` or
+        `training_start_date` and `training_end_date` is used for training_row_count.
+    training_duration : str or None
+        For datetime partitioned projects only. If specified, defines the duration spanned by the data used to train
+        the model and evaluate backtest scores.
+    training_start_date : datetime or None
+        For frozen models in datetime partitioned projects only. If specified, the start
+        date of the data used to train the model.
+    training_end_date : datetime or None
+        For frozen models in datetime partitioned projects only. If specified, the end
+        date of the data used to train the model.
+    model_type : str
+        Type of model, for example 'Nystroem Kernel SVM Regressor'.
+    model_category : str
+        Category of model, for example 'prime' for DataRobot Prime models, 'blend' for blender models, and
+        'model' for other models.
+    is_frozen : bool
+        Whether this model is a frozen model.
+    is_n_clusters_dynamically_determined : bool
+        (New in version v2.27) Optional. Whether this model determines the number of clusters dynamically.
+    blueprint_id : str
+        ID of the blueprint used to build this model.
+    metrics : dict
+        Mapping from each metric to the model's score for that metric.
+    monotonic_increasing_featurelist_id : str
+        Optional. ID of the featurelist that defines the set of features with
+        a monotonically increasing relationship to the target.
+        If None, no such constraints are enforced.
+    monotonic_decreasing_featurelist_id : str
+        Optional. ID of the featurelist that defines the set of features with
+        a monotonically decreasing relationship to the target.
+        If None, no such constraints are enforced.
+    n_clusters : int
+        (New in version v2.27) Optional. Number of data clusters discovered by model.
+    has_empty_clusters: bool
+        (New in version v2.27) Optional. Whether clustering model produces empty clusters.
+    supports_monotonic_constraints : bool
+        Optional. Whether this model supports enforcing monotonic constraints.
+    is_starred : bool
+        Whether this model is marked as a starred model.
+    prediction_threshold : float
+        Binary classification projects only. Threshold used for predictions.
+    prediction_threshold_read_only : bool
+        Whether modification of the prediction threshold is forbidden. Threshold
+        modification is forbidden once a model has had a deployment created or predictions made via
+        the dedicated prediction API.
+    model_number : integer
+        Model number assigned to the model.
+    parent_model_id : str or None
+        (New in version v2.20) ID of the model that tuning parameters are derived from.
+    supports_composable_ml : bool or None
+        (New in version v2.26)
+        Whether this model is supported Composable ML.
+
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("id"): String,
+            t.Key("processes", optional=True): t.List(String),
+            t.Key("featurelist_name", optional=True): String,
+            t.Key("featurelist_id", optional=True): String,
+            t.Key("project_id"): String,
+            t.Key("sample_pct", optional=True): t.Float,
+            t.Key("model_type"): String,
+            t.Key("model_category"): String,
+            t.Key("is_frozen"): t.Bool,
+            t.Key("blueprint_id"): String,
+            t.Key("metrics"): t.Dict().allow_extra("*"),
+            t.Key("is_starred"): t.Bool,
+            t.Key("is_n_clusters_dynamically_determined", optional=True): t.Bool,
+            t.Key("monotonic_increasing_featurelist_id", optional=True): t.Or(String(), t.Null()),
+            t.Key("monotonic_decreasing_featurelist_id", optional=True): t.Or(String(), t.Null()),
+            t.Key("n_clusters", optional=True): Int,
+            t.Key("has_empty_clusters", optional=True): t.Bool(),
+            t.Key("supports_monotonic_constraints", optional=True): t.Bool(),
+            t.Key("prediction_threshold", optional=True): t.Float,
+            t.Key("prediction_threshold_read_only", optional=True): t.Bool,
+            t.Key("model_number", optional=True): Int,
+            t.Key("parent_model_id", optional=True): t.Or(String(), t.Null),
+            t.Key("supports_composable_ml", optional=True): t.Bool,
+            t.Key("n_clusters", optional=True): t.Int,
+            t.Key("is_n_clusters_dynamically_determined", optional=True): t.Bool,
+            t.Key("is_trained_into_validation", optional=True): t.Bool,
+            t.Key("is_trained_into_holdout", optional=True): t.Bool,
+            t.Key(
+                "model_family_full_name", optional=True, to_name="model_family_full_name"
+            ): String,
+            t.Key("training_row_count", optional=True): Int,
+            t.Key("training_duration", optional=True): String,
+            t.Key("training_start_date", optional=True): parse_time,
+            t.Key("training_end_date", optional=True): parse_time,
+            t.Key("data_selection_method", optional=True): String,
+            t.Key("time_window_sample_pct", optional=True): Int,
+            t.Key("sampling_method", optional=True): String,
+        }
+    ).allow_extra("*")
+
+    def __init__(
+        self,
+        id=None,
+        processes=None,
+        featurelist_name=None,
+        featurelist_id=None,
+        project_id=None,
+        sample_pct=None,
+        model_type=None,
+        model_category=None,
+        is_frozen=None,
+        is_n_clusters_dynamically_determined=None,
+        blueprint_id=None,
+        metrics=None,
+        monotonic_increasing_featurelist_id=None,
+        monotonic_decreasing_featurelist_id=None,
+        n_clusters=None,
+        has_empty_clusters=None,
+        supports_monotonic_constraints=None,
+        is_starred=None,
+        prediction_threshold=None,
+        prediction_threshold_read_only=None,
+        model_number=None,
+        parent_model_id=None,
+        supports_composable_ml=None,
+        training_row_count=None,
+        training_duration=None,
+        training_start_date=None,
+        training_end_date=None,
+        data_selection_method=None,
+        time_window_sample_pct=None,
+        sampling_method=None,
+        model_family_full_name=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
+    ) -> None:
+        self.is_n_clusters_dynamically_determined = is_n_clusters_dynamically_determined
+        self.monotonic_increasing_featurelist_id = monotonic_increasing_featurelist_id
+        self.monotonic_decreasing_featurelist_id = monotonic_decreasing_featurelist_id
+        self.n_clusters = n_clusters
+        self.has_empty_clusters = has_empty_clusters
+        self.supports_monotonic_constraints = supports_monotonic_constraints
+        self.prediction_threshold = prediction_threshold
+        self.prediction_threshold_read_only = prediction_threshold_read_only
+        self.supports_composable_ml = supports_composable_ml
+        super().__init__(
+            id=id,
+            processes=processes,
+            featurelist_name=featurelist_name,
+            featurelist_id=featurelist_id,
+            project_id=project_id,
+            sample_pct=sample_pct,
+            training_row_count=training_row_count,
+            training_duration=training_duration,
+            training_start_date=training_start_date,
+            training_end_date=training_end_date,
+            model_type=model_type,
+            model_category=model_category,
+            is_frozen=is_frozen,
+            blueprint_id=blueprint_id,
+            metrics=metrics,
+            is_starred=is_starred,
+            model_family=model_family_full_name,
+            model_number=model_number,
+            parent_model_id=parent_model_id,
+            data_selection_method=data_selection_method,
+            time_window_sample_pct=time_window_sample_pct,
+            sampling_method=sampling_method,
+            is_trained_into_validation=is_trained_into_validation,
+            is_trained_into_holdout=is_trained_into_holdout,
+        )
+
+    def __repr__(self) -> str:
+        return f"Model({self.model_type or self.id!r})"
+
+    @classmethod
+    def get(cls, project: str, model_id: str) -> Model:
+        """
+        Retrieve a specific model.
+
+        Parameters
+        ----------
+        project : str
+            Project ID.
+        model_id : str
+            ID of the model to retrieve.
+
+        Returns
+        -------
+        model : Model
+            Queried instance.
+
+        Raises
+        ------
+        ValueError
+            passed ``project`` parameter value is of not supported type
+        """
+        from . import Project  # pylint: disable=import-outside-toplevel,cyclic-import
+
+        if isinstance(project, Project):
+            project_id = project.id
+            project_instance = project
+        elif isinstance(project, str):
+            project_id = project
+            project_instance = Project.get(project_id)
+        else:
+            raise ValueError("Project arg can be Project instance or str")
+
+        if project_instance.is_datetime_partitioned:
+            return DatetimeModel.get(project=project_id, model_id=model_id)
+        else:
+            url = cls._base_model_path_template.format(project_id) + model_id + "/"
+            resp_data = cls._server_data(url)
+            return cls.from_server_data(resp_data)
+
+
 class PrimeModel(Model):
     """Represents a DataRobot Prime model approximating a parent model with downloadable code.
 
     All durations are specified with a duration string such as those returned
     by the :meth:`partitioning_methods.construct_duration_string
     <datarobot.helpers.partitioning_methods.construct_duration_string>` helper method.
     Please see :ref:`datetime partitioned project documentation <date_dur_spec>`
@@ -3631,35 +3795,41 @@
         self,
         id=None,
         processes=None,
         featurelist_name=None,
         featurelist_id=None,
         project_id=None,
         sample_pct=None,
-        training_row_count=None,
-        training_duration=None,
-        training_start_date=None,
-        training_end_date=None,
         model_type=None,
         model_category=None,
         is_frozen=None,
         blueprint_id=None,
         metrics=None,
-        parent_model_id=None,
         ruleset_id=None,
         rule_count=None,
         score=None,
         monotonic_increasing_featurelist_id=None,
         monotonic_decreasing_featurelist_id=None,
         supports_monotonic_constraints=None,
         is_starred=None,
         prediction_threshold=None,
         prediction_threshold_read_only=None,
         model_number=None,
+        parent_model_id=None,
         supports_composable_ml=None,
+        training_row_count=None,
+        training_duration=None,
+        training_start_date=None,
+        training_end_date=None,
+        data_selection_method=None,
+        time_window_sample_pct=None,
+        sampling_method=None,
+        model_family_full_name=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
     ) -> None:
         super().__init__(
             id=id,
             processes=processes,
             featurelist_name=featurelist_name,
             featurelist_id=featurelist_id,
             project_id=project_id,
@@ -3676,26 +3846,33 @@
             monotonic_increasing_featurelist_id=monotonic_increasing_featurelist_id,
             monotonic_decreasing_featurelist_id=monotonic_decreasing_featurelist_id,
             supports_monotonic_constraints=supports_monotonic_constraints,
             is_starred=is_starred,
             prediction_threshold=prediction_threshold,
             prediction_threshold_read_only=prediction_threshold_read_only,
             supports_composable_ml=supports_composable_ml,
+            model_family_full_name=model_family_full_name,
+            model_number=model_number,
+            parent_model_id=parent_model_id,
+            data_selection_method=data_selection_method,
+            time_window_sample_pct=time_window_sample_pct,
+            sampling_method=sampling_method,
+            is_trained_into_validation=is_trained_into_validation,
+            is_trained_into_holdout=is_trained_into_holdout,
         )
         ruleset_data = {
             "ruleset_id": ruleset_id,
             "rule_count": rule_count,
             "score": score,
             "model_id": id,
             "parent_model_id": parent_model_id,
             "project_id": project_id,
         }
         ruleset = Ruleset.from_data(ruleset_data)
         self.ruleset = ruleset
-        self.parent_model_id = parent_model_id
 
     def __repr__(self) -> str:
         return f"PrimeModel({self.model_type or self.id!r})"
 
     def train(
         self,
         sample_pct: Optional[float] = None,
@@ -3844,18 +4021,14 @@
         self,
         id=None,
         processes=None,
         featurelist_name=None,
         featurelist_id=None,
         project_id=None,
         sample_pct=None,
-        training_row_count=None,
-        training_duration=None,
-        training_start_date=None,
-        training_end_date=None,
         model_type=None,
         model_category=None,
         is_frozen=None,
         blueprint_id=None,
         metrics=None,
         model_ids=None,
         blender_method=None,
@@ -3864,14 +4037,24 @@
         supports_monotonic_constraints=None,
         is_starred=None,
         prediction_threshold=None,
         prediction_threshold_read_only=None,
         model_number=None,
         parent_model_id=None,
         supports_composable_ml=None,
+        training_row_count=None,
+        training_duration=None,
+        training_start_date=None,
+        training_end_date=None,
+        data_selection_method=None,
+        time_window_sample_pct=None,
+        sampling_method=None,
+        model_family_full_name=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
     ) -> None:
         super().__init__(
             id=id,
             processes=processes,
             featurelist_name=featurelist_name,
             featurelist_id=featurelist_id,
             project_id=project_id,
@@ -3887,17 +4070,23 @@
             metrics=metrics,
             monotonic_increasing_featurelist_id=monotonic_increasing_featurelist_id,
             monotonic_decreasing_featurelist_id=monotonic_decreasing_featurelist_id,
             supports_monotonic_constraints=supports_monotonic_constraints,
             is_starred=is_starred,
             prediction_threshold=prediction_threshold,
             prediction_threshold_read_only=prediction_threshold_read_only,
+            supports_composable_ml=supports_composable_ml,
+            model_family_full_name=model_family_full_name,
             model_number=model_number,
             parent_model_id=parent_model_id,
-            supports_composable_ml=supports_composable_ml,
+            data_selection_method=data_selection_method,
+            time_window_sample_pct=time_window_sample_pct,
+            sampling_method=sampling_method,
+            is_trained_into_validation=is_trained_into_validation,
+            is_trained_into_holdout=is_trained_into_holdout,
         )
         self.model_ids = model_ids
         self.blender_method = blender_method
 
     @classmethod
     def get(cls, project_id, model_id):  # pylint: disable=arguments-renamed
         """Retrieve a specific blender.
@@ -4004,32 +4193,41 @@
         self,
         id=None,
         processes=None,
         featurelist_name=None,
         featurelist_id=None,
         project_id=None,
         sample_pct=None,
-        training_row_count=None,
-        training_duration=None,
-        training_start_date=None,
-        training_end_date=None,
         model_type=None,
         model_category=None,
         is_frozen=None,
+        is_n_clusters_dynamically_determined=None,
         blueprint_id=None,
         metrics=None,
-        parent_model_id=None,
         monotonic_increasing_featurelist_id=None,
         monotonic_decreasing_featurelist_id=None,
+        n_clusters=None,
+        has_empty_clusters=None,
         supports_monotonic_constraints=None,
         is_starred=None,
         prediction_threshold=None,
         prediction_threshold_read_only=None,
         model_number=None,
+        parent_model_id=None,
         supports_composable_ml=None,
+        training_row_count=None,
+        training_duration=None,
+        training_start_date=None,
+        training_end_date=None,
+        data_selection_method=None,
+        time_window_sample_pct=None,
+        sampling_method=None,
+        model_family_full_name=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
     ) -> None:
         super().__init__(
             id=id,
             processes=processes,
             featurelist_name=featurelist_name,
             featurelist_id=featurelist_id,
             project_id=project_id,
@@ -4038,25 +4236,34 @@
             training_duration=training_duration,
             training_start_date=training_start_date,
             training_end_date=training_end_date,
             model_type=model_type,
             model_category=model_category,
             is_frozen=is_frozen,
             blueprint_id=blueprint_id,
+            is_n_clusters_dynamically_determined=is_n_clusters_dynamically_determined,
             metrics=metrics,
             monotonic_increasing_featurelist_id=monotonic_increasing_featurelist_id,
             monotonic_decreasing_featurelist_id=monotonic_decreasing_featurelist_id,
+            n_clusters=n_clusters,
+            has_empty_clusters=has_empty_clusters,
             supports_monotonic_constraints=supports_monotonic_constraints,
             is_starred=is_starred,
             prediction_threshold=prediction_threshold,
             prediction_threshold_read_only=prediction_threshold_read_only,
-            model_number=model_number,
             supports_composable_ml=supports_composable_ml,
+            model_family_full_name=model_family_full_name,
+            model_number=model_number,
+            parent_model_id=parent_model_id,
+            data_selection_method=data_selection_method,
+            time_window_sample_pct=time_window_sample_pct,
+            sampling_method=sampling_method,
+            is_trained_into_validation=is_trained_into_validation,
+            is_trained_into_holdout=is_trained_into_holdout,
         )
-        self.parent_model_id = parent_model_id
 
     def __repr__(self) -> str:
         return f"FrozenModel({self.model_type or self.id!r})"
 
     @classmethod
     def get(cls, project_id, model_id):  # pylint: disable=arguments-renamed
         """
@@ -4210,17 +4417,15 @@
         Indicates which unit is the basis for the feature derivation window and the forecast window.
         Note that this field will be the same as what is shown in the project settings. In time
         series projects, will be either the detected time unit or "ROW", and `None` otherwise.
     model_number : integer
         model number assigned to a model
     parent_model_id : str or None
         (New in version v2.20) the id of the model that tuning parameters are derived from
-    use_project_settings : bool or None
-        (New in version v2.20) If ``True``, indicates that the custom backtest partitioning settings
-        specified by the user were used to train the model and evaluate backtest scores.
+
     supports_composable_ml : bool or None
         (New in version v2.26)
         whether this model is supported in the Composable ML.
     is_n_clusters_dynamically_determined : bool, optional
         (New in version 2.27) if ``True``, indicates that model determines number of clusters
         automatically.
     n_clusters : int, optional
@@ -4307,18 +4512,21 @@
         effective_feature_derivation_window_start=None,
         effective_feature_derivation_window_end=None,
         forecast_window_start=None,
         forecast_window_end=None,
         windows_basis_unit=None,
         model_number=None,
         parent_model_id=None,
-        use_project_settings=None,
         supports_composable_ml=None,
         n_clusters=None,
         is_n_clusters_dynamically_determined=None,
+        has_empty_clusters=None,
+        model_family_full_name=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
         **kwargs,
     ) -> None:
         super().__init__(
             id=id,
             processes=processes,
             featurelist_name=featurelist_name,
             featurelist_id=featurelist_id,
@@ -4328,34 +4536,37 @@
             training_duration=training_duration,
             training_start_date=training_start_date,
             training_end_date=training_end_date,
             model_type=model_type,
             model_category=model_category,
             is_frozen=is_frozen,
             blueprint_id=blueprint_id,
+            is_n_clusters_dynamically_determined=is_n_clusters_dynamically_determined,
             metrics=metrics,
             monotonic_increasing_featurelist_id=monotonic_increasing_featurelist_id,
             monotonic_decreasing_featurelist_id=monotonic_decreasing_featurelist_id,
+            n_clusters=n_clusters,
+            has_empty_clusters=has_empty_clusters,
             supports_monotonic_constraints=supports_monotonic_constraints,
             is_starred=is_starred,
             prediction_threshold=prediction_threshold,
             prediction_threshold_read_only=prediction_threshold_read_only,
+            supports_composable_ml=supports_composable_ml,
+            model_family_full_name=model_family_full_name,
             model_number=model_number,
             parent_model_id=parent_model_id,
-            use_project_settings=use_project_settings,
-            supports_composable_ml=supports_composable_ml,
-            n_clusters=n_clusters,
-            is_n_clusters_dynamically_determined=is_n_clusters_dynamically_determined,
+            data_selection_method=data_selection_method,
+            time_window_sample_pct=time_window_sample_pct,
+            sampling_method=sampling_method,
+            is_trained_into_validation=is_trained_into_validation,
+            is_trained_into_holdout=is_trained_into_holdout,
         )
-        self.time_window_sample_pct = time_window_sample_pct
-        self.sampling_method = sampling_method
         self.training_info = training_info
         self.holdout_score = holdout_score
         self.holdout_status = holdout_status
-        self.data_selection_method = data_selection_method
         self.backtests = backtests
         self.effective_feature_derivation_window_start = effective_feature_derivation_window_start
         self.effective_feature_derivation_window_end = effective_feature_derivation_window_end
         self.forecast_window_start = forecast_window_start
         self.forecast_window_end = forecast_window_end
         self.windows_basis_unit = windows_basis_unit
         # Private attributes
@@ -4772,25 +4983,16 @@
         if sampling_method:
             payload["samplingMethod"] = sampling_method
         if n_clusters:
             payload["nClusters"] = n_clusters
         response = self._client.post(url, data=payload)
         return ModelJob.from_id(self.project_id, get_id_from_response(response))
 
-    def _get_datetime_model_url(self) -> str:
-        if self.id is None:
-            # This check is why this is a method instead of an attribute. Once we stop creating
-            # models without model id's in the tests, we can make this an attribute we set in the
-            # constructor.
-            raise ValueError("Sorry, id attribute is None so I can't make the url to this model.")
-        return f"{self._base_datetime_model_path}{self.id}/"
-
     def _get_feature_effect_metadata_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_datetime_model_url() + "featureEffectsMetadata/"
+        return f"{self._base_datetime_model_path}{self.id}/featureEffectsMetadata/"
 
     def get_feature_effect_metadata(self):
         """
         Retrieve Feature Effect metadata for each backtest. Response contains status and available
         sources for each backtest of the model.
 
         * Each backtest is available for `training` and `validation`
@@ -4822,19 +5024,33 @@
 
         """
         fe_metadata_url = self._get_feature_effect_metadata_url()
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadataDatetime.from_server_data(server_data)
 
     def _get_feature_effect_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_datetime_model_url() + "featureEffects/"
+        return f"{self._base_datetime_model_path}{self.id}/featureEffects/"
 
-    # pylint: disable-next=arguments-differ
-    def request_feature_effect(self, backtest_index):
+    @staticmethod
+    def _get_source_for_feature_effect(source, backtest_index):
+        """Return source for Feature Effect"""
+        if backtest_index == INSIGHTS_SOURCES.HOLDOUT:
+            fe_source = INSIGHTS_SOURCES.HOLDOUT
+        else:
+            fe_source = "backtest_{}".format(backtest_index)
+
+        if source == INSIGHTS_SOURCES.TRAINING:
+            fe_source += "_training"
+
+        return fe_source
+
+    # pylint: disable-next=arguments-renamed
+    def request_feature_effect(
+        self, backtest_index: str, data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE
+    ):
         """
         Request feature effects to be computed for the model.
 
         See :meth:`get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` for more
         information on the result of the job.
 
         See :meth:`get_feature_effect_metadata \
@@ -4855,22 +5071,39 @@
         Raises
         ------
         JobAlreadyRequested (422)
             If the feature effect have already been requested.
         """
         from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
-        payload = {"backtestIndex": backtest_index}
-        route = self._get_feature_effect_url()
+        if data_slice_filter and data_slice_filter is not DATA_SLICE_WITH_ID_NONE:
+            route = self._post_insights_url("featureEffects")
+            payload = {
+                "source": self._get_source_for_feature_effect(
+                    source=INSIGHTS_SOURCES.TRAINING, backtest_index=backtest_index
+                ),
+                "dataSliceId": data_slice_filter.id,
+                "entityType": "datarobotModel",
+                "entityId": self.id,
+            }
+        else:
+            route = self._get_feature_effect_url()
+            payload = {"backtestIndex": backtest_index}
+
         response = self._client.post(route, data=payload)
         job_id = get_id_from_response(response)
         return Job.get(self.project_id, job_id)
 
     # pylint: disable-next=arguments-renamed
-    def get_feature_effect(self, source, backtest_index):
+    def get_feature_effect(
+        self,
+        source,
+        backtest_index,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ):
         """
         Retrieve Feature Effects for the model.
 
         Feature Effects provides partial dependence and predicted vs actual values for top-500
         features ordered by feature impact score.
 
         The partial dependence shows marginal effect of a feature on the target variable after
@@ -4901,24 +5134,44 @@
            The feature effects data.
 
         Raises
         ------
         ClientError (404)
             If the feature effects have not been computed or source is not valid value.
         """
-        params = {
-            "source": source,
-            "backtestIndex": backtest_index,
-        }
-        fe_url = self._get_feature_effect_url()
-        server_data = self._client.get(fe_url, params=params).json()
-        return FeatureEffects.from_server_data(server_data)
+        insight_name = "featureEffects"
 
-    # pylint: disable-next=arguments-differ
-    def get_or_request_feature_effect(self, source, backtest_index, max_wait=DEFAULT_MAX_WAIT):
+        params = {"source": self._get_source_for_feature_effect(source, backtest_index)}
+        if data_slice_filter and data_slice_filter is not DATA_SLICE_WITH_ID_NONE:
+            params["dataSliceId"] = data_slice_filter.id
+        try:
+            insights_fe_url = self._get_insights_url(insight_name)
+            server_data = self._client.get(insights_fe_url, params=params).json()
+            use_insights_format = True
+        except ClientError as e:
+            self._raise_if_not_slice_forbidden_error(e)
+            server_data = self._client.get(
+                self._get_feature_effect_url(),
+                params={
+                    "source": source,
+                    "backtestIndex": backtest_index,
+                },
+            ).json()
+            use_insights_format = False
+
+        return FeatureEffects.from_server_data(server_data, use_insights_format=use_insights_format)
+
+    # pylint: disable-next=arguments-renamed
+    def get_or_request_feature_effect(
+        self,
+        source,
+        backtest_index,
+        max_wait=DEFAULT_MAX_WAIT,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ):
         """
         Retrieve Feature Effects computations for the model, requesting a new job if it hasn't been run previously.
 
         See :meth:`get_feature_effect_metadata \
         <datarobot.models.DatetimeModel.get_feature_effect_metadata>`
         for retrieving information of source, backtest_index.
 
@@ -4937,23 +5190,30 @@
 
         Returns
         -------
         feature_effects : FeatureEffects
            The feature effects data.
         """
         try:
-            feature_effect_job = self.request_feature_effect(backtest_index)
+            feature_effect_job = self.request_feature_effect(backtest_index, data_slice_filter)
         except JobAlreadyRequested as e:
             # if already requested it may be still running
             # check and get the jobid in that case
             qid = e.json["jobId"]
             from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
             feature_effect_job = Job.get(self.project_id, qid)
 
+        if data_slice_filter and data_slice_filter is not DATA_SLICE_WITH_ID_NONE:
+            # if we have slice that mean that feature_effect_job object is of type StatusCheckJob
+            feature_effect_job.wait_for_completion(max_wait=max_wait)
+            return self.get_feature_effect(
+                source=source, backtest_index=backtest_index, data_slice_filter=data_slice_filter
+            )
+
         params = {"source": source}
         return feature_effect_job.get_result_when_complete(max_wait=max_wait, params=params)
 
     # pylint: disable-next=arguments-renamed
     def request_feature_effects_multiclass(
         self,
         backtest_index,
@@ -5915,17 +6175,33 @@
             source=source,
             series_id=series_id,
             limit=limit,
             offset=offset,
             with_data_only=with_data_only,
         )
 
+    @staticmethod
+    def _get_source_for_feature_impact(backtest_index):
+        """Return source for Feature Impact"""
+        if backtest_index is None:
+            return INSIGHTS_SOURCES.TRAINING
+        else:
+            if backtest_index == INSIGHTS_SOURCES.HOLDOUT:
+                return "holdout_training"
+            else:
+                backtest_index = int(backtest_index)
+                backtest_index += 1
+                return "backtest_{}_training".format(str(backtest_index))
+
     def get_feature_impact(
-        self, with_metadata=False, backtest=None
-    ):  # pylint: disable=arguments-renamed,arguments-differ
+        self,
+        with_metadata=False,
+        backtest=None,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ):  # pylint: disable=arguments-renamed
         """
         Retrieve the computed Feature Impact results, a measure of the relevance of each
         feature in the model.
 
         Feature Impact is computed for each column by creating new data with that column randomly
         permuted (but the others left unchanged), and seeing how the error metric score for the
         predictions is affected. The 'impactUnnormalized' is how much worse the error metric score
@@ -5934,26 +6210,30 @@
 
         If a feature is a redundant feature, i.e. once other features are considered it doesn't
         contribute much in addition, the 'redundantWith' value is the name of feature that has the
         highest correlation with this feature. Note that redundancy detection is only available for
         jobs run after the addition of this feature. When retrieving data that predates this
         functionality, a NoRedundancyImpactAvailable warning will be used.
 
-        Elsewhere this technique is sometimes called 'Permutation Importance'.
+        Else where this technique is sometimes called 'Permutation Importance'.
 
         Requires that Feature Impact has already been computed with
         :meth:`request_feature_impact <datarobot.models.Model.request_feature_impact>`.
 
         Parameters
         ----------
         with_metadata : bool
             The flag indicating if the result should include the metadata as well.
         backtest : int or string
             The index of the backtest unless it is holdout then it is string 'holdout'. This is supported
             only in DatetimeModels
+        data_slice_filter : DataSlice, optional
+            (New in version v3.4) A data slice used to filter the return values based on the dataslice.id.
+            By default, this function will use data_slice_filter.id == None which returns an unsliced insight.
+            If data_slice_filter is None then get_roc_curve will raise a ValueError.
 
         Returns
         -------
         list or dict
             The feature impact data response depends on the with_metadata parameter. The response is
             either a dict with metadata and a list with actual data or just a list with that data.
 
@@ -5975,99 +6255,122 @@
               - ``count`` - An integer with the number of features under the ``featureImpacts``.
 
         Raises
         ------
         ClientError (404)
             If the feature impacts have not been computed.
         """
-        route = self._get_feature_impact_url()
-        params = {}
-        if backtest is not None:
-            params["backtest"] = backtest
-        data = self._client.get(route, params=params).json()
-        valid_vata = feature_impact_trafaret.check(data)
-        if not valid_vata["ranRedundancyDetection"]:
-            warnings.warn(
-                "Redundancy detection is not available for this model",
-                NoRedundancyImpactAvailable,
-                stacklevel=2,
-            )
-        from .job import (  # pylint: disable=import-outside-toplevel,cyclic-import
-            filter_feature_impact_result,
-        )
+        self._validate_data_slice_filter(data_slice_filter)
+
+        if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
+            data_slice_filter = DataSlice(id=None)
 
-        return filter_feature_impact_result(valid_vata, with_metadata=with_metadata)
+        params = self._data_slice_to_query_params(data_slice_filter)
+        params["source"] = self._get_source_for_feature_impact(backtest)
+        return self._make_get_insights_feature_impact_request(params, with_metadata)
 
     def request_feature_impact(
-        self, row_count=None, with_metadata=False, backtest=None
+        self,
+        row_count=None,
+        with_metadata=False,
+        backtest=None,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
     ):  # pylint: disable=arguments-renamed
         """
         Request feature impacts to be computed for the model.
 
         See :meth:`get_feature_impact <datarobot.models.Model.get_feature_impact>` for more
         information on the result of the job.
 
         Parameters
         ----------
         row_count : int
             The sample size (specified in rows) to use for Feature Impact computation. This is not
             supported for unsupervised, multi-class (that has a separate method) and time series
             projects.
+        with_metadata : bool
+            The flag indicating if the result should include the metadata as well.
         backtest : int or string
             The index of the backtest unless it is holdout then it is string 'holdout'. This is supported
             only in DatetimeModels
+        data_slice_filter : DataSlice, optional
+            (New in version v3.4) A data slice used to filter the return values based on the dataslice.id.
+            By default, this function will use data_slice_filter.id == None which returns an unsliced insight.
+            If data_slice_filter is None then get_roc_curve will raise a ValueError.
 
         Returns
         -------
          job : Job
             A Job representing the feature impact computation. To get the completed feature impact
             data, use `job.get_result` or `job.get_result_when_complete`.
 
         Raises
         ------
         JobAlreadyRequested (422)
             If the feature impacts have already been requested.
         """
         from .job import FeatureImpactJob  # pylint: disable=import-outside-toplevel,cyclic-import
 
+        if data_slice_filter and data_slice_filter is not DATA_SLICE_WITH_ID_NONE:
+            source = self._get_source_for_feature_impact(backtest)
+            return self._make_post_insights_feature_impact_request(
+                source=source, data_slice_id=data_slice_filter.id, row_count=row_count
+            )
+
         route = self._get_feature_impact_url()
         payload = {}
         if row_count is not None:
             payload["row_count"] = row_count
         if backtest is not None:
             payload["backtest"] = backtest
         response = self._client.post(route, data=payload)
         job_id = get_id_from_response(response)
         return FeatureImpactJob.get(self.project_id, job_id, with_metadata=with_metadata)
 
     # pylint: disable-next=arguments-differ
     def get_or_request_feature_impact(
-        self, max_wait=DEFAULT_MAX_WAIT, row_count=None, with_metadata=False, backtest=None
+        self,
+        max_wait=DEFAULT_MAX_WAIT,
+        row_count=None,
+        with_metadata=False,
+        backtest=None,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
     ):
         """
         Retrieve feature impact for the model, requesting a job if it hasn't been run previously
 
         Parameters
         ----------
         max_wait : int, optional
             The maximum time to wait for a requested feature impact job to complete before erroring
-        **kwargs
-            Arbitrary keyword arguments passed to
-            :meth:`request_feature_impact <datarobot.models.Model.request_feature_impact>`.
-
+        row_count : int
+            The sample size (specified in rows) to use for Feature Impact computation. This is not
+            supported for unsupervised, multi-class (that has a separate method) and time series
+            projects.
+        with_metadata : bool
+            The flag indicating if the result should include the metadata as well.
+        backtest : str
+            Feature Impact backtest. Can be 'holdout' or numbers from 0 up to max number of backtests in project.
+        data_slice_filter : DataSlice, optional
+            (New in version v3.4) A data slice used to filter the return values based on the dataslice.id.
+            By default, this function will use data_slice_filter.id == None which returns an unsliced insight.
+            If data_slice_filter is None then get_roc_curve will raise a ValueError.
         Returns
         -------
          feature_impacts : list or dict
             The feature impact data. See
             :meth:`get_feature_impact <datarobot.models.Model.get_feature_impact>` for the exact
             schema.
         """
         try:
             feature_impact_job = self.request_feature_impact(
-                row_count=row_count, with_metadata=with_metadata, backtest=backtest
+                row_count=row_count,
+                with_metadata=with_metadata,
+                backtest=backtest,
+                data_slice_filter=data_slice_filter,
             )
         except JobAlreadyRequested as e:
             # If already requested it may be still running. Check and get the job id in that case.
             qid = e.json["jobId"]
             if qid is None:
                 # There are rare cases, when existing (old) job can not be retrieved.
                 # Last resort: optimistically try to return an existing result.
@@ -6077,16 +6380,219 @@
                 FeatureImpactJob,
             )
 
             feature_impact_job = FeatureImpactJob.get(
                 self.project_id, qid, with_metadata=with_metadata
             )
 
+        if data_slice_filter and data_slice_filter is not DATA_SLICE_WITH_ID_NONE:
+            # if we have slice that mean that feature_impact_job object is of type StatusCheckJob
+            feature_impact_job.wait_for_completion(max_wait=max_wait)
+            return self.get_feature_impact(
+                backtest=backtest, data_slice_filter=data_slice_filter, with_metadata=with_metadata
+            )
+
         return feature_impact_job.get_result_when_complete(max_wait=max_wait)
 
+    @staticmethod
+    def _get_source_for_lift_and_roc(backtest_index):
+        if backtest_index == CHART_DATA_SOURCE.HOLDOUT:
+            return CHART_DATA_SOURCE.HOLDOUT
+        elif backtest_index == "0":
+            return CHART_DATA_SOURCE.VALIDATION
+        else:
+            backtest_index = int(backtest_index)
+            backtest_index += 1
+            return "backtest_{}".format(str(backtest_index))
+
+    # pylint: disable-next=arguments-renamed
+    def request_lift_chart(
+        self,
+        source: CHART_DATA_SOURCE = None,
+        backtest_index: str = None,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ) -> StatusCheckJob:
+        """
+        (New in version v3.4)
+        Request the model Lift Chart for the specified backtest data slice.
+
+        Parameters
+        ----------
+        source : str
+            (Deprecated in version v3.4)
+            Lift chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
+            If `backtest_index` is present then this will be ignored.
+        backtest_index : str
+            Lift chart data backtest. Can be 'holdout' or numbers from 0 up to max number of backtests in project.
+        data_slice_filter : DataSlice, optional
+            A data slice used to filter the return values based on the dataslice.id. By default this function will
+            use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
+            then request_lift_chart will raise a ValueError.
+
+        Returns
+        -------
+        status_check_job : StatusCheckJob
+            Object contains all needed logic for a periodical status check of an async job.
+        """
+
+        if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
+            data_slice_filter = DataSlice(id=None)
+
+        if backtest_index is not None:
+            source = self._get_source_for_lift_and_roc(backtest_index=backtest_index)
+
+        return super().request_lift_chart(source=source, data_slice_id=data_slice_filter.id)
+
+    # pylint: disable-next=arguments-renamed
+    def get_lift_chart(
+        self,
+        source: str = None,
+        backtest_index: str = None,
+        fallback_to_parent_insights: Optional[bool] = False,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ):
+        """
+        (New in version v3.4)
+        Retrieve the model Lift chart for the specified backtest and data slice.
+
+        Parameters
+        ----------
+        source : str
+            (Deprecated in version v3.4)
+            Lift chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
+            For time series and OTV models, also accepts values `backtest_2`, `backtest_3`, ...,
+            up to the number of backtests in the model.
+            If `backtest_index` is present then this will be ignored.
+        backtest_index : str
+            Lift chart data backtest. Can be 'holdout' or numbers from 0 up to max number of backtests in project.
+        fallback_to_parent_insights : bool
+            Optional, if True, this will return lift chart data for this
+            model's parent if the lift chart is not available for this model and the model has a
+            defined parent model. If omitted or False, or there is no parent model, will not
+            attempt to return insight data from this model's parent.
+        data_slice_filter : DataSlice, optional
+            A data slice used to filter the return values based on the dataslice.id. By default this function will
+            use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
+            then get_lift_chart will raise a ValueError.
+
+        Returns
+        -------
+        LiftChart
+            Model lift chart data
+
+        Raises
+        ------
+        ClientError
+            If the insight is not available for this model
+        ValueError
+            If data_slice_filter passed as None
+        """
+        if backtest_index is not None:
+            source = self._get_source_for_lift_and_roc(backtest_index=backtest_index)
+
+        return super().get_lift_chart(
+            source=source,
+            fallback_to_parent_insights=fallback_to_parent_insights,
+            data_slice_filter=data_slice_filter,
+        )
+
+    # pylint: disable-next=arguments-renamed
+    def request_roc_curve(
+        self,
+        source: CHART_DATA_SOURCE = None,
+        backtest_index: str = None,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ) -> StatusCheckJob:
+        """
+        (New in version v3.4)
+        Request the binary model Roc Curve for the specified backtest and data slice.
+
+        Parameters
+        ----------
+        source : str
+            (Deprecated in version v3.4)
+            Roc Curve data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
+            If `backtest_index` is present then this will be ignored.
+        backtest_index : str
+            ROC curve data backtest. Can be 'holdout' or numbers from 0 up to max number of backtests in project.
+        data_slice_filter : DataSlice, optional
+            A data slice used to filter the return values based on the dataslice.id. By default this function will
+            use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
+            then request_roc_curve will raise a ValueError.
+
+        Returns
+        -------
+        status_check_job : StatusCheckJob
+            Object contains all needed logic for a periodical status check of an async job.
+        """
+
+        if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
+            data_slice_filter = DataSlice(id=None)
+
+        if backtest_index is not None:
+            source = self._get_source_for_lift_and_roc(backtest_index=backtest_index)
+
+        return super().request_roc_curve(source=source, data_slice_id=data_slice_filter.id)
+
+    # pylint: disable-next=arguments-renamed
+    def get_roc_curve(
+        self,
+        source: str = None,
+        backtest_index: str = None,
+        fallback_to_parent_insights: bool = False,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
+    ):
+        """
+        (New in version v3.4)
+        Retrieve the ROC curve for a binary model for the specified backtest and data slice.
+
+        Parameters
+        ----------
+        source : str
+            (Deprecated in version v3.4)
+            ROC curve data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
+            For time series and OTV models, also accepts values `backtest_2`, `backtest_3`, ...,
+            up to the number of backtests in the model.
+            If `backtest_index` is present then this will be ignored.
+        backtest_index : str
+            ROC curve data backtest. Can be 'holdout' or numbers from 0 up to max number of backtests in project.
+        fallback_to_parent_insights : bool
+            Optional, if True, this will return ROC curve data for this
+            model's parent if the ROC curve is not available for this model and the model has a
+            defined parent model. If omitted or False, or there is no parent model, will not
+            attempt to return data from this model's parent.
+        data_slice_filter : DataSlice, optional
+            A data slice used to filter the return values based on the data slice.id. By default, this function will
+            use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
+            then get_roc_curve will raise a ValueError.
+
+        Returns
+        -------
+        RocCurve
+            Model ROC curve data
+
+        Raises
+        ------
+        ClientError
+            If the insight is not available for this model
+        TypeError
+            If the underlying project type is multilabel
+        ValueError
+            If data_slice_filter passed as None
+        """
+
+        if backtest_index is not None:
+            source = self._get_source_for_lift_and_roc(backtest_index=backtest_index)
+
+        return super().get_roc_curve(
+            source=source,
+            fallback_to_parent_insights=fallback_to_parent_insights,
+            data_slice_filter=data_slice_filter,
+        )
+
 
 class RatingTableModel(Model):
     """A model that has a rating table.
 
     All durations are specified with a duration string such as those returned
     by the :meth:`partitioning_methods.construct_duration_string
     <datarobot.helpers.partitioning_methods.construct_duration_string>` helper method.
@@ -6168,32 +6674,39 @@
         self,
         id=None,
         processes=None,
         featurelist_name=None,
         featurelist_id=None,
         project_id=None,
         sample_pct=None,
-        training_row_count=None,
-        training_duration=None,
-        training_start_date=None,
-        training_end_date=None,
         model_type=None,
         model_category=None,
         is_frozen=None,
         blueprint_id=None,
         metrics=None,
         rating_table_id=None,
         monotonic_increasing_featurelist_id=None,
         monotonic_decreasing_featurelist_id=None,
         supports_monotonic_constraints=None,
         is_starred=None,
         prediction_threshold=None,
         prediction_threshold_read_only=None,
         model_number=None,
+        parent_model_id=None,
         supports_composable_ml=None,
+        training_row_count=None,
+        training_duration=None,
+        training_start_date=None,
+        training_end_date=None,
+        data_selection_method=None,
+        time_window_sample_pct=None,
+        sampling_method=None,
+        model_family_full_name=None,
+        is_trained_into_validation=None,
+        is_trained_into_holdout=None,
     ) -> None:
         super().__init__(
             id=id,
             processes=processes,
             featurelist_name=featurelist_name,
             featurelist_id=featurelist_id,
             project_id=project_id,
@@ -6209,16 +6722,23 @@
             metrics=metrics,
             monotonic_increasing_featurelist_id=monotonic_increasing_featurelist_id,
             monotonic_decreasing_featurelist_id=monotonic_decreasing_featurelist_id,
             supports_monotonic_constraints=supports_monotonic_constraints,
             is_starred=is_starred,
             prediction_threshold=prediction_threshold,
             prediction_threshold_read_only=prediction_threshold_read_only,
-            model_number=model_number,
             supports_composable_ml=supports_composable_ml,
+            model_family_full_name=model_family_full_name,
+            model_number=model_number,
+            parent_model_id=parent_model_id,
+            data_selection_method=data_selection_method,
+            time_window_sample_pct=time_window_sample_pct,
+            sampling_method=sampling_method,
+            is_trained_into_validation=is_trained_into_validation,
+            is_trained_into_holdout=is_trained_into_holdout,
         )
         self.rating_table_id = rating_table_id
 
     def __repr__(self) -> str:
         return f"RatingTableModel({self.model_type or self.id!r})"
 
     @classmethod
```

### Comparing `datarobot-3.3.2/datarobot/models/model_registry/deployment.py` & `datarobot-3.4.0/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/model_registry/registered_model.py` & `datarobot-3.4.0/datarobot/models/model_registry/registered_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,30 +36,30 @@
     type: str
 
 
 class RegisteredModelVersionsListFilters:
     """
     Filters for listing of registered model versions.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     target_name: str or None
         Name of the target to filter by.
     target_type: str or None
         Type of the target to filter by.
     compatible_with_leaderboard_model_id: str or None.
         If specified, limit results to versions (model packages) of the Leaderboard model with the specified ID.
     compatible_with_model_package_id: str or None.
-        Returns versions compatible with the given model package ID. If used, it will only return versions that match
-        `target.name`, `target.type`, `target.classNames` (for classification models), `modelKind.isTimeSeries`,
-        and `modelKind.isMultiseries` for the specified model package.
+        Returns versions compatible with the given model package (version) ID. If used, it will only return versions
+        that match `target.name`, `target.type`, `target.classNames` (for classification models),
+        `modelKind.isTimeSeries` and `modelKind.isMultiseries` for the specified model package (version).
     for_challenger: bool or None
         Can be used with compatibleWithModelPackageId to request similar versions that can be used as challenger
-        models; for external model packages, instead of returning similar external model packages,
-        similar DataRobot and Custom model packages will be retrieved.
+        models; for external model packages (versions), instead of returning similar external model packages (versions),
+        similar DataRobot and Custom model packages (versions) will be retrieved.
     prediction_threshold: float or None
         Return versions with the specified prediction threshold used for binary classification models.
     imported: bool or None
         If specified, return either imported (true) or non-imported (false) versions (model packages).
     prediction_environment_id: str or None
         Can be used to filter versions (model packages) by what is supported by the prediction environment
     model_kind: str or None
@@ -152,23 +152,23 @@
         Type of the target to filter by.
     created_by : str
         Email of the user that created registered model to filter by.
     compatible_with_leaderboard_model_id : str
         If specified, limit results to registered models containing versions (model packages)
         for the leaderboard model with the specified ID.
     compatible_with_model_package_id : str
-        Return registered models that have versions (model packages) compatible with given model package ID.
+        Return registered models that have versions (model packages) compatible with given model package (version) ID.
         If used, will only return registered models which have versions that match `target.name`, `target.type`,
         `target.classNames` (for classification models), `modelKind.isTimeSeries`, and `modelKind.isMultiseries`
-        of the specified model package.
+        of the specified model package (version).
     for_challenger : bool
         Can be used with compatibleWithModelPackageId to request similar registered models that contain
-        versions (model packages) that can be used as challenger models; for external model packages,
-        instead of returning similar external model packages, similar DataRobot and Custom model packages will be
-        retrieved.
+        versions (model packages) that can be used as challenger models; for external model packages (versions),
+        instead of returning similar external model packages (versions), similar DataRobot and Custom model packages
+        will be retrieved.
     prediction_threshold : float
         If specified, return any registered models containing one or more versions matching the prediction
         threshold used for binary classification models.
     imported : bool
         If specified, return any registered models that contain either imported (true) or non-imported (false)
         versions (model packages).
     prediction_environment_id : str
@@ -258,15 +258,15 @@
         return query_args
 
 
 TRegisteredModel = TypeVar("TRegisteredModel", bound="RegisteredModel")
 
 
 class RegisteredModel(APIObject, BrowserMixin):
-    """A registered model is a logical grouping of model packages that are related to each other.
+    """A registered model is a logical grouping of model packages (versions) that are related to each other.
 
     Attributes
     ----------
     id : str
         The ID of the registered model.
     name : str
         The name of the registered model.
```

### Comparing `datarobot-3.3.2/datarobot/models/model_registry/registered_model_version.py` & `datarobot-3.4.0/datarobot/models/model_registry/registered_model_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,38 @@
 class MlpkgFileContents(TypedDict):
     all_time_series_prediction_intervals: Optional[bool]
 
 
 class ModelDescription(TypedDict):
     description: Optional[str]
     model_name: Optional[str]
+    model_creator_id: Optional[str]
+    model_creator_name: Optional[str]
+    model_creator_email: Optional[str]
+    model_created_at: Optional[str]
     location: Optional[str]
     build_environment_type: Optional[str]
 
 
-class Dataset(TypedDict):
+class Dataset(TypedDict):  # pylint: disable=missing-class-docstring
     dataset_name: Optional[str]
     training_data_catalog_id: Optional[str]
+    training_data_catalog_version_id: Optional[str]
+    training_data_creator_id: Optional[str]
+    training_data_creator_name: Optional[str]
+    training_data_creator_email: Optional[str]
+    training_data_created_at: Optional[str]
     training_data_size: Optional[int]
     holdout_dataset_name: Optional[str]
     holdout_data_catalog_id: Optional[str]
+    holdout_data_catalog_version_id: Optional[str]
+    holdout_data_creator_id: Optional[str]
+    holdout_data_creator_name: Optional[str]
+    holdout_data_creator_email: Optional[str]
+    holdout_data_created_at: Optional[str]
     target_histogram_baseline: Optional[str]
     baseline_segmented_by: Optional[str]
 
 
 class BiasAndFairness(TypedDict):
     protected_features: Optional[List[str]]
     preferable_target_value: Optional[Union[str, int, bool]]
@@ -123,29 +137,44 @@
 class ScoringCodeMeta(TypedDict):
     location: Optional[str]
     data_robot_prediction_version: Optional[str]
 
 
 class UseCaseDetails(TypedDict):
     id: Optional[str]
+    name: Optional[str]
     creator_name: Optional[str]
     creator_id: str
     creator_email: Optional[str]
     created_at: str
 
 
-class SourceMeta(TypedDict):
+class CustomModelDetails(TypedDict):
+    id: Optional[str]
+    creator_name: Optional[str]
+    creator_id: str
+    creator_email: Optional[str]
+    created_at: str
+    version_label: Optional[str]
+
+
+class SourceMeta(TypedDict):  # pylint: disable=missing-class-docstring
     project_id: Optional[str]
     project_name: Optional[str]
+    project_creator_id: Optional[str]
+    project_creator_name: Optional[str]
+    project_creator_email: Optional[str]
+    project_created_at: Optional[str]
     environment_url: Optional[str]
     scoring_code: Optional[ScoringCodeMeta]
     decision_flow_id: Optional[str]
     decision_flow_version_id: Optional[str]
     fips_140_2_enabled: Optional[bool]
     use_case_details: Optional[UseCaseDetails]
+    custom_model_details: Optional[CustomModelDetails]
 
 
 TRegisteredModelVersion = TypeVar("TRegisteredModelVersion", bound="RegisteredModelVersion")
 
 
 class RegisteredModelVersion(APIObject):
     """
@@ -160,22 +189,22 @@
     registered_model_version : int
         The version of the registered model.
     name : str
         The name of the registered model version.
     model_id : str
         The ID of the model.
     model_execution_type : str
-        Type of model package. `dedicated` (native DataRobot models) and
+        Type of model package (version). `dedicated` (native DataRobot models) and
         custom_inference_model` (user added inference models) both execute on DataRobot
         prediction servers, `external` do not
     is_archived : bool
-        Whether the model package(version) is permanently archived (cannot be used in deployment or
+        Whether the model package (version) is permanently archived (cannot be used in deployment or
             replacement)
     import_meta : ImportMeta
-        Information from when this Model Package was first saved.
+        Information from when this Model Package (version) was first saved.
     source_meta : SourceMeta
         Meta information from where this model was generated
     model_kind : ModelKind
         Model attribute information.
     target : Target
         Target information for the registered model version.
     model_description : ModelDescription
@@ -183,22 +212,22 @@
     datasets : Dataset
         Dataset information for the registered model version.
     timeseries : Timeseries
         Timeseries information for the registered model version.
     bias_and_fairness : BiasAndFairness
         Bias and fairness information for the registered model version.
     is_deprecated : bool
-        Whether the model package(version) is deprecated (cannot be used in deployment or
+        Whether the model package (version) is deprecated (cannot be used in deployment or
             replacement)
     permissions : List[str]
         Permissions for the registered model version.
     active_deployment_count : int or None
         Number of the active deployments associated with the registered model version.
     build_status : str or None
-        Model package build status. One of `complete`, `inProgress`, `failed`.
+        Model package (version) build status. One of `complete`, `inProgress`, `failed`.
     user_provided_id : str or None
         User provided ID for the registered model version.
     updated_at : str or None
         The time the registered model version was last updated.
     updated_by : UserMetadata or None
         The user who last updated the registered model version.
     tags : List[TagWithId] or None
@@ -318,20 +347,20 @@
             ID of the DataRobot distribution prediction model
             trained on predictions from the DataRobot model.
         description : str or None
             Description of the version (model package).
         compute_all_ts_intervals : bool or None
             Whether to compute all time series prediction intervals (1-100 percentiles).
         registered_model_name : Optional[str]
-            Name of the new registered model that will be created from this model package.
-            The model package will be created as version 1 of the created registered model.
+            Name of the new registered model that will be created from this model package (version).
+            The model package (version) will be created as version 1 of the created registered model.
             If neither registeredModelName nor registeredModelId is provided,
-            it defaults to the model package name. Mutually exclusive with registeredModelId.
+            it defaults to the model package (version) name. Mutually exclusive with registeredModelId.
         registered_model_id : Optional[str]
-            Creates a model package as a new version for the provided registered model ID.
+            Creates a model package (version) as a new version for the provided registered model ID.
             Mutually exclusive with registeredModelName.
         tags : Optional[List[Tag]]
             Tags for the registered model version.
         registered_model_tags: Optional[List[Tag]]
             Tags for the registered model.
         registered_model_description: Optional[str]
             Description for the registered model.
@@ -399,20 +428,20 @@
         model_description : Optional[ModelDescription]
             Information about the model.
         datasets : Optional[ExternalDatasets]
             Dataset information for the registered model version.
         timeseries : Optional[Timeseries]
             Timeseries properties for the registered model version.
         registered_model_name : Optional[str]
-            Name of the new registered model that will be created from this model package.
-            The model package will be created as version 1 of the created registered model.
+            Name of the new registered model that will be created from this model package (version).
+            The model package (version) will be created as version 1 of the created registered model.
             If neither registeredModelName nor registeredModelId is provided,
-            it defaults to the model package name. Mutually exclusive with registeredModelId.
+            it defaults to the model package (version) name. Mutually exclusive with registeredModelId.
         registered_model_id : Optional[str]
-            Creates a model package as a new version for the provided registered model ID.
+            Creates a model package (version) as a new version for the provided registered model ID.
             Mutually exclusive with registeredModelName.
         tags : Optional[List[Tag]]
             Tags for the registered model version.
         registered_model_tags: Optional[List[Tag]]
             Tags for the registered model.
         registered_model_description: Optional[str]
             Description for the registered model.
@@ -470,20 +499,20 @@
         custom_model_version_id : str
             ID of the custom model version.
         name : Optional[str]
             Name of the registered model version.
         description : Optional[str]
             Description of the registered model version.
         registered_model_name : Optional[str]
-            Name of the new registered model that will be created from this model package.
-            The model package will be created as version 1 of the created registered model.
+            Name of the new registered model that will be created from this model package (version).
+            The model package (version) will be created as version 1 of the created registered model.
             If neither registeredModelName nor registeredModelId is provided,
-            it defaults to the model package name. Mutually exclusive with registeredModelId.
+            it defaults to the model package (version) name. Mutually exclusive with registeredModelId.
         registered_model_id : Optional[str]
-            Creates a model package as a new version for the provided registered model ID.
+            Creates a model package (version) as a new version for the provided registered model ID.
             Mutually exclusive with registeredModelName.
         tags : Optional[List[Tag]]
             Tags for the registered model version.
         registered_model_tags: Optional[List[Tag]]
             Tags for the registered model.
         registered_model_description: Optional[str]
             Description for the registered model.
```

### Comparing `datarobot-3.3.2/datarobot/models/modeljob.py` & `datarobot-3.4.0/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/pairwise_statistics.py` & `datarobot-3.4.0/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/pareto_front.py` & `datarobot-3.4.0/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/payoff_matrix.py` & `datarobot-3.4.0/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/predict_job.py` & `datarobot-3.4.0/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/prediction_dataset.py` & `datarobot-3.4.0/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/prediction_environment.py` & `datarobot-3.4.0/datarobot/models/prediction_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         The description of the prediction environment.
     platform: str, optional
         Indicates which platform is in use (AWS, GCP, DataRobot, etc.).
     permissions: list, optional
         A set of permissions for the prediction environment.
     is_deleted: boolean, optional
         The flag that shows if this prediction environment deleted.
-    supported_model_formats: list, optional
-        The list of supported model formats (datarobot, datarobotScoringCode, customModel, externalModel).
+    supported_model_formats: list[PredictionEnvironmentModelFormats], optional
+        The list of supported model formats.
     is_managed_by_management_agent : boolean, optional
         Determines if the prediction environment should be managed by the management agent. False by default.
     datastore_id : str, optional
         The ID of the data store connection configuration.
         Only applicable for external prediction environments managed by DataRobot.
     credential_id : str, optional
         The ID of the credential associated with the data connection.
@@ -142,15 +142,15 @@
             self.platform,
             self.description,
         )
 
     @classmethod
     def list(cls) -> List[PredictionEnvironment]:
         """
-        Returns list of available extrenal prediction environments.
+        Returns list of available external prediction environments.
 
         Returns
         -------
         prediction_environments : list of PredictionEnvironment instances
             contains a list of available prediction environments.
 
         Examples
@@ -231,17 +231,17 @@
             The name of the prediction environment.
         description : str, optional
             The description of the prediction environment.
         platform : str
             Indicates which platform is in use (AWS, GCP, DataRobot, etc.).
         plugin : str
             Optional. The plugin name to use.
-        supported_model_formats : list, optional
-            The list of supported model formats [datarobot, datarobotScoringCode, customModel, externalModel].
-            When not provided , the default value is inferred based on platform, (DataRobot platform: DataRobot,
+        supported_model_formats : list[PredictionEnvironmentModelFormats], optional
+            The list of supported model formats.
+            When not provided, the default value is inferred based on platform, (DataRobot platform: DataRobot,
             Custom Models; All other platforms: DataRobot, Custom Models, External Models).
         is_managed_by_management_agent : boolean, optional
             Determines if this prediction environment should be managed by the management agent. default: False
         datastore : DataStore|str, optional]
             The datastore object or ID of the data store connection configuration.
             Only applicable for external Prediction Environments managed by DataRobot.
         credential : Credential|str, optional]
```

### Comparing `datarobot-3.3.2/datarobot/models/prediction_explanations.py` & `datarobot-3.4.0/datarobot/models/prediction_explanations.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,32 +251,37 @@
         explanations to be computed for a row in the dataset
     num_columns : int
         the number of columns prediction explanations were computed for
     finish_time : float
         timestamp referencing when computation for these prediction explanations finished
     prediction_explanations_location : str
         where to retrieve the prediction explanations
+    source: str
+        For OTV/TS in-training predictions. Holds the portion of the training dataset used to generate
+        predictions.
     """
 
     _path_template = "projects/{}/predictionExplanationsRecords/"
     _expls_path_template = "projects/{}/predictionExplanations/"
+    _training_path_template = "projects/{}/predictionExplanationsOnTrainingData/"
     _converter = t.Dict(
         {
             t.Key("id"): String,
             t.Key("project_id"): String,
             t.Key("model_id"): String,
             t.Key("dataset_id"): String,
             t.Key("max_explanations"): Int,
             t.Key("threshold_low", optional=True): t.Float,
             t.Key("threshold_high", optional=True): t.Float,
             t.Key("class_names", optional=True): t.List(t.String),
             t.Key("num_top_classes", optional=True): t.Int(),
             t.Key("num_columns"): Int,
             t.Key("finish_time"): t.Float,
             t.Key("prediction_explanations_location"): String,
+            t.Key("source", optional=True): String,
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id,
         project_id,
@@ -286,27 +291,29 @@
         num_columns,
         finish_time,
         prediction_explanations_location,
         threshold_low=None,
         threshold_high=None,
         class_names=None,
         num_top_classes=None,
+        source=None,
     ):
         self.project_id = project_id
         self.model_id = model_id
         self.dataset_id = dataset_id
         self.max_explanations = max_explanations
         self.threshold_low = threshold_low
         self.threshold_high = threshold_high
         self.id = id
         self.num_columns = num_columns
         self.finish_time = datetime.fromtimestamp(finish_time)
         self.prediction_explanations_location = prediction_explanations_location
         self.class_names = class_names
         self.num_top_classes = num_top_classes
+        self.source = source
 
         self._path = self._path_template.format(self.project_id)
 
     def __repr__(self):
         return "{}(id={}, project_id={}, model_id={})".format(
             type(self).__name__, self.id, self.project_id, self.model_id
         )
@@ -381,14 +388,15 @@
         max_explanations : int, optional
             the maximum number of prediction explanations to supply per row of the dataset,
             default: 3.
         mode : PredictionExplanationsMode, optional
             mode of calculation for multiclass models, if not specified - server default is
             to explain only the predicted class, identical to passing TopPredictionsMode(1).
 
+
         Returns
         -------
         job: Job
             an instance of created async job
         """
         from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
@@ -400,19 +408,111 @@
             payload["max_explanations"] = max_explanations
         if threshold_low is not None:
             payload["threshold_low"] = threshold_low
         if threshold_high is not None:
             payload["threshold_high"] = threshold_high
         if mode is not None:
             payload.update(mode.get_api_parameters(batch_route=False))
+
         response = cls._client.post(cls._expls_path_template.format(project_id), data=payload)
         job_id = get_id_from_response(response)
         return Job.get(project_id, job_id)
 
     @classmethod
+    def create_on_training_data(
+        cls,
+        project_id,
+        model_id,
+        dataset_id,
+        max_explanations=None,
+        threshold_low=None,
+        threshold_high=None,
+        mode=None,
+        datetime_prediction_partition=None,
+    ):
+        """
+        Create prediction explanations for the the dataset used to train the model.
+        This can be retrieved by calling ``dr.Model.get().featurelist_id``.
+        For OTV and timeseries projects, ``datetime_prediction_partition`` is required and limited to the
+        first backtest ('0') or holdout ('holdout').
+
+        In order to create PredictionExplanations for a particular model and dataset, you must
+        first:
+
+          * Compute Feature Impact for the model via ``datarobot.Model.get_feature_impact()``/
+          * Compute a PredictionExplanationsInitialization for the model via
+            ``datarobot.PredictionExplanationsInitialization.create(project_id, model_id)``.
+          * Compute predictions for the model and dataset via
+            ``datarobot.Model.request_predictions(dataset_id)``.
+
+        ``threshold_high`` and ``threshold_low`` are optional filters applied to speed up
+        computation.  When at least one is specified, only the selected outlier rows will have
+        prediction explanations computed. Rows are considered to be outliers if their predicted
+        value (in case of regression projects) or probability of being the positive
+        class (in case of classification projects) is less than ``threshold_low`` or greater than
+        ``thresholdHigh``.  If neither is specified, prediction explanations will be computed for
+        all rows.
+
+        Parameters
+        ----------
+        project_id : str
+            The ID of the project the model belongs to.
+        model_id : str
+            The ID of the model for which prediction explanations are requested.
+        dataset_id : str
+            The ID of the prediction dataset for which prediction explanations are requested.
+        threshold_low : float, optional
+            The lower threshold, below which a prediction must score in order for prediction
+            explanations to be computed for a row in the dataset. If neither ``threshold_high`` nor
+            ``threshold_low`` is specified, prediction explanations will be computed for all rows.
+        threshold_high : float, optional
+            The high threshold, above which a prediction must score in order for prediction
+            explanations to be computed. If neither ``threshold_high`` nor ``threshold_low`` is
+            specified, prediction explanations will be computed for all rows.
+        max_explanations : int, optional
+            The maximum number of prediction explanations to supply per row of the dataset
+            (default: 3).
+        mode : PredictionExplanationsMode, optional
+            The mode of calculation for multiclass models. If not specified, the server default is
+            to explain only the predicted class, identical to passing TopPredictionsMode(1).
+        datetime_prediction_partition: str
+            Options: '0', 'holdout' or None.
+            Used only by time series and OTV projects to indicate what part of the dataset
+            will be used to generate predictions for computing prediction explanation. Current
+            options are '0' (first backtest) and 'holdout'.
+            Note that only the validation partition of the first backtest will be used to
+            generation predictions.
+
+        Returns
+        -------
+        job: Job
+            An instance of created async job.
+        """
+        from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
+
+        payload = {
+            "model_id": model_id,
+            "dataset_id": dataset_id,
+        }
+        if max_explanations is not None:
+            payload["max_explanations"] = max_explanations
+        if threshold_low is not None:
+            payload["threshold_low"] = threshold_low
+        if threshold_high is not None:
+            payload["threshold_high"] = threshold_high
+        if mode is not None:
+            payload.update(mode.get_api_parameters(batch_route=False))
+        if datetime_prediction_partition is not None:
+            payload["datetime_prediction_partition"] = datetime_prediction_partition
+
+        response = cls._client.post(cls._training_path_template.format(project_id), data=payload)
+        job_id = get_id_from_response(response)
+        return Job.get(project_id, job_id)
+
+    @classmethod
     def list(cls, project_id, model_id=None, limit=None, offset=None):
         """
         List of prediction explanations metadata for a specified project.
 
         Parameters
         ----------
         project_id : str
@@ -468,15 +568,15 @@
         # This method will exist now only to maintain backwards compatibility.
 
         return (self.num_top_classes or self.class_names) and ProjectOptions.get(
             project_id=self.project_id
         ).target == TARGET_TYPE.MULTICLASS
 
     def is_unsupervised_clustering_or_multiclass(self):
-        """Clustering and muliclass XEMP always has either one of num_top_classes or class_names
+        """Clustering and multiclass XEMP always has either one of num_top_classes or class_names
         parameters set"""
         return bool(self.num_top_classes or self.class_names)
 
     def get_number_of_explained_classes(self):
         """How many classes we attempt to explain for each row"""
         if self.is_unsupervised_clustering_or_multiclass():
             return self.num_top_classes or len(self.class_names)
```

### Comparing `datarobot-3.3.2/datarobot/models/prediction_server.py` & `datarobot-3.4.0/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/predictions.py` & `datarobot-3.4.0/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/prime_file.py` & `datarobot-3.4.0/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/project.py` & `datarobot-3.4.0/datarobot/models/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from datarobot.models.model import (
     BiasMitigatedModelInfo,
     BiasMitigationFeatureInfo,
     BlenderModel,
     CombinedModel,
     DatetimeModel,
     FrozenModel,
+    GenericModel,
     Model,
     PrimeModel,
     RatingTableModel,
 )
 from datarobot.models.modeljob import ModelJob
 from datarobot.models.predict_job import PredictJob
 from datarobot.models.prediction_dataset import PredictionDataset
@@ -128,24 +129,39 @@
         credentialType: CredentialTypes
 
     class BasicCredentialsDataDict(BaseCredentialsDataDict):
         user: str
         password: str
 
     class S3CredentialsDataDict(BaseCredentialsDataDict):
-        awsAccessKeyId: str
-        awsSecretAccessKey: str
-        awsSessionToken: str
+        awsAccessKeyId: Optional[str]
+        awsSecretAccessKey: Optional[str]
+        awsSessionToken: Optional[str]
+        configId: Optional[str]
 
     class OAuthCredentialsDataDict(BaseCredentialsDataDict):
         oauthRefreshToken: str
         oauthClientId: str
         oauthClientSecret: str
         oauthAccessToken: str
 
+    class SnowflakeKeyPairCredentialsDataDict(BaseCredentialsDataDict):
+        user: Optional[str]
+        privateKeyStr: Optional[str]
+        passphrase: Optional[str]
+        configId: Optional[str]
+
+    class DatabricksAccessTokenCredentialsDataDict(BaseCredentialsDataDict):
+        databricksAccessToken: str
+
+    class DatabricksServicePrincipalCredentialsDataDict(BaseCredentialsDataDict):
+        clientId: Optional[str]
+        clientSecret: Optional[str]
+        configId: Optional[str]
+
     class BasicCredentialsDict(TypedDict):
         user: str
         password: str
 
     class CredentialIdCredentialsDict(TypedDict):
         credentialId: str
 
@@ -259,14 +275,18 @@
             t.Key("external_time_series_baseline_dataset_id", optional=True): t.String(),
             t.Key("bias_mitigation_feature_name", optional=True): t.String(),
             t.Key("bias_mitigation_technique", optional=True): t.String(),
             t.Key("include_bias_mitigation_feature_as_predictor_variable", optional=True): t.Bool(),
             t.Key("model_group_id", optional=True): String(),
             t.Key("model_regime_id", optional=True): String(),
             t.Key("model_baselines", optional=True): t.List(String()),
+            t.Key("incremental_learning_only_mode", optional=True): t.Bool(),
+            t.Key("incremental_learning_on_best_model", optional=True): t.Bool(),
+            t.Key("chunk_definition_id", optional=True): t.String(),
+            t.Key("incremental_learning_early_stopping_rounds", optional=True): Int(),
         }
     ).ignore_extra("*")
 
     _feature_engineering_graph_converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("linkage_keys", optional=True): t.List(String, min_length=1, max_length=10),
@@ -427,15 +447,15 @@
     @_options.setter
     def _options(self, options: Optional[ProjectOptions]) -> None:
         self.__options = options
 
     def set_options(self, options: Optional[AdvancedOptions] = None, **kwargs: Any) -> None:
         """Update the advanced options of this project.
 
-        Either accepts an AdvancedOptions object or indiviudal keyword arguments.
+        Either accepts an AdvancedOptions object or individual keyword arguments.
         This is an inplace update.
 
         Raises
         ------
         ValueError
             Raised if an object passed to the ``options`` parameter is not an ``AdvancedOptions`` instance,
             a valid keyword argument from the ``AdvancedOptions`` class, or a combination of an ``AdvancedOptions``
@@ -1082,20 +1102,22 @@
         autopilot_with_feature_discovery: Optional[bool] = None,
         feature_discovery_supervised_feature_reduction: Optional[bool] = None,
         unsupervised_type: Optional[UnsupervisedTypeEnum] = None,
         autopilot_cluster_list: Optional[List[int]] = None,
         bias_mitigation_feature_name: Optional[str] = None,
         bias_mitigation_technique: Optional[str] = None,
         include_bias_mitigation_feature_as_predictor_variable: Optional[bool] = None,
+        incremental_learning_only_mode: Optional[bool] = None,
+        incremental_learning_on_best_model: Optional[bool] = None,
     ) -> TProject:
         """
         Chain together project creation, file upload, and target selection.
 
         .. note:: While this function provides a simple means to get started, it does not expose
-            all possible parameters. For advanced usage, using ``create``, ``set_options``
+            all possible parameters. For advanced usage, using ``create``, ``set_advanced_options``
             and ``analyze_and_model`` directly is recommended.
 
         Parameters
         ----------
         sourcedata : str or pandas.DataFrame
             The path to the file to upload. Can be either a path to a
             local file or a publicly accessible URL (starting with ``http://``, ``https://``,
@@ -1252,14 +1274,16 @@
             autopilot_with_feature_discovery=autopilot_with_feature_discovery,
             feature_discovery_supervised_feature_reduction=sfd,
             bias_mitigation_feature_name=bias_mitigation_feature_name,
             bias_mitigation_technique=bias_mitigation_technique,
             include_bias_mitigation_feature_as_predictor_variable=(
                 include_bias_mitigation_feature_as_predictor_variable
             ),
+            incremental_learning_only_mode=incremental_learning_only_mode,
+            incremental_learning_on_best_model=incremental_learning_on_best_model,
         )
 
         project.analyze_and_model(
             target=target,
             metric=metric,
             mode=mode,
             worker_count=worker_count,
@@ -1325,15 +1349,15 @@
             p_list
             >>> [Project('Project One'), Project('Two')]
 
         Search for projects by name
         .. code-block:: python
 
             Project.list(search_params={'project_name': 'red'})
-            >>> [Project('Predtime'), Project('Fred Project')]
+            >>> [Project('Prediction Time'), Project('Fred Project')]
 
         List 2nd and 3rd projects
         .. code-block:: python
 
             Project.list(offset=1, limit=2)
             >>> [Project('Project 2'), Project('Project 3')]
 
@@ -1344,15 +1368,15 @@
                 get_params.update(search_params)
             else:
                 raise TypeError(
                     "Provided search_params argument {} is invalid type {}".format(
                         search_params, type(search_params)
                     )
                 )
-        # This is a special case we needed to cover. A user could pass in "experiment_container_id" themselves to
+        # This is a special case we needed to cover. A user could pass in "use_case_id" themselves to
         # `search_params`, so we need to check for that and default to `use_cases` if that was passed in.
         # Then we proceed to check if resolve_use_case(`use_case_id`) arg was set, and use a global use case if
         # it's available.
         get_params = resolve_use_cases(use_cases=use_cases, params=get_params)
         r_data = cls._client.get(cls._path, params=get_params).json()
         return [cls.from_server_data(item) for item in r_data]
 
@@ -1821,20 +1845,107 @@
             relationships_configuration_id=relationships_configuration_id,
             class_mapping_aggregation_settings=class_mapping_aggregation_settings,
             segmentation_task_id=segmentation_task_id,
             unsupervised_type=unsupervised_type,
             autopilot_cluster_list=autopilot_cluster_list,
         )
 
+    def get_model_records(
+        self,
+        # sorting
+        sort_by_partition: Optional[str] = "validation",
+        sort_by_metric: Optional[str] = None,
+        # if result should contain specific metric, not all of them
+        with_metric: Optional[str] = None,
+        # search in model name or processes,
+        search_term: Optional[str] = None,
+        # filtering options
+        featurelists: Optional[List[str]] = None,
+        families: Optional[List[str]] = None,
+        blueprints: Optional[List[str]] = None,
+        labels: Optional[List[str]] = None,
+        characteristics: Optional[List[str]] = None,
+        training_filters: Optional[List[Any]] = None,
+        # pagination
+        limit: int = 100,
+        offset: int = 0,
+    ) -> List[GenericModel]:
+        """
+        Retrieve paginated model records, sorted by scores, with optional filtering.
+
+        Parameters
+        ----------
+        sort_by_partition: str, one of `validation`, `backtesting`, `crossValidation` or `holdout`
+            Set the partition to use for sorted (by score) list of models. `validation` is the default.
+        sort_by_metric: str
+            Set the project metric to use for model sorting. DataRobot-selected project optimization metric
+             is the default.
+        with_metric: str
+            For a single-metric list of results, specify that project metric.
+        search_term: str
+            If specified, only models containing the term in their name or processes are returned.
+        featurelists: list of str
+           If specified, only models trained on selected featurelists are returned.
+        families: list of str
+            If specified, only models belonging to selected families are returned.
+        blueprints: list of str
+             If specified, only models trained on specified blueprint IDs are returned.
+        labels: list of str, `starred` or `prepared for deployment`
+            If specified, only models tagged with all listed labels are returned.
+        characteristics: list of str
+            If specified, only models matching all listed characteristics are returned.
+        training_filters: list of str
+            If specified, only models matching at least one of the listed training conditions are returned.
+            The following formats are supported for autoML and datetime partitioned projects:
+            - number of rows in training subset
+            For datetime partitioned projects:
+            - <training duration>, example `P6Y0M0D`
+            - <training_duration>-<time_window_sample_percent>-<sampling_method> Example: `P6Y0M0D-78-Random`,
+            (returns models trained on 6 years of data, sampling rate 78%, random sampling).
+            - `Start/end date`
+            - `Project settings`
+        limit: int
+        offset: int
+
+        Returns
+        -------
+        generic_models: list of GenericModel
+        """
+
+        return GenericModel.list(
+            self.id,
+            sort_by_partition=sort_by_partition,
+            sort_by_metric=sort_by_metric,
+            with_metric=with_metric,
+            search_term=search_term,
+            featurelists=featurelists,
+            families=families,
+            blueprints=blueprints,
+            labels=labels,
+            characteristics=characteristics,
+            training_filters=training_filters,
+            limit=limit,
+            offset=offset,
+        )
+
+    @deprecated(
+        deprecated_since_version="3.4",
+        will_remove_version="3.7",
+        message="Use get_model_records instead. Flag `use_new_models_retrieval` = True will be the only "
+        "available option in 3.6. New retrieval route supports filtering and returns fewer attributes per "
+        "individual model.",
+    )
     def get_models(
         self,
         order_by: Optional[Union[str, List[str]]] = None,
         search_params: Optional[Dict[str, Any]] = None,
         with_metric: Optional[str] = None,
-    ) -> List[Optional[Model]]:
+        # will be changed to True in 3.6
+        use_new_models_retrieval=False,
+    ) -> Union[List[Model], List[GenericModel]]:
         """
         List all completed, successful models in the leaderboard for the given project.
 
         Parameters
         ----------
         order_by : str or list of strings, optional
             If not `None`, the returned models are ordered by this
@@ -1861,19 +1972,22 @@
             * ``name``
             * ``sample_pct``
             * ``is_starred``
 
         with_metric : str, optional.
             If not `None`, the returned models will only have scores for this
             metric. Otherwise all the metrics are returned.
+        use_new_models_retrieval: bool, False by default
+            Use new retrieval route, which supports filtering and returns fewer attributes per
+            individual model.
 
         Returns
         -------
-        models : a list of Model instances.
-            All of the models that have been trained in this project.
+        models : a list of Model or a list of GenericModel if `use_new_models_retrieval` is True.
+            All models trained in the project.
 
         Raises
         ------
         TypeError
             Raised if ``order_by`` or ``search_params`` parameter is provided,
             but is not of supported type.
 
@@ -1892,14 +2006,24 @@
                     'sample_pct__gt': 64,
                     'name': "Ridge"
                 })
 
             # Filtering models based on 'starred' flag:
             Project.get('pid').get_models(search_params={'is_starred': True})
         """
+        if use_new_models_retrieval:
+            labels, search_term = None, None
+            if isinstance(search_params, dict):
+                if search_params.get("is_starred"):
+                    labels = ["starred"]
+                search_term = search_params.get("name")
+            # experimental option
+            return self.get_model_records(
+                with_metric=with_metric, limit=0, offset=0, labels=labels, search_term=search_term
+            )
         url = f"{self._path}{self.id}/models/"
         get_params = {}
         if order_by is not None:
             order_by = self._canonize_order_by(order_by)
             get_params.update({"order_by": order_by})
         else:
             get_params.update({"order_by": "-metric"})
@@ -1909,16 +2033,15 @@
             else:
                 raise TypeError("Provided search_params argument is invalid")
         if with_metric is not None:
             get_params.update({"with_metric": with_metric})
         if "is_starred" in get_params:
             get_params["is_starred"] = "true" if get_params["is_starred"] else "false"
         resp_data = self._client.get(url, params=get_params).json()
-        init_data = [dict(Model._safe_data(item), project=self) for item in resp_data]
-        return [Model(**data) for data in init_data]
+        return [Model.from_server_data(item) for item in resp_data]
 
     def recommended_model(self) -> Optional[Model]:
         """Returns the default recommended model, or None if there is no default recommended model.
 
         Returns
         -------
         recommended_model : Model or None
@@ -2371,15 +2494,22 @@
         return PredictionDataset.from_server_data(dataset_data)
 
     def upload_dataset_from_catalog(
         self,
         dataset_id: str,
         credential_id: Optional[str] = None,
         credential_data: Optional[
-            Union[BasicCredentialsDataDict, S3CredentialsDataDict, OAuthCredentialsDataDict]
+            Union[
+                BasicCredentialsDataDict,
+                S3CredentialsDataDict,
+                OAuthCredentialsDataDict,
+                SnowflakeKeyPairCredentialsDataDict,
+                DatabricksAccessTokenCredentialsDataDict,
+                DatabricksServicePrincipalCredentialsDataDict,
+            ]
         ] = None,
         dataset_version_id: Optional[str] = None,
         max_wait: Optional[int] = DEFAULT_MAX_WAIT,
         forecast_point: Optional[datetime] = None,
         relax_known_in_advance_features_check: Optional[bool] = None,
         credentials: Optional[
             List[Union[BasicCredentialsDict, CredentialIdCredentialsDict]]
@@ -2409,32 +2539,71 @@
                 password : str
                     The password for database authentication.
                     The password is encrypted at rest and never saved or stored.
 
             S3 Credentials
                 credentialType : str
                     The credential type. For S3 credentials, this value must be CredentialTypes.S3.
-                awsAccessKeyId : str
+                awsAccessKeyId : str, optional
                     The S3 AWS access key ID.
-                awsSecretAccessKey : str
+                awsSecretAccessKey : str, optional
                     The S3 AWS secret access key.
-                awsSessionToken : str
+                awsSessionToken : str, optional
                     The S3 AWS session token.
+                config_id: str, optional
+                    The ID of the saved shared secure configuration. If specified, cannot include awsAccessKeyId,
+                    awsSecretAccessKey or awsSessionToken.
 
             OAuth Credentials
                 credentialType : str
                     The credential type. For OAuth credentials, this value must be CredentialTypes.OAUTH.
                 oauthRefreshToken : str
                     The oauth refresh token.
                 oauthClientId : str
                     The oauth client ID.
                 oauthClientSecret : str
                     The oauth client secret.
                 oauthAccessToken : str
                     The oauth access token.
+
+            Snowflake Key Pair Credentials
+                credentialType : str
+                    The credential type. For Snowflake Key Pair, this value must be
+                    CredentialTypes.SNOWFLAKE_KEY_PAIR_AUTH.
+                user : str, optional
+                    The Snowflake login name.
+                privateKeyStr : str, optional
+                    The private key copied exactly from user private key file. Since it contains
+                    multiple lines, when assign to a variable,
+                    put the key string inside triple-quotes
+                passphrase : str, optional
+                    The string used to encrypt the private key.
+                configId : str, optional
+                    The ID of the saved shared secure configuration. If specified, cannot include user,
+                    privateKeyStr or passphrase.
+
+            Databricks Access Token Credentials
+                credentialType : str
+                    The credential type. For a Databricks access token, this value must be
+                    CredentialTypes.DATABRICKS_ACCESS_TOKEN.
+                databricksAccessToken : str
+                    The Databricks personal access token.
+
+            Databricks Service Principal Credentials
+                credentialType : str
+                    The credential type. For Databricks service principal, this value must be
+                    CredentialTypes.DATABRICKS_SERVICE_PRINCIPAL.
+                clientId : str, optional
+                    The client ID for Databricks service principal.
+                clientSecret : str, optional
+                    The client secret for Databricks service principal.
+                configId : str, optional
+                    The ID of the saved shared secure configuration. If specified, cannot include clientId
+                    and clientSecret.
+
         dataset_version_id : str, optional
             The version id of the dataset to use.
         max_wait : int, optional
             Optional, the maximum number of seconds to wait before giving up.
         forecast_point : datetime.datetime or None, optional
             For time series projects only. This is the default point relative
             to which predictions will be generated, based on the forecast window of the project. See
@@ -2523,15 +2692,15 @@
     def get_blueprints(self):
         """
         List all blueprints recommended for a project.
 
         Returns
         -------
         menu : list of Blueprint instances
-            All the blueprints recommended by DataRobot for a project
+            All blueprints in a project's repository.
         """
         from . import Blueprint  # pylint: disable=import-outside-toplevel,cyclic-import
 
         url = f"{self._path}{self.id}/blueprints/"
         resp_data = self._client.get(url).json()
         return [Blueprint.from_data(from_api(item)) for item in resp_data]
 
@@ -3949,14 +4118,186 @@
         worker_count : int
             The number of concurrent workers to request from the pool of workers.
             (New in version v2.14) Setting this to -1 will update the number of workers to the
             maximum available to your account.
         """
         return self._update(worker_count=worker_count)
 
+    @deprecated(
+        deprecated_since_version="3.0",
+        will_remove_version="3.2",
+        message="The method 'set_advanced_options' is deprecated. Please use the method 'set_options' instead.",
+    )
+    def set_advanced_options(
+        self, advanced_options: Optional[AdvancedOptions] = None, **kwargs: Any
+    ) -> None:
+        """Update the advanced options of this project.
+
+        .. note:: project options will not be stored at the database level, so the options
+            set via this method will only be attached to a project instance for the lifetime of a
+            client session (if you quit your session and reopen a new one before running autopilot,
+            the advanced options will be lost).
+
+        Either accepts an AdvancedOptions object to replace all advanced options or individual keyword
+        arguments. This is an inplace update, not a new object. The options set will only remain for the
+        life of this project instance within a given session.
+
+
+        Parameters
+        ----------
+        advanced_options : AdvancedOptions, optional
+            AdvancedOptions instance as an alternative to passing individual parameters.
+        weights : string, optional
+            The name of a column indicating the weight of each row
+        response_cap : float in [0.5, 1), optional
+            Quantile of the response distribution to use for response capping.
+        blueprint_threshold : int, optional
+            Number of hours models are permitted to run before being excluded from later autopilot
+            stages
+            Minimum 1
+        seed : int, optional
+            a seed to use for randomization
+        smart_downsampled : bool, optional
+            whether to use smart downsampling to throw away excess rows of the majority class.  Only
+            applicable to classification and zero-boosted regression projects.
+        majority_downsampling_rate : float, optional
+            The percentage between 0 and 100 of the majority rows that should be kept.  Specify only if
+            using smart downsampling.  May not cause the majority class to become smaller than the
+            minority class.
+        offset : list of str, optional
+            (New in version v2.6) the list of the names of the columns containing the offset
+            of each row
+        exposure : string, optional
+            (New in version v2.6) the name of a column containing the exposure of each row
+        accuracy_optimized_mb : bool, optional
+            (New in version v2.6) Include additional, longer-running models that will be run by the
+            autopilot and available to run manually.
+        events_count : string, optional
+            (New in version v2.8) the name of a column specifying events count.
+        monotonic_increasing_featurelist_id : string, optional
+            (new in version 2.11) the id of the featurelist that defines the set of features
+            with a monotonically increasing relationship to the target. If None,
+            no such constraints are enforced. When specified, this will set a default for the project
+            that can be overridden at model submission time if desired.
+        monotonic_decreasing_featurelist_id : string, optional
+            (new in version 2.11) the id of the featurelist that defines the set of features
+            with a monotonically decreasing relationship to the target. If None,
+            no such constraints are enforced. When specified, this will set a default for the project
+            that can be overridden at model submission time if desired.
+        only_include_monotonic_blueprints : bool, optional
+            (new in version 2.11) when true, only blueprints that support enforcing
+            monotonic constraints will be available in the project or selected for the autopilot.
+        allowed_pairwise_interaction_groups : list of tuple, optional
+            (New in version v2.19) For GA2M models - specify groups of columns for which pairwise
+            interactions will be allowed. E.g. if set to [(A, B, C), (C, D)] then GA2M models will
+            allow interactions between columns A x B, B x C, A x C, C x D. All others (A x D, B x D) will
+            not be considered.
+        blend_best_models: bool, optional
+            (New in version v2.19) blend best models during Autopilot run
+        scoring_code_only: bool, optional
+            (New in version v2.19) Keep only models that can be converted to scorable java code
+            during Autopilot run
+        shap_only_mode: bool, optional
+            (New in version v2.21) Keep only models that support SHAP values during Autopilot run. Use
+            SHAP-based insights wherever possible. Defaults to False.
+        prepare_model_for_deployment: bool, optional
+            (New in version v2.19) Prepare model for deployment during Autopilot run.
+            The preparation includes creating reduced feature list models, retraining best model
+            on higher sample size, computing insights and assigning "RECOMMENDED FOR DEPLOYMENT" label.
+        consider_blenders_in_recommendation: bool, optional
+            (New in version 2.22.0) Include blenders when selecting a model to prepare for
+            deployment in an Autopilot Run. Defaults to False.
+        min_secondary_validation_model_count: int, optional
+            (New in version v2.19) Compute "All backtest" scores (datetime models) or cross validation
+            scores for the specified number of highest ranking models on the Leaderboard,
+            if over the Autopilot default.
+        autopilot_data_sampling_method: str, optional
+            (New in version v2.23) one of ``datarobot.enums.DATETIME_AUTOPILOT_DATA_SAMPLING_METHOD``.
+            Applicable for OTV projects only, defines if autopilot uses "random" or "latest" sampling
+            when iteratively building models on various training samples. Defaults to "random" for
+            duration-based projects and to "latest" for row-based projects.
+        run_leakage_removed_feature_list: bool, optional
+            (New in version v2.23) Run Autopilot on Leakage Removed feature list (if exists).
+        autopilot_with_feature_discovery: bool, optional.
+            (New in version v2.23) If true, autopilot will run on a feature list that includes features
+            found via search for interactions.
+        feature_discovery_supervised_feature_reduction: bool, optional
+            (New in version v2.23) Run supervised feature reduction for feature discovery projects.
+        exponentially_weighted_moving_alpha: float, optional
+            (New in version v2.26) defaults to None, value between 0 and 1 (inclusive), indicates
+            alpha parameter used in exponentially weighted moving average within feature derivation
+            window.
+        external_time_series_baseline_dataset_id: str, optional.
+            (New in version v2.26) If provided, will generate metrics scaled by external model
+            predictions metric for time series projects. The external predictions catalog
+            must be validated before autopilot starts, see
+            ``Project.validate_external_time_series_baseline`` and
+            :ref:`external baseline predictions documentation <external_baseline_predictions>`
+            for further explanation.
+        use_supervised_feature_reduction: bool, default ``True` optional
+            Time Series only. When true, during feature generation DataRobot runs a supervised
+            algorithm to retain only qualifying features. Setting to false can
+            severely impact autopilot duration, especially for datasets with many features.
+        primary_location_column: str, optional.
+            The name of primary location column.
+        protected_features: list of str, optional.
+            (New in version v2.24) A list of project features to mark as protected for
+            Bias and Fairness testing calculations. Max number of protected features allowed is 10.
+        preferable_target_value: str, optional.
+            (New in version v2.24) A target value that should be treated as a favorable outcome
+            for the prediction. For example, if we want to check gender discrimination for
+            giving a loan and our target is named ``is_bad``, then the positive outcome for
+            the prediction would be ``No``, which means that the loan is good and that's
+            what we treat as a favorable result for the loaner.
+        fairness_metrics_set: str, optional.
+            (New in version v2.24) Metric to use for calculating fairness.
+            Can be one of ``proportionalParity``, ``equalParity``, ``predictionBalance``,
+            ``trueFavorableAndUnfavorableRateParity`` or
+            ``favorableAndUnfavorablePredictiveValueParity``.
+            Used and required only if *Bias & Fairness in AutoML* feature is enabled.
+        fairness_threshold: str, optional.
+            (New in version v2.24) Threshold value for the fairness metric.
+            Can be in a range of ``[0.0, 1.0]``. If the relative (i.e. normalized) fairness
+            score is below the threshold, then the user will see a visual indication on the
+        bias_mitigation_feature_name : str, optional
+            The feature from protected features that will be used in a bias mitigation task to
+            mitigate bias
+        bias_mitigation_technique : str, optional
+            One of datarobot.enums.BiasMitigationTechnique
+            Options:
+            - 'preprocessingReweighing'
+            - 'postProcessingRejectionOptionBasedClassification'
+            The technique by which we'll mitigate bias, which will inform which bias mitigation task
+            we insert into blueprints
+        include_bias_mitigation_feature_as_predictor_variable : bool, optional
+            Whether we should also use the mitigation feature as in input to the modeler just like
+            any other categorical used for training, i.e. do we want the model to "train on" this
+            feature in addition to using it for bias mitigation
+        model_group_id : string, optional
+            (New in version v3.3) The name of a column containing the model group ID for each row.
+        model_regime_id : string, optional
+            (New in version v3.3) The name of a column containing the model regime ID for each row.
+        model_baselines : list of str, optional
+            (New in version v3.3) The list of the names of the columns containing the model baselines
+        for each row.
+        incremental_learning_only_mode : bool, optional
+            (New in version v3.4) Keep only models that support incremental learning during Autopilot run.
+        incremental_learning_on_best_model : bool, optional
+            (New in version v3.4) Run incremental learning on the best model during Autopilot run.
+        chunk_definition_id : string, optional
+            (New in version v3.4) Unique definition for chunks needed to run automated incremental learning.
+        incremental_learning_early_stopping_rounds: int, optional
+            (New in version v3.4) Early stopping rounds used in the automated incremental learning service.
+
+        """
+        if advanced_options is not None:
+            self.advanced_options = advanced_options
+            return
+        self.advanced_options.update_individual_options(**kwargs)
+
     def list_advanced_options(self) -> Dict[str, Any]:
         """View the advanced options that have been set on a project instance.
         Includes those that haven't been set (with value of None).
 
         Returns
         -------
         dict of advanced options and their values
@@ -4749,22 +5090,22 @@
         .. versionadded:: v3.0
 
         Parameters
         ----------
         datetime_partition_spec :
             :class:`DatetimePartitioningSpecification <datarobot.DatetimePartitioningSpecification>`,
             optional
-            The customizeable aspects of datetime partitioning for a time series project. An alternative
+            The customizable aspects of datetime partitioning for a time series project. An alternative
             to passing individual settings (attributes of the `DatetimePartitioningSpecification` class).
 
 
         Returns
         -------
         DatetimePartitioning
-            Full partitioning inluding user-specified attributes as well as those determined by DR
+            Full partitioning including user-specified attributes as well as those determined by DR
             based on the dataset.
         """
         if datetime_partition_spec is not None:
             self.partitioning_method = datetime_partition_spec
 
         elif self.partitioning_method is not None:
             self.partitioning_method.update(**kwargs)
```

### Comparing `datarobot-3.3.2/datarobot/models/project_options.py` & `datarobot-3.4.0/datarobot/models/project_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1115,14 +1115,18 @@
             "treat_as_exponential": self.treat_as_exponential,
             "use_gpu": self.use_gpu,
             "unsupervised_mode": self.unsupervised_mode,
             "use_supervised_feature_reduction": self.use_supervised_feature_reduction,
             "use_time_series": self.use_time_series,
             "validation_duration": self.validation_duration,
             "windows_basis_unit": self.windows_basis_unit,
+            "incremental_learning_only_mode": self.incremental_learning_only_mode,
+            "incremental_learning_on_best_model": self.incremental_learning_on_best_model,
+            "incremental_learning_early_stopping_rounds": self.incremental_learning_early_stopping_rounds,
+            "chunk_definition_id": self.chunk_definition_id,
         }
 
     def collect_autopilot_payload(self) -> Dict[str, Any]:
         if not self.is_empty:
             return super().collect_payload()
         return {
             default_field: getattr(self, default_field)
```

### Comparing `datarobot-3.3.2/datarobot/models/rating_table.py` & `datarobot-3.4.0/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/recommended_model.py` & `datarobot-3.4.0/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/relationships_configuration.py` & `datarobot-3.4.0/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/residuals.py` & `datarobot-3.4.0/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/restore_discarded_features.py` & `datarobot-3.4.0/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/roc_curve.py` & `datarobot-3.4.0/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/ruleset.py` & `datarobot-3.4.0/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/secondary_dataset.py` & `datarobot-3.4.0/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/segmentation.py` & `datarobot-3.4.0/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/shap_impact.py` & `datarobot-3.4.0/datarobot/models/shap_impact.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from typing import List, Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
-from datarobot.utils import get_id_from_response
+from datarobot.utils import deprecation, get_id_from_response
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.job import Job
 
     class ShapImpactType(TypedDict):
@@ -67,26 +67,36 @@
                         t.Key("impact_unnormalized"): t.Float(),
                     }
                 ).allow_extra("*")
             ),
         }
     ).allow_extra("*")
 
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapImpact' instead.",
+    )
     def __init__(
         self, count: int, shap_impacts: List[ShapImpactType], row_count: Optional[int] = None
     ) -> None:
         self.count = count
         self.shap_impacts = shap_impacts
         self.row_count = row_count
 
     def __repr__(self) -> str:
         template = "{}(count={!r})"
         return template.format(type(self).__name__, self.count)
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapImpact.create' instead.",
+    )
     def create(cls, project_id: str, model_id: str, row_count: Optional[int] = None) -> Job:
         """Create SHAP impact for the specified model.
 
         Parameters
         ----------
         project_id : str
             id of the project the model belongs to
@@ -105,14 +115,19 @@
         response = cls._client.post(url, data=payload)
         job_id = get_id_from_response(response)
         from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
         return Job.get(project_id=project_id, job_id=job_id)
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapImpact.list' instead.",
+    )
     def get(cls, project_id: str, model_id: str) -> ShapImpact:
         """
         Retrieve SHAP impact scores for features in a model.
 
         Parameters
         ----------
         project_id : str
```

### Comparing `datarobot-3.3.2/datarobot/models/shap_matrix.py` & `datarobot-3.4.0/datarobot/models/shap_matrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pandas as pd
 import trafaret as t
 
 from datarobot import errors
 from datarobot._compat import String
 from datarobot.enums import DEFAULT_TIMEOUT
 from datarobot.models.api_object import APIObject
-from datarobot.utils import get_id_from_response
+from datarobot.utils import deprecation, get_id_from_response
 from datarobot.utils.pagination import unpaginate
 
 if TYPE_CHECKING:
     from datarobot.models.shap_matrix_job import ShapMatrixJob
 
 
 class ShapMatrix(APIObject):
@@ -67,14 +67,19 @@
             t.Key("id"): String(),
             t.Key("project_id"): String(),
             t.Key("model_id"): String(),
             t.Key("dataset_id"): String(),
         }
     ).allow_extra("*")
 
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix' instead.",
+    )
     def __init__(
         self,
         project_id: str,
         id: str,
         model_id: Optional[str] = None,
         dataset_id: Optional[str] = None,
     ) -> None:
@@ -90,14 +95,19 @@
             self.id,
             self.project_id,
             self.model_id,
             self.dataset_id,
         )
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix.create' instead.",
+    )
     def create(cls, project_id: str, model_id: str, dataset_id: str) -> ShapMatrixJob:
         """Calculate SHAP based prediction explanations against previously uploaded dataset.
 
         Parameters
         ----------
         project_id : str
             id of the project the model belongs to
@@ -138,17 +148,24 @@
         cls,
         location: str,
         model_id: Optional[str] = None,
         dataset_id: Optional[str] = None,
     ) -> ShapMatrix:
         head, tail = location.split("/shapMatrices/", 1)
         project_id, id = head.split("/")[-1], tail.split("/")[0]
-        return cls(project_id=project_id, id=id, model_id=model_id, dataset_id=dataset_id)
+        return cls(  # type: ignore[no-any-return]
+            project_id=project_id, id=id, model_id=model_id, dataset_id=dataset_id
+        )
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix.list' instead.",
+    )
     def list(cls, project_id: str) -> List[ShapMatrix]:
         """
         Fetch all the computed SHAP prediction explanations for a project.
 
         Parameters
         ----------
         project_id : str
@@ -169,14 +186,19 @@
         data = unpaginate(
             initial_url=cls._path.format(project_id), initial_params=None, client=cls._client
         )
         result = [cls.from_server_data(item) for item in data]
         return result
 
     @classmethod
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix.list' instead.",
+    )
     def get(cls, project_id: str, id: str) -> ShapMatrix:
         """
         Retrieve the specific SHAP matrix.
 
         Parameters
         ----------
         project_id : str
@@ -184,16 +206,21 @@
         id : str
             id of the SHAP matrix
 
         Returns
         -------
         :py:class:`ShapMatrix <datarobot.models.ShapMatrix>` object representing specified record
         """
-        return cls(project_id=project_id, id=id)
+        return cls(project_id=project_id, id=id)  # type: ignore[no-any-return]
 
+    @deprecation.deprecated(
+        deprecated_since_version="v3.4",
+        will_remove_version="v3.6",
+        message="This class is deprecated, please use 'datarobot.insights.ShapMatrix' instead.",
+    )
     def get_as_dataframe(self, read_timeout: int = DEFAULT_TIMEOUT.READ) -> pd.DataFrame:
         """
         Retrieve SHAP matrix values as dataframe.
 
         Returns
         -------
         dataframe : pandas.DataFrame
```

### Comparing `datarobot-3.3.2/datarobot/models/shap_matrix_job.py` & `datarobot-3.4.0/datarobot/models/shap_matrix_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             data,
             model_id=model_id,
             dataset_id=dataset_id,
             completed_resource_url=completed_url,
         )
 
     def _make_result_from_location(self, location: str, params: Optional[Any] = None) -> ShapMatrix:
-        return ShapMatrix.from_location(
+        return ShapMatrix.from_location(  # type: ignore[no-any-return]
             location,
             model_id=self._model_id,
             dataset_id=self._dataset_id,
         )
 
     def refresh(self) -> None:
         """
```

### Comparing `datarobot-3.3.2/datarobot/models/sharing.py` & `datarobot-3.4.0/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/status_check_job.py` & `datarobot-3.4.0/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/trafarets.py` & `datarobot-3.4.0/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/training_predictions.py` & `datarobot-3.4.0/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/types.py` & `datarobot-3.4.0/datarobot/models/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -72,7 +72,15 @@
 
 
 class RegionExplanationsData(TypedDict):
     """Typed dict for region explanations"""
 
     explanations: List[AnomalyAssessmentDataPoint]
     shap_base_value: Optional[float]
+
+
+class Schedule(TypedDict):
+    day_of_week: List[Union[int, str]]
+    month: List[Union[int, str]]
+    hour: List[Union[int, str]]
+    minute: List[Union[int, str]]
+    day_of_month: List[Union[int, str]]
```

### Comparing `datarobot-3.3.2/datarobot/models/use_cases/use_case.py` & `datarobot-3.4.0/datarobot/models/use_cases/use_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SHARING_RECIPIENT_TYPE,
     SHARING_ROLE,
     UseCaseAPIPathEntityType,
     UseCaseEntityType,
     UseCaseReferenceEntityMap,
 )
 from datarobot.errors import InvalidUsageError
+from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject
 from datarobot.models.sharing import SharingRole
 from datarobot.utils.pagination import unpaginate
 
 T = TypeVar("T")
 
 use_case_user_trafaret = t.Dict(
@@ -164,15 +165,15 @@
         error_message = (
             error_message + " PredictionDataset is not a subclass of Dataset and "
             "cannot be added to a UseCase at this time."
         )
     raise TypeError(error_message)
 
 
-class UseCase(APIObject):
+class UseCase(APIObject, BrowserMixin):
     """Representation of a Use Case.
 
     Attributes
     ----------
     id : str
         The ID of the Use Case.
     name : str
@@ -194,15 +195,15 @@
     datasets_count: int
         The number of datasets in a Use Case.
     notebooks_count: int
         The number of notebooks in a Use Case.
     applications_count: int
         The number of applications in a Use Case.
     playgrounds_count: int
-        The number of playgronuds in a Use Case.
+        The number of playgrounds in a Use Case.
     vector_databases_count: int
         The number of vector databases in a Use Case.
     owners : List[UseCaseUser]
         The most recent user to update the Use Case.
     members : List[UseCaseUser]
         The most recent user to update the Use Case.
 
@@ -285,14 +286,23 @@
             f"models={self.models_count}, "
             f"projects={self.projects_count}, "
             f"datasets={self.datasets_count}, "
             f"notebooks={self.notebooks_count}, "
             f"applications={self.applications_count})"
         )
 
+    def get_uri(self) -> str:
+        """
+        Returns
+        -------
+        url : str
+            Permanent static hyperlink to this Use Case.
+        """
+        return f"{self._client.domain}/usecases/{self.id}/overview/recent"
+
     @classmethod
     def get(cls, use_case_id: str) -> UseCase:
         """
         Gets information about a Use Case.
 
         Parameters
         ----------
@@ -319,17 +329,17 @@
             Currently, you can query use cases by:
 
             * ``offset`` - The number of records to skip over. Default 0.
             * ``limit`` - The number of records to return in the range from 1 to 100. Default 100.
             * ``search`` - Only return Use Cases with names that match the given string.
             * ``project_id`` - Only return Use Cases associated with the given project ID.
             * ``application_id`` - Only return Use Cases associated with the given app.
-            * ``sort`` - The order to sort the Use Cases.
+            * ``orderBy`` - The order to sort the Use Cases.
 
-            ``sort`` queries can use the following options:
+            ``orderBy`` queries can use the following options:
 
             * ``id`` or ``-id``
             * ``name`` or ``-name``
             * ``description`` or ``-description``
             * ``projects_count`` or ``-projects_count``
             * ``datasets_count`` or ``-datasets_count``
             * ``notebooks_count`` or ``-notebooks_count``
@@ -647,15 +657,15 @@
         Returns
         -------
         projects : List[Project]
             All projects associated with this Use Case.
         """
         from ..project import Project
 
-        return Project.list(search_params={"experiment_container_ids": self.id})  # type: ignore[return-value]
+        return Project.list(search_params={"use_case_ids": self.id})  # type: ignore[return-value]
 
     def list_datasets(self) -> List[T]:
         """
         List all datasets associated with this Use Case.
 
         Returns
         -------
```

### Comparing `datarobot-3.3.2/datarobot/models/use_cases/utils.py` & `datarobot-3.4.0/datarobot/models/use_cases/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 
 logger = get_logger(__name__)
 
 
 def resolve_use_cases(
     params: Dict[str, Any],
     use_cases: Optional[UseCaseLike] = None,
-    use_case_key: str = "experiment_container_ids",
+    use_case_key: str = "use_case_ids",
 ) -> Dict[str, Any]:
     """
     Add a global Use Case ID or IDs to query params for a list operation if no use_case_id has been passed
     This method supports checking for `use_case_id` in a params dict if users can build their own params dict.
     Parameters
     ----------
     params : Dict[str, Any]
         The query params dict to add a Use Case ID to, if a global ID exists, or if one was passed in directly.
     use_cases : Optional[Union[List[UseCase], UseCase, List[str], str]]
         Optional. The use case or cases to add to a query params dict. May be Use Case ID or the Use Case entity.
     use_case_key : Optional[str]
-        Optional. The key that will be used in the query params for Use Case ID. Default is 'experiment_container_ids'.
+        Optional. The key that will be used in the query params for Use Case ID. Default is 'use_case_ids'.
     Returns
     -------
     params : Dict[str, Any]
         If a Use Case ID is available, the params with the ID added. Otherwise, return the dict unmodified.
     """
     # Check to see if a use_case_id is already in the params dict
     if not params.get(use_case_key):
```

### Comparing `datarobot-3.3.2/datarobot/models/user_blueprints/models.py` & `datarobot-3.4.0/datarobot/models/user_blueprints/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,51 +86,51 @@
 
     Parameters
     ----------
     blender: bool
         Whether the blueprint is a blender.
     blueprint_id: string
         The deterministic id of the blueprint, based on its content.
-    custom_task_version_metadata: list(list(string)), Optional
+    custom_task_version_metadata: list[list[string]], Optional
         An association of custom entity ids and task ids.
     diagram: string
         The diagram used by the UI to display the blueprint.
-    features: list(string)
+    features: list[string]
         A list of the names of tasks used in the blueprint.
     features_text: string
         A description of the blueprint via the names of tasks used.
-    hex_column_name_lookup: list(UserBlueprintsHexColumnNameLookupEntry), Optional
+    hex_column_name_lookup: list[UserBlueprintsHexColumnNameLookupEntry], Optional
         A lookup between hex values and data column names used in the blueprint.
-    icons: list(int)
+    icons: list[int]
         The icon(s) associated with the blueprint.
     insights: string
         An indication of the insights generated by the blueprint.
     is_time_series: bool (Default=False)
         Whether the blueprint contains time-series tasks.
     model_type: string
         The generated or provided title of the blueprint.
     project_id: string, Optional
         The id of the project the blueprint was originally created with, if applicable.
     reference_model: bool (Default=False)
         Whether the blueprint is a reference model.
     shap_support: bool (Default=False)
         Whether the blueprint supports shapley additive explanations.
-    supported_target_types: list(enum('binary', 'multiclass', 'multilabel', 'nonnegative',
-    'regression', 'unsupervised', 'unsupervisedclustering'))
+    supported_target_types: list[enum('binary', 'multiclass', 'multilabel', 'nonnegative',
+    'regression', 'unsupervised', 'unsupervisedclustering')]
         The list of supported targets of the current blueprint.
     supports_gpu: bool (Default=False)
         Whether the blueprint supports execution on the GPU.
     user_blueprint_id: string
         The unique id associated with the user blueprint.
     user_id: string
         The id of the user who owns the blueprint.
-    blueprint: list(dict) or list(UserBlueprintTask), Optional
+    blueprint: list[dict] or list[UserBlueprintTask], Optional
         The representation of a directed acyclic graph defining a pipeline of data through tasks
         and a final estimator.
-    vertex_context: list(VertexContextItem), Optional
+    vertex_context: list[VertexContextItem], Optional
         Info about, warnings about, and errors with a specific vertex in the blueprint.
     blueprint_context: VertexContextItemMessages
         Warnings and errors which may describe or summarize warnings or errors in the blueprint's
         vertices
     """
 
     _path = "userBlueprints/{userBlueprintId}/"
@@ -206,15 +206,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        list(UserBlueprint)
+        list[UserBlueprint]
         """
         path = "userBlueprints/"
         params = dict(
             offset=offset,
             limit=limit or DEFAULT_BATCH_SIZE,
             project_id=None if project_id is None else str(project_id),
         )
@@ -263,15 +263,15 @@
         save_to_catalog: bool = True,
     ) -> UserBlueprint:
         """
         Create a user blueprint
 
         Parameters
         ----------
-        blueprint: list(dict) or list(UserBlueprintTask)
+        blueprint: list[dict] or list[UserBlueprintTask]
             A list of tasks in the form of dictionaries which define a blueprint.
         model_type: string, Optional
             The title to give to the blueprint.
         project_id: string, Optional
             The project associated with the blueprint. Necessary in the event of project specific
             tasks, such as column selection tasks.
         save_to_catalog: bool, (Default=True)
@@ -681,15 +681,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        list(UserBlueprintSharedRolesResponseValidator)
+        list[UserBlueprintSharedRolesResponseValidator]
         """
         return UserBlueprintSharingListController.list_shared_roles(
             user_blueprint_id=user_blueprint_id,
             limit=limit,
             offset=offset,
             id=id,
             name=name,
@@ -716,15 +716,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        list(VertexContextItem)
+        list[VertexContextItem]
         """
         return UserBlueprintValidate.validate_blueprint(blueprint, project_id=project_id)
 
     @classmethod
     def update_shared_roles(
         cls,
         user_blueprint_id: str,
```

### Comparing `datarobot-3.3.2/datarobot/models/user_blueprints/trafarets.py` & `datarobot-3.4.0/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/validators.py` & `datarobot-3.4.0/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/visualai/augmentation.py` & `datarobot-3.4.0/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/visualai/images.py` & `datarobot-3.4.0/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/visualai/insights.py` & `datarobot-3.4.0/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/models/word_cloud.py` & `datarobot-3.4.0/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/rest.py` & `datarobot-3.4.0/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/__init__.py` & `datarobot-3.4.0/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/deprecation.py` & `datarobot-3.4.0/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/pagination.py` & `datarobot-3.4.0/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/retry.py` & `datarobot-3.4.0/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/source.py` & `datarobot-3.4.0/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/sourcedata.py` & `datarobot-3.4.0/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot/utils/waiters.py` & `datarobot-3.4.0/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/datarobot.egg-info/SOURCES.txt` & `datarobot-3.4.0/datarobot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setup.py
 setup_major.py
 datarobot/__init__.py
 datarobot/_compat.py
 datarobot/_version.py
 datarobot/analytics.py
 datarobot/client.py
+datarobot/config.py
 datarobot/context.py
 datarobot/enums.py
 datarobot/errors.py
 datarobot/py.typed
 datarobot/rest.py
 datarobot.egg-info/PKG-INFO
 datarobot.egg-info/SOURCES.txt
@@ -24,14 +25,19 @@
 datarobot.egg-info/top_level.txt
 datarobot/helpers/__init__.py
 datarobot/helpers/binary_data_utils.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
 datarobot/helpers/image_utils.py
 datarobot/helpers/partitioning_methods.py
+datarobot/insights/__init__.py
+datarobot/insights/base.py
+datarobot/insights/shap_impact.py
+datarobot/insights/shap_matrix.py
+datarobot/insights/shap_preview.py
 datarobot/mixins/__init__.py
 datarobot/mixins/browser_mixin.py
 datarobot/mixins/update_attributes_mixin.py
 datarobot/models/__init__.py
 datarobot/models/advanced_tuning.py
 datarobot/models/anomaly_assessment.py
 datarobot/models/api_object.py
@@ -67,14 +73,15 @@
 datarobot/models/external_baseline_validation.py
 datarobot/models/feature.py
 datarobot/models/feature_effect.py
 datarobot/models/feature_impact.py
 datarobot/models/featurelist.py
 datarobot/models/imported_model.py
 datarobot/models/job.py
+datarobot/models/key_values.py
 datarobot/models/lift_chart.py
 datarobot/models/missing_report.py
 datarobot/models/model.py
 datarobot/models/modeljob.py
 datarobot/models/pairwise_statistics.py
 datarobot/models/pareto_front.py
 datarobot/models/payoff_matrix.py
@@ -90,14 +97,15 @@
 datarobot/models/rating_table.py
 datarobot/models/recommended_model.py
 datarobot/models/relationships_configuration.py
 datarobot/models/residuals.py
 datarobot/models/restore_discarded_features.py
 datarobot/models/roc_curve.py
 datarobot/models/ruleset.py
+datarobot/models/runtime_parameters.py
 datarobot/models/secondary_dataset.py
 datarobot/models/segmentation.py
 datarobot/models/shap_impact.py
 datarobot/models/shap_matrix.py
 datarobot/models/shap_matrix_job.py
 datarobot/models/sharing.py
 datarobot/models/status_check_job.py
@@ -105,15 +113,19 @@
 datarobot/models/training_predictions.py
 datarobot/models/types.py
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
 datarobot/models/deployment/bias_and_fairness.py
+datarobot/models/deployment/challenger.py
+datarobot/models/deployment/champion_model_package.py
+datarobot/models/deployment/custom_metrics.py
 datarobot/models/deployment/data_drift.py
+datarobot/models/deployment/data_exports.py
 datarobot/models/deployment/deployment.py
 datarobot/models/deployment/mixins.py
 datarobot/models/deployment/service_stats.py
 datarobot/models/deployment/sharing.py
 datarobot/models/documentai/__init__.py
 datarobot/models/documentai/document.py
 datarobot/models/external_dataset_scores_insights/__init__.py
@@ -123,19 +135,34 @@
 datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
 datarobot/models/external_dataset_scores_insights/external_roc_curve.py
 datarobot/models/external_dataset_scores_insights/external_scores.py
 datarobot/models/feature_association_matrix/__init__.py
 datarobot/models/feature_association_matrix/feature_association_featurelists.py
 datarobot/models/feature_association_matrix/feature_association_matrix.py
 datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+datarobot/models/genai/__init__.py
+datarobot/models/genai/chat.py
+datarobot/models/genai/chat_prompt.py
+datarobot/models/genai/comparison_chat.py
+datarobot/models/genai/comparison_prompt.py
+datarobot/models/genai/custom_model_llm_validation.py
+datarobot/models/genai/custom_model_validation.py
+datarobot/models/genai/llm.py
+datarobot/models/genai/llm_blueprint.py
+datarobot/models/genai/playground.py
+datarobot/models/genai/user_limits.py
+datarobot/models/genai/vector_database.py
 datarobot/models/model_registry/__init__.py
 datarobot/models/model_registry/common.py
 datarobot/models/model_registry/deployment.py
 datarobot/models/model_registry/registered_model.py
 datarobot/models/model_registry/registered_model_version.py
+datarobot/models/registry/__init__.py
+datarobot/models/registry/job.py
+datarobot/models/registry/job_run.py
 datarobot/models/use_cases/__init__.py
 datarobot/models/use_cases/use_case.py
 datarobot/models/use_cases/utils.py
 datarobot/models/user_blueprints/__init__.py
 datarobot/models/user_blueprints/models.py
 datarobot/models/user_blueprints/trafarets.py
 datarobot/models/visualai/__init__.py
```

### Comparing `datarobot-3.3.2/datarobot.egg-info/requires.txt` & `datarobot-3.4.0/datarobot.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 strenum>=0.4.15
 
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
-pytest-asyncio
+pytest-asyncio==0.21.1
+pyarrow
 Pillow==9.2.0
 black==22.8.0
 black[jupyter]==22.8.0
 isort==5.10.1
 flake8==5.0.4
 pylint==2.15.0
 mypy==1.0.0
@@ -28,14 +29,16 @@
 types-requests==2.28.11
 types-urllib3==1.26.25
 sphinx_rtd_theme==1.0.0
 nbsphinx==0.8.9
 numpydoc==1.4.0
 jupyter_contrib_nbextensions
 sphinx-autodoc-typehints==1.17.1
+sphinxcontrib-spelling==8.0.0
+pyenchant==3.2.2
 
 [examples]
 jupyter<=5.0
 fredapi==0.4.0
 matplotlib>=2.1.0
 seaborn<=0.8
 scikit-learn<=0.18.2
@@ -63,9 +66,10 @@
 zest.releaser[recommended]==6.22.0
 
 [test]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
-pytest-asyncio
+pytest-asyncio==0.21.1
+pyarrow
 Pillow==9.2.0
```

### Comparing `datarobot-3.3.2/pyproject.toml` & `datarobot-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/setup.py` & `datarobot-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.3.2/setup_major.py` & `datarobot-3.4.0/setup_major.py`

 * *Files identical despite different names*

