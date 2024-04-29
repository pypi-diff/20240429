# Comparing `tmp/vectice-24.2.2.0.tar.gz` & `tmp/vectice-24.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.2.2.0.tar", last modified: Mon Apr 22 08:07:13 2024, max compression
+gzip compressed data, was "vectice-24.2.3.0.tar", last modified: Mon Apr 29 07:48:51 2024, max compression
```

## Comparing `vectice-24.2.2.0.tar` & `vectice-24.2.3.0.tar`

### file list

```diff
@@ -1,166 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.081815 vectice-24.2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 08:06:59.000000 vectice-24.2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-22 08:07:13.081815 vectice-24.2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 08:06:59.000000 vectice-24.2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 08:06:59.000000 vectice-24.2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 08:07:13.081815 vectice-24.2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-22 08:06:59.000000 vectice-24.2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.041815 vectice-24.2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.045815 vectice-24.2.2.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.049815 vectice-24.2.2.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.057815 vectice-24.2.2.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.057815 vectice-24.2.2.0/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.061815 vectice-24.2.2.0/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/pytorch_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    30734 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.065815 vectice-24.2.2.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.065815 vectice-24.2.2.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.065815 vectice-24.2.2.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/models/test_library/
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/test_library/binary_classification_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.073815 vectice-24.2.2.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.073815 vectice-24.2.2.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.054334 vectice-24.2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 07:48:44.000000 vectice-24.2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-29 07:48:51.054334 vectice-24.2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 07:48:44.000000 vectice-24.2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-29 07:48:44.000000 vectice-24.2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 07:48:51.058334 vectice-24.2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-29 07:48:44.000000 vectice-24.2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.014334 vectice-24.2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.018334 vectice-24.2.3.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.022334 vectice-24.2.3.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.030334 vectice-24.2.3.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.030334 vectice-24.2.3.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.034334 vectice-24.2.3.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/pytorch_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30199 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.038334 vectice-24.2.3.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.038334 vectice-24.2.3.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.038334 vectice-24.2.3.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/models/test_library/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/test_library/binary_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.046334 vectice-24.2.3.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.046334 vectice-24.2.3.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-29 07:48:50.000000 vectice-24.2.3.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-29 07:48:51.000000 vectice-24.2.3.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:48:50.000000 vectice-24.2.3.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-29 07:48:51.000000 vectice-24.2.3.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:48:51.000000 vectice-24.2.3.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.2.2.0/LICENSE` & `vectice-24.2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/PKG-INFO` & `vectice-24.2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.2.0
+Version: 24.2.3.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -40,20 +40,20 @@
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: dataclasses-json==0.5.8
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
-Requires-Dist: pyright==1.1.354; extra == "dev"
+Requires-Dist: pyright==1.1.360; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
-Requires-Dist: boto3-stubs[essential]; extra == "dev"
+Requires-Dist: mypy_boto3_s3==1.34.65; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: black==24.2.0; extra == "doc"
 Requires-Dist: markdown-callouts>=0.2; extra == "doc"
 Requires-Dist: markdown-exec>=1.2; extra == "doc"
 Requires-Dist: mkdocs==1.4.2; extra == "doc"
 Requires-Dist: mkdocs-material>=7.3; extra == "doc"
