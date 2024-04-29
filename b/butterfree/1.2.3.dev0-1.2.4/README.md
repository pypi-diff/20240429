# Comparing `tmp/butterfree-1.2.3.dev0.tar.gz` & `tmp/butterfree-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/butterfree-1.2.3.dev0.tar", last modified: Mon Nov 13 15:03:56 2023, max compression
+gzip compressed data, was "dist/butterfree-1.2.4.tar", last modified: Mon Apr 29 13:04:39 2024, max compression
```

## Comparing `butterfree-1.2.3.dev0.tar` & `butterfree-1.2.4.tar`

### file list

```diff
@@ -1,129 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/
--rw-r--r--   0 root         (0) root         (0)    11370 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5054 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4646 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/
--rw-r--r--   0 root         (0) root         (0)       68 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      152 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/_cli/main.py
--rw-r--r--   0 root         (0) root         (0)     6033 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/_cli/migrate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/clients/
--rw-r--r--   0 root         (0) root         (0)      278 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/clients/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     5124 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/clients/cassandra_client.py
--rw-r--r--   0 root         (0) root         (0)    11705 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/clients/spark_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/configs/
--rw-r--r--   0 root         (0) root         (0)       59 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/configs/db/
--rw-r--r--   0 root         (0) root         (0)      423 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/db/abstract_config.py
--rw-r--r--   0 root         (0) root         (0)     8902 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/db/cassandra_config.py
--rw-r--r--   0 root         (0) root         (0)     4848 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/db/kafka_config.py
--rw-r--r--   0 root         (0) root         (0)     4528 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/db/metastore_config.py
--rw-r--r--   0 root         (0) root         (0)     1796 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/environment.py
--rw-r--r--   0 root         (0) root         (0)      643 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/configs/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/constants/
--rw-r--r--   0 root         (0) root         (0)      140 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/constants/__init__.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/constants/columns.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/constants/data_type.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/constants/migrations.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/constants/spark_constants.py
--rw-r--r--   0 root         (0) root         (0)      307 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/constants/window_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/dataframe_service/
--rw-r--r--   0 root         (0) root         (0)      435 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/dataframe_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/dataframe_service/incremental_strategy.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/dataframe_service/partitioning.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/dataframe_service/repartition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/extract/
--rw-r--r--   0 root         (0) root         (0)      112 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/
--rw-r--r--   0 root         (0) root         (0)      529 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/explode_json_column_transform.py
--rw-r--r--   0 root         (0) root         (0)      570 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/filter_transform.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/forward_fill_transform.py
--rw-r--r--   0 root         (0) root         (0)     6397 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/pivot_transform.py
--rw-r--r--   0 root         (0) root         (0)     2370 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/pre_processing/replace_transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/extract/readers/
--rw-r--r--   0 root         (0) root         (0)      286 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/readers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/readers/file_reader.py
--rw-r--r--   0 root         (0) root         (0)     6565 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/readers/kafka_reader.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/readers/reader.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/readers/table_reader.py
--rw-r--r--   0 root         (0) root         (0)     3920 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/extract/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/hooks/
--rw-r--r--   0 root         (0) root         (0)      177 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/hooks/hook.py
--rw-r--r--   0 root         (0) root         (0)     5264 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/hooks/hookable_component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/hooks/schema_compatibility/
--rw-r--r--   0 root         (0) root         (0)      428 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/hooks/schema_compatibility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/hooks/schema_compatibility/cassandra_table_schema_compatibility_hook.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/hooks/schema_compatibility/spark_table_schema_compatibility_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/load/
--rw-r--r--   0 root         (0) root         (0)      117 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/load/processing/
--rw-r--r--   0 root         (0) root         (0)      150 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/processing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/processing/json_transform.py
--rw-r--r--   0 root         (0) root         (0)     3912 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/sink.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/load/writers/
--rw-r--r--   0 root         (0) root         (0)      334 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10926 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/writers/historical_feature_store_writer.py
--rw-r--r--   0 root         (0) root         (0)    10470 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/writers/online_feature_store_writer.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/load/writers/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/migrations/
--rw-r--r--   0 root         (0) root         (0)       34 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/migrations/database_migration/
--rw-r--r--   0 root         (0) root         (0)      490 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/migrations/database_migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4686 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/migrations/database_migration/cassandra_migration.py
--rw-r--r--   0 root         (0) root         (0)     9712 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/migrations/database_migration/database_migration.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/migrations/database_migration/metastore_migration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/pipelines/
--rw-r--r--   0 root         (0) root         (0)      128 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9655 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/pipelines/feature_set_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/reports/
--rw-r--r--   0 root         (0) root         (0)       95 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/reports/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/testing/
--rw-r--r--   0 root         (0) root         (0)       60 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/testing/dataframe/
--rw-r--r--   0 root         (0) root         (0)     2869 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/testing/dataframe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/transform/
--rw-r--r--   0 root         (0) root         (0)      131 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25615 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/aggregated_feature_set.py
--rw-r--r--   0 root         (0) root         (0)    16929 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/feature_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/transform/features/
--rw-r--r--   0 root         (0) root         (0)      316 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/features/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/features/feature.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/features/key_feature.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/features/timestamp_feature.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/
--rw-r--r--   0 root         (0) root         (0)      943 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4808 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/aggregated_transform.py
--rw-r--r--   0 root         (0) root         (0)     3692 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/custom_transform.py
--rw-r--r--   0 root         (0) root         (0)     4953 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/h3_transform.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/spark_function_transform.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/sql_expression_transform.py
--rw-r--r--   0 root         (0) root         (0)     4767 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/stack_transform.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/transform_component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/user_defined_functions/
--rw-r--r--   0 root         (0) root         (0)      468 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/user_defined_functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/user_defined_functions/mode.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/transformations/user_defined_functions/most_frequent_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/transform/utils/
--rw-r--r--   0 root         (0) root         (0)      210 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/utils/date_range.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/utils/function.py
--rw-r--r--   0 root         (0) root         (0)     3842 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/transform/utils/window_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree/validations/
--rw-r--r--   0 root         (0) root         (0)      157 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/validations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/validations/basic_validaton.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/butterfree/validations/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5054 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4149 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      191 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/butterfree.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      939 2023-11-13 15:03:56.000000 butterfree-1.2.3.dev0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1158 2023-11-13 15:02:44.000000 butterfree-1.2.3.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)    11370 2024-04-29 12:59:38.000000 butterfree-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5049 2024-04-29 13:04:39.000000 butterfree-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4646 2024-04-29 12:59:38.000000 butterfree-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/_cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     6033 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/_cli/migrate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/automated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/automated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6198 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/automated/feature_set_creation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/clients/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/clients/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     5124 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/clients/cassandra_client.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/clients/spark_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/configs/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/configs/db/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/db/abstract_config.py
+-rw-r--r--   0 root         (0) root         (0)     8902 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/db/cassandra_config.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/db/kafka_config.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/db/metastore_config.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/environment.py
+-rw-r--r--   0 root         (0) root         (0)      643 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/configs/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/constants/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/constants/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/constants/columns.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/constants/data_type.py
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/constants/migrations.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/constants/spark_constants.py
+-rw-r--r--   0 root         (0) root         (0)      307 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/constants/window_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/dataframe_service/
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/dataframe_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/dataframe_service/incremental_strategy.py
+-rw-r--r--   0 root         (0) root         (0)      662 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/dataframe_service/partitioning.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/dataframe_service/repartition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/extract/
+-rw-r--r--   0 root         (0) root         (0)      112 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/extract/pre_processing/
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/pre_processing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/pre_processing/explode_json_column_transform.py
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/pre_processing/filter_transform.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/pre_processing/forward_fill_transform.py
+-rw-r--r--   0 root         (0) root         (0)     6397 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/pre_processing/pivot_transform.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/pre_processing/replace_transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/extract/readers/
+-rw-r--r--   0 root         (0) root         (0)      286 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/readers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/readers/file_reader.py
+-rw-r--r--   0 root         (0) root         (0)     6565 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/readers/kafka_reader.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/readers/reader.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/readers/table_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/extract/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/hooks/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      441 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/hooks/hook.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/hooks/hookable_component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/hooks/schema_compatibility/
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/hooks/schema_compatibility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/hooks/schema_compatibility/cassandra_table_schema_compatibility_hook.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/hooks/schema_compatibility/spark_table_schema_compatibility_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/load/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/load/processing/
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/processing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      518 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/processing/json_transform.py
+-rw-r--r--   0 root         (0) root         (0)     3912 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/sink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/load/writers/
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/writers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10926 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/writers/historical_feature_store_writer.py
+-rw-r--r--   0 root         (0) root         (0)    10470 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/writers/online_feature_store_writer.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/load/writers/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/migrations/
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/migrations/database_migration/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/migrations/database_migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/migrations/database_migration/cassandra_migration.py
+-rw-r--r--   0 root         (0) root         (0)     9712 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/migrations/database_migration/database_migration.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/migrations/database_migration/metastore_migration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/pipelines/
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9655 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/pipelines/feature_set_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/reports/
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/reports/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/testing/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/testing/dataframe/
+-rw-r--r--   0 root         (0) root         (0)     2869 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/testing/dataframe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/transform/
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25615 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/aggregated_feature_set.py
+-rw-r--r--   0 root         (0) root         (0)    16929 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/feature_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/transform/features/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/features/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/features/feature.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/features/key_feature.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/features/timestamp_feature.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/transform/transformations/
+-rw-r--r--   0 root         (0) root         (0)      943 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/aggregated_transform.py
+-rw-r--r--   0 root         (0) root         (0)     3692 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/custom_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4953 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/h3_transform.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/spark_function_transform.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/sql_expression_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4767 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/stack_transform.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/transform_component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/transform/transformations/user_defined_functions/
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/user_defined_functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/user_defined_functions/mode.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/transformations/user_defined_functions/most_frequent_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/transform/utils/
+-rw-r--r--   0 root         (0) root         (0)      210 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/utils/date_range.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)     3842 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/transform/utils/window_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree/validations/
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/validations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/validations/basic_validaton.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-04-29 12:59:38.000000 butterfree-1.2.4/butterfree/validations/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5049 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-29 13:04:39.000000 butterfree-1.2.4/butterfree.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-29 13:04:39.000000 butterfree-1.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-29 12:59:38.000000 butterfree-1.2.4/setup.py
```

### Comparing `butterfree-1.2.3.dev0/LICENSE` & `butterfree-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/PKG-INFO` & `butterfree-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterfree
-Version: 1.2.3.dev0
+Version: 1.2.4
 Summary: A tool for building feature stores - Transform your raw data into beautiful features.
 Home-page: https://github.com/quintoandar/butterfree
 Author: QuintoAndar
 License: Copyright
 Keywords: feature store sets ETL
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `butterfree-1.2.3.dev0/README.md` & `butterfree-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/_cli/migrate.py` & `butterfree-1.2.4/butterfree/_cli/migrate.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/clients/abstract_client.py` & `butterfree-1.2.4/butterfree/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/clients/cassandra_client.py` & `butterfree-1.2.4/butterfree/clients/cassandra_client.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/clients/spark_client.py` & `butterfree-1.2.4/butterfree/clients/spark_client.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/configs/db/abstract_config.py` & `butterfree-1.2.4/butterfree/configs/db/abstract_config.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/configs/db/cassandra_config.py` & `butterfree-1.2.4/butterfree/configs/db/cassandra_config.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/configs/db/kafka_config.py` & `butterfree-1.2.4/butterfree/configs/db/kafka_config.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/configs/db/metastore_config.py` & `butterfree-1.2.4/butterfree/configs/db/metastore_config.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/configs/environment.py` & `butterfree-1.2.4/butterfree/configs/environment.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/configs/logger.py` & `butterfree-1.2.4/butterfree/configs/logger.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/constants/data_type.py` & `butterfree-1.2.4/butterfree/constants/data_type.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/dataframe_service/incremental_strategy.py` & `butterfree-1.2.4/butterfree/dataframe_service/incremental_strategy.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/dataframe_service/partitioning.py` & `butterfree-1.2.4/butterfree/dataframe_service/partitioning.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/dataframe_service/repartition.py` & `butterfree-1.2.4/butterfree/dataframe_service/repartition.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/pre_processing/__init__.py` & `butterfree-1.2.4/butterfree/extract/pre_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/pre_processing/explode_json_column_transform.py` & `butterfree-1.2.4/butterfree/extract/pre_processing/explode_json_column_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/pre_processing/filter_transform.py` & `butterfree-1.2.4/butterfree/extract/pre_processing/filter_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/pre_processing/forward_fill_transform.py` & `butterfree-1.2.4/butterfree/extract/pre_processing/forward_fill_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/pre_processing/pivot_transform.py` & `butterfree-1.2.4/butterfree/extract/pre_processing/pivot_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/pre_processing/replace_transform.py` & `butterfree-1.2.4/butterfree/extract/pre_processing/replace_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/readers/file_reader.py` & `butterfree-1.2.4/butterfree/extract/readers/file_reader.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/readers/kafka_reader.py` & `butterfree-1.2.4/butterfree/extract/readers/kafka_reader.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/readers/reader.py` & `butterfree-1.2.4/butterfree/extract/readers/reader.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/readers/table_reader.py` & `butterfree-1.2.4/butterfree/extract/readers/table_reader.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/extract/source.py` & `butterfree-1.2.4/butterfree/extract/source.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/hooks/hookable_component.py` & `butterfree-1.2.4/butterfree/hooks/hookable_component.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/hooks/schema_compatibility/cassandra_table_schema_compatibility_hook.py` & `butterfree-1.2.4/butterfree/hooks/schema_compatibility/cassandra_table_schema_compatibility_hook.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/hooks/schema_compatibility/spark_table_schema_compatibility_hook.py` & `butterfree-1.2.4/butterfree/hooks/schema_compatibility/spark_table_schema_compatibility_hook.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/load/processing/json_transform.py` & `butterfree-1.2.4/butterfree/load/processing/json_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/load/sink.py` & `butterfree-1.2.4/butterfree/load/sink.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/load/writers/historical_feature_store_writer.py` & `butterfree-1.2.4/butterfree/load/writers/historical_feature_store_writer.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/load/writers/online_feature_store_writer.py` & `butterfree-1.2.4/butterfree/load/writers/online_feature_store_writer.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/load/writers/writer.py` & `butterfree-1.2.4/butterfree/load/writers/writer.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/migrations/database_migration/cassandra_migration.py` & `butterfree-1.2.4/butterfree/migrations/database_migration/cassandra_migration.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/migrations/database_migration/database_migration.py` & `butterfree-1.2.4/butterfree/migrations/database_migration/database_migration.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/migrations/database_migration/metastore_migration.py` & `butterfree-1.2.4/butterfree/migrations/database_migration/metastore_migration.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/pipelines/feature_set_pipeline.py` & `butterfree-1.2.4/butterfree/pipelines/feature_set_pipeline.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/reports/metadata.py` & `butterfree-1.2.4/butterfree/reports/metadata.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/testing/dataframe/__init__.py` & `butterfree-1.2.4/butterfree/testing/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/aggregated_feature_set.py` & `butterfree-1.2.4/butterfree/transform/aggregated_feature_set.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/feature_set.py` & `butterfree-1.2.4/butterfree/transform/feature_set.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/features/feature.py` & `butterfree-1.2.4/butterfree/transform/features/feature.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/features/key_feature.py` & `butterfree-1.2.4/butterfree/transform/features/key_feature.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/features/timestamp_feature.py` & `butterfree-1.2.4/butterfree/transform/features/timestamp_feature.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/__init__.py` & `butterfree-1.2.4/butterfree/transform/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/aggregated_transform.py` & `butterfree-1.2.4/butterfree/transform/transformations/aggregated_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/custom_transform.py` & `butterfree-1.2.4/butterfree/transform/transformations/custom_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/h3_transform.py` & `butterfree-1.2.4/butterfree/transform/transformations/h3_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/spark_function_transform.py` & `butterfree-1.2.4/butterfree/transform/transformations/spark_function_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/sql_expression_transform.py` & `butterfree-1.2.4/butterfree/transform/transformations/sql_expression_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/stack_transform.py` & `butterfree-1.2.4/butterfree/transform/transformations/stack_transform.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/transform_component.py` & `butterfree-1.2.4/butterfree/transform/transformations/transform_component.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/user_defined_functions/mode.py` & `butterfree-1.2.4/butterfree/transform/transformations/user_defined_functions/mode.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/transformations/user_defined_functions/most_frequent_set.py` & `butterfree-1.2.4/butterfree/transform/transformations/user_defined_functions/most_frequent_set.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/utils/date_range.py` & `butterfree-1.2.4/butterfree/transform/utils/date_range.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/utils/function.py` & `butterfree-1.2.4/butterfree/transform/utils/function.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/transform/utils/window_spec.py` & `butterfree-1.2.4/butterfree/transform/utils/window_spec.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/validations/basic_validaton.py` & `butterfree-1.2.4/butterfree/validations/basic_validaton.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree/validations/validation.py` & `butterfree-1.2.4/butterfree/validations/validation.py`

 * *Files identical despite different names*