```

### Comparing `vectice-24.2.2.0/pyproject.toml` & `vectice-24.2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/setup.py` & `vectice-24.2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,20 +46,20 @@
         "typing-extensions>=4.5.0",  # Prior to 4.6.2 because of colab issues with tensorflow 2.13.0
         "dataclasses-json==0.5.8",
     ],
     extras_require={
         "dev": [
             "black==24.2.0",
             "gitpython",
-            "pyright==1.1.354",
+            "pyright==1.1.360",
             "ruff",
             "types-requests",
             "types-urllib3",
             "types-mock",
-            "boto3-stubs[essential]",
+            "mypy_boto3_s3==1.34.65",
             "pandas-stubs",
         ],
         "doc": [
             "black==24.2.0",
             "markdown-callouts>=0.2",
             "markdown-exec>=1.2",
             "mkdocs==1.4.2",
```

### Comparing `vectice-24.2.2.0/src/vectice/__init__.py` & `vectice-24.2.3.0/src/vectice/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 )
 from vectice.models.table import Table
 from vectice.utils.logging_utils import configure_vectice_loggers, disable_logging
 
 connect = Connection.connect
 
 code_capture = True
+
 """Global code capture flag, enabled by default.
 
 Code capture is triggered when registering a dataset or a model,
 and only works when a valid Git repository is found.
 Otherwise a warning is logged, telling what might be misconfigured in the repository.
 
 Captured information include the repository name, URL, branch name, commit hash,
@@ -74,14 +75,31 @@
 
     To re-enable code capture globally:
 
     >>> import vectice
     >>> vectice.code_capture = True
 """
 
+auto_extract = True
+"""Global auto extraction flag, enabled by default.
+
+Extraction is automatically performed when registering a dataset or a model with an attachment. Currently, it exclusively operates on Excel files and extracts sheets (as CSV files) and images to be referenced inside Vectice.
+
+Examples:
+    To disable auto extraction of files globally globally:
+
+    >>> import vectice
+    >>> vectice.auto_extract = False
+
+    To re-enable auto extraction globally:
+
+    >>> import vectice
+    >>> vectice.auto_extract = True
+"""
+
 configure_vectice_loggers(root_module_name=__name__)
 silent = disable_logging
 warnings.simplefilter("always", DeprecationWarning)
 
 version = __version__
 
 __all__ = [
```

### Comparing `vectice-24.2.2.0/src/vectice/api/_auth.py` & `vectice-24.2.3.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/attachment.py` & `vectice-24.2.3.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/client.py` & `vectice-24.2.3.0/src/vectice/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from gql import Client as GQLClient
 from gql.transport.requests import RequestsHTTPTransport
 
 from vectice.__version__ import __version__
 from vectice.api._auth import Auth
 from vectice.api.attachment import AttachmentApi
 from vectice.api.compatibility import CompatibilityApi
+from vectice.api.gql_attachment import GqlAttachmentApi
 from vectice.api.gql_dataset import GqlDatasetApi
 from vectice.api.gql_entity_file import GqlEntityFileApi
 from vectice.api.gql_feature_flag import GqlFeatureFlagApi
 from vectice.api.gql_metric import GqlMetricApi
 from vectice.api.gql_model import GqlModelApi
 from vectice.api.gql_organization import GqlOrganizationApi
 from vectice.api.gql_property import GqlPropertyApi
@@ -49,14 +50,15 @@
 from vectice.models.dataset import Dataset
 from vectice.models.iteration import Iteration
 from vectice.models.model import Model
 from vectice.models.phase import Phase
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 from vectice.models.resource.metadata.base import MetadataSettings
+from vectice.models.table import Table
 from vectice.types.version import TVersion
 from vectice.utils.vectice_ids_regex import WORKSPACE_VID_REG
 
 if TYPE_CHECKING:
     from io import BytesIO, IOBase
 
     from requests import Response
@@ -179,14 +181,34 @@
             version: The version to attach files to.
 
         Returns:
             The JSON structure.
         """
         return AttachmentApi(self.auth).post_attachment(files, version)
 
+    def upsert_version_tables(self, tables: list[Table], version: TVersion):
+        """Upsert a table.
+
+        Parameters:
+            tables: The tables to attach.
+            version: The version to attach tables to.
+
+        Returns:
+            The JSON structure.
+        """
+        return GqlAttachmentApi(self._gql_client, self.auth).upsert(
+            version.id,
+            (
+                "MODEL_VERSION"
+                if isinstance(version, (ModelVersionOutput, ModelVersionRepresentationOutput))
+                else "DATASET_VERSION"
+            ),
+            tables,
+        )
+
     def upsert_iteration_attachments(
         self,
         files: list[tuple[str, tuple[str, BytesIO | IOBase]]],
         iteration_id: str,
         step_name: str | None = None,
     ):
         """Create an attachment.
```

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_api.py` & `vectice-24.2.3.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_dataset.py` & `vectice-24.2.3.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_entity_file.py` & `vectice-24.2.3.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.3.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_metric.py` & `vectice-24.2.3.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_model.py` & `vectice-24.2.3.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_organization.py` & `vectice-24.2.3.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_property.py` & `vectice-24.2.3.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.3.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/http_error.py` & `vectice-24.2.3.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/http_error_handlers.py` & `vectice-24.2.3.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/iteration.py` & `vectice-24.2.3.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/__init__.py` & `vectice-24.2.3.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/artifact_version.py` & `vectice-24.2.3.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/code.py` & `vectice-24.2.3.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/code_version.py` & `vectice-24.2.3.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/dataset_register.py` & `vectice-24.2.3.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.3.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/dataset_version.py` & `vectice-24.2.3.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.3.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/files_metadata.py` & `vectice-24.2.3.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/iteration.py` & `vectice-24.2.3.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/json_to_class.py` & `vectice-24.2.3.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/last_assets.py` & `vectice-24.2.3.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/metric.py` & `vectice-24.2.3.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/model.py` & `vectice-24.2.3.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/model_register.py` & `vectice-24.2.3.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/model_representation.py` & `vectice-24.2.3.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/model_version.py` & `vectice-24.2.3.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.3.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/paged_response.py` & `vectice-24.2.3.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/phase.py` & `vectice-24.2.3.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/project.py` & `vectice-24.2.3.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/property.py` & `vectice-24.2.3.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/public_config.py` & `vectice-24.2.3.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/requirement.py` & `vectice-24.2.3.0/src/vectice/api/json/requirement.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.3.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/json/workspace.py` & `vectice-24.2.3.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/phase.py` & `vectice-24.2.3.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/project.py` & `vectice-24.2.3.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/rest_api.py` & `vectice-24.2.3.0/src/vectice/api/rest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,24 @@
             url=self.auth.api_base_url + path, headers=headers, data=data, verify=self.auth.verify_certificate
         )
         return self._response(self.auth.api_base_url + path, headers, response, "DELETE", data)
 
     def _post_attachments(
         self, path: str, files: Sequence[tuple[str, tuple[Any, BinaryIO | str]]] | None = None
     ) -> Response | None:
+        from vectice import auto_extract
+
         headers = self.auth.http_headers
+        params = {"extract": str(auto_extract).lower()}
         response = requests.post(  # noqa: S113
             url=self.auth.api_base_url + path,
             headers=headers,
             files=files,
             verify=self.auth.verify_certificate,
+            params=params,
         )
         return self._attachment_response(self.auth.api_base_url + path, headers, response, "POST")
 
     def _put_attachments(
         self, path: str, files: list[tuple[str, tuple[Any, BinaryIO]]] | None = None
     ) -> Response | None:
         headers = self.auth.http_headers
```

### Comparing `vectice-24.2.2.0/src/vectice/api/version.py` & `vectice-24.2.3.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/api/workspace.py` & `vectice-24.2.3.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import TYPE_CHECKING
 
 from vectice.autolog.asset_services.metric_service import MetricService
 from vectice.autolog.model_library import ModelLibrary
 
 if TYPE_CHECKING:
-    from keras.models import Model as KerasModel
+    from keras.models import Model as KerasModel  # type: ignore[reportMissingImports]
 
 
 class AutologKerasService(MetricService):
     def __init__(self, key: str, asset: KerasModel, data: dict):
         self._asset = asset
         self._key = key
```

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/metric_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/metric_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import ast
 from functools import reduce
 from typing import TYPE_CHECKING, Any
 
 from vectice.utils.code_parser import VariableVisitor, preprocess_code
 
 if TYPE_CHECKING:
-    from keras.models import Model as KerasModel
+    from keras.models import Model as KerasModel  # type: ignore[reportMissingImports]
 
 
 class MetricService:
     def __init__(self, cell_data: dict):
         self._cell_data = cell_data
         self._model_cell = None
```

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/pytorch_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/pytorch_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.3.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/autolog.py` & `vectice-24.2.3.0/src/vectice/autolog/autolog.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.3.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if is_catboost:
             from catboost.core import CatBoost
 
             if isinstance(asset, CatBoost):
                 return AutologCatboostService(key, asset, data)
 
         if is_keras:
-            from keras.models import Model as KerasModel
+            from keras.models import Model as KerasModel  # type: ignore[reportMissingImports]
 
             if isinstance(asset, KerasModel):
                 return AutologKerasService(key, asset, data)
 
         if is_pytorch:
             from torch.nn import Module
```

### Comparing `vectice-24.2.2.0/src/vectice/autolog/autolog_class.py` & `vectice-24.2.3.0/src/vectice/autolog/autolog_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 from vectice.api.http_error_handlers import VecticeException
 from vectice.autolog.autolog_asset_factory import AssetFactory
 from vectice.autolog.model_library import ModelLibrary
 from vectice.models.dataset import Dataset
 from vectice.models.model import Model
 from vectice.models.table import Table
-from vectice.utils.code_parser import VariableVisitor, parse_comments, preprocess_code
+from vectice.utils.code_parser import FilePathVisitor, VariableVisitor, parse_comments, preprocess_code
 
 if TYPE_CHECKING:
     from tempfile import TemporaryDirectory
 
     from catboost.core import CatBoost
-    from keras import Model as KerasModel
-    from keras.layers import InputLayer
+    from keras import Model as KerasModel  # type: ignore[reportMissingImports]
+    from keras.layers import InputLayer  # type: ignore[reportMissingImports]
     from lightgbm.basic import Booster
     from pandas import DataFrame
     from pyspark.sql import DataFrame as SparkDF
     from sklearn.base import BaseEstimator
     from torch.nn import Module as TorchModel
 
     # Vectice Object types
@@ -120,45 +120,30 @@
         if "seaborn" in cell_content or "sns" in cell_content:
             return True
         if "plotly" in cell_content or "px" in cell_content:
             _logger.warning("Plotly is not supported currently.")
             return False
         return False
 
-    def _get_graph_path(cell_content: str, graph: str) -> str | None:
-        # check if the `path` is a var or a graph and get the path
-        # because it's pre_run_cell we can't get the var from locals and it's possible the graph doesn't exist yet
-        match = re.search(rf"{graph}\s*=\s*(.*?)\n", cell_content)
-        if match:
-            graph = match.group(1)
-        try:
-            return literal_eval(graph)
-        except ValueError as e:
-            _logger.debug(f"Graph path failed {e}")
-            return None
-
     def _get_graphs(remove: bool) -> list[str]:
-        graphs = []
         cell_content = ipython.get_parent()["content"]["code"]  # type: ignore
         # get commented lines and not lines with comments
         lines = cell_content.split("\n")
         matched_lines = "\n".join(
             [line for line in lines if (remove and re.search(r"^#.*", line)) or not re.search(r"^#.*", line)]
         )
+        cell = preprocess_code(matched_lines)
+        tree = ast.parse(cell)
+        visitor = FilePathVisitor()
+        visitor.visit(tree)
 
-        # seaborn and matplotlib support
-        graphs += re.findall(r"(?<=\.savefig\()[^)\n]*[^\)\n]", matched_lines)
-        # plotly support
-        graphs += re.findall(r"(?<=\.write_image\()[^)\n]*[^\)\n]", matched_lines)
-        # ensure we have paths
         graph_paths = []
-        for graph in graphs:
-            graph_path = _get_graph_path(cell_content, graph)
-            if graph_path:
-                graph_paths.append(graph_path)
+        for graph in visitor.file_paths:
+            if "http" not in graph:
+                graph_paths.append(graph)
         return graph_paths
 
     def _remove_commented_graphs():
         # removes a saved graph if commented out
         graphs = _get_graphs(True)
 
         for graph in graphs:
@@ -397,15 +382,17 @@
         return "sklearn"
 
     def _get_sklearn_or_xgboost_or_lgbm_info(
         self, model: BaseEstimator
     ) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         try:
             library = self._get_model_library(model)
-            params = {str(key): value for key, value in model.get_params().items() if value is not None}
+            params = {
+                str(key): value for key, value in model.get_params().items() if value is not None and bool(str(value))
+            }
             return library, params
         except AttributeError:
             return None, None
 
     def _format_keras_params(self, model: KerasModel) -> dict[str, Any]:
         params: dict[str, Any] = {}
 
@@ -580,15 +567,15 @@
     def _log_model(self, model: TModel):
         temp_dir: TemporaryDirectory | None = None
         temp_file_path: str | None = None
         if model["library"] is ModelLibrary.KERAS:
             graph = None
 
             try:
-                from keras.utils import plot_model
+                from keras.utils import plot_model  # type: ignore[reportMissingImports]
 
                 temp_dir = tempfile.TemporaryDirectory()
                 file_name = f"{model['variable']!s}_plot.png"
                 temp_file_path = rf"{temp_dir.name}\{file_name}"
                 graph = plot_model(model["model"], to_file=temp_file_path, show_shapes=True, show_layer_names=False)
 
                 if graph is None:
```

### Comparing `vectice-24.2.2.0/src/vectice/connection.py` & `vectice-24.2.3.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/__init__.py` & `vectice-24.2.3.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/additional_info.py` & `vectice-24.2.3.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/attachment_container.py` & `vectice-24.2.3.0/src/vectice/models/attachment_container.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
 import io
 import logging
 import os
+from functools import reduce
 from typing import TYPE_CHECKING, BinaryIO, List
 
 from vectice.api.json.model_version import ModelVersionOutput
+from vectice.models.attachment import TFormattedAttachment
+from vectice.models.table import Table
 from vectice.types.version import TVersion
+from vectice.utils.common_utils import capture_unique_attachments
 
 if TYPE_CHECKING:
     from vectice.api import Client
 
 _logger = logging.getLogger(__name__)
 
 FILE_PATH_DOES_NOT_EXIST_ERROR_MESSAGE = "The file path '%s' is not valid. The file does not exist."
@@ -31,29 +35,47 @@
     def name(self):
         return self._name
 
     @property
     def id(self):
         return self._id
 
-    def upsert_attachments(self, file_paths: str | list[str]):
+    def upsert_attachments(self, attachments: list[TFormattedAttachment]):
         """Add an attachment or set of attachments to the entity.
 
         Parameters:
-            file_paths: The paths of the attachment(s).
+            attachments: The paths of the attachment(s).
 
         Returns:
             A list of dictionaries describing the attachments.
         """
-        file_paths = [file_paths] if isinstance(file_paths, str) else file_paths
-        attachments = self._add_files_to_attachments(file_paths)
-        try:
-            return self._client.upsert_version_attachments(attachments, self._version)
-        finally:
-            self._close_attached_files(attachments)
+
+        def _upsert_files(files: list[str]) -> list[str]:
+            if len(files) > 0:
+                files_attachments = self._add_files_to_attachments(files)
+                try:
+                    return list(
+                        map(
+                            lambda curr: curr.fileName,
+                            self._client.upsert_version_attachments(files_attachments, self._version),
+                        )
+                    )
+                finally:
+                    self._close_attached_files(files_attachments)
+            return []
+
+        def _upsert_tables(tables: list[Table]) -> list[str]:
+            return (
+                list(map(lambda curr: curr["name"], self._client.upsert_version_tables(tables, self._version)))
+                if len(tables) > 0
+                else []
+            )
+
+        files, tables = reduce(capture_unique_attachments, attachments, ([], []))
+        return [*_upsert_files(files), *_upsert_tables(tables)]
 
     def _add_files_to_attachments(self, file_paths: list[str]) -> list[tuple[str, tuple[str, BinaryIO]]]:
         attachments: List[tuple[str, tuple[str, BinaryIO]]] = []
         for file_path in file_paths:
             if not os.path.exists(file_path):
                 raise ValueError(FILE_PATH_DOES_NOT_EXIST_ERROR_MESSAGE % file_path)
             curr_file = ("file", (file_path, open(file_path, "rb")))
```

### Comparing `vectice-24.2.2.0/src/vectice/models/code_version.py` & `vectice-24.2.3.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/dataset.py` & `vectice-24.2.3.0/src/vectice/models/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from datetime import datetime
 from typing import Union
 
 from typing_extensions import get_args
 
 from vectice.api.http_error_handlers import VecticeException
+from vectice.models.attachment import TAttachment, TFormattedAttachment
 from vectice.models.property import Property
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
 from vectice.models.resource.snowflake_resource import SnowflakeResource
 from vectice.utils.common_utils import format_attachments, format_properties
@@ -18,25 +19,26 @@
 _logger = logging.getLogger(__name__)
 
 
 TBaseDerivedFrom = Union[str, DatasetRepresentation, DatasetVersionRepresentation]
 
 
 class Dataset:
+
     def __init__(
         self,
         type: DatasetType,
         name: str | None = None,
         resource: Resource | None = None,
         training_resource: Resource | None = None,
         testing_resource: Resource | None = None,
         validation_resource: Resource | None = None,
         derived_from: list[TBaseDerivedFrom | Dataset] | TBaseDerivedFrom | Dataset | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
-        attachments: str | list[str] | None = None,
+        attachments: TAttachment | None = None,
     ):
         self._type = type
         self._name = name or f"dataset {datetime.now()}"
         self._resource = resource
         self._training_resource = training_resource
         self._testing_resource = testing_resource
         self._validation_resource = validation_resource
@@ -258,24 +260,24 @@
         Parameters:
             properties: The properties of the dataset.
         """
         _logger.warning("To save your updated dataset properties, you must reassign your dataset to an iteration.")
         self._properties = format_properties(properties) if properties else None
 
     @property
-    def attachments(self) -> list[str] | None:
+    def attachments(self) -> list[TFormattedAttachment] | None:
         """The attachments associated with the dataset.
 
         Returns:
             The attachments associated with the dataset.
         """
         return self._attachments
 
     @attachments.setter
-    def attachments(self, attachments: list[str] | str):
+    def attachments(self, attachments: TAttachment):
         """Attach a file or files to the dataset.
 
         Parameters:
             attachments: The filename or filenames of the file or set of files to attach to the dataset.
         """
         self._attachments = format_attachments(attachments)
```

### Comparing `vectice-24.2.2.0/src/vectice/models/iteration.py` & `vectice-24.2.3.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/metric.py` & `vectice-24.2.3.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/model.py` & `vectice-24.2.3.0/src/vectice/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import logging
 import pickle  # nosec
 from typing import TYPE_CHECKING, Any, List
 
+from vectice.models.attachment import TAttachment, TFormattedAttachment
+
 if TYPE_CHECKING:
     from mlflow import MlflowClient
 
 from vectice.models import AdditionalInfo, ExtraInfo, Metric, Property
 from vectice.models.dataset import TDerivedFrom, get_derived_from
 from vectice.utils.common_utils import check_key_duplicates, format_attachments, format_metrics, format_properties
 
@@ -196,24 +198,24 @@
         Parameters:
             properties: The properties of the model.
         """
         _logger.warning("To save your updated model properties, you must reassign your model to an iteration.")
         self._properties = format_properties(properties) if properties else None
 
     @property
-    def attachments(self) -> list[str] | None:
+    def attachments(self) -> list[TFormattedAttachment] | None:
         """The attachments associated with the model.
 
         Returns:
             The attachments associated with the model.
         """
         return self._attachments
 
     @attachments.setter
-    def attachments(self, attachments: list[str] | str):
+    def attachments(self, attachments: TAttachment):
         """Attach a file or files to the model.
 
         Parameters:
             attachments: The filename or filenames of the file or set of files to attach to the model.
         """
         self._attachments = format_attachments(attachments)
```

### Comparing `vectice-24.2.2.0/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.3.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/model_mlflow.py` & `vectice-24.2.3.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/phase.py` & `vectice-24.2.3.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/project.py` & `vectice-24.2.3.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/property.py` & `vectice-24.2.3.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.3.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.3.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List
 
 from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
+from vectice.models.attachment import TAttachment
 from vectice.models.attachment_container import AttachmentContainer
 from vectice.models.property import Property
 from vectice.models.representation.dataset_representation import DatasetRepresentation
-from vectice.utils.common_utils import format_properties, repr_class, strip_dict_list
+from vectice.utils.common_utils import format_attachments, format_properties, repr_class, strip_dict_list
 from vectice.utils.dataframe_utils import repr_list_as_pd_dataframe
 
 if TYPE_CHECKING:
     from pandas import DataFrame
 
     from vectice.api.client import Client
 
@@ -128,11 +129,11 @@
 
     def _upsert_properties(self, properties: dict[str, str | int] | list[Property] | Property):
         clean_properties = list(map(lambda property: property.key_val_dict(), format_properties(properties)))
         new_properties = self._client.upsert_properties("dataSetVersion", self.id, clean_properties)
         self.properties = strip_dict_list(new_properties)
         _logger.info(f"Dataset version {self.id!r} properties successfully updated.")
 
-    def _update_attachments(self, attachments: str | list[str]):
+    def _update_attachments(self, attachments: TAttachment):
         container = AttachmentContainer(self._output, self._client)
-        container.upsert_attachments(attachments)
+        container.upsert_attachments(format_attachments(attachments))
         _logger.info(f"Dataset version {self.id!r} attachments successfully updated.")
```

### Comparing `vectice-24.2.2.0/src/vectice/models/representation/model_representation.py` & `vectice-24.2.3.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.3.0/src/vectice/models/representation/model_version_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Any, Dict
 
 from vectice.api.json.model_version import ModelVersionStatus
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput, ModelVersionUpdateInput
+from vectice.models.attachment import TAttachment
 from vectice.models.attachment_container import AttachmentContainer
 from vectice.models.metric import Metric
 from vectice.models.property import Property
 from vectice.utils.common_utils import (
     convert_list_keyvalue_to_dict,
+    format_attachments,
     format_metrics,
     format_properties,
     repr_class,
     strip_dict_list,
 )
 from vectice.utils.dataframe_utils import repr_list_as_pd_dataframe
 
@@ -157,11 +159,11 @@
         _logger.info(f"Model version {self.id!r} properties successfully updated.")
 
     def _upsert_metrics(self, metrics: dict[str, int | float] | list[Metric] | Metric):
         clean_metrics = list(map(lambda metric: metric.key_val_dict(), format_metrics(metrics)))
         self.metrics = self._client.upsert_metrics("modelVersion", self.id, clean_metrics)
         _logger.info(f"Model version {self.id!r} metrics successfully updated.")
 
-    def _update_attachments(self, attachments: str | list[str]):
+    def _update_attachments(self, attachments: TAttachment):
         container = AttachmentContainer(self._output, self._client)
-        container.upsert_attachments(attachments)
+        container.upsert_attachments(format_attachments(attachments))
         _logger.info(f"Model version {self.id!r} attachments successfully updated.")
```

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/__init__.py` & `vectice-24.2.3.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/base.py` & `vectice-24.2.3.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/description.py` & `vectice-24.2.3.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/file_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.3.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/no_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.3.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/table.py` & `vectice-24.2.3.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/test_library/binary_classification_test.py` & `vectice-24.2.3.0/src/vectice/models/test_library/binary_classification_test.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/validation.py` & `vectice-24.2.3.0/src/vectice/models/validation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/models/workspace.py` & `vectice-24.2.3.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/services/phase_service.py` & `vectice-24.2.3.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/types/version.py` & `vectice-24.2.3.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/utils/code_parser.py` & `vectice-24.2.3.0/src/vectice/utils/code_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,92 @@
 from __future__ import annotations
 
 import ast
+import os
 import re
 from collections import OrderedDict
 from typing import Any
 
 
+class FilePathVisitor(ast.NodeVisitor):
+    def __init__(self):
+        self.file_paths = set()
+
+    def visit_Call(self, node: ast.Call) -> None:  # noqa: N802
+        if isinstance(node.func, ast.Name) or isinstance(node.func, ast.Attribute):
+            # Record function args, kwargs.
+            try:
+                func_name = node.func.attr  # pyright: ignore[reportAttributeAccessIssue]
+                supported_graph = self._is_supported_graph_library(func_name)
+            except AttributeError:
+                supported_graph = False
+
+            args = node.args + node.keywords
+            for arg in args:
+                arg_value = self._get_arg_or_kwarg_val(arg)
+                if arg_value and self._is_valid_file(arg_value) and supported_graph:
+                    self.file_paths.add(arg_value)
+        self.generic_visit(node)
+
+    def visit_Assign(self, node: ast.Assign) -> None:
+        try:
+            if len(node.targets) == 1 and isinstance(
+                node.targets[0], ast.Name
+            ):  # pyright: ignore[reportAttributeAccessIssue]
+                if isinstance(node.value, ast.Str):  # pyright: ignore[reportDeprecated]
+                    path = node.value.s  # pyright: ignore[reportAttributeAccessIssue]
+                    if self._is_valid_file(path):
+                        self.file_paths.add(path)
+        except Exception:
+            pass
+        self.generic_visit(node)
+
+    def _get_arg_or_kwarg_val(self, arg: Any) -> Any | None:
+        try:
+            # arg value
+            if isinstance(arg.id, str):
+                return arg.id  # pyright: ignore[reportAttributeAccessIssue]
+        except AttributeError:
+            pass
+        try:
+            # kwarg value if not a variable
+            if isinstance(arg.value.value, str):
+                return arg.value.value  # pyright: ignore[reportAttributeAccessIssue]
+        except AttributeError:
+            pass
+        try:
+            # kwarg value if it is a variable
+            if isinstance(arg.value.id, str):
+                return arg.value.id  # pyright: ignore[reportAttributeAccessIssue]
+        except AttributeError:
+            pass
+        try:
+            if isinstance(arg.value, str):
+                return arg.value  # pyright: ignore[reportAttributeAccessIssue]
+        except AttributeError:
+            pass
+        return None
+
+    def _is_valid_file(self, path: str) -> bool:
+        is_file = os.path.isfile(path)
+        _, extension = os.path.splitext(path)
+        if is_file or extension:
+            return True
+        return False
+
+    def _is_supported_graph_library(self, func_name: str) -> bool:
+        vectice_supported_graphs = [
+            "savefig",
+            "write_image",
+        ]
+        if func_name in vectice_supported_graphs:
+            return True
+        return False
+
+
 class VariableVisitor(ast.NodeVisitor):
     def __init__(self, model_metrics: bool = False):
         self.variables: OrderedDict[str, None] = OrderedDict()
         self.processed_variables: set[str] = set()
         self.function_call_args: set[str] = set()
         self.function_call_kwargs: set[str] = set()
         self.variable_calls: set[str] = set()
```

### Comparing `vectice-24.2.2.0/src/vectice/utils/common_utils.py` & `vectice-24.2.3.0/src/vectice/utils/common_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import logging
 import mimetypes
 import os
 import pickle  # nosec
 import re
 from contextlib import contextmanager
 from enum import Enum
+from functools import reduce
 from io import BufferedReader, BytesIO, IOBase
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from PIL import Image, ImageFile
 from rich.console import Console
 from rich.table import Table
 
 from vectice.api.http_error_handlers import VecticeException
 from vectice.api.json.iteration import IterationStatus
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
-from vectice.models.attachment_container import AttachmentContainer
+from vectice.models.attachment import TAttachment, TFormattedAttachment
 from vectice.models.metric import Metric
 from vectice.models.property import Property
+from vectice.models.table import Table as VecticeTable
 
 if TYPE_CHECKING:
     from vectice.api.client import Client
-    from vectice.api.json import AttachmentOutput
     from vectice.api.json.dataset_version import DatasetVersionOutput
     from vectice.api.json.model_version import ModelVersionOutput
     from vectice.models.dataset import Dataset
     from vectice.models.iteration import Iteration
     from vectice.models.model import Model
 
 
@@ -149,22 +150,42 @@
         if isinstance(value, dict):
             value = convert_keys_to_camel_case(value)
         camel_case_dict[camel_case_key] = value
 
     return camel_case_dict
 
 
-def format_attachments(attachments: str | list[str]) -> list[str]:
-    list_attachments = (
-        [attachment for attachment in set(attachments)] if isinstance(attachments, list) else [attachments]
-    )
+def capture_unique_attachments(attachments: tuple[list[str], list[VecticeTable]], curr: TFormattedAttachment | Any):
+
+    str_list, table_list = attachments
+    if isinstance(curr, str):
+        if curr not in str_list:
+            return [*str_list, curr], table_list
+    elif isinstance(curr, VecticeTable):
+        if curr not in table_list:
+            return str_list, [*table_list, curr]
+    else:
+        raise ValueError(
+            f"The element '{curr}' in 'attachments' is of type '{type(curr)}', which is invalid. Only strings and Vectice Tables instances are supported."
+        )
+    return str_list, table_list
+
+
+def format_attachments(attachments: TAttachment) -> list[TFormattedAttachment]:
+    if not isinstance(attachments, list):
+        attachments = [attachments]
+    str_list, table_list = reduce(capture_unique_attachments, attachments, ([], []))
+    list_attachments = [*str_list, *table_list]
+
     for attachment in list_attachments:
-        if not isinstance(attachment, str):  # pyright: ignore[reportUnnecessaryIsInstance]
+        if not isinstance(attachment, str) and not isinstance(
+            attachment, VecticeTable
+        ):  # pyright: ignore[reportUnnecessaryIsInstance]
             raise ValueError(
-                f"Argument 'attachments' with type '{type(attachment)}' is invalid, only str are supported."
+                f"Argument 'attachments' with type '{type(attachment)}' is invalid, only str and tables are supported."
             )
     return list_attachments
 
 
 def check_string_sanity(value: str):
     if value == "":
         raise VecticeException("Cannot assign an empty comment. Please provide a valid comment")
@@ -183,15 +204,17 @@
         or isinstance(value, ModelVersionRepresentation)
     ) and value.project_id != project_id:
         raise VecticeException("Assigning an asset coming from another project is forbidden")
 
 
 def set_model_attachments(
     client: Client, model: Model, model_version: ModelVersionOutput
-) -> tuple[list[AttachmentOutput] | None, bool]:
+) -> tuple[list[str] | None, bool]:
+    from vectice.models.attachment_container import AttachmentContainer
+
     logging.getLogger("vectice.models.attachment_container").propagate = True
     attachments = None
     if model.attachments:
         container = AttachmentContainer(model_version, client)
         attachments = container.upsert_attachments(model.attachments)
 
     success_pickle: bool = False