### Comparing `butterfree-1.2.3.dev0/butterfree.egg-info/PKG-INFO` & `butterfree-1.2.4/butterfree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterfree
-Version: 1.2.3.dev0
+Version: 1.2.4
 Summary: A tool for building feature stores - Transform your raw data into beautiful features.
 Home-page: https://github.com/quintoandar/butterfree
 Author: QuintoAndar
 License: Copyright
 Keywords: feature store sets ETL
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `butterfree-1.2.3.dev0/butterfree.egg-info/SOURCES.txt` & `butterfree-1.2.4/butterfree.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 butterfree.egg-info/dependency_links.txt
 butterfree.egg-info/entry_points.txt
 butterfree.egg-info/requires.txt
 butterfree.egg-info/top_level.txt
 butterfree/_cli/__init__.py
 butterfree/_cli/main.py
 butterfree/_cli/migrate.py
+butterfree/automated/__init__.py
+butterfree/automated/feature_set_creation.py
 butterfree/clients/__init__.py
 butterfree/clients/abstract_client.py
 butterfree/clients/cassandra_client.py
 butterfree/clients/spark_client.py
 butterfree/configs/__init__.py
 butterfree/configs/environment.py
 butterfree/configs/logger.py
```

### Comparing `butterfree-1.2.3.dev0/setup.cfg` & `butterfree-1.2.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [flake8]
 docstring-convention = google
 max-line-length = 88
 max-complexity = 12
-ignore = W503, E203, D203, D401, D107, S101, D105
+ignore = W503, E203, D203, D401, D107, S101, D105, D100, W605, D202, D212, D104, E261
 exclude = dist/*,build/*,.pytest_cache/*,.git/*,pip/*
 per-file-ignores = 
 	tests/*:D,S101
 	setup.py:D,S101
 
 [isort]
 line_length = 88
```

### Comparing `butterfree-1.2.3.dev0/setup.py` & `butterfree-1.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 __package_name__ = "butterfree"
-__version__ = "1.2.3.dev0"
+__version__ = "1.2.4"
 __repository_url__ = "https://github.com/quintoandar/butterfree"
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read()
```