@@ -205,14 +228,16 @@
         except Exception:
             success_pickle = False
 
     return attachments, success_pickle
 
 
 def set_dataset_attachments(client: Client, dataset: Dataset, dataset_version: DatasetVersionOutput):
+    from vectice.models.attachment_container import AttachmentContainer
+
     logging.getLogger("vectice.models.attachment_container").propagate = True
     attachments = None
     if dataset.attachments:
         container = AttachmentContainer(dataset_version, client)
         attachments = container.upsert_attachments(dataset.attachments)
     return attachments
```

### Comparing `vectice-24.2.2.0/src/vectice/utils/configuration.py` & `vectice-24.2.3.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/utils/deprecation.py` & `vectice-24.2.3.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/utils/instance_helper.py` & `vectice-24.2.3.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice/utils/last_assets.py` & `vectice-24.2.3.0/src/vectice/utils/last_assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
 from PIL import Image
 
-from vectice.api.json.attachment import AttachmentOutput
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_representation import ModelRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 
 if TYPE_CHECKING:
     from logging import Logger
@@ -97,18 +96,18 @@
     _logger.info(logging_output)
 
 
 def _get_full_asset_log(
     asset_log: str,
     iteration: Iteration,
     section: str | None,
-    attachments: list[AttachmentOutput] | None,
+    attachments: list[str] | None,
     existing_asset: bool = False,
 ):
-    attachments_output = ", ".join([attach.fileName for attach in attachments]) if attachments else "None"
+    attachments_output = ", ".join([attach for attach in attachments]) if attachments else "None"
     assignment_log, iteration_link_log = _get_iteration_log(iteration, section, existing_asset)
     return dedent(
         f"""
             {asset_log} {assignment_log}
             Attachments: {attachments_output}
             {iteration_link_log}
         """
@@ -125,29 +124,29 @@
     return f"New dataset: {value.name!r} version: {dsv_name!r} added"
 
 
 def register_dataset_logging(
     iteration: Iteration,
     data: DatasetRegisterOutput,
     value: Dataset,
-    attachments: list[AttachmentOutput] | None,
+    attachments: list[str] | None,
     _logger: Logger,
     section: str | None = None,
 ):
     asset_log = _get_register_dataset_log(data, value)
     extisting_asset: bool = True if data.use_existing_version else False
     logging_output = _get_full_asset_log(asset_log, iteration, section, attachments, extisting_asset)
     _logger.info(logging_output)
 
 
 def register_model_logging(
     iteration: Iteration,
     data: ModelRegisterOutput,
     value: Model,
-    attachments: list[AttachmentOutput] | None,
+    attachments: list[str] | None,
     success_pickle: bool,
     _logger: Logger,
     section: str | None = None,
 ):
     mv_name = data.model_version.name
     asset_log = (
         f"New version: {mv_name!r} of model: {value.name!r} added"
```

### Comparing `vectice-24.2.2.0/src/vectice/utils/logging_utils.py` & `vectice-24.2.3.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.2.0/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.3.0/src/vectice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.2.0
+Version: 24.2.3.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -40,20 +40,20 @@
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: dataclasses-json==0.5.8
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
-Requires-Dist: pyright==1.1.354; extra == "dev"
+Requires-Dist: pyright==1.1.360; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
-Requires-Dist: boto3-stubs[essential]; extra == "dev"
+Requires-Dist: mypy_boto3_s3==1.34.65; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: black==24.2.0; extra == "doc"
 Requires-Dist: markdown-callouts>=0.2; extra == "doc"
 Requires-Dist: markdown-exec>=1.2; extra == "doc"
 Requires-Dist: mkdocs==1.4.2; extra == "doc"
 Requires-Dist: mkdocs-material>=7.3; extra == "doc"
```

### Comparing `vectice-24.2.2.0/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.3.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/vectice/api/__init__.py
 src/vectice/api/_auth.py
 src/vectice/api/_utils.py
 src/vectice/api/attachment.py
 src/vectice/api/client.py
 src/vectice/api/compatibility.py
 src/vectice/api/gql_api.py
+src/vectice/api/gql_attachment.py
 src/vectice/api/gql_dataset.py
 src/vectice/api/gql_entity_file.py
 src/vectice/api/gql_feature_flag.py
 src/vectice/api/gql_metric.py
 src/vectice/api/gql_model.py
 src/vectice/api/gql_organization.py
 src/vectice/api/gql_property.py
@@ -82,14 +83,15 @@
 src/vectice/autolog/asset_services/pandas_service.py
 src/vectice/autolog/asset_services/pyspark_service.py
 src/vectice/autolog/asset_services/pytorch_service.py
 src/vectice/autolog/asset_services/sklearn_service.py
 src/vectice/autolog/asset_services/vectice_asset_service.py
 src/vectice/models/__init__.py
 src/vectice/models/additional_info.py
+src/vectice/models/attachment.py
 src/vectice/models/attachment_container.py
 src/vectice/models/code_version.py
 src/vectice/models/dataset.py
 src/vectice/models/errors.py
 src/vectice/models/iteration.py
 src/vectice/models/metric.py
 src/vectice/models/model.py
```

### Comparing `vectice-24.2.2.0/src/vectice.egg-info/requires.txt` & `vectice-24.2.3.0/src/vectice.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 [autolog]
 IPython
 
 [dev]
 black==24.2.0
 gitpython
-pyright==1.1.354
+pyright==1.1.360
 ruff
 types-requests
 types-urllib3
 types-mock
-boto3-stubs[essential]
+mypy_boto3_s3==1.34.65
 pandas-stubs
 
 [doc]
 black==24.2.0
 markdown-callouts>=0.2
 markdown-exec>=1.2
 mkdocs==1.4.2
```

