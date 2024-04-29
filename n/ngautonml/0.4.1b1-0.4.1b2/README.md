# Comparing `tmp/ngautonml-0.4.1b1.tar.gz` & `tmp/ngautonml-0.4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngautonml-0.4.1b1.tar", max compression
+gzip compressed data, was "ngautonml-0.4.1b2.tar", max compression
```

## Comparing `ngautonml-0.4.1b1.tar` & `ngautonml-0.4.1b2.tar`

### file list

```diff
@@ -1,217 +1,283 @@
--rw-r--r--   0        0        0    11338 2024-01-04 16:46:44.089646 ngautonml-0.4.1b1/LICENSE
--rw-r--r--   0        0        0     3653 2024-01-04 16:46:44.089646 ngautonml-0.4.1b1/README.md
--rw-r--r--   0        0        0    12644 2024-01-04 16:46:44.089646 ngautonml-0.4.1b1/classification_example.ipynb
--rw-r--r--   0        0        0    12477 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/forecasting_example.ipynb
--rw-r--r--   0        0        0     5039 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/io_1_save_example.ipynb
--rw-r--r--   0        0        0     6151 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/io_2_load_example.ipynb
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/aggregators/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/aggregators/impl/__init__.py
--rw-r--r--   0        0        0     1398 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregate_ranker.py
--rw-r--r--   0        0        0     3657 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator.py
--rw-r--r--   0        0        0      773 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_auto.py
--rw-r--r--   0        0        0     1465 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_auto_test.py
--rw-r--r--   0        0        0      787 2024-01-04 16:46:44.888658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_catalog.py
--rw-r--r--   0        0        0      863 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_test.py
--rw-r--r--   0        0        0      444 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/test_aggregators.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/distributions/__init__.py
--rw-r--r--   0        0        0    29882 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/distributions/mallows_kendall.py
--rw-r--r--   0        0        0     1718 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/distributions/mallows_model.py
--rw-r--r--   0        0        0    17540 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/rank_aggregation.py
--rw-r--r--   0        0        0     3767 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/test_aggregator_test.py
--rw-r--r--   0        0        0      678 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/test_aggregators.py
--rw-r--r--   0        0        0     3420 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/tsad_aggregator.py
--rw-r--r--   0        0        0     3243 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/tsad_aggregator_test.py
--rw-r--r--   0        0        0     1424 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/aggregators/tsad_aggregators.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/algorithms/__init__.py
--rw-r--r--   0        0        0     2600 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/binarizer.py
--rw-r--r--   0        0        0     1778 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/binarizer_test.py
--rw-r--r--   0        0        0     2231 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/column_parser.py
--rw-r--r--   0        0        0     1409 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/column_parser_test.py
--rw-r--r--   0        0        0     2733 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/connect.py
--rw-r--r--   0        0        0     3394 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/connect_test.py
--rw-r--r--   0        0        0     3089 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/extract_columns_by_role.py
--rw-r--r--   0        0        0     3662 2024-01-04 16:46:44.889658 ngautonml-0.4.1b1/ngautonml/algorithms/extract_columns_by_role_test.py
--rw-r--r--   0        0        0     1125 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/identity.py
--rw-r--r--   0        0        0      496 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/identity_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/algorithms/impl/__init__.py
--rw-r--r--   0        0        0     6412 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm.py
--rw-r--r--   0        0        0     1164 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_auto.py
--rw-r--r--   0        0        0     2141 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_auto_test.py
--rw-r--r--   0        0        0     1387 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_instance.py
--rw-r--r--   0        0        0     4444 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_test.py
--rw-r--r--   0        0        0     6320 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/binder.py
--rw-r--r--   0        0        0     1239 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/fake_algorithm.py
--rw-r--r--   0        0        0     2759 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/fittable_algorithm_instance.py
--rw-r--r--   0        0        0     1774 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/fittable_algorithm_instance_test.py
--rw-r--r--   0        0        0     2085 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/sklearn_like_algorithm_instance.py
--rw-r--r--   0        0        0     2272 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/impl/sklearn_like_algorithm_instance_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/impute/__init__.py
--rw-r--r--   0        0        0     9788 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/impute/simple_imputer.py
--rw-r--r--   0        0        0     1504 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/impute/simple_imputer_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.961659 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/preprocessing/__init__.py
--rw-r--r--   0        0        0     6680 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder.py
--rw-r--r--   0        0        0     2942 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder_test.py
--rw-r--r--   0        0        0     6783 2024-01-04 16:46:44.890658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/sklearn_algorithm.py
--rw-r--r--   0        0        0    10634 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/sklearn_algorithm_test.py
--rw-r--r--   0        0        0    18513 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/sklearn_algorithms.py
--rw-r--r--   0        0        0     3848 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/algorithms/wide_to_long.py
--rw-r--r--   0        0        0     2417 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/algorithms/wide_to_long_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/bugs/__init__.py
--rw-r--r--   0        0        0     1470 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/bugs/bug1.py
--rw-r--r--   0        0        0     1908 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/bugs/bug1_test.py
--rw-r--r--   0        0        0     1087 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/bugs/bug3_test.py
--rw-r--r--   0        0        0     1229 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/bugs/virtual_module.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/catalog/__init__.py
--rw-r--r--   0        0        0     2046 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/catalog.py
--rw-r--r--   0        0        0     1662 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/catalog_element_mixin.py
--rw-r--r--   0        0        0     1467 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/catalog_element_mixin_test.py
--rw-r--r--   0        0        0     2886 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/catalog_shelf.py
--rw-r--r--   0        0        0     5775 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/catalog_shelf_test.py
--rw-r--r--   0        0        0    10395 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/memory_catalog.py
--rw-r--r--   0        0        0     8291 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/memory_catalog_test.py
--rw-r--r--   0        0        0      613 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/pathed_catalog.py
--rw-r--r--   0        0        0     1389 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/pathed_catalog_test.py
--rw-r--r--   0        0        0     1724 2024-01-04 16:46:44.891658 ngautonml-0.4.1b1/ngautonml/catalog/plugin_catalog.py
--rw-r--r--   0        0        0     2656 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/catalog/plugin_catalog_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/catalog/widgets/__init__.py
--rw-r--r--   0        0        0      932 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/catalog/widgets/doodad.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/catalog/widgets/impl/__init__.py
--rw-r--r--   0        0        0      104 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/catalog/widgets/impl/no_register.py
--rw-r--r--   0        0        0      435 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/catalog/widgets/impl/widget_catalog.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/catalog/widgets/some_subfolder/__init__.py
--rw-r--r--   0        0        0      892 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/catalog/widgets/some_subfolder/gizmo.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/cross_validators/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.962659 ngautonml-0.4.1b1/ngautonml/cross_validators/impl/__init__.py
--rw-r--r--   0        0        0     2178 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator.py
--rw-r--r--   0        0        0      763 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator_auto.py
--rw-r--r--   0        0        0      496 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator_auto_test.py
--rw-r--r--   0        0        0      961 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator_test.py
--rw-r--r--   0        0        0     5448 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/k_fold_cross_validator.py
--rw-r--r--   0        0        0     7355 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/k_fold_cross_validator_test.py
--rw-r--r--   0        0        0     2737 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/single_fold_validator.py
--rw-r--r--   0        0        0     2128 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/single_fold_validator_test.py
--rw-r--r--   0        0        0     1790 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/cross_validators/stub_cross_validator.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/dataset_formats/__init__.py
--rw-r--r--   0        0        0     1095 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/dataset_formats/ignore.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/__init__.py
--rw-r--r--   0        0        0     4557 2024-01-04 16:46:44.892658 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataframe_dataset_config.py
--rw-r--r--   0        0        0     2059 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataframe_dataset_config_test.py
--rw-r--r--   0        0        0    12457 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataset_config.py
--rw-r--r--   0        0        0      567 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataset_config_catalog_test.py
--rw-r--r--   0        0        0     4217 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataset_config_test.py
--rw-r--r--   0        0        0     1880 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataset_format_catalog.py
--rw-r--r--   0        0        0     7971 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/local.py
--rw-r--r--   0        0        0     9154 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/local_test.py
--rw-r--r--   0        0        0     2029 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/memory.py
--rw-r--r--   0        0        0     4579 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/dataset_formats/memory_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/executor/__init__.py
--rw-r--r--   0        0        0     4271 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/cucumber.py
--rw-r--r--   0        0        0     2009 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/cucumber_test.py
--rw-r--r--   0        0        0     2470 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/executor.py
--rw-r--r--   0        0        0     1302 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/executor_kind.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/executor/simple/__init__.py
--rw-r--r--   0        0        0     4240 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_pipeline.py
--rw-r--r--   0        0        0     6810 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_pipeline_test.py
--rw-r--r--   0        0        0     4005 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_step.py
--rw-r--r--   0        0        0     3094 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_step_test.py
--rw-r--r--   0        0        0     2601 2024-01-04 16:46:44.893658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executor.py
--rw-r--r--   0        0        0    10687 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executor_test.py
--rw-r--r--   0        0        0      927 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_instantiator.py
--rw-r--r--   0        0        0     1249 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_instantiator_test.py
--rw-r--r--   0        0        0     4001 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_parallel_executable_step.py
--rw-r--r--   0        0        0     1169 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/executor/simple/simple_parallel_executable_step_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/generator/__init__.py
--rw-r--r--   0        0        0     4214 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/generator/bound_pipeline.py
--rw-r--r--   0        0        0     2674 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/generator/bound_pipeline_test.py
--rw-r--r--   0        0        0      657 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/generator/designator.py
--rw-r--r--   0        0        0     2677 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/generator/generator.py
--rw-r--r--   0        0        0     5035 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/generator/generator_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/instantiator/__init__.py
--rw-r--r--   0        0        0     9784 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/executable_pipeline.py
--rw-r--r--   0        0        0     3030 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/executable_pipeline_test.py
--rw-r--r--   0        0        0     2915 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/instantiator.py
--rw-r--r--   0        0        0     1991 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/instantiator_factory.py
--rw-r--r--   0        0        0     1142 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/instantiator_test.py
--rw-r--r--   0        0        0     5386 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/json_instantiator.py
--rw-r--r--   0        0        0     5381 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/json_instantiator_test.py
--rw-r--r--   0        0        0     3657 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/json_loader.py
--rw-r--r--   0        0        0     4876 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/json_loader_test.py
--rw-r--r--   0        0        0       99 2024-01-04 16:46:44.894658 ngautonml-0.4.1b1/ngautonml/instantiator/loader.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/metrics/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/metrics/impl/__init__.py
--rw-r--r--   0        0        0     3178 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/impl/metric.py
--rw-r--r--   0        0        0      733 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_auto.py
--rw-r--r--   0        0        0     1753 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_auto_test.py
--rw-r--r--   0        0        0     1466 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_catalog.py
--rw-r--r--   0        0        0     1766 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_catalog_test.py
--rw-r--r--   0        0        0      997 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_test.py
--rw-r--r--   0        0        0     4557 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/sklearn_metrics.py
--rw-r--r--   0        0        0     3871 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/metrics/sklearn_metrics_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/problem_def/__init__.py
--rw-r--r--   0        0        0     1356 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/aggregation_config.py
--rw-r--r--   0        0        0     5120 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/config_component.py
--rw-r--r--   0        0        0     2083 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/cross_validation_config.py
--rw-r--r--   0        0        0     4782 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/hyperparam_config.py
--rw-r--r--   0        0        0     4980 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/hyperparam_config_test.py
--rw-r--r--   0        0        0     2392 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/metric_config.py
--rw-r--r--   0        0        0      500 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/metric_config_test.py
--rw-r--r--   0        0        0     2677 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/output_config.py
--rw-r--r--   0        0        0     1743 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/output_config_test.py
--rw-r--r--   0        0        0    13012 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/problem_def.py
--rw-r--r--   0        0        0    16304 2024-01-04 16:46:44.895658 ngautonml-0.4.1b1/ngautonml/problem_def/problem_def_test.py
--rw-r--r--   0        0        0     4698 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/problem_def/task.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/ranker/__init__.py
--rw-r--r--   0        0        0     9911 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/ranker/ranker.py
--rw-r--r--   0        0        0      255 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/ranker/ranker_impl.py
--rw-r--r--   0        0        0     6790 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/ranker/ranker_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/searcher/__init__.py
--rw-r--r--   0        0        0     1601 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/frozen_overrides.py
--rw-r--r--   0        0        0     2997 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/matchers.py
--rw-r--r--   0        0        0     5135 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/matchers_test.py
--rw-r--r--   0        0        0     2261 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/param_range.py
--rw-r--r--   0        0        0     2753 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/params.py
--rw-r--r--   0        0        0     1241 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/params_test.py
--rw-r--r--   0        0        0     8613 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/searcher.py
--rw-r--r--   0        0        0    12133 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/searcher/searcher_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/splitters/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/splitters/impl/__init__.py
--rw-r--r--   0        0        0     3371 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter.py
--rw-r--r--   0        0        0      632 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter_auto.py
--rw-r--r--   0        0        0      849 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter_auto_test.py
--rw-r--r--   0        0        0      991 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter_test.py
--rw-r--r--   0        0        0     2649 2024-01-04 16:46:44.896658 ngautonml-0.4.1b1/ngautonml/splitters/k_fold_splitter.py
--rw-r--r--   0        0        0     3962 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/splitters/k_fold_splitter_test.py
--rw-r--r--   0        0        0     2345 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/splitters/single_fold_splitter.py
--rw-r--r--   0        0        0     1859 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/splitters/single_fold_splitter_test.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/templates/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.963659 ngautonml-0.4.1b1/ngautonml/templates/impl/__init__.py
--rw-r--r--   0        0        0     4510 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/parallel_step.py
--rw-r--r--   0        0        0     1181 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/parallel_step_test.py
--rw-r--r--   0        0        0     8915 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_step.py
--rw-r--r--   0        0        0     2788 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_step_test.py
--rw-r--r--   0        0        0     4027 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_template.py
--rw-r--r--   0        0        0      803 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_template_test.py
--rw-r--r--   0        0        0     2267 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/query_step.py
--rw-r--r--   0        0        0      942 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/query_step_test.py
--rw-r--r--   0        0        0     3191 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/template.py
--rw-r--r--   0        0        0      659 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/template_auto.py
--rw-r--r--   0        0        0     1294 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/template_auto_test.py
--rw-r--r--   0        0        0     6624 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/impl/template_test.py
--rw-r--r--   0        0        0     3226 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/tabular_classification.py
--rw-r--r--   0        0        0     2936 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/templates/tabular_regression.py
--rw-r--r--   0        0        0        0 2024-01-04 16:46:44.964659 ngautonml-0.4.1b1/ngautonml/wrangler/__init__.py
--rw-r--r--   0        0        0     8293 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/wrangler/constants.py
--rw-r--r--   0        0        0    10440 2024-01-04 16:46:44.897658 ngautonml-0.4.1b1/ngautonml/wrangler/dataset.py
--rw-r--r--   0        0        0     2610 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/dataset_test.py
--rw-r--r--   0        0        0     3671 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/examples_problem_def_test.py
--rw-r--r--   0        0        0     5886 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/examples_test.py
--rw-r--r--   0        0        0     4579 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/saver.py
--rw-r--r--   0        0        0     4803 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/saver_test.py
--rw-r--r--   0        0        0    18019 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/wrangler.py
--rw-r--r--   0        0        0    26096 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/ngautonml/wrangler/wrangler_test.py
--rwxr-xr-x   0        0        0     4045 2024-01-04 16:46:44.898658 ngautonml-0.4.1b1/picard.py
--rw-r--r--   0        0        0     1462 2024-01-04 16:46:44.901658 ngautonml-0.4.1b1/pyproject.toml
--rw-r--r--   0        0        0    11525 2024-01-04 16:46:44.901658 ngautonml-0.4.1b1/regression_example.ipynb
--rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 ngautonml-0.4.1b1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-04-29 18:54:57.336347 ngautonml-0.4.1b2/LICENSE
+-rw-r--r--   0        0        0     3653 2024-04-29 18:54:57.336347 ngautonml-0.4.1b2/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.210353 ngautonml-0.4.1b2/ngautonml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.210353 ngautonml-0.4.1b2/ngautonml/aggregators/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.210353 ngautonml-0.4.1b2/ngautonml/aggregators/impl/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregate_ranker.py
+-rw-r--r--   0        0        0     3709 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator.py
+-rw-r--r--   0        0        0      773 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_auto.py
+-rw-r--r--   0        0        0     1465 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_auto_test.py
+-rw-r--r--   0        0        0      787 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_catalog.py
+-rw-r--r--   0        0        0      889 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_test.py
+-rw-r--r--   0        0        0      444 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/test_aggregators.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/distributions/__init__.py
+-rw-r--r--   0        0        0    29882 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/distributions/mallows_kendall.py
+-rw-r--r--   0        0        0     1718 2024-04-29 18:54:58.133352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/distributions/mallows_model.py
+-rw-r--r--   0        0        0    17540 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/rank_aggregation.py
+-rw-r--r--   0        0        0     3818 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/aggregators/test_aggregator_test.py
+-rw-r--r--   0        0        0      678 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/aggregators/test_aggregators.py
+-rw-r--r--   0        0        0     3556 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/aggregators/tsad_aggregator.py
+-rw-r--r--   0        0        0     3294 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/aggregators/tsad_aggregator_test.py
+-rw-r--r--   0        0        0     1424 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/aggregators/tsad_aggregators.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/algorithms/__init__.py
+-rw-r--r--   0        0        0     2893 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/binarizer.py
+-rw-r--r--   0        0        0     1778 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/binarizer_test.py
+-rw-r--r--   0        0        0     2419 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/column_parser.py
+-rw-r--r--   0        0        0     1409 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/column_parser_test.py
+-rw-r--r--   0        0        0     2901 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/connect.py
+-rw-r--r--   0        0        0     3394 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/connect_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/algorithms/distributed/__init__.py
+-rw-r--r--   0        0        0     8326 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/distributed/auton_linear_regression.py
+-rw-r--r--   0        0        0    18158 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/distributed/auton_linear_regression_test.py
+-rw-r--r--   0        0        0    13843 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/distributed/auton_logistic_regression.py
+-rw-r--r--   0        0        0    24535 2024-04-29 18:54:58.134352 ngautonml-0.4.1b2/ngautonml/algorithms/distributed/auton_logistic_regression_test.py
+-rw-r--r--   0        0        0     3249 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/extract_columns_by_role.py
+-rw-r--r--   0        0        0     3809 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/extract_columns_by_role_test.py
+-rw-r--r--   0        0        0     1312 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/identity.py
+-rw-r--r--   0        0        0      496 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/identity_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/algorithms/impl/__init__.py
+-rw-r--r--   0        0        0     8468 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm.py
+-rw-r--r--   0        0        0     1164 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_auto.py
+-rw-r--r--   0        0        0     2141 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_auto_test.py
+-rw-r--r--   0        0        0     2054 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_instance.py
+-rw-r--r--   0        0        0     4559 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_test.py
+-rw-r--r--   0        0        0     6320 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/binder.py
+-rw-r--r--   0        0        0    11128 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/distributed_algorithm_instance.py
+-rw-r--r--   0        0        0     1279 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/fake_algorithm.py
+-rw-r--r--   0        0        0     3150 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/fittable_algorithm_instance.py
+-rw-r--r--   0        0        0     1884 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/fittable_algorithm_instance_test.py
+-rw-r--r--   0        0        0     9271 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/linear_distributed_algorithm_instance.py
+-rw-r--r--   0        0        0     3853 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/linear_distributed_algorithm_instance_test.py
+-rw-r--r--   0        0        0     2291 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/sklearn_like_algorithm_instance.py
+-rw-r--r--   0        0        0     2312 2024-04-29 18:54:58.135352 ngautonml-0.4.1b2/ngautonml/algorithms/impl/sklearn_like_algorithm_instance_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/impute/__init__.py
+-rw-r--r--   0        0        0     9994 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/impute/simple_imputer.py
+-rw-r--r--   0        0        0     1572 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/impute/simple_imputer_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/preprocessing/__init__.py
+-rw-r--r--   0        0        0     7020 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder.py
+-rw-r--r--   0        0        0     3040 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder_test.py
+-rw-r--r--   0        0        0     7244 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/sklearn_algorithm.py
+-rw-r--r--   0        0        0    10634 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/sklearn_algorithm_test.py
+-rw-r--r--   0        0        0    18590 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/sklearn_algorithms.py
+-rw-r--r--   0        0        0     4033 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/wide_to_long.py
+-rw-r--r--   0        0        0     2423 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/algorithms/wide_to_long_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/bugs/__init__.py
+-rw-r--r--   0        0        0     1470 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/bugs/bug1.py
+-rw-r--r--   0        0        0     2295 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/bugs/bug1_test.py
+-rw-r--r--   0        0        0     1339 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/bugs/bug3_test.py
+-rw-r--r--   0        0        0     1000 2024-04-29 18:54:58.136352 ngautonml-0.4.1b2/ngautonml/bugs/virtual_module.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/catalog/__init__.py
+-rw-r--r--   0        0        0     2175 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/catalog.py
+-rw-r--r--   0        0        0     2126 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/catalog_element_mixin.py
+-rw-r--r--   0        0        0     1467 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/catalog_element_mixin_test.py
+-rw-r--r--   0        0        0     3032 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/catalog_shelf.py
+-rw-r--r--   0        0        0     6293 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/catalog_shelf_test.py
+-rw-r--r--   0        0        0    10722 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/memory_catalog.py
+-rw-r--r--   0        0        0     8745 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/memory_catalog_test.py
+-rw-r--r--   0        0        0      613 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/pathed_catalog.py
+-rw-r--r--   0        0        0     1389 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/pathed_catalog_test.py
+-rw-r--r--   0        0        0     1724 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/plugin_catalog.py
+-rw-r--r--   0        0        0     2985 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/plugin_catalog_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/catalog/widgets/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/widgets/doodad.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/catalog/widgets/impl/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/widgets/impl/no_register.py
+-rw-r--r--   0        0        0      435 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/widgets/impl/widget_catalog.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/catalog/widgets/some_subfolder/__init__.py
+-rw-r--r--   0        0        0      892 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/catalog/widgets/some_subfolder/gizmo.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/communicators/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/communicators/impl/__init__.py
+-rw-r--r--   0        0        0     2158 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/communicators/impl/communicator.py
+-rw-r--r--   0        0        0      805 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/communicators/impl/communicator_auto.py
+-rw-r--r--   0        0        0     2564 2024-04-29 18:54:58.137352 ngautonml-0.4.1b2/ngautonml/communicators/impl/communicator_auto_test.py
+-rw-r--r--   0        0        0      773 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/impl/communicator_catalog.py
+-rw-r--r--   0        0        0     1880 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/impl/communicator_catalog_test.py
+-rw-r--r--   0        0        0      221 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/impl/endpoint.py
+-rw-r--r--   0        0        0     1272 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/impl/ip_endpoint.py
+-rw-r--r--   0        0        0     5376 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/sockets_communicator.py
+-rw-r--r--   0        0        0    11384 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/sockets_communicator_test.py
+-rw-r--r--   0        0        0     1374 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/communicators/stub_communicator.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/config_components/__init__.py
+-rw-r--r--   0        0        0     8730 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/dataset_config.py
+-rw-r--r--   0        0        0     2262 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/dataset_config_test.py
+-rw-r--r--   0        0        0     7659 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/distributed_config.py
+-rw-r--r--   0        0        0     1962 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/distributed_config_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/config_components/impl/__init__.py
+-rw-r--r--   0        0        0     6854 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/impl/config_component.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/impl/config_component_auto.py
+-rw-r--r--   0        0        0      784 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/impl/config_component_catalog.py
+-rw-r--r--   0        0        0      995 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/config_components/impl/config_component_catalog_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/cross_validators/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/cross_validators/impl/__init__.py
+-rw-r--r--   0        0        0     2178 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator.py
+-rw-r--r--   0        0        0      763 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator_auto.py
+-rw-r--r--   0        0        0      496 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator_auto_test.py
+-rw-r--r--   0        0        0      961 2024-04-29 18:54:58.138352 ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator_test.py
+-rw-r--r--   0        0        0     5775 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/cross_validators/k_fold_cross_validator.py
+-rw-r--r--   0        0        0     7800 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/cross_validators/k_fold_cross_validator_test.py
+-rw-r--r--   0        0        0     2737 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/cross_validators/single_fold_validator.py
+-rw-r--r--   0        0        0     2128 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/cross_validators/single_fold_validator_test.py
+-rw-r--r--   0        0        0     1790 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/cross_validators/stub_cross_validator.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.211353 ngautonml-0.4.1b2/ngautonml/data_loaders/__init__.py
+-rw-r--r--   0        0        0      979 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/ignore_data_loader.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.212353 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/__init__.py
+-rw-r--r--   0        0        0     2728 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/data_loader.py
+-rw-r--r--   0        0        0      789 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/data_loader_auto.py
+-rw-r--r--   0        0        0     3798 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/data_loader_auto_test.py
+-rw-r--r--   0        0        0     2005 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/data_loader_catalog.py
+-rw-r--r--   0        0        0     1905 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/data_loader_catalog_test.py
+-rw-r--r--   0        0        0     2995 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/data_loader_test.py
+-rw-r--r--   0        0        0     9485 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/dataframe_loader.py
+-rw-r--r--   0        0        0     8708 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/impl/dataframe_loader_test.py
+-rw-r--r--   0        0        0     6545 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/local_data_loader.py
+-rw-r--r--   0        0        0     5278 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/local_data_loader_test.py
+-rw-r--r--   0        0        0     3182 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/memory_data_loader.py
+-rw-r--r--   0        0        0     3127 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/memory_data_loader_test.py
+-rw-r--r--   0        0        0     2331 2024-04-29 18:54:58.139352 ngautonml-0.4.1b2/ngautonml/data_loaders/queue_loader.py
+-rw-r--r--   0        0        0     4264 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/data_loaders/queue_loader_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.212353 ngautonml-0.4.1b2/ngautonml/data_loaders/sklearn/__init__.py
+-rw-r--r--   0        0        0     3693 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/data_loaders/sklearn/sklearn_loader_generator.py
+-rw-r--r--   0        0        0     3531 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/data_loaders/sklearn/sklearn_loader_generator_test.py
+-rw-r--r--   0        0        0      702 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/data_loaders/sklearn/sklearn_loader_interface.py
+-rw-r--r--   0        0        0     1240 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/data_loaders/sklearn/sklearn_loaders.py
+-rw-r--r--   0        0        0     1157 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/data_loaders/stub_data_loader.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.212353 ngautonml-0.4.1b2/ngautonml/discoverers/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/dynamic_discoverer.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.212353 ngautonml-0.4.1b2/ngautonml/discoverers/impl/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/impl/discoverer.py
+-rw-r--r--   0        0        0      785 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/impl/discoverer_auto.py
+-rw-r--r--   0        0        0     2491 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/impl/discoverer_auto_test.py
+-rw-r--r--   0        0        0      762 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/impl/discoverer_catalog.py
+-rw-r--r--   0        0        0     1800 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/impl/discoverer_catalog_test.py
+-rw-r--r--   0        0        0     1510 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/discoverers/static_discoverer.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.213353 ngautonml-0.4.1b2/ngautonml/executor/__init__.py
+-rw-r--r--   0        0        0     4271 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/executor/cucumber.py
+-rw-r--r--   0        0        0     2009 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/executor/cucumber_test.py
+-rw-r--r--   0        0        0     2500 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/executor/executor.py
+-rw-r--r--   0        0        0     1302 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/executor/executor_kind.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.213353 ngautonml-0.4.1b2/ngautonml/executor/simple/__init__.py
+-rw-r--r--   0        0        0     5100 2024-04-29 18:54:58.140352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_pipeline.py
+-rw-r--r--   0        0        0     7084 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_pipeline_test.py
+-rw-r--r--   0        0        0     4328 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_step.py
+-rw-r--r--   0        0        0     3094 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_step_test.py
+-rw-r--r--   0        0        0     2621 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executor.py
+-rw-r--r--   0        0        0    10883 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executor_test.py
+-rw-r--r--   0        0        0      927 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_instantiator.py
+-rw-r--r--   0        0        0     1295 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_instantiator_test.py
+-rw-r--r--   0        0        0     4001 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_parallel_executable_step.py
+-rw-r--r--   0        0        0     1161 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/executor/simple/simple_parallel_executable_step_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.214353 ngautonml-0.4.1b2/ngautonml/generator/__init__.py
+-rw-r--r--   0        0        0     4781 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/generator/bound_pipeline.py
+-rw-r--r--   0        0        0     2780 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/generator/bound_pipeline_test.py
+-rw-r--r--   0        0        0      657 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/generator/designator.py
+-rw-r--r--   0        0        0     2677 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/generator/generator.py
+-rw-r--r--   0        0        0     5035 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/generator/generator_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.215353 ngautonml-0.4.1b2/ngautonml/instantiator/__init__.py
+-rw-r--r--   0        0        0    10684 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/instantiator/executable_pipeline.py
+-rw-r--r--   0        0        0     3068 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/instantiator/executable_pipeline_test.py
+-rw-r--r--   0        0        0     2915 2024-04-29 18:54:58.141352 ngautonml-0.4.1b2/ngautonml/instantiator/instantiator.py
+-rw-r--r--   0        0        0     1991 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/instantiator_factory.py
+-rw-r--r--   0        0        0     1142 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/instantiator_test.py
+-rw-r--r--   0        0        0     5386 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/json_instantiator.py
+-rw-r--r--   0        0        0     5381 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/json_instantiator_test.py
+-rw-r--r--   0        0        0     3657 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/json_loader.py
+-rw-r--r--   0        0        0     4876 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/json_loader_test.py
+-rw-r--r--   0        0        0       99 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/instantiator/loader.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.215353 ngautonml-0.4.1b2/ngautonml/metrics/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.215353 ngautonml-0.4.1b2/ngautonml/metrics/impl/__init__.py
+-rw-r--r--   0        0        0     4435 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/impl/metric.py
+-rw-r--r--   0        0        0      733 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_auto.py
+-rw-r--r--   0        0        0     1753 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_auto_test.py
+-rw-r--r--   0        0        0     1466 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_catalog.py
+-rw-r--r--   0        0        0     1766 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_catalog_test.py
+-rw-r--r--   0        0        0      997 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_test.py
+-rw-r--r--   0        0        0     4502 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/sklearn_metrics.py
+-rw-r--r--   0        0        0     3871 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/metrics/sklearn_metrics_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.216353 ngautonml-0.4.1b2/ngautonml/neighbor_manager/__init__.py
+-rw-r--r--   0        0        0     1380 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/neighbor_manager/event.py
+-rw-r--r--   0        0        0     4191 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/neighbor_manager/neighbor_manager.py
+-rw-r--r--   0        0        0     2040 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/neighbor_manager/neighbor_manager_impl.py
+-rw-r--r--   0        0        0     1533 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/neighbor_manager/neighbor_manager_impl_test.py
+-rw-r--r--   0        0        0     1894 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/neighbor_manager/neighbor_manager_test.py
+-rw-r--r--   0        0        0      258 2024-04-29 18:54:58.142352 ngautonml-0.4.1b2/ngautonml/neighbor_manager/node_id.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.216353 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.216353 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/__init__.py
+-rw-r--r--   0        0        0     1845 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/pipeline_loader.py
+-rw-r--r--   0        0        0      816 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/pipeline_loader_auto.py
+-rw-r--r--   0        0        0     2232 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/pipeline_loader_auto_test.py
+-rw-r--r--   0        0        0     1313 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/pipeline_loader_catalog.py
+-rw-r--r--   0        0        0     1978 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/pipeline_loader_catalog_test.py
+-rw-r--r--   0        0        0      525 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/impl/pipeline_loader_test.py
+-rw-r--r--   0        0        0     1465 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/pipeline_loaders/just.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.217353 ngautonml-0.4.1b2/ngautonml/problem_def/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/aggregation_config.py
+-rw-r--r--   0        0        0     2336 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/cross_validation_config.py
+-rw-r--r--   0        0        0     5008 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/hyperparam_config.py
+-rw-r--r--   0        0        0     4980 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/hyperparam_config_test.py
+-rw-r--r--   0        0        0     2956 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/metric_config.py
+-rw-r--r--   0        0        0      500 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/metric_config_test.py
+-rw-r--r--   0        0        0     2887 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/output_config.py
+-rw-r--r--   0        0        0     1743 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/output_config_test.py
+-rw-r--r--   0        0        0     9880 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/problem_def.py
+-rw-r--r--   0        0        0     1345 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/problem_def_interface.py
+-rw-r--r--   0        0        0    11452 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/problem_def_test.py
+-rw-r--r--   0        0        0     4286 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/problem_def/task.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.217353 ngautonml-0.4.1b2/ngautonml/ranker/__init__.py
+-rw-r--r--   0        0        0    11407 2024-04-29 18:54:58.143352 ngautonml-0.4.1b2/ngautonml/ranker/ranker.py
+-rw-r--r--   0        0        0      255 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/ranker/ranker_impl.py
+-rw-r--r--   0        0        0     8636 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/ranker/ranker_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.217353 ngautonml-0.4.1b2/ngautonml/searcher/__init__.py
+-rw-r--r--   0        0        0     1601 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/frozen_overrides.py
+-rw-r--r--   0        0        0     2997 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/matchers.py
+-rw-r--r--   0        0        0     5251 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/matchers_test.py
+-rw-r--r--   0        0        0     2261 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/param_range.py
+-rw-r--r--   0        0        0     3074 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/params.py
+-rw-r--r--   0        0        0     1241 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/params_test.py
+-rw-r--r--   0        0        0     9474 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/searcher.py
+-rw-r--r--   0        0        0    12535 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/searcher/searcher_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.217353 ngautonml-0.4.1b2/ngautonml/splitters/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.217353 ngautonml-0.4.1b2/ngautonml/splitters/impl/__init__.py
+-rw-r--r--   0        0        0     3371 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter.py
+-rw-r--r--   0        0        0      632 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter_auto.py
+-rw-r--r--   0        0        0      808 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter_auto_test.py
+-rw-r--r--   0        0        0      991 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter_test.py
+-rw-r--r--   0        0        0     2649 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/splitters/k_fold_splitter.py
+-rw-r--r--   0        0        0     3962 2024-04-29 18:54:58.144352 ngautonml-0.4.1b2/ngautonml/splitters/k_fold_splitter_test.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.219353 ngautonml-0.4.1b2/ngautonml/templates/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.219353 ngautonml-0.4.1b2/ngautonml/templates/impl/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/parallel_step.py
+-rw-r--r--   0        0        0     1181 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/parallel_step_test.py
+-rw-r--r--   0        0        0     8898 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_step.py
+-rw-r--r--   0        0        0     2788 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_step_test.py
+-rw-r--r--   0        0        0     5276 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_template.py
+-rw-r--r--   0        0        0      803 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_template_test.py
+-rw-r--r--   0        0        0     2267 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/query_step.py
+-rw-r--r--   0        0        0      942 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/query_step_test.py
+-rw-r--r--   0        0        0     3159 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/template.py
+-rw-r--r--   0        0        0      659 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/template_auto.py
+-rw-r--r--   0        0        0     1294 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/template_auto_test.py
+-rw-r--r--   0        0        0     6624 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/impl/template_test.py
+-rw-r--r--   0        0        0     3226 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/tabular_classification.py
+-rw-r--r--   0        0        0     2936 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/templates/tabular_regression.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:54:58.220353 ngautonml-0.4.1b2/ngautonml/wrangler/__init__.py
+-rw-r--r--   0        0        0      375 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/wrangler/base_port.py
+-rw-r--r--   0        0        0     6892 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/wrangler/constants.py
+-rw-r--r--   0        0        0    11310 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/wrangler/dataset.py
+-rw-r--r--   0        0        0     2543 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/wrangler/dataset_test.py
+-rw-r--r--   0        0        0     8643 2024-04-29 18:54:58.145352 ngautonml-0.4.1b2/ngautonml/wrangler/distributed_wrangler.py
+-rw-r--r--   0        0        0    13068 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/distributed_wrangler_test.py
+-rw-r--r--   0        0        0     2796 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/examples_problem_def_test.py
+-rw-r--r--   0        0        0     6152 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/examples_test.py
+-rw-r--r--   0        0        0      563 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/exception_thread.py
+-rw-r--r--   0        0        0      737 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/exception_thread_test.py
+-rw-r--r--   0        0        0     2521 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/logger.py
+-rw-r--r--   0        0        0     4698 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/saver.py
+-rw-r--r--   0        0        0     4861 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/saver_test.py
+-rw-r--r--   0        0        0     6054 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/wrangler.py
+-rw-r--r--   0        0        0    15178 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/wrangler_base.py
+-rw-r--r--   0        0        0     2440 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/wrangler_result.py
+-rw-r--r--   0        0        0    28190 2024-04-29 18:54:58.146352 ngautonml-0.4.1b2/ngautonml/wrangler/wrangler_test.py
+-rwxr-xr-x   0        0        0     5472 2024-04-29 18:54:58.147352 ngautonml-0.4.1b2/picard.py
+-rw-r--r--   0        0        0     1499 2024-04-29 18:54:58.150352 ngautonml-0.4.1b2/pyproject.toml
+-rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 ngautonml-0.4.1b2/PKG-INFO
```

### Comparing `ngautonml-0.4.1b1/LICENSE` & `ngautonml-0.4.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/README.md` & `ngautonml-0.4.1b2/README.md`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregate_ranker.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregate_ranker.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         params.update(overrides)
         self._hyperparams = params
 
     def __str__(self):
         return self.name
 
     @abc.abstractmethod
-    def aggregate(self, rankings: Rankings) -> Ranking:
+    def aggregate(self, rankings: Rankings, all_scores: bool = False) -> Ranking:
         '''Calculates the Aggregator results.'''
 
     def calculate(self, pred: Dataset, ground_truth: Optional[Dataset] = None) -> float:
         '''Calculates the metric results.'''
         raise AggregatorError('calculate is not implemented for Aggregators')
 
     def hyperparams(self, **overrides) -> Dict[str, Any]:
@@ -73,15 +73,15 @@
 
 
 class AggregatorStub(Aggregator):
     '''This is a stub'''
     _name = 'stub_aggregator'
     _high = True
 
-    def aggregate(self, rankings: Rankings) -> Ranking:
+    def aggregate(self, rankings: Rankings, all_scores: bool = False) -> Ranking:
         return RankingStub(metric=MetricStub(self._name), results=PipelineResults())
 
 
 class AggregatorRanking(Ranking):
     '''This is the Aggregator version of a Ranking.
 
     We pass the scores in at init time.
```

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_auto.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_auto.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_auto_test.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_auto_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_catalog.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_catalog.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/aggregator_test.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/aggregator_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # pylint: disable=missing-class-docstring
 # pylint: disable=too-few-public-methods
 
 
 class ExampleAggregator(Aggregator):
     _name = 'TestAggregator'
 
-    def aggregate(self, rankings: Rankings) -> Ranking:
+    def aggregate(self, rankings: Rankings, all_scores: bool = False) -> Ranking:
         return RankingStub(MetricStub(), PipelineResults())
 
 
 def test_name():
     dut = ExampleAggregator()
     assert dut.name == 'testaggregator'
     got = dut.aggregate({})
```

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/distributions/mallows_kendall.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/distributions/mallows_kendall.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/distributions/mallows_model.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/distributions/mallows_model.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/impl/tsad/rank_aggregation.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/impl/tsad/rank_aggregation.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/test_aggregator_test.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/test_aggregator_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     })
 
     rankings = Rankings({'MinRanking': Ranking(metric=MetricMinVal(), results=pipeline_results)})
 
     identity_ranking = aggregator.aggregate(rankings=rankings)
     reverse_ranking = aggregator.aggregate(rankings=rankings, reverse=True)
 
-    assert [s.pipeline_des for s in identity_ranking.scores] \
+    assert [s.pipeline_des for s in identity_ranking.scores(all_scores=True)] \
         == ['pipeline_1', 'pipeline_2', 'pipeline_3']
-    assert [s.pipeline_des for s in reverse_ranking.scores] \
+    assert [s.pipeline_des for s in reverse_ranking.scores(all_scores=True)] \
         == ['pipeline_3', 'pipeline_2', 'pipeline_1']
 
 
 def test_fail_aggregator():
     '''Tests aggregators which raise exceptions.'''
     catalog = AggregatorCatalogAuto()
     catalog.register(TSADAggregator(
@@ -89,12 +89,12 @@
 
     rankings = Rankings({'MinRanking': Ranking(metric=MetricMinVal(), results=pipeline_results)})
 
     new_rankings = AggregateRanker(methods=[aggregator],
                                    rankings=rankings,
                                    results=pipeline_results,
                                    )()
-    new_scores = new_rankings['test_aggregators.identity'].scores
+    new_scores = new_rankings['test_aggregators.identity'].scores(all_scores=True)
 
     assert new_scores[0].score == 'intentional failure'
     assert new_scores[1].score == 'intentional failure'
     assert new_scores[2].score == 'intentional failure'
```

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/test_aggregators.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/tsad_aggregator.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/tsad_aggregator.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,21 @@
         # and constructor part (e.g. LinearRegression)
         parts = name.split('.')
         constructor_part = parts[-1]
         module = importlib.import_module('.'.join(parts[:-1]), package='ngautonml.aggregators.impl')
         # Load the constructor.
         return getattr(module, constructor_part)
 
-    def aggregate(self, rankings: Rankings, **overrides) -> AggregatorRanking:
+    def aggregate(self,
+                  rankings: Rankings,
+                  all_scores: bool = False, **overrides) -> AggregatorRanking:
         rankings_list = list(rankings.values())
         first_ranking = rankings_list[0]
-        num_of_pipelines = len(first_ranking.scores)
+        first_scores = first_ranking.scores(all_scores=all_scores)
+        num_of_pipelines = len(first_scores)
         num_of_metrics = len(rankings_list)
 
         assert self._tags is not None, (
             'BUG: self._tags should have been initialized in TSADGenerator.__init__().'
         )
         if 'required_number_of_pipelines' in self._tags:
             num_of_pipelines_required = int(self._tags['required_number_of_pipelines'][0])
@@ -55,24 +58,24 @@
                     f'Given {num_of_pipelines} pipelines but '
                     f'require {num_of_pipelines_required} pipelines'
                 )
 
         pipeline_to_index = {}
         index_to_pipeline = {}
         pipeline_results = PipelineResults()
-        for i, scored_result in enumerate(first_ranking.scores):
+        for i, scored_result in enumerate(first_scores):
             pipeline_des = scored_result.pipeline_des
             pipeline_to_index[pipeline_des] = i
             index_to_pipeline[i] = pipeline_des
             pipeline_results[pipeline_des] = scored_result.result
 
         # ranks[i, j] = the rank of the jth pipeline under the ith metric
         ranks = np.zeros((num_of_metrics, num_of_pipelines))
         for m, ranking in enumerate(rankings_list):
-            for rank, scored_result in enumerate(ranking.scores):
+            for rank, scored_result in enumerate(ranking.scores(all_scores=all_scores)):
                 pipeline_des = scored_result.pipeline_des
                 n = pipeline_to_index[pipeline_des]
                 ranks[m, n] = rank
 
         _, aggregate_rank = self._aggregator(ranks, **self.hyperparams(**overrides))
 
         scores = {}
```

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/tsad_aggregator_test.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/tsad_aggregator_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,11 +81,11 @@
 
     rank_1 = Ranking(metric=MetricSumPred(), results=pipeline_results)
     rank_2 = Ranking(metric=MetricStub(), results=pipeline_results)
     rank_3 = Ranking(metric=MetricMinVal(), results=pipeline_results)
 
     rankings = Rankings({'rank_1': rank_1, 'rank_2': rank_2, 'rank_3': rank_3})
 
-    aggregate_ranking = aggregator.aggregate(rankings=rankings)
+    aggregate_ranking = aggregator.aggregate(rankings=rankings, all_scores=True)
 
-    assert [s.score for s in aggregate_ranking.scores] == [2, 1, 0]
-    assert [s.pipeline_des for s in aggregate_ranking.scores] == final_ranking
+    assert [s.score for s in aggregate_ranking.scores(all_scores=True)] == [2, 1, 0]
+    assert [s.pipeline_des for s in aggregate_ranking.scores(all_scores=True)] == final_ranking
```

### Comparing `ngautonml-0.4.1b1/ngautonml/aggregators/tsad_aggregators.py` & `ngautonml-0.4.1b2/ngautonml/aggregators/tsad_aggregators.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/binarizer.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/binarizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 '''Convert two-valued fields into binary fields.'''
 import logging
-from typing import Any, Dict
+from typing import Any, Dict, Optional
+
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from ..algorithms.impl.algorithm import Algorithm, MemoryAlgorithmCatalog
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
 from ..catalog.catalog import upcast
 from ..wrangler.dataset import Dataset, RoleName
+from ..wrangler.logger import Logger
+
+logger = Logger(__file__, level=logging.INFO, to_file=False, to_stdout=False).logger()
 
 
 class BinarizerModelInstance(AlgorithmInstance):
     '''Connect one model to another by transforming names.'''
     _pos_labels: Dict[RoleName, Any]
 
     def __init__(self, parent, **hyperparams: Any):
         super().__init__(parent=parent)
 
         self._pos_labels = {
             RoleName[n.upper()]: v
-            for n, v in self._algorithm.hyperparams(**hyperparams).items()
+            for n, v in self.algorithm.hyperparams(**hyperparams).items()
         }
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         retval = dataset.output()
 
         pos_labels = self._pos_labels.copy()  # take care not to update the base values.
         pos_labels.update(dataset.metadata.pos_labels)
 
         retval_data = dataset.get_dataframe()
         for role in pos_labels:
@@ -38,15 +44,15 @@
 
             positive = pos_labels[role]
             for col in columns_satisfying_role:
                 # json lacks a bytes representation. We use str.
                 first = retval_data[col.name].iloc[0]
                 if isinstance(first, bytes) and isinstance(positive, str):
                     positive = positive.encode()
-                logging.debug('positive: %r', positive)
+                logger.debug('positive: %r', positive)
                 retval_data[col.name] = (
                     retval_data[col.name].apply(lambda x, pos=positive: x == pos))
 
         retval.dataframe = retval_data
 
         return retval
 
@@ -62,14 +68,18 @@
 
     If the field is already boolean, no change is made.
 
     If the field is bytes, the pos_label will be converted
     to bytes for the default encoding with str.encode().
     '''
     _name = 'binarize'
+    _tags = {
+        'source': ['auton_lab'],
+        'preprocessor': ['true'],
+    }
     _instance_constructor = BinarizerModelInstance
 
 
 def register(catalog: MemoryAlgorithmCatalog, *args, **kwargs) -> None:
     '''Register all the objects in this file.'''
     model = BinarizerModel(*args, **kwargs)
     catalog.register(model, model.name, upcast(model.tags))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/binarizer_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/binarizer_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/column_parser.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/column_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 A model that takes a dataset and parses its columns
 by data type (int, float, string, datetime)
 
 Currently only parses object columns into categorical.
 '''
 # pylint: disable=duplicate-code
+from typing import Optional
 import pandas as pd
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from ..algorithms.impl.algorithm import Algorithm, MemoryAlgorithmCatalog
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
@@ -18,16 +19,19 @@
 
 class ColumnParserInstance(AlgorithmInstance):
     '''Parses columns of dataset by data type'''
 
     def __init__(self, parent: Algorithm):
         super().__init__(parent=parent)
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         '''Parses columns of dataset by data type'''
+        if dataset is None:
+            return None
+
         retval = dataset.output()
 
         data = dataset.dataframe
 
         if RoleName.TIME in dataset.metadata.roles:
             assert len(dataset.metadata.roles[RoleName.TIME]) == 1, (
                 'BUG: dataset must have exactly 1 time column in roles metadata.')
@@ -47,13 +51,17 @@
         return retval
 
 
 class ColumnParser(Algorithm):
     '''Parses columns of dataset by data type'''
     _name: str = 'Column Parser'
     _instance_constructor: type = ColumnParserInstance
+    _tags = {
+        'source': ['auton_lab'],
+        'preprocessor': ['true'],
+    }
 
 
 def register(catalog: MemoryAlgorithmCatalog, *args, **kwargs) -> None:
     '''Register all the objects in this file.'''
     model = ColumnParser(*args, **kwargs)
     catalog.register(model, model.name, upcast(model.tags))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/column_parser_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/column_parser_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/connect.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/connect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 '''A connector model that changes the names in dictionaries.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from ..algorithms.impl.algorithm import Algorithm, MemoryAlgorithmCatalog, InputKeyError
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
 from ..catalog.catalog import upcast
 from ..wrangler.dataset import Dataset
 
 
 class ConnectorModelInstance(AlgorithmInstance):
     '''Connect one model to another by transforming names.'''
     _transforms: Dict[str, List[str]]
 
     def __init__(self, parent, **hyperparams: Union[str, List[str]]):
         super().__init__(parent=parent)
         self._transforms = {}
-        transforms = self._algorithm.hyperparams(**hyperparams)
+        transforms = self.algorithm.hyperparams(**hyperparams)
         for new_key, old_path in transforms.items():
             if isinstance(old_path, str):
                 self._transforms[new_key] = [old_path]
             else:
                 self._transforms[new_key] = old_path
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         retval = dataset.output()
         for new_key, old_path in self._transforms.items():
             here = dataset
             for old_key in old_path:
                 try:
                     there = here[old_key]
                 except KeyError as exc:
@@ -57,13 +59,17 @@
     If you want to drop a key and its corresponding value, don't pass it in as a new key.
 
     You get only the keys that are mentioned in the arguments to instantiate.
     All other key/value pairs are discarded.
     '''
     _name = 'connect'
     _instance_constructor = ConnectorModelInstance
+    _tags = {
+        'source': ['auton_lab'],
+        'preprocessor': ['true'],
+    }
 
 
 def register(catalog: MemoryAlgorithmCatalog, *args, **kwargs) -> None:
     '''Register all the objects in this file.'''
     model = ConnectorModel(*args, **kwargs)
     catalog.register(model, model.name, upcast(model.tags))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/connect_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/connect_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/extract_columns_by_role.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/extract_columns_by_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
         assert desired_roles is not None
 
         if isinstance(desired_roles, RoleName):
             desired_roles = [desired_roles]
 
         self._desired_roles = desired_roles
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
+
         retval = dataset.output()
         retval_data = {}
         for desired_role in self._desired_roles:
             if desired_role not in dataset.roles.keys():
                 continue
 
             columns_satisfying_role = dataset.roles[desired_role]
@@ -53,14 +56,18 @@
         return retval
 
 
 class ExtractColumnsByRoleModel(Algorithm):
     '''Returns only columns with a specific role.'''
     _name: str = 'Extract Columns by Role'
     _instance_constructor = ExtractColumnsByRoleModelInstance
+    _tags = {
+        'source': ['auton_lab'],
+        'preprocessor': ['true'],
+    }
 
     def _param_from_json(self, hyperparam_name: str, json_value: Any) -> Any:
         if hyperparam_name == 'desired_roles':
             if isinstance(json_value, str):
                 return RoleName[json_value]
             assert isinstance(json_value, list)
             return [RoleName[role] for role in json_value]
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/extract_columns_by_role_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/extract_columns_by_role_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 '''Tests from ExtractColumnsByRoleModel'''
-import os
-from pathlib import Path
-from typing import Dict, Any, List
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+# pylint: disable=missing-function-docstring, duplicate-code
+
+from pathlib import Path
+from typing import Dict, Any, List, Optional
+
 import pandas as pd
 
 from .extract_columns_by_role import ExtractColumnsByRoleModel, ExtractColumnsByRoleModelInstance
+from ..config_components.dataset_config import DatasetConfig
+from ..data_loaders.local_data_loader import LocalDataLoader
 from ..wrangler.dataset import Dataset, RoleName, Metadata, Column
-from ..dataset_formats.local import LocalDatasetConfig
-# pylint: disable=missing-function-docstring, duplicate-code
 
 
 def valid_csv() -> str:
     '''Returns a path (in the form of a string) to a valid csv file.'''
-    current_path = str(os.getenv('PYTEST_CURRENT_TEST')).split('::', maxsplit=1)[0]
-    pathobj = Path(current_path).resolve()
-    module_parent = pathobj.parents[2]
+    module_parent = Path(__file__).parents[2]
     path = module_parent / 'examples' / 'classification' / 'credit.csv'
     return str(path)
 
 
 def make_dataset_clause() -> Dict[str, Any]:
     retval = {
         'config': 'local',
@@ -37,22 +37,24 @@
         }
     }
     return retval
 
 
 def test_simple_extraction() -> None:
     clause: Dict[str, Any] = make_dataset_clause()
-    dataset_config: LocalDatasetConfig = LocalDatasetConfig(clause=clause)
-    dataset: Dataset = dataset_config.load_train()
+    dataset_config = DatasetConfig(clause=clause)
+    data_loader = LocalDataLoader(dataset_config)
+    dataset = data_loader.load_train()
     desired_role: RoleName = RoleName.TARGET
 
     dut: ExtractColumnsByRoleModelInstance = ExtractColumnsByRoleModel().instantiate(
         desired_roles=desired_role
     )
-    dut_result: Dataset = dut.predict(dataset=dataset)
+    dut_result: Optional[Dataset] = dut.predict(dataset=dataset)
+    assert dut_result is not None
     result_cols: List[str] = list(dut_result.dataframe.columns)
     assert len(result_cols) == 1
     assert result_cols[0] == 'class'
 
 
 def test_nonexistent_role_extraction() -> None:
     desired_roles: List[RoleName] = [RoleName.TIME]
@@ -68,39 +70,44 @@
             })
     )
 
     dut: ExtractColumnsByRoleModelInstance = ExtractColumnsByRoleModel().instantiate(
         desired_roles=desired_roles
     )
     got = dut.predict(dataset=fake_dataset)
+    assert got is not None
     assert got['dataframe'].shape == (0, 0)
 
 
 def test_multi_role_extraction() -> None:
     clause: Dict[str, Any] = make_dataset_clause()
-    dataset_config: LocalDatasetConfig = LocalDatasetConfig(clause=clause)
-    dataset: Dataset = dataset_config.load_train()
+    dataset_config = DatasetConfig(clause=clause)
+    data_loader = LocalDataLoader(dataset_config)
+    dataset = data_loader.load_train()
     desired_roles: List[RoleName] = [RoleName.TARGET, RoleName.INDEX]
 
     dut: ExtractColumnsByRoleModelInstance = ExtractColumnsByRoleModel().instantiate(
         desired_roles=desired_roles
     )
-    dut_result: Dataset = dut.predict(dataset=dataset)
+    dut_result: Optional[Dataset] = dut.predict(dataset=dataset)
+    assert dut_result is not None
     result_cols: List[str] = sorted(list(dut_result.dataframe.columns))
     assert len(result_cols) == 2
     assert result_cols[0] == 'checking_status'
     assert result_cols[1] == 'class'
 
 
 def test_multi_role_extraction_with_one_nonexistent() -> None:
     clause: Dict[str, Any] = make_dataset_clause()
-    dataset_config: LocalDatasetConfig = LocalDatasetConfig(clause=clause)
-    dataset: Dataset = dataset_config.load_train()
+    dataset_config = DatasetConfig(clause=clause)
+    data_loader = LocalDataLoader(dataset_config)
+    dataset = data_loader.load_train()
     desired_roles: List[RoleName] = [RoleName.TARGET, RoleName.TIME]
 
     dut: ExtractColumnsByRoleModelInstance = ExtractColumnsByRoleModel().instantiate(
         desired_roles=desired_roles
     )
-    dut_result: Dataset = dut.predict(dataset=dataset)
+    dut_result: Optional[Dataset] = dut.predict(dataset=dataset)
+    assert dut_result is not None
     result_cols: List[str] = list(dut_result.dataframe.columns)
     assert len(result_cols) == 1
     assert result_cols[0] == 'class'
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/identity.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/identity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 '''A model that returns output identical to input.
 
 Used for parallel subpipelines where one of them has no operations in it.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from typing import Optional
 from ..algorithms.impl.algorithm import Algorithm, MemoryAlgorithmCatalog
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
 from ..catalog.catalog import upcast
 from ..wrangler.dataset import Dataset
 
 
 class IdentityModelInstance(AlgorithmInstance):
     '''A model that returns output identical to input.'''
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         new_dataset = dataset.output()
         new_dataset.update(dataset)
         return new_dataset
 
 
 class IdentityModel(Algorithm):
     '''A model that returns output identical to input.'''
     _name = 'identity'
     _instance_constructor = IdentityModelInstance
+    _tags = {
+        'source': ['auton_lab'],
+        'preprocessor': ['true'],
+    }
 
 
 def register(catalog: MemoryAlgorithmCatalog, *args, **kwargs) -> None:
     '''Register all the objects in this file.'''
     model = IdentityModel(*args, **kwargs)
     catalog.register(model, model.name, upcast(model.tags))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,26 +5,34 @@
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from .binder import BinderFactory
 from ...catalog.catalog import Catalog
 from ...catalog.memory_catalog import MemoryCatalog
 from ...catalog.catalog_element_mixin import CatalogElementMixin
+from ...communicators.impl.communicator_auto import CommunicatorCatalogAuto
+from ...communicators.impl.communicator_catalog import CommunicatorCatalog
+from ...discoverers.impl.discoverer_auto import DiscovererCatalogAuto
+from ...discoverers.impl.discoverer_catalog import DiscovererCatalog
 from ...searcher.param_range import ParamRange
 
 # Things that go in catalogs (like Models) typically have a name and a
 # dictionary of tags. Consider extracting this pattern as a mixin.
 # We could then remove the following pylint disable.
 # pylint: disable=duplicate-code
 
 
 class Error(BaseException):
     '''Base class for all model-related exceptions.'''
 
 
+class HyperparamError(Error):
+    '''A hyperparam has an unknown name or incorrect value'''
+
+
 class InputKeyError(Error, KeyError):
     '''Raise when a fit() or predict() method is passed an input dataset
     that is missing required keys.'''
 
 
 class InputValueError(Error, ValueError):
     '''Raise when a fit() or predict() method is passed an input dataset
@@ -32,26 +40,49 @@
 
 
 class Algorithm(CatalogElementMixin, metaclass=abc.ABCMeta):
     '''This object holds an algorithm.
 
     This can be an algorithm for training a model, a preprocessing
     algorithm, or a complete trained model.
+
+    .. rubric:: Parameters:
+
+    * ``communincator_catalog``: ``Optional[CommunicatorCatalog]``.
+      Catalog that holds communicators for distributed algorithms,
+      unused otherwise.
+    * ``discoverer_catalog``: ``Optional[DiscovererCatalog]``.
+      Catalog that holds discoverers for distributed algorithms,
+      unused otherwise.
+    * ``**hyperparams``: ``Any``.
+      Arbitrary hyperparams that are interpreted by each individual algorithm.
+
     '''
     _instance_constructor: type  # This is really Type[AlgorithmInstance]
     _name: str = "unnamed"
     _default_hyperparams: Optional[Dict[str, Any]] = None
     _basename: str = ''
+
+    # These two catalogs are only used by distributed algorithms
+    _communicator_catalog: CommunicatorCatalog
+    _discoverer_catalog: DiscovererCatalog
+
     # Map from json representation to python representation for specifically named hyperparams.
     # Both json and python elements need to be comparable with ==.
     # Format: {hyperparam_name: {json_value: python_value}}
     _hyperparam_lookup: Dict[str, Dict[Any, Any]]
 
-    def __init__(self, name: Optional[str] = None, **hyperparams):
+    def __init__(self,
+                 name: Optional[str] = None,
+                 communicator_catalog: Optional[CommunicatorCatalog] = None,
+                 discoverer_catalog: Optional[DiscovererCatalog] = None,
+                 **hyperparams):
         self._name = name or self._name
+        self._communicator_catalog = (communicator_catalog or CommunicatorCatalogAuto())
+        self._discoverer_catalog = (discoverer_catalog or DiscovererCatalogAuto())
         super().__init__()
 
         # Convert class _default_hyperparams to an instance-specific
         # data structure.
         if self._default_hyperparams is None:
             self._default_hyperparams = {}
         params = self._default_hyperparams.copy()
@@ -65,14 +96,24 @@
         '''Return the base name of the model.
 
         This should be the name used by nf.NeuralForecast to
         label the output column.
         '''
         return self._basename
 
+    @property
+    def communicator_catalog(self) -> CommunicatorCatalog:
+        '''The communicator catalog'''
+        return self._communicator_catalog
+
+    @property
+    def discoverer_catalog(self) -> DiscovererCatalog:
+        '''The discoverer catalog'''
+        return self._discoverer_catalog
+
     def instantiate(self, **hyperparams) -> Any:
         '''Create an instance of an algorithm that can hold training data.
 
         Args:
           serialized_model is a saved form of a trained model that instantiate
           can restore.
           hyperparams includes hyperparameters and other parameters needed
@@ -147,15 +188,21 @@
 
     def instantiate(self, **hyperparams) -> Any:
         return None
 
 
 class AlgorithmCatalog(Catalog[Algorithm], metaclass=abc.ABCMeta):
     '''Base class for algorithm catalogs'''
+    # pylint: disable=unused-argument
+    # These unused arguments are to make signatures match. quack.
+    def __init__(self, communicator_catalog: Optional[CommunicatorCatalog] = None,
+                 discoverer_catalog: Optional[DiscovererCatalog] = None, **kwargs):
+        # This makes mypy happy. We make the signature compatable with MemoryAlgorithmCatalog.
+        super().__init__(**kwargs)
 
 
 class MemoryAlgorithmCatalog(MemoryCatalog[Algorithm], AlgorithmCatalog):
-    '''A Algorithm catalog that has load and register.'''
+    '''An Algorithm catalog that has load and register.'''
 
 
 class AlgorithmCatalogStub(MemoryCatalog[Algorithm], AlgorithmCatalog):
     '''stub'''
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_auto.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_auto.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_auto_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_auto_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_instance.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_instance.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''Holds an instance of a model.'''
 import abc
-from typing import Any
+from typing import Any, Optional
 from typing_extensions import Protocol
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from ...wrangler.dataset import Dataset
 
@@ -17,31 +17,52 @@
 
 class DatasetError(Error):
     '''Something is malformed about the dataset.'''
 
 
 class AlgorithmInstance(metaclass=abc.ABCMeta):
     '''Holds an instance of an algorithm as made by the instantiator.'''
-    _algorithm: Algorithm
+    _algorithm: Optional[Algorithm]
 
     def __init__(self, parent: Algorithm):
         self._algorithm = parent
 
+    @property
+    def algorithm(self) -> Algorithm:
+        '''self._algorithm asserted to non-optional'''
+        assert self._algorithm is not None, (
+            'BUG: we should never access AlgorithmInstance.algorithm if it is not set.'
+        )
+        return self._algorithm
+
     @abc.abstractmethod
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         '''Apply model to input dataset to create output.
 
         This may require that the model is fit (self.trained == True) before it is called.
         '''
 
     @property
     def catalog_name(self) -> str:
         '''The catalog name of our algorithm.'''
+        assert self._algorithm is not None
         return self._algorithm.name
 
+    def start(self) -> None:
+        '''Start any threads that the algorithm needs.
+
+        This is a no-op if the algorithm does not have threads.
+        '''
+
+    def stop(self) -> None:
+        '''Stop all the threads.
+
+        This is a no-op if the algorithm does not have threads.
+        '''
+
 
 class Constructor(Protocol):
     '''Match the signature of a generic model constructor.'''
     def __call__(self, **kwargs: Any) -> Any:
         ...
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/algorithm_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/algorithm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 '''Tests for Algorithm object'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from typing import Optional
 import pytest
 
 from ...problem_def.task import TaskType
 from ...wrangler.dataset import Dataset
 from .algorithm import Algorithm, AlgorithmCatalogStub
 from .algorithm_instance import AlgorithmInstance
 
-# pylint: disable=missing-function-docstring,missing-class-docstring,
-# pylint: disable=protected-access
+# pylint: disable=missing-function-docstring,missing-class-docstring
+# pylint: disable=protected-access, duplicate-code
 
 
 class FakeAlgorithmInstance(AlgorithmInstance):
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         return Dataset(dataset.copy())
 
 
 class FakeAlgorithm(Algorithm):
     _name = 'fake algorithm'
     _default_hyperparams = {
         'base_param': 'base_value',
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/binder.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/binder.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/fake_algorithm.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/fake_algorithm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''A fake algorithm used for tests.'''
 
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from .algorithm import Algorithm
 from .fittable_algorithm_instance import FittableAlgorithmInstance
 
 from ...wrangler.dataset import Dataset
 
 
@@ -32,13 +32,13 @@
     def deserialize(self, serialized_model: bytes) -> 'FakeInstance':
         self.evidence_of_deserialize = serialized_model
         return self
 
     def serialize(self) -> bytes:
         return FAKE_SERIALIZED
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         _ = dataset
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         return dataset
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/fittable_algorithm_instance.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/fittable_algorithm_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 '''Holds an instance of a fittable algorithm.'''
 import abc
+from copy import deepcopy
 import pickle
-from typing import Any
+from typing import Any, Optional
 from typing_extensions import Protocol
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from ...wrangler.dataset import Dataset
 
@@ -41,33 +42,38 @@
                 'Is there a missing implementation of deserialize()?'
             ) from err
         if not isinstance(instance, FittableAlgorithmInstance):
             raise DeserializationError(
                 f'Base AlgorithmInstance unexpectedly handed a {instance} '
                 f'of type {type(instance)}, expected a subtype of AlgorithmInstance. '
                 'Is there a missing implementation of deserialize()?')
+        # The algorithm may contain catalogs which are not pickleable.
+        instance._algorithm = self._algorithm   # pylint: disable=protected-access
         return instance
 
     def serialize(self) -> bytes:
         '''Return a serialized version of a trained model.
 
         By default, we save the whole AlgorithmInstance.'''
         if not self._trained:
-            raise UntrainedError(f'attempt to serialize before fit for {self._algorithm.name}')
-        return pickle.dumps(self)
+            raise UntrainedError(f'attempt to serialize before fit for {self.catalog_name}')
+        minime = deepcopy(self)
+        # The algorithm may contain catalogs which are not pickleable.
+        minime._algorithm = None  # pylint: disable=protected-access
+        return pickle.dumps(minime)
 
     @abc.abstractmethod
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit a model based on train data.
 
         This should set self._trained to True
         '''
 
     @abc.abstractmethod
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         '''Apply model to input dataset to create output.
 
         This may require that the model is fit (self.trained == True) before it is called.
         '''
 
 
 class Constructor(Protocol):
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/fittable_algorithm_instance_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/fittable_algorithm_instance_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 '''Tests for fittable_algorithm_instance.py'''
 import pickle
+from typing import Optional
 import pytest
 
 from ...wrangler.dataset import Dataset
 
 from .algorithm import Algorithm
 from .fake_algorithm import FakeAlgorithm
 from .fittable_algorithm_instance import (FittableAlgorithmInstance,
@@ -17,19 +18,21 @@
 class FakeFitterInstance(FittableAlgorithmInstance):
     _some_attr: str
 
     def __init__(self, parent: Algorithm):
         super().__init__(parent=parent)
         self._some_attr = '1'
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         self._some_attr = '2'
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         dataset['some_attr'] = self._some_attr
         return dataset
 
 
 def test_serialize_deserialize_round_trip() -> None:
     dut = FakeFitterInstance(parent=FakeAlgorithm())
     dut.fit(dataset=Dataset())
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/sklearn_like_algorithm_instance.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/sklearn_like_algorithm_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''An instance of a fittable algorithm that follows sklearn conventions.'''
 import pickle
-from typing import Any
+from typing import Any, Optional
 
 from ...wrangler.dataset import Dataset
 from ...wrangler.dataset import DatasetKeys
 from .algorithm import Algorithm
 from .algorithm_instance import DatasetError
 from .fittable_algorithm_instance import FittableAlgorithmInstance, UntrainedError
 
@@ -12,40 +12,44 @@
 class SklearnLikeAlgorithmInstance(FittableAlgorithmInstance):
     '''An instance of a fittable algorithm that follows sklearn conventions.'''
     _impl: Any
     _constructor: type
 
     def __init__(self, parent: Algorithm, *args, **kwargs):
         super().__init__(parent, *args)
-        self._impl = self._constructor(**self._algorithm.hyperparams(**kwargs))
+        self._impl = self._constructor(**self.algorithm.hyperparams(**kwargs))
 
     def deserialize(self, serialized_model: bytes) -> 'SklearnLikeAlgorithmInstance':
         '''Restore the serialized version of a model.'''
         self._impl = pickle.loads(serialized_model)
         self._trained = True
         return self
 
     def serialize(self) -> bytes:
         '''Return a serialized version of a trained model.'''
         if not self._trained:
-            raise UntrainedError(f'attempt to save training before fit for {self._algorithm.name}')
+            raise UntrainedError(f'attempt to save training before fit for {self.algorithm.name}')
 
         return pickle.dumps(self._impl, pickle.HIGHEST_PROTOCOL)
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit a model based on input dataset.'''
+        if dataset is None:
+            raise DatasetError(f'attempt to fit with no data for {self.algorithm.name}')
         try:
             self._impl.fit(dataset[DatasetKeys.COVARIATES.value], dataset[DatasetKeys.TARGET.value])
         except KeyError as err:
             raise DatasetError(f'fit dataset malformed {dataset!r}') from err
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         if not self._trained:
-            raise UntrainedError(f'attempt to predict before fit for {self._algorithm.name}')
+            raise UntrainedError(f'attempt to predict before fit for {self.algorithm.name}')
+        if dataset is None:
+            return None
         try:
             result = self._impl.predict(dataset[DatasetKeys.COVARIATES.value])
         except KeyError as err:
             raise DatasetError(f'predict dataset malformed {dataset!r}') from err
         retval = dataset.output()
         retval.predictions = result
         return retval
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/impl/sklearn_like_algorithm_instance_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/impl/sklearn_like_algorithm_instance_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 class FakeImpl():
     '''Fake implementation of a model.'''
     dataset: Optional[Dataset] = None
 
     def __init__(self, **kwargs):
         pass
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         self.dataset = dataset
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         return dataset
 
 
 class FakeFitter(Algorithm):
     '''Pretend to do something with data.'''
     _name = 'fake_model'
 
@@ -39,15 +39,15 @@
     '''Pretend to fit data.'''
     _impl = FakeImpl()
     _constructor = FakeImpl
 
     def __init__(self, parent, **kwargs):
         super().__init__(parent=parent, **kwargs)
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit a model based on train data.'''
         self._impl.fit(dataset)
         self._trained = True
 
     @property
     def dataset(self) -> Optional[Dataset]:
         return self._impl.dataset
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/impute/simple_imputer.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/impute/simple_imputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 '''Wrapper for sklearn.impute.SimpleImputer'''
 import pickle
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from sklearn import impute  # type: ignore[import]
 import pandas as pd
 import numpy as np
 
 from ....algorithms.impl.algorithm import Algorithm, MemoryAlgorithmCatalog
-from ....algorithms.impl.algorithm_instance import AlgorithmInstance
+from ....algorithms.impl.algorithm_instance import AlgorithmInstance, DatasetError
 from ....algorithms.impl.fittable_algorithm_instance import (FittableAlgorithmInstance,
                                                              UntrainedError)
 from ....catalog.catalog import upcast
 from ....problem_def.task import DataType
 from ....wrangler.dataset import Dataset
 from ....wrangler.constants import ColumnType
 
@@ -134,16 +134,16 @@
         If True, features that consist exclusively of missing values when fit is
         called are returned in results when transform is called. The imputed
         value is always 0 except when strategy="constant" in which case
         fill_value will be used instead.
     '''
     _name = 'sklearn.impute.SimpleImputer'
     _tags = {
-        'preprocess_type': ['impute'],
-        'wrap_source': ['sklearn'],
+        'source': ['sklearn'],
+        'preprocessor': ['true'],
         'data_type': [DataType.TABULAR.name]
     }
     _default_hyperparams = {
         ColumnType.NUMERIC.value: {
             'missing_values': np.nan,
             'strategy': 'mean',
             'fill_value': None,
@@ -177,15 +177,15 @@
     '''Wrapper for sklearn.impute.SimpleImputer'''
     _imputers: Dict[ColumnType, impute.SimpleImputer]
 
     def __init__(self,
                  parent: SimpleImputerModel,
                  **hyperparams: Dict[str, Any]):
         super().__init__(parent=parent)
-        self._imputers = self._make_imputers(**self._algorithm.hyperparams(**hyperparams))
+        self._imputers = self._make_imputers(**self.algorithm.hyperparams(**hyperparams))
 
     @classmethod
     def _make_imputers(cls, **hyperparams: Dict[str, Any]
                        ) -> Dict[ColumnType, impute.SimpleImputer]:
         retval: Dict[ColumnType, impute.SimpleImputer] = {}
         for col_type, params in hyperparams.items():
             imputer = impute.SimpleImputer(**params)
@@ -220,21 +220,26 @@
                 self._imputers[col_type].fit(X=data_split[col_type])
             elif col_type in self._imputers:
                 del self._imputers[col_type]
 
         # ignore ColumnType.OTHER
         self._trained = True
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Imputers can be fit, but they don't need to.'''
+        if dataset is None:
+            raise DatasetError(f'attempt to fit {self.catalog_name} with no data')
         data_df = dataset.dataframe
         data_split = self._split_df_by_col_type(data_df=data_df)
         self._fit_imputers(data_split=data_split)
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
+
         data_df = dataset.dataframe
         data_split = self._split_df_by_col_type(data_df=data_df)
 
         if not self._trained:
             self._fit_imputers(data_split=data_split)
 
         output_list: List[pd.DataFrame] = [data_split[ColumnType.OTHER]]
@@ -253,15 +258,15 @@
         self._trained = True
         return self
 
     def serialize(self) -> bytes:
         '''Return a serialized version of a trained model.'''
         if not self._trained:
             raise UntrainedError(
-                f'attempt to serialize model before fit for {self._algorithm.name}')
+                f'attempt to serialize model before fit for {self.algorithm.name}')
         return pickle.dumps(self._imputers, pickle.HIGHEST_PROTOCOL)
 
 
 def register(catalog: MemoryAlgorithmCatalog, *args, **kwargs) -> None:
     '''Register all the objects in this file.'''
     model = SimpleImputerModel(*args, **kwargs)
     catalog.register(model, model.name, upcast(model.tags))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/impute/simple_imputer_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/impute/simple_imputer_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 '''Tests for simple_imputer.'''
+from typing import Optional
 import pytest
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import numpy as np
 import pandas as pd
@@ -28,15 +29,16 @@
                 [92, 'F', 'verygood'],
                 [98, 'M', 'excellent']]
     students_df = pd.DataFrame(students, columns=['marks', 'gender', 'result'])
 
     students_dataset = Dataset()
     students_dataset.dataframe = students_df
 
-    result: Dataset = instance.predict(students_dataset)
+    result: Optional[Dataset] = instance.predict(students_dataset)
+    assert result is not None
     result_df: pd.DataFrame = result.dataframe
 
     # we want default strategy to be 'mean' for numerical values (in this case, ~85.83)
     # and 'most_frequent' for categorical values (in this case, 'M')
     assert set(result_df.columns) == set(['marks', 'gender', 'result'])
     assert pytest.approx(85.8333333, 1e-6) == result_df.iat[3, 0]
     assert 'M' == result_df.iat[2, 1]
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 '''An AutonML implementation of sklearn.preprocessing.OneHotEncoder.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from typing import Optional
 from sklearn import preprocessing  # type: ignore[import]
 import pandas as pd
 
+
 from ....catalog.catalog import upcast
 from ....problem_def.task import DataType
 from ....wrangler.dataset import Dataset
 from ...impl.algorithm import Algorithm, MemoryAlgorithmCatalog
+from ...impl.algorithm_instance import DatasetError
 from ...impl.fittable_algorithm_instance import UntrainedError
 from ...impl.sklearn_like_algorithm_instance import SklearnLikeAlgorithmInstance
 
 
 class OneHotModel(Algorithm):
     '''Wrapper for sklearn.preprocessing.OneHotEncoder
 
@@ -89,15 +92,17 @@
         Specifies an upper limit to the number of output features for each input feature when
         considering infrequent categories. If there are infrequent categories, max_categories
         includes the category representing the infrequent categories along with the frequent
         categories. If None, there is no limit to the number of output features.
    '''
     _name = 'sklearn.preprocessing.OneHotEncoder'
     _tags = {
-        'data_type': [DataType.TABULAR.name]
+        'data_type': [DataType.TABULAR.name],
+        'preprocessor': ['true'],
+        'source': ['sklearn']
     }
     _default_hyperparams = {
         'categories': 'auto',
         'drop': None,
         'sparse_output': False,
         'dtype': float,
         'handle_unknown': 'ignore',
@@ -124,23 +129,28 @@
     _constructor = preprocessing.OneHotEncoder
 
     def __init__(self, parent: Algorithm, **kwargs):
         super().__init__(parent=parent, **kwargs)
         assert hasattr(self, '_impl')
         self._impl.set_output(transform='pandas')
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
+        if dataset is None:
+            raise DatasetError('attempt to fit with no data for {self.catalog_name}')
         cov_df = dataset.dataframe
         cov_cat_df = cov_df.select_dtypes(include=CATEGORICAL_TYPES)
         self._impl.fit(X=cov_cat_df)
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         if not self._trained:
-            raise UntrainedError(f'attempt to predict before fit for {self._algorithm.name}')
+            raise UntrainedError(f'attempt to predict before fit for {self.catalog_name}')
+
+        if dataset is None:
+            return None
 
         cov_df = dataset.dataframe
         cov_cat_df = cov_df.select_dtypes(include=CATEGORICAL_TYPES)
         cov_rest_df = cov_df.select_dtypes(exclude=CATEGORICAL_TYPES)
         output_list = [cov_rest_df]
         if not cov_cat_df.empty:
             encoded_cat_df = self._impl.transform(X=cov_cat_df)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/preprocessing/one_hot_encoder_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''Tests for one_hot_encoder.'''
 # pylint: disable=missing-function-docstring, duplicate-code, missing-class-docstring
 # pylint: disable=redefined-outer-name
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from typing import Generator, Tuple
+from typing import Generator, Optional, Tuple
 
 import pandas as pd
 import pytest
 
 from ....algorithms.impl.fittable_algorithm_instance import UntrainedError
 from ....wrangler.dataset import Dataset, DatasetKeys
 
@@ -36,16 +36,17 @@
 class TestOneHotEncoder:
     def test_sunny_day(self, model_and_data) -> None:
         instance, students_dataset = model_and_data
         assert isinstance(instance, OneHotModelInstance)
         assert isinstance(students_dataset, Dataset)
 
         instance.fit(students_dataset)
-        result: Dataset = instance.predict(students_dataset)
+        result: Optional[Dataset] = instance.predict(students_dataset)
 
+        assert result is not None
         students = [[1, 0.0, 1.0], [3, 1.0, 0.0], [2, 1.0, 0.0]]
         expected_result = pd.DataFrame(students, columns=['group', 'gender_Female', 'gender_Male'])
 
         assert result.dataframe.equals(expected_result)
 
     def test_untrained(self, model_and_data) -> None:
         instance, students_dataset = model_and_data
@@ -63,16 +64,17 @@
         assert isinstance(students_dataset, Dataset)
 
         instance.fit(students_dataset)
 
         df1: pd.DataFrame = students_dataset.dataframe
         df2 = pd.DataFrame({'gender': ['Non-binary'], 'group': [2]})
         students_dataset.dataframe = pd.concat([df1, df2], ignore_index=True)
-        result: Dataset = instance.predict(students_dataset)
+        result: Optional[Dataset] = instance.predict(students_dataset)
 
+        assert result is not None
         students = [
             [1, 0.0, 1.0],
             [3, 1.0, 0.0],
             [2, 1.0, 0.0],
             [2, 0.0, 0.0]]
         expected_result = pd.DataFrame(students, columns=['group', 'gender_Female', 'gender_Male'])
         assert result.dataframe.equals(expected_result)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/sklearn_algorithm.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/sklearn_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # pylint: disable=duplicate-code,too-many-arguments
 from typing import Any, Dict, List, Optional
 import importlib
 
 import numpy as np
 from numpy.random import RandomState
 import pandas as pd
+from sklearn.base import BaseEstimator  # type: ignore[import]
 
 from ..impl.algorithm import Algorithm, AlgorithmCatalog
 from ..impl.sklearn_like_algorithm_instance import SklearnLikeAlgorithmInstance
 from ..impl.algorithm_instance import DatasetError
 from ..impl.fittable_algorithm_instance import UntrainedError
 
-from ...problem_def.task import DataType, TaskType
-from ...wrangler.constants import ProblemDefKeys, Defaults
+from ...problem_def.task import DataType, Task, TaskType
+from ...wrangler.constants import Defaults
 from ...wrangler.dataset import Dataset, DatasetKeys
 
 
 def is_empty(frame) -> bool:
     '''Determine if an array-like object is empty.'''
     if frame is None:
         return True
@@ -54,16 +55,17 @@
         if data_types is None:
             data_types = []
         if tags is not None:
             self._tags = tags.copy()
         else:
             self._tags = {}
         self._tags.update({
-            ProblemDefKeys.TASK_TYPE.value: [t.name.lower() for t in tasks],
-            ProblemDefKeys.DATA_TYPE.value: [d.name.lower() for d in data_types],
+            Task.Keys.TASK_TYPE.value: [t.name.lower() for t in tasks],
+            Task.Keys.DATA_TYPE.value: [d.name.lower() for d in data_types],
+            'source': ['sklearn'],
         })
         super().__init__(**hyperparams)
 
     def _load_module(self, name: str):
         # Split name into module part (e.g. sklearn.linear_model)
         # and constructor part (e.g. LinearRegression)
         parts = name.split('.')
@@ -91,15 +93,17 @@
         if parent._tags.get('supports_random_seed', ['false'])[0] == 'true':
             if 'random_seed' in kwargs:
                 kwargs['random_state'] = RandomState(kwargs.pop('random_seed'))
             elif kwargs.get('random_state', None) is None:
                 kwargs['random_state'] = RandomState(Defaults.SEED)
         super().__init__(parent, *args, **kwargs)
 
-    def fit(self, dataset: Dataset):
+    def fit(self, dataset: Optional[Dataset]):
+        if dataset is None:
+            raise DatasetError(f'attempt to fit with no data for {self.catalog_name}')
         assert DatasetKeys.TARGET.value in dataset, (
             "BUG: dataset.metadata.target is unexpectedly None")
         target_data = dataset[DatasetKeys.TARGET.value]
         if isinstance(target_data, pd.DataFrame):
             assert dataset.metadata.target is not None
             target_for_sklearn = list(
                 target_data[dataset.metadata.target.name])
@@ -109,29 +113,32 @@
         covariates = dataset[DatasetKeys.COVARIATES.value]
 
         new_dataset = dataset.output()
         new_dataset[DatasetKeys.TARGET.value] = target_for_sklearn
         new_dataset[DatasetKeys.COVARIATES.value] = covariates
         super().fit(dataset=new_dataset)
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         if not self._trained:
-            raise UntrainedError(f'attempt to predict before fit for {self._algorithm.name}')
+            raise UntrainedError(f'attempt to predict before fit for {self.catalog_name}')
+
+        if dataset is None:
+            return None
 
         # this is not typed because it is supposed to hold the return value from sklearn
         # we expect it to be np.ndarray, but there is no guarantee in sklearn
         predictions_result = np.empty(0)
         probabilities_result = np.empty((0, 0))
 
         try:
             if not is_empty(dataset[DatasetKeys.COVARIATES.value]):
                 predictions_result = self._impl.predict(dataset[DatasetKeys.COVARIATES.value])
 
                 # assume the algorithm has a predict_proba function unless otherwise marked
-                has_predict_proba = 'false' not in self._algorithm.tags.get(
+                has_predict_proba = 'false' not in self.algorithm.tags.get(
                     'has_predict_proba', ['true'])
                 if dataset.metadata.task == TaskType.BINARY_CLASSIFICATION and has_predict_proba:
                     probabilities_result = self._impl.predict_proba(
                         dataset[DatasetKeys.COVARIATES.value])
 
         except KeyError as err:
             raise DatasetError(f'predict dataset malformed {dataset!r}') from err
@@ -154,13 +161,19 @@
             probabilities_result = np.delete(probabilities_result, 0, axis=1).flatten()
             retval.probabilities = pd.DataFrame({
                 dataset.metadata.target.name: probabilities_result
             })
 
         return retval
 
+    @property
+    def impl(self) -> BaseEstimator:
+        '''Get the underlying sklearn model.'''
+        assert isinstance(self._impl, BaseEstimator)
+        return self._impl
+
 
-def register(catalog: AlgorithmCatalog):  # pylint: disable=unused-argument
+def register(catalog: AlgorithmCatalog, **kwargs):  # pylint: disable=unused-argument
     '''Nothing to register.
 
     All subclasses of SklearnAlgorithm are registered in sklearn_algorithms.py
     '''
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/sklearn_algorithm_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/sklearn_algorithm_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,43 +236,43 @@
     assert got.predictions.shape == (1, 1)
     assert got.predictions.iat[0, 0] == 'predict'
 
 
 @pytest.mark.parametrize('name,want_number,want_des', [
     ('sklearn.linear_model.LogisticRegression',
      8,
-     'test_pipe@sklearn.linear_model.logisticregression:C=0.1,class_weight=balanced'),
+     'test_pipe@sklearn.linear_model.logisticregression:c=0.1,class_weight=balanced'),
     ('sklearn.ensemble.RandomForestClassifier',
      24,
      'test_pipe@sklearn.ensemble.randomforestclassifier:'
-     'class_weight=balanced,max_depth=None,min_samples_split=10'),
+     'class_weight=balanced,max_depth=none,min_samples_split=10'),
     ('sklearn.svm.SVC',
      10,
-     'test_pipe@sklearn.svm.svc:C=0.01,class_weight=None'),
+     'test_pipe@sklearn.svm.svc:c=0.01,class_weight=none'),
     ('sklearn.svm.LinearSVC',
      10,
-     'test_pipe@sklearn.svm.linearsvc:C=0.01,class_weight=None'),
+     'test_pipe@sklearn.svm.linearsvc:c=0.01,class_weight=none'),
     ('sklearn.tree.ExtraTreeClassifier',
      24,
      'test_pipe@sklearn.tree.extratreeclassifier:'
      'class_weight=balanced,max_depth=8,min_samples_split=2'),
     ('sklearn.ensemble.GradientBoostingClassifier',
      90,
      'test_pipe@sklearn.ensemble.gradientboostingclassifier:'
-     'max_depth=8,max_features=None,min_samples_leaf=2,min_samples_split=10'),
+     'max_depth=8,max_features=none,min_samples_leaf=2,min_samples_split=10'),
     ('sklearn.ensemble.GradientBoostingRegressor',
      90,
      'test_pipe@sklearn.ensemble.gradientboostingregressor:'
-     'max_depth=10,max_features=None,min_samples_leaf=2,min_samples_split=10'),
+     'max_depth=10,max_features=none,min_samples_leaf=2,min_samples_split=10'),
     ('sklearn.svm.SVR',
      5,
-     'test_pipe@sklearn.svm.svr:C=0.01'),
+     'test_pipe@sklearn.svm.svr:c=0.01'),
     ('sklearn.svm.LinearSVR',
      5,
-     'test_pipe@sklearn.svm.linearsvr:C=0.1'),
+     'test_pipe@sklearn.svm.linearsvr:c=0.1'),
     ('sklearn.ensemble.RandomForestRegressor',
      12,
      'test_pipe@sklearn.ensemble.randomforestregressor:max_depth=8,min_samples_split=2'),
     ('sklearn.linear_model.Ridge',
      5,
      'test_pipe@sklearn.linear_model.ridge:alpha=0.001'),
     ('sklearn.linear_model.Lasso',
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/sklearn/sklearn_algorithms.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/sklearn/sklearn_algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,11 +539,13 @@
         'n_jobs': None,
         'random_state': None,
         'verbose': 0
     },
 ]
 
 
-def register(catalog: MemoryAlgorithmCatalog):
+def register(catalog: MemoryAlgorithmCatalog, **kwargs):
     '''Register all the algorithms in this file.'''
     for alg in ALGORITHMS:
-        catalog.register(SklearnAlgorithm(**alg))
+        new_args = alg.copy()
+        new_args.update(kwargs)
+        catalog.register(SklearnAlgorithm(**new_args))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/wide_to_long.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/wide_to_long.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 '''A model that transforms time series forecasting data from wide format to long format.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from typing import Optional
 import pandas as pd
 
 from ..algorithms.impl.algorithm import Algorithm, MemoryAlgorithmCatalog
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
 from ..catalog.catalog import upcast
 from ..wrangler.dataset import Column, Dataset, RoleName
 
 
 class WideToLongModelInstance(AlgorithmInstance):
     '''A model that transforms time series forecasting data from wide format to long format.'''
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         '''Transform time series dataset from wide to long format.'''
+        if dataset is None:
+            return None
+
         input_roles = dataset.metadata.roles
 
         # Ensure the dataset has exactly 1 time column and at least 1 target column.
         assert RoleName.TIME in input_roles, (
             'BUG: input to WideToLongModel has no time column. \n'
             f'Roles: {input_roles}'
         )
@@ -92,13 +96,17 @@
     3      ts1     1.3
     1      ts2     2.1
     2      ts2     2.2
     3      ts3     2.3
     '''
     _name = 'wide_to_long'
     _instance_constructor = WideToLongModelInstance
+    _tags = {
+        'source': ['pandas'],
+        'preprocessor': ['true'],
+    }
 
 
 def register(catalog: MemoryAlgorithmCatalog, *args, **kwargs) -> None:
     '''Register all the objects in this file.'''
     model = WideToLongModel(*args, **kwargs)
     catalog.register(model, model.name, upcast(model.tags))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/algorithms/wide_to_long_test.py` & `ngautonml-0.4.1b2/ngautonml/algorithms/wide_to_long_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         'timestamp': [1, 2, 3, 4, 1, 2, 3, 4],
         'variable': ['col_a', 'col_a', 'col_a', 'col_a',
                      'col_b', 'col_b', 'col_b', 'col_b'],
         'value': ['a1', 'a2', 'a3', 'a4',
                   'b1', 'b2', 'b3', 'b4'],
     })
 
-    metadata = Metadata({
+    metadata = Metadata(roles={
         RoleName.TIME: [
             Column('timestamp')],
         RoleName.TIMESERIES_ID: [
             Column('variable')],
         RoleName.TARGET: [
             Column('value')],
     })
```

### Comparing `ngautonml-0.4.1b1/ngautonml/bugs/bug1.py` & `ngautonml-0.4.1b2/ngautonml/bugs/bug1.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/bugs/bug1_test.py` & `ngautonml-0.4.1b2/ngautonml/bugs/bug1_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 '''Test for issue #1 on gitlab (https://gitlab.com/autonlab/ngautonml/-/issues/1)'''
+# Copyright (c) 2024 Carnegie Mellon University
+# This code is subject to the license terms contained in the LICENSE file.
+
+# pylint: disable=missing-function-docstring,redefined-outer-name,duplicate-code
+
 import pandas as pd
 import pytest
 
 from ..problem_def.problem_def import ProblemDefinition
 from ..wrangler.wrangler import Wrangler
 
-# pylint: disable=missing-function-docstring,redefined-outer-name,duplicate-code
-
 
 @pytest.fixture(scope='session')
 def bug1_problem_def() -> ProblemDefinition:
-    config = '''
-    {
+    config = {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "data_type": "tabular",
             "task": "binary_classification"
         },
-        "metrics" : {
+        "metrics": {
             "roc_auc_score": {},
             "accuracy_score": {}
         },
         "hyperparams": [
             "disable_grid_search"
         ]
     }
-    '''
-    train_data = pd.DataFrame(
+
+    return ProblemDefinition(clause=config)
+
+
+def test_bug1(bug1_problem_def: ProblemDefinition) -> None:
+    train_data = pd.DataFrame(  # noqa: F841 pylint: disable=unused-variable
         {
             'a': range(1, 101),
             'b': range(101, 201),
             'c': [0, 1] * 50
         }
     )
-    test_data = pd.DataFrame(
+    test_data = pd.DataFrame(  # noqa: F841 pylint: disable=unused-variable
         {
             'a': range(101, 151),
             'b': range(201, 251),
             'c': [0, 1] * 25
         }
     )
-
-    return ProblemDefinition(
-        problem_def=config,
-        train_df=train_data,
-        test_df=test_data)
-
-
-def test_bug1(bug1_problem_def: ProblemDefinition) -> None:
     dut = Wrangler(
         problem_definition=bug1_problem_def)
 
     got = dut.fit_predict_rank()
     assert got.test_results is not None
     pred1 = got.test_results.predictions
 
     new_data = dut.load_test_dataset()
     assert new_data is not None
     got2 = dut.predict(new_data=new_data)
     pred2 = got2.predictions
 
     for des in pred1.keys():
-        df1 = pred1[des].predictions
-        df2 = pred2[des].predictions
+        pred1_des = pred1[des]
+        pred2_des = pred2[des]
+        assert pred1_des is not None
+        assert pred2_des is not None
+        df1 = pred1_des.predictions
+        df2 = pred2_des.predictions
         print(des)
         print(pd.concat([df1, df2], axis=1))
         pd.testing.assert_frame_equal(df1, df2)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/bugs/virtual_module.py` & `ngautonml-0.4.1b2/ngautonml/bugs/virtual_module.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-'''Run a test under a venv environment.*args
+'''Build a virtual environment and install a module in it.
 
 Based loosely on https://gist.github.com/mpurdon/be7f88ee4707f161215187f41c3077f6
 '''
 
-import os
 from pathlib import Path
 from shutil import rmtree
-import sys
 import subprocess
+import sys
 
 
 class VirtualModule:
     '''Create a virtual environment to install a package in.'''
-    def __init__(self, virtual_dir):
+    def __init__(self, virtual_dir: Path):
         self.virtual_dir = virtual_dir
-        self.virtual_python = os.path.join(self.virtual_dir, "bin", "python")
-        self.root = Path(__file__).parents[2]
-
-    def build_module_at_root(self):
-        '''Build a module with poetry at the root directory.'''
-        subprocess.run([sys.executable, "-m", "poetry", "build"], cwd=self.root, check=True)
+        self.virtual_python = self.virtual_dir / 'bin' / 'python'
 
-    def install_virtual_env(self):
+    def install_virtual_env(self) -> None:
         '''Install a virtual environment at self.virtual_dir.'''
-        subprocess.run([sys.executable, "-m", "virtualenv", self.virtual_dir], check=True)
+        subprocess.run([sys.executable, '-m', 'virtualenv', self.virtual_dir], check=True)
 
-    def install_under_venv(self, module):
+    def install_under_venv(self, module: Path) -> None:
         '''Install a module under the virtual environment.'''
-        subprocess.run([self.virtual_python, "-m", "pip", "install", module], check=True)
+        subprocess.run([str(self.virtual_python), '-m', 'pip', 'install', str(module)], check=True)
 
-    def finalize(self):
+    def finalize(self) -> None:
         '''Clean up the virtual environment.'''
-        rmtree(self.virtual_dir)
-        self.virtual_dir = None
+        rmtree(str(self.virtual_dir))
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/catalog.py` & `ngautonml-0.4.1b2/ngautonml/catalog/catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Base module for catalogs in AutonML.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import abc
-from typing import Generic, TypeVar, Dict, Iterable, List, Set, Union
+from typing import Dict, Generic, Iterable, List, Set, Tuple, TypeVar, Union
 
 T = TypeVar("T")
 
 
 class CatalogError(Exception):
     '''Base error class for the catalog module'''
 
@@ -38,14 +38,18 @@
         '''Retrieve list of all tag types present in catalog'''
 
     @abc.abstractmethod
     def all_objects(self) -> Iterable[T]:
         '''Retrieve all registered objects.'''
 
     @abc.abstractmethod
+    def items(self) -> Iterable[Tuple[str, T]]:
+        '''List all the items in the catalog.'''
+
+    @abc.abstractmethod
     def tagvals(self, tagtype: str) -> Set[str]:
         '''Retrieve all tag values present for a given tag type'''
 
     @abc.abstractmethod
     def lookup_by_name(self, name: str) -> T:
         '''Find an object registered under name.'''
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/catalog_element_mixin.py` & `ngautonml-0.4.1b2/ngautonml/catalog/catalog_element_mixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,7 +45,20 @@
         return self._name
 
     @property
     def tags(self) -> Dict[str, List[str]]:
         '''The catalog tags of the object'''
         assert self._tags is not None
         return self._tags.copy()
+
+    def _tag_to_bool(self, tagname: str, default: bool) -> bool:
+        '''Interprets a list of tag values as a boolean.
+
+        As of 01-03-2024, only looks at first value in list,
+        and checks if it equals 'true' (case-insensitive).
+
+        If the tag is not set, will return default.
+        '''
+        assert self._tags is not None
+        if tagname in self._tags:
+            return self._tags[tagname][0].lower() == 'true'
+        return default
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/catalog_element_mixin_test.py` & `ngautonml-0.4.1b2/ngautonml/catalog/catalog_element_mixin_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/catalog_shelf.py` & `ngautonml-0.4.1b2/ngautonml/catalog/catalog_shelf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''An object that glues together a sequence of catalogs.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from typing import Any, Dict, Iterable, List, Optional, Set, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, TypeVar, Union
 
 from .catalog import Catalog, CatalogLookupError
 from .memory_catalog import MemoryCatalog
 
 T = TypeVar('T')
 
 
@@ -32,16 +32,20 @@
     def all_objects(self) -> Iterable[T]:
         '''Retrieve all objects in all catalogs.
 
         Note that some objects may be returned which are otherwise
         masked during lookups.
         '''
         for catalog in self._catalogs:
-            for obj in catalog.all_objects():
-                yield obj
+            yield from catalog.all_objects()
+
+    def items(self) -> Iterable[Tuple[str, T]]:
+        for catalog in self._catalogs:
+            for key, obj in catalog.items():
+                yield (key, obj)
 
     def tagvals(self, tagtype: str) -> Set[str]:
         '''Retrieve all tag values present for a given tag type'''
         retval = set()
         for catalog in self._catalogs:
             retval.update(catalog.tagvals(tagtype=tagtype))
         return retval
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/catalog_shelf_test.py` & `ngautonml-0.4.1b2/ngautonml/catalog/catalog_shelf_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''Test the catalog shelf module.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from typing import Dict, Iterable, Set, Union
+from typing import Dict, Iterable, Set, Tuple, Union
 import pytest
 
 from .catalog import Catalog, CatalogLookupError
 from .memory_catalog import MemoryCatalog
 from .catalog_shelf import CatalogShelf
 from .catalog_element_mixin import CatalogElementMixin
 
@@ -32,24 +32,42 @@
     @property
     def tagtypes(self) -> Set[str]:
         return set()
 
     def all_objects(self) -> Iterable[Widget]:
         return []
 
+    def items(self) -> Iterable[Tuple[str, Widget]]:
+        return []
+
     def tagvals(self, tagtype: str) -> Set[str]:
         return set()
 
     def lookup_by_name(self, name: str) -> Widget:
         raise CatalogLookupError()
 
     def lookup_by_tag_and(self, **tags: Union[str, Iterable[str]]) -> Dict[str, Widget]:
         return {}
 
 
+def test_items():
+    '''Register a widget into a shelf with an empty catalog at the start.'''
+    catalog1 = WidgetCatalog()
+    catalog2 = WidgetCatalog()
+    widget1 = NamedWidget(name='widget1')
+    catalog2.register(widget1)
+    widget2 = NamedWidget(name='widget2')
+    dut = CatalogShelf(catalog1, catalog2)
+    dut.register(widget2)
+    assert dict(dut.items()) == {
+        'widget1': widget1,
+        'widget2': widget2,
+    }
+
+
 def test_one_catalog():
     '''Load a catalog into the Shelf'''
     catalog1 = WidgetCatalog()
     widget1 = NamedWidget(name='widget1')
     catalog1.register(widget1)
     dut = CatalogShelf(catalog1)
     assert dut.lookup_by_name('widget1') == widget1
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/memory_catalog.py` & `ngautonml-0.4.1b2/ngautonml/catalog/memory_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from collections import defaultdict
 from importlib import util
 import logging
 import os
 from pathlib import Path
 import sys
-from typing import Any, Iterable, TypeVar, Optional, Dict, List, Set, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, TypeVar, Union
 
 from .catalog import (Catalog, CatalogError, CatalogLookupError,
                       CatalogNameError, CatalogValueError)
 from ..wrangler.constants import CATALOG_IGNORE
 
 T = TypeVar("T")
 
@@ -75,15 +75,22 @@
                  tags: Optional[Dict[str, Union[str, List[str]]]] = None) -> str:
         '''Register an object under the name.'''
         obj_name = name
         if obj_name is None:
             if hasattr(obj, 'name'):
                 obj_name = getattr(obj, 'name')
             else:
-                raise CatalogNameError("Name not defined for Catalog Object.")
+                if isinstance(obj, type):
+                    obj_signifier = obj.__name__
+                else:
+                    obj_signifier = obj.__class__.__name__
+
+                raise CatalogNameError(
+                    'Name must be defined for Catalog Object: '
+                    f'{obj_signifier}')
         obj_name = obj_name.lower()
 
         if obj_name in self.__cat_names:
             raise CatalogDuplicateError(obj_name)
 
         self.__cat_names[obj_name] = obj
 
@@ -222,14 +229,17 @@
             module = util.module_from_spec(spec)
             if spec.loader is None:
                 raise ImportError(f'loader for module {modname} is None')
             spec.loader.exec_module(module)
             sys.modules[modname] = module
         return module
 
+    def items(self) -> Iterable[Tuple[str, T]]:
+        return self.__cat_names.items()
+
 
 def module_name_from_filepath(filepath: str, root_path: str) -> str:
     """Converts a path to a .py file into a Python module name.
 
     E.g. for a root_path of "/home/piggy/src/autonml" and a filepath of
     "/home/piggy/src/autonml/ngautonml/algorithms/connect.py", we get
     a module name of "ngautonml.algorithms.connect".
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/memory_catalog_test.py` & `ngautonml-0.4.1b2/ngautonml/catalog/memory_catalog_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,7 +220,21 @@
 
     by_name = dut.lookup_by_name(name='widget_named_tagged')
     assert hasattr(by_name, 'name')
     assert by_name.name == widget.name
 
     by_tag = dut.lookup_by_tag_and(tag_key='tag_value2')
     assert by_tag[widget.name].name == widget.name
+
+
+def test_lookup_items() -> None:
+    '''Find a list of several widgets by arbitrary tag.'''
+    dut = WidgetCatalog()
+    test_widgetone = NamedWidget('TestWidget')
+    dut.register(obj=test_widgetone, name='TestWidget')
+    test_widgettwo = NamedWidget('TestWidgetTwo')
+    dut.register(obj=test_widgettwo, name='TestWidgetTwo')
+
+    assert dut.items() == {
+        'testwidget': test_widgetone,
+        'testwidgettwo': test_widgettwo,
+    }.items()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/pathed_catalog.py` & `ngautonml-0.4.1b2/ngautonml/catalog/pathed_catalog.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/pathed_catalog_test.py` & `ngautonml-0.4.1b2/ngautonml/catalog/pathed_catalog_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/plugin_catalog.py` & `ngautonml-0.4.1b2/ngautonml/catalog/plugin_catalog.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/plugin_catalog_test.py` & `ngautonml-0.4.1b2/ngautonml/catalog/plugin_catalog_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,37 +39,41 @@
 
 
 def test_home_directory_auto(home_path) -> None:
     os.environ['HOME'] = str(home_path)
     dut: Catalog = PluginCatalog('widgets', default_root=Path(__file__).parent)
     got1 = dut.lookup_by_name('Gizmo')
     assert isinstance(got1, NamedWidget)
+    # if this were using the Gizmo in ./widgets/some_subfolder/gizmo.py,
+    #   the value of 'some_tag' would be 'test_dir'
     assert got1.tags['some_tag'] == ['home_directory']
 
     got2 = dut.lookup_by_name('DooDad')
     assert isinstance(got2, NamedWidget)
+    # we are using the DooDad in ./widgets/doodad.py, so the
+    #   value of 'some_tag_ is 'test_dir'
     assert got2.tags['some_tag'] == ['test_dir']
     assert hasattr(got2, 'quux')
 
 
-def test_home_directory_auto_with_plugin(home_path) -> None:
+def test_with_plugin() -> None:
     pluginpath = (Path(__file__).parents[2] / 'plugins' / 'testplugin'
                   / 'dist' / 'testplugin-0.0.1-py3-none-any.whl')
     subprocess.run(['python', '-m', 'build'], cwd=pluginpath.parents[1], check=True)
     subprocess.run(['pip', 'install', pluginpath], check=False)
-    os.environ['HOME'] = str(home_path)
     try:
         dut: Catalog = PluginCatalog('widgets', default_root=Path(__file__).parent)
+        got = dut.lookup_by_name('DooDad')
+        assert isinstance(got, NamedWidget)
+        # because testplugin is installed, DooDad will be overridden by the one
+        #   in testplugin, where the value of 'some_tag' is 'plugin_dir'
+        assert got.tags['some_tag'] == ['plugin_dir']
+        assert hasattr(got, 'quux')
     finally:
-        subprocess.run(['pip', 'uninstall', '-y', pluginpath], check=False)
-
-    got = dut.lookup_by_name('DooDad')
-    assert isinstance(got, NamedWidget)
-    assert got.tags['some_tag'] == ['plugin_dir']
-    assert hasattr(got, 'quux')
+        subprocess.run(['pip', 'uninstall', '-y', 'testplugin'], check=False)
 
 
 def test_register_to_plugin_catalog(home_path) -> None:
     os.environ['HOME'] = str(home_path)
     dut: PluginCatalog = PluginCatalog('widgets', default_root=Path(__file__).parent)
 
     new_doodad = NamedWidget(name='DooDad', tags={'some_tag': ['hand_registered']})
```

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/widgets/doodad.py` & `ngautonml-0.4.1b2/ngautonml/catalog/widgets/doodad.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/catalog/widgets/some_subfolder/gizmo.py` & `ngautonml-0.4.1b2/ngautonml/catalog/widgets/some_subfolder/gizmo.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator_auto.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator_auto.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/impl/cross_validator_test.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/impl/cross_validator_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/k_fold_cross_validator.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/k_fold_cross_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Performs k-fold cross-validation.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 # pylint: disable=duplicate-code
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import pandas as pd
 
 from ..catalog.catalog import upcast
 from ..executor.executor import Executor
 from ..generator.bound_pipeline import BoundPipeline
 from ..generator.designator import Designator
@@ -26,50 +26,59 @@
 
     Works for single-fold validation as well
     '''
 
     _name = 'k_fold_cross_validator'
 
     def _concatenate_predictions(self,
-                                 datasets: List[Dataset]) -> Dataset:
+                                 datasets: List[Optional[Dataset]]) -> Optional[Dataset]:
         '''Concatenate a list of fold prediction Datasets into a single Dataset
         that covers the entire train set.'''
         assert len(datasets) > 0, 'BUG: _concatenate() called when length of dataset list is 0'
 
+        if any(dset is None for dset in datasets):
+            return None
+
+        assert datasets[0] is not None
         retval = datasets[0].output()
 
         errors: List[PredictError] = []
         for dset in datasets:
+            assert dset is not None
             if DatasetKeys.ERROR.value in dset:
                 errors.append(dset[DatasetKeys.ERROR.value])
 
         if len(errors) > 0:
             # handle errors
             error_text = 'Pipeline errors occurred during cross-validation: \n' + '\n'.join([
                 str(error) for error in errors
             ])
             retval[DatasetKeys.ERROR.value] = PredictError(error_text)
             return retval
 
         retval.predictions = datasets[0].predictions
         for dset in datasets[1:]:
+            assert dset is not None
             retval.predictions = pd.concat([retval.predictions, dset.predictions], axis=0)
 
         if DatasetKeys.PROBABILITIES.value in datasets[0]:
             retval.probabilities = datasets[0].probabilities
             for dset in datasets[1:]:
+                assert dset is not None
                 retval.probabilities = pd.concat([retval.probabilities, dset.probabilities], axis=0)
 
         return retval
 
-    def _concatenate_all(self,
-                         predictions: Dict[Designator, List[Dataset]]) -> Dict[Designator, Dataset]:
+    def _concatenate_all(
+            self,
+            predictions: Dict[Designator,
+                              List[Optional[Dataset]]]) -> Dict[Designator, Optional[Dataset]]:
         '''Concatenate each list of fold prediction Datasets into a single Dataset
         that covers the entire train set.'''
-        retval: Dict[Designator, Dataset] = {
+        retval: Dict[Designator, Optional[Dataset]] = {
             des: self._concatenate_predictions(data) for des, data in predictions.items()}
         return retval
 
     def validate_pipelines(self,
                            split_dataset: SplitDataset,
                            bound_pipelines: Dict[Designator, BoundPipeline],
                            instantiator: InstantiatorFactory,
@@ -77,15 +86,15 @@
                            **overrides
                            ) -> Dict[Designator, PipelineResult]:
         '''Do cross-validation by running pipelines on a split dataset.
 
         Returns the split dataset and an ExecutorResult for each pipeline.'''
         # For each fold, we will append that fold's predictions to the list of datasets for the
         # corresponding pipeline
-        train_predictions: Dict[Designator, List[Dataset]] = {
+        train_predictions: Dict[Designator, List[Optional[Dataset]]] = {
             des: [] for des in bound_pipelines}
 
         executable_pipelines: Dict[Designator, ExecutablePipeline] = {}
 
         for fold in split_dataset.folds:
             # Instantiate new executable pipelines for each bound pipeline
             # TODO(Piggy/Merritt): run this cross validator in parallel to take advantage of
```

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/k_fold_cross_validator_test.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/k_fold_cross_validator_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,18 +98,24 @@
     assert got[des1].bound_pipeline.name == bp1.name
     assert got[des2].bound_pipeline.name == bp2.name
     assert got[des1].split_dataset == split_dataset
     assert got[des2].split_dataset == split_dataset
     expected_frame = pd.DataFrame({
         'a': [53, 4, 5030, 53, 4, 5030],
         'id': [0, 1, 2, 0, 1, 2]}).set_index('id')
+
+    got_des1 = got[des1]
+    got_des2 = got[des2]
+    assert got_des1.prediction is not None
+    assert got_des2.prediction is not None
+
     pd.testing.assert_frame_equal(
-        got[des1].prediction.predictions, expected_frame)
+        got_des1.prediction.predictions, expected_frame)
     pd.testing.assert_frame_equal(
-        got[des2].prediction.predictions, expected_frame)
+        got_des2.prediction.predictions, expected_frame)
 
 
 def test_probabilities_preserved(
         split_dataset: SplitDataset) -> None:
 
     bp1 = BoundPipelineStub('bound_pipeline_stub_1')
     bp2 = BoundPipelineStub('bound_pipeline_stub_2')
@@ -124,19 +130,25 @@
         bound_pipelines=bound_pipelines,
         instantiator=InstantiatorFactory(),
         executor=FakeExecutor(return_proba=True))
 
     expected_frame = pd.DataFrame({
         'prob': [0.5, 0.6, 0.7, 0.5, 0.6, 0.7],
         'id': [0, 1, 2, 0, 1, 2]}).set_index('id')
+
+    got_des1 = got[des1]
+    got_des2 = got[des2]
+    assert got_des1.prediction is not None
+    assert got_des2.prediction is not None
+
     pd.testing.assert_frame_equal(
-        got[des1].prediction.probabilities,
+        got_des1.prediction.probabilities,
         expected_frame)
     pd.testing.assert_frame_equal(
-        got[des2].prediction.probabilities, expected_frame)
+        got_des2.prediction.probabilities, expected_frame)
 
 
 def test_error_catching(split_dataset: SplitDataset) -> None:
     '''Properly handle pipeline errors that are caught by the executor
 
     We expect to find no 'predictions' key in the dataset, but an 'errors' key instead
     '''
@@ -157,23 +169,27 @@
     assert des1 in got and des2 in got
     assert len(got) == 2
     assert got[des1].bound_pipeline.name == bp1.name
     assert got[des2].bound_pipeline.name == bp2.name
     assert got[des1].split_dataset == split_dataset
     assert got[des2].split_dataset == split_dataset
 
-    assert 'predictions' not in got[des1].prediction
-    assert isinstance(got[des1].prediction['error'], PredictError)
-
-    assert 'error' not in got[des2].prediction
+    got_des1 = got[des1]
+    assert got_des1.prediction is not None
+    assert 'predictions' not in got_des1.prediction
+    assert isinstance(got_des1.prediction['error'], PredictError)
+
+    got_des2 = got[des2]
+    assert got_des2.prediction is not None
+    assert 'error' not in got_des2.prediction
     expected_frame = pd.DataFrame({
         'a': [53, 4, 5030, 53, 4, 5030],
         'id': [0, 1, 2, 0, 1, 2]}).set_index('id')
     pd.testing.assert_frame_equal(
-        got[des2].prediction.predictions, expected_frame)
+        got_des2.prediction.predictions, expected_frame)
 
 
 def test_order() -> None:
     bp1 = BoundPipelineStub('bound_pipeline_stub_1')
     des1 = Designator('des1')
 
     bound_pipelines: Dict[Designator, BoundPipeline] = {des1: bp1}
@@ -198,9 +214,10 @@
     got = dut.validate_pipelines(
         split_dataset=split_dataset,
         bound_pipelines=bound_pipelines,
         instantiator=InstantiatorFactory(),
         executor=FakeExecutor(order_test=True))
 
     result = got[des1]
+    assert result.prediction is not None
     print(result.prediction.predictions)
     assert list(result.prediction.predictions['target']) == [2, 3, 4, 5, 6, 7, 8, 9, 10]
```

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/single_fold_validator.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/single_fold_validator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/single_fold_validator_test.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/single_fold_validator_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/cross_validators/stub_cross_validator.py` & `ngautonml-0.4.1b2/ngautonml/cross_validators/stub_cross_validator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/dataset_formats/impl/dataset_config.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,314 +1,313 @@
-'''Holds cofirguration information about the dataset.'''
+'''Holds a dataset.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-# pylint: disable=protected-access
-
-import abc
-from typing import Any, Dict, List, Optional, Union
+import copy
+from enum import Enum
+from typing import Any, Dict, List, Optional
 
 import pandas as pd
 
-from ...problem_def.config_component import (ConfigComponent, ConfigError,
-                                             InvalidKeyError, InvalidValueError,
-                                             MissingKeyError, ValidationErrors)
-from ...problem_def.task import Task
-from ...wrangler.dataset import Dataset, Metadata, RoleName, Column
-from ...wrangler.constants import Defaults, ProblemDefKeys, ProblemDefKeySet
+from ..config_components.impl.config_component import ConfigComponent
+from ..problem_def.task import DataType, TaskType
+from ..problem_def.problem_def_interface import ProblemDefInterface
 
 
-class DatasetConfigError(ConfigError):
-    '''Base class for errors in DatasetConfig.'''
+class Error(BaseException):
+    '''Base class for all model-related exceptions.'''
 
 
-class UnknownConfigClassError(DatasetConfigError):
-    '''Problem definition specified a dataset config that is not recognized.'''
+class DatasetKeyError(Error, KeyError):
+    '''Raise when a fit() or predict() method is passed an input dataset
+    that is missing required keys.'''
 
 
-class DatasetFileError(DatasetConfigError):
-    '''The dataset file does not match information given in the problem definition.'''
+class DatasetValueError(Error, ValueError):
+    '''Raise when a dataset has the correct keys but invalid value(s)'''
 
 
-class DatasetConfigTypeError(DatasetConfigError, TypeError):
-    '''An object in the dataset config was not the right type.'''
+class RoleName(Enum):
+    '''Possible column roles'''
+    INDEX = 'index'
+    TARGET = 'target'
+    ATTRIBUTE = 'attribute'
 
+    # For testing only
+    TEST_ROLE = 'test_role'
 
-class ParsingErrors(DatasetConfigError):
-    '''At least one parsing error occured.'''
-    def __init__(self, errors: List[DatasetConfigError]):
-        super().__init__(f'At least one parsing error occured: {errors!r}')
-        self.errors = errors
+    # For time series only
+    TIME = 'time'
+    TIMESERIES_ID = 'timeseries_id'
+    PAST_EXOGENOUS = 'past_exogenous'
+    FUTURE_EXOGENOUS = 'future_exogenous'
 
 
-class DatasetConfig(ConfigComponent, metaclass=abc.ABCMeta):
-    '''Holds confirguration information about the dataset.'''
-    _roles: Dict[RoleName, List[Column]]
-    _pos_labels: Dict[RoleName, Any]
-    _forecasting_metadata: Dict[str, Any]
-    _task: Optional[Task]
+class Column():
+    '''Defines a column in a dataset'''
+    _name: str
 
     def __init__(self,
-                 clause: Dict[str, Any],
-                 parents: Optional[List[str]] = None,
-                 task: Optional[Task] = None,
-                 **unused_kwargs):
-        parents = self._add_parent(parents, ProblemDefKeys.CONFIG.value)
-        super().__init__(clause=clause, parents=parents)
-        self._roles = self._build_roles()
-        self._pos_labels = self._build_pos_labels()
-        self._forecasting_metadata = self._build_forecasting_metadata()
-        self._task = task
-
-    def __str__(self):
-        return f'{{Index: {self.index_cols}, Target: {self.target}}}'
-
-    def _build_roles(self) -> Dict[RoleName, List[Column]]:
-        '''Build dict of column roles'''
-        retval: Dict[RoleName, List[Column]] = {}
-        for role in self._get_with_default(ProblemDefKeys.COL_ROLES, dflt={}):
-            # this will throw a parsing error if the key does not match any known role name
-            rolename = RoleName[role.upper()]
-
-            col_names = self._get_with_default(ProblemDefKeys.COL_ROLES,
-                                               role,
-                                               ProblemDefKeys.COL_NAME,
-                                               dflt=None)
-            if col_names is not None:
-                retval[rolename] = [Column(name=col_names)]
-            # TODO(Merritt): make this more sensible
-
-        return retval
-
-    def _build_pos_labels(self) -> Dict[RoleName, Any]:
-        '''Build dict of pos labels for binary classification.
-
-        In the vast majority of cases, the only key will be RoleName.TARGET'''
-        retval: Dict[RoleName, Any] = {}
-        for role in self._get_with_default(ProblemDefKeys.COL_ROLES, dflt={}):
-            rolename = RoleName[role.upper()]
-            retval[rolename] = self._get_with_default(
-                ProblemDefKeys.COL_ROLES, role, ProblemDefKeys.POS_LABEL, dflt=None)
-        return retval
+                 name: str):
+        self._name = name
 
-    def _build_forecasting_metadata(self) -> Dict[str, Any]:
-        '''Build dict of additional metadata for forecasting problems.
+    @property
+    def name(self) -> str:
+        '''The column's name'''
+        return str(self._name)
+
+    def __eq__(self, other: Any):
+        if not isinstance(other, Column):
+            return False
+        return self.name == other.name
+
+    def __hash__(self) -> int:
+        return self._name.__hash__()
+
+    def __str__(self) -> str:
+        return f'Column({self.name})'
+
+    def __repr__(self) -> str:
+        return f'ngautonml.wrangler.dataset.Column ({self.name})'
+
+
+class DatasetKeys(Enum):
+    '''Standard keys used in the Dataset object passed between models'''
+    DATAFRAME = 'dataframe'
+    TARGET = 'target'
+    COVARIATES = 'covariates'
+    PREDICTIONS = 'predictions'
+    PROBABILITIES = 'probabilities'
+    TRAIN = 'train'
+    VALIDATE = 'validate'
+    GROUND_TRUTH = 'ground_truth'
+    ERROR = 'error'
+
+    # for time series forecasting only
+    STATIC_EXOGENOUS = 'static_exogenous'
+    DYNAMIC_EXOGENOUS = 'dynamic_exogenous'
+
+    # for keras image processing only
+    KERAS_DS = 'keras_ds'
+    KERAS_VALIDATE = 'keras_validate'
 
-        This includes 'horizon', 'input_size', and 'frequency'.
-        '''
-        retval: Dict[str, Any] = {}
-        clause = self._get_with_default(ProblemDefKeys.FORECASTING, dflt={})
-        if not isinstance(clause, dict):
-            return retval
-        for key, val in clause.items():
-            retval[key] = val
-        if ProblemDefKeys.FREQUENCY.value not in retval:
-            retval[ProblemDefKeys.FREQUENCY.value] = Defaults.FREQUENCY
-
-        # If step_size is not defined, set as equal to horizon
-        if (ProblemDefKeys.STEP_SIZE.value not in retval
-                and ProblemDefKeys.HORIZON.value in retval):
-            retval[ProblemDefKeys.STEP_SIZE.value] = retval[ProblemDefKeys.HORIZON.value]
-
-        return retval
-
-    def validate(self, **kwargs) -> None:
-        '''Check the problem definition dataset clause for errors.'''
-        errors: List[ConfigError] = []
-
-        dataset_keys = set(self._clause.keys())
-        if not ProblemDefKeySet.DATASET.REQUIRED.issubset(dataset_keys):
-            errors.append(MissingKeyError(
-                'Required keys missing in dataset clause: '
-                f'{ProblemDefKeySet.DATASET.REQUIRED.difference(dataset_keys)}'))
-
-        if not dataset_keys.issubset(ProblemDefKeySet.DATASET.ALLOWED):
-            errors.append(InvalidKeyError(
-                'Invalid key(s) in dataset clause: '
-                f'{dataset_keys.difference(ProblemDefKeySet.DATASET.ALLOWED)}'
-            ))
-
-        try:
-            self._validate_roles()
-        except ValidationErrors as err:
-            errors.extend(err.errors)
-
-        if self._exists(ProblemDefKeys.FORECASTING.value):
-            data_keys = set(self._get(ProblemDefKeys.FORECASTING.value).keys())
-            if not ProblemDefKeySet.DATASET.FORECASTING.REQUIRED.issubset(data_keys):
-                errors.append(MissingKeyError(
-                    'Required keys missing in forecasting metadata: '
-                    f'{ProblemDefKeySet.DATASET.FORECASTING.REQUIRED.difference(data_keys)}'))
-
-            if not data_keys.issubset(ProblemDefKeySet.DATASET.FORECASTING.ALLOWED):
-                errors.append(InvalidKeyError(
-                    'Invalid key(s) in forecasting metadata: '
-                    f'{data_keys.difference(ProblemDefKeySet.DATASET.FORECASTING.ALLOWED)}'))
-
-            freq_val = self._get_with_default(
-                ProblemDefKeys.FORECASTING.value,
-                ProblemDefKeys.FREQUENCY.value,
-                dflt=Defaults.FREQUENCY)
-            offset_strs = [x for x in dir(pd.offsets) if DatasetConfig._is_valid_offset(x)]
-            allowed_freq = [getattr(pd.offsets, x)().freqstr for x in offset_strs]
-
-            if freq_val not in allowed_freq:
-                errors.append(InvalidValueError(
-                    'Invalid value in forecasting metadata: '
-                    f'{freq_val} is not a valid value for frequency. '
-                    f'Allowed frequency values are: {allowed_freq}'))
-
-            if ProblemDefKeys.HORIZON.value in data_keys:
-                step_size = self.metadata.step_size or 0
-                horizon = self._get(ProblemDefKeys.FORECASTING.value,
-                                    ProblemDefKeys.HORIZON.value)
-                if (step_size < 1) or (step_size > horizon):
-                    errors.append(InvalidValueError(
-                        'Invalid value in forecasting metadata: '
-                        f'{step_size} is not a valid value for step_size. '
-                        f'Value for step_size must be between 1 and {horizon}'
-                    ))
-
-        if len(errors) > 0:
-            raise ValidationErrors(errors=errors)
-
-    def _validate_roles(self) -> None:
-        if ProblemDefKeys.COL_ROLES.value not in set(self._clause.keys()):
-            return
-
-        errors: List[ConfigError] = []
-
-        for role_name in self._get(ProblemDefKeys.COL_ROLES.value):
-            role_keys = set(self._get(ProblemDefKeys.COL_ROLES.value,
-                                      role_name).keys())
-            if not ProblemDefKeySet.DATASET.ROLES.REQUIRED.issubset(role_keys):
-                errors.append(MissingKeyError(
-                    f'Required key(s) missing in role clause for role {role_name}: '
-                    f'{ProblemDefKeySet.DATASET.ROLES.REQUIRED.difference(role_keys)}'))
-
-            if not role_keys.issubset(ProblemDefKeySet.DATASET.ROLES.ALLOWED):
-                errors.append(InvalidKeyError(
-                    f'Invalid key(s) in role clause for role {role_name}: '
-                    f'{role_keys.difference(ProblemDefKeySet.DATASET.ROLES.ALLOWED)}'
-                ))
-
-        if len(errors) > 0:
-            raise ValidationErrors(errors=errors)
-
-    @staticmethod
-    def _is_valid_offset(offset: str) -> bool:
-        invalid_offsets = set(['BaseOffset', 'Tick', 'DateOffset', 'Easter'])
-        obj = getattr(pd.offsets, offset)
-
-        return not offset.startswith('_') and callable(obj) and offset not in invalid_offsets
-
-    def cols_with_role(self, role: Union[str, RoleName]) -> List[Column]:
-        '''Return a list of Columns that have the given role'''
-        if isinstance(role, str):
-            role = RoleName[role.upper()]
-        if role not in self._roles:
-            return []
-        return self._roles[role]
 
-    @property
-    def target(self) -> Optional[Column]:
-        '''Column with role "target".'''
-        cols = self.cols_with_role(role=RoleName.TARGET)
-        if len(cols) == 0:
-            return None
-        if len(cols) == 1:
-            return cols[0]
-        raise DatasetConfigError(f'Must have at most 1 target column, instead found {cols}')
+class Metadata():
+    '''Metadata.'''
+    _roles: Dict[RoleName, List[Column]]
+    _pos_labels: Dict[RoleName, Any]
+    _task: Optional[TaskType]
+    _data_type: Optional[DataType]
+    _problem_def: Optional[ProblemDefInterface]
+
+    def __init__(self,
+                 problem_def: Optional[ProblemDefInterface] = None,
+                 roles: Optional[Dict[RoleName, List[Column]]] = None,
+                 pos_labels: Optional[Dict[RoleName, Any]] = None,
+                 task: Optional[TaskType] = None,
+                 data_type: Optional[DataType] = None) -> None:
+        self._problem_def = problem_def
+        self._roles = roles or {}
+        self._pos_labels = pos_labels or {}
+        if problem_def is None:
+            self._task = task
+            self._data_type = data_type
+        else:
+            self._task = task or problem_def.task.task_type
+            self._data_type = data_type or problem_def.task.data_type
+
+    def get_conf(self, config_name: str) -> ConfigComponent:
+        '''Get a plugin conf ConfigComponent'''
+        assert self._problem_def is not None, 'BUG: _problem_def should be resolved in __init__().'
+        return self._problem_def.get_conf(config_name=config_name)
 
     @property
     def roles(self) -> Dict[RoleName, List[Column]]:
-        '''Full mapping of roles to lists of columns.'''
-        return self._roles
+        '''roles maps role names to lists of columns with that role.'''
+        return self._roles.copy()
 
     @property
-    def index_cols(self) -> List[Column]:
-        '''Column(s) containing indices for rows.'''
-        return self.cols_with_role(role=RoleName.INDEX)
+    def task(self) -> Optional[TaskType]:
+        '''Data science task that is being approached with this dataset.'''
+        return self._task
 
     @property
-    def train_fraction(self) -> float:
-        '''Config for the fraction of data to use for train.'''
-        return self._get_with_default(
-            ProblemDefKeys.SPLIT, ProblemDefKeys.TRAIN_FRAC, dflt=Defaults.SPLIT_FRACTION)
-
-    def pos_label(self, role: RoleName) -> Optional[Any]:
-        '''If this is a binary classification problem, return the positive label; otherwise None.'''
-        return self._pos_labels[role]
+    def data_type(self) -> Optional[DataType]:
+        '''Type of data contained in this dataset (image, tabular, etc)'''
+        return self._data_type
 
     @property
-    def forecasting(self) -> Optional[Dict[str, Any]]:
-        '''Forecasting metadata'''
-        retval = self._forecasting_metadata
-        if not retval:
+    def target(self) -> Optional[Column]:
+        '''Get name and index of target column if it exists.'''
+        if RoleName.TARGET not in self._roles or len(self._roles[RoleName.TARGET]) == 0:
             return None
-        return retval
+        assert len(self._roles[RoleName.TARGET]) <= 1, 'Must have at most 1 target column'
+        return self._roles[RoleName.TARGET][0]
 
     @property
-    def metadata(self) -> Metadata:
-        '''The metadata needed by models.'''
-        task = None
+    def pos_labels(self) -> Dict[RoleName, Any]:
+        '''maps role names to a positive value for columns with that role'''
+        return self._pos_labels.copy()
+
+    def override_roles(self, roles=Dict[RoleName, List[Column]]) -> 'Metadata':
+        '''Return a copy of metadata with new roles.'''
+        other = copy.deepcopy(self)
+        other._roles = roles  # pylint: disable=protected-access
+        return other
 
-        if self._task is not None:
-            task = self._task.task_type
-
-        return Metadata(roles=self._roles, pos_labels=self._pos_labels, task=task,
-                        forecasting=self._forecasting_metadata)
-
-    @abc.abstractmethod
-    def load_train(self) -> Dataset:
-        '''Load a Dataset from the information in the problem description'''
+    @property
+    def problem_def(self) -> Optional[ProblemDefInterface]:
+        '''Get the problem definition object'''
+        return self._problem_def
 
-    @abc.abstractmethod
-    def load_test(self) -> Optional[Dataset]:
-        '''Load test data if it exists, otherwise None'''
 
-    @abc.abstractmethod
-    def dataset(self, data: Any, **kwargs) -> Dataset:
-        '''Load a Dataset object, by placing data at supplied key.'''
+class Dataset(Dict[str, Any]):
+    '''Holds a dataset.
+    Allows for arbitrary keys and values as long as the keys are strings.
+
+    Standard keys: covariates, target, dataframe
+    '''
+    _metadata: Metadata
 
+    def __init__(self,
+                 *args,
+                 metadata: Optional[Metadata] = None,
+                 **kwargs):
+        super().__init__(*args, **kwargs)
+        if metadata is None:
+            metadata = Metadata(roles={}, pos_labels={})
+        self._metadata = metadata
 
-class D3MDatasetConfig(DatasetConfig):
-    '''Holds information about a local D3M formatted dataset.'''
+    @property
+    def roles(self) -> Dict[RoleName, List[Column]]:
+        '''Information about column roles in the dataset'''
+        return self._metadata.roles
 
-    def load_train(self) -> Dataset:
-        raise NotImplementedError
+    @property
+    def metadata(self) -> Metadata:
+        '''Config metadata for use by models'''
+        return self._metadata
 
-    def load_test(self) -> Optional[Dataset]:
-        '''Load test data if it exists, otherwise None'''
-        raise NotImplementedError
+    @property
+    def dataframe(self) -> pd.DataFrame:
+        '''Return the dataframe at DatasetKeys.DATAFRAME, or raise an error if it doesn't exist.'''
 
-    def dataset(self, data: Any, **kwargs) -> Dataset:
-        raise NotImplementedError
+        if DatasetKeys.DATAFRAME.value not in self:
+            if DatasetKeys.ERROR.value in self:
+                raise DatasetKeyError(
+                    f'Attempting to extract key "{DatasetKeys.DATAFRAME.value}" '
+                    f'as input, instead found keys {list(self.keys())}. '
+                    f'Error: {self[DatasetKeys.ERROR.value]}')
+            raise DatasetKeyError(
+                f'Attempting to extract key "{DatasetKeys.DATAFRAME.value}" '
+                f'as input, instead found keys {list(self.keys())}.')
+        df_value = self[DatasetKeys.DATAFRAME.value]
+        if not isinstance(df_value, pd.DataFrame):
+            raise DatasetValueError(
+                f'Input key key {DatasetKeys.DATAFRAME.value} must point to '
+                f'a pandas.DataFrame, instead found a {type(df_value)}: '
+                f'{df_value}')
+        return pd.DataFrame(df_value)
+
+    @dataframe.setter
+    def dataframe(self, data: pd.DataFrame) -> None:
+        self[DatasetKeys.DATAFRAME.value] = data
 
+    @property
+    def ground_truth(self) -> pd.DataFrame:
+        '''Return the dataframe at DatasetKeys.GROUND_TRUTH
 
-class TensorFlowDatasetConfig(DatasetConfig):
-    '''Holds information about a local TensorFlow dataset.'''
+        or raise an error if it doesn't exist.'''
 
-    def load_train(self) -> Dataset:
-        raise NotImplementedError
+        if DatasetKeys.GROUND_TRUTH.value not in self:
+            if DatasetKeys.ERROR.value in self:
+                raise DatasetKeyError(
+                    f'Attempting to extract key "{DatasetKeys.GROUND_TRUTH.value}" '
+                    f'as input, instead found keys {list(self.keys())}. '
+                    f'Error: {self[DatasetKeys.ERROR.value]}')
+            raise DatasetKeyError(
+                f'Attempting to extract key "{DatasetKeys.GROUND_TRUTH.value}" '
+                f'as input, instead found keys {list(self.keys())}.')
+        df_value = self[DatasetKeys.GROUND_TRUTH.value]
+        if not isinstance(df_value, pd.DataFrame):
+            raise DatasetValueError(
+                f'Input key key {DatasetKeys.GROUND_TRUTH.value} must point to '
+                f'a pandas.DataFrame, instead found a {type(df_value)}: '
+                f'{df_value}')
+        return pd.DataFrame(df_value)
+
+    @ground_truth.setter
+    def ground_truth(self, data: pd.DataFrame) -> None:
+        self[DatasetKeys.GROUND_TRUTH.value] = data
 
-    def load_test(self) -> Optional[Dataset]:
-        '''Load test data if it exists, otherwise None'''
-        raise NotImplementedError
+    @property
+    def predictions(self) -> pd.DataFrame:
+        '''Return the dataframe at DatasetKeys.PREDICTIONS
+        or raise an error if it doesn't exist.'''
+
+        if DatasetKeys.PREDICTIONS.value not in self:
+            if DatasetKeys.ERROR.value in self:
+                raise DatasetKeyError(
+                    f'Attempting to extract key "{DatasetKeys.PREDICTIONS.value}" '
+                    f'as input, instead found keys {list(self.keys())}. '
+                    f'Error: {self[DatasetKeys.ERROR.value]}')
+            raise DatasetKeyError(
+                f'Attempting to extract key "{DatasetKeys.PREDICTIONS.value}" '
+                f'as input, instead found keys {list(self.keys())}.')
+        df_value = self[DatasetKeys.PREDICTIONS.value]
+        if not isinstance(df_value, pd.DataFrame):
+            raise DatasetValueError(
+                f'Input key key {DatasetKeys.PREDICTIONS.value} must point to '
+                f'a pandas.DataFrame, instead found a {type(df_value)}: '
+                f'{df_value}')
+        return pd.DataFrame(df_value)
+
+    @predictions.setter
+    def predictions(self, data: pd.DataFrame) -> None:
+        self[DatasetKeys.PREDICTIONS.value] = data
 
-    def dataset(self, data: Any, **kwargs) -> Dataset:
-        raise NotImplementedError
+    @property
+    def probabilities(self) -> pd.DataFrame:
+        '''
+        Return the dataframe at `DatasetKeys.PROBABILITIES`
+        or raise an error if it doesn't exist.
+        '''
 
+        if DatasetKeys.PROBABILITIES.value not in self:
+            if DatasetKeys.ERROR.value in self:
+                raise DatasetKeyError(
+                    f'Attempting to extract key "{DatasetKeys.PROBABILITIES.value}" '
+                    f'as input, instead found keys {list(self.keys())}. '
+                    f'Error: {self[DatasetKeys.ERROR.value]}')
+            raise DatasetKeyError(
+                f'Attempting to extract key "{DatasetKeys.PROBABILITIES.value}" '
+                f'as input, instead found keys {list(self.keys())}.'
+            )
+
+        df_value = self[DatasetKeys.PROBABILITIES.value]
+
+        if not isinstance(df_value, pd.DataFrame):
+            raise DatasetValueError(
+                f'Input key key {DatasetKeys.PROBABILITIES.value} must point to '
+                f'a pandas.DataFrame, instead found a {type(df_value)}: '
+                f'{df_value}'
+            )
+
+        return pd.DataFrame(df_value)
+
+    @probabilities.setter
+    def probabilities(self, data: pd.DataFrame) -> None:
+        self[DatasetKeys.PROBABILITIES.value] = data
 
-class CloudDatasetConfig(DatasetConfig):
-    '''Holds information about a tabular dataset stored in the cloud.'''
+    def output(self, override_metadata: Optional[Metadata] = None) -> 'Dataset':
+        '''Return a new dataset containing same metadata and nothing else.
 
-    def load_train(self) -> Dataset:
-        raise NotImplementedError
+        Metadata can also be overriden, all preexisting metadata will be lost.
+        Generally called to create a new dataset to fill with a model's output.
+        '''
+        return self.__class__(metadata=override_metadata or self._metadata)
 
-    def load_test(self) -> Optional[Dataset]:
-        '''Load test data if it exists, otherwise None'''
-        raise NotImplementedError
+    def get_dataframe(self) -> pd.DataFrame:
+        '''Return the dataframe at DatasetKeys.DATAFRAME, or raise an error if it doesn't exist.'''
 
-    def dataset(self, data: Any, **kwargs) -> Dataset:
-        raise NotImplementedError
+        return self.dataframe
```

### Comparing `ngautonml-0.4.1b1/ngautonml/dataset_formats/local.py` & `ngautonml-0.4.1b2/ngautonml/data_loaders/local_data_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,144 @@
-'''Holds information about a local tabular dataset.'''
-import logging
-from pathlib import Path
-from typing import Optional, Dict, Any, List, Union
+'''Loads a local file as a pandas DataFrame.'''
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+import logging
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Union
+
 import pandas as pd
 from scipy.io.arff import loadarff  # type: ignore[import]
 
-from .impl.dataframe_dataset_config import DataframeDatasetConfig
-from .impl.dataset_config import DatasetFileError
-from .impl.dataset_format_catalog import DatasetFormat, DatasetFormatCatalog
-from ..problem_def.task import Task, TaskType
-from ..wrangler.constants import ProblemDefKeys, FileType
-from ..wrangler.dataset import Dataset, DatasetKeys, RoleName
-
+from ..config_components.dataset_config import DatasetConfig
+from ..wrangler.constants import FileType
+from ..wrangler.dataset import Dataset, DatasetKeys, RoleName, TaskType
+from ..wrangler.logger import Logger
+from .impl.dataframe_loader import DataframeLoader, DatasetFileError
+from .impl.data_loader_catalog import DataLoaderCatalog
+
+logger = Logger(__file__, logging.DEBUG).logger()
+
+
+class LocalDataLoader(DataframeLoader):
+    '''Loads a local file as a pandas DataFrame.'''
+
+    name: str = 'local'
+    tags: Dict[str, List[str]] = {
+        'input_format': ['csv', 'arff', 'tabular_file'],
+        'loaded_format': ['pandas_dataframe'],
+    }
 
-class LocalDatasetConfig(DataframeDatasetConfig):
-    '''Holds information about a local tabular dataset.'''
-    _ext: Optional[str] = None
-    _train_path: Optional[Path] = None
+    _train_path: Path
     _test_path: Optional[Path] = None
-    _static_path: Optional[Path] = None
+    _ext: str
 
-    def __init__(self,
-                 clause: Dict[str, Any],
-                 parents: Optional[List[str]] = None,
-                 task: Optional[Task] = None,
-                 **unused_kwargs):
-        super().__init__(clause=clause, parents=parents, task=task)
-
-        # This may throw errors, which will caught by ProblemDefinition
-        # possible error states:
-        # train path key doesn't exist
-        # train path does not point to a csv
-        # column roles key does not point to a dictionary
-        # any of the roles have invalid names
-        # any of the roles do not point to a dictionary
-        # any of the roles have an invalid col name xor an invalid col id
-
-        train_path: Path = Path(self._get(ProblemDefKeys.TRAIN_PATH.value))
-        train_path = train_path.expanduser().resolve()
+    def __init__(self, config: DatasetConfig):
+        train_path: Path = Path(config.params[config.Keys.TRAIN_PATH.value])
+        self._train_path = train_path.expanduser().resolve()
         ext: str = train_path.suffix[1:]
 
         if ext not in FileType.list():
             raise DatasetFileError(
                 f'Train path from the problem definition ({train_path})'
                 f' does not point to a file with one of these extensions: {FileType.list()}'
             )
 
         self._ext = ext
 
-        try:
-            train_cols = self._load_dataframe(train_path)
-            assert train_cols is not None
-            self._train_cols = train_cols
-        except FileNotFoundError as exc:
-            raise DatasetFileError(f'train_path: "{train_path}" not found') from exc
-        self._train_path = train_path
-
-        if ProblemDefKeys.TEST_PATH.value in clause:
-            test_path = Path(self._get(ProblemDefKeys.TEST_PATH)).expanduser().resolve()
+        if config.Keys.TEST_PATH.value in config.params:
+            test_path = Path(config.params[config.Keys.TEST_PATH.value])
+            test_path = test_path.expanduser().resolve()
             test_ext = test_path.suffix[1:]
             if test_ext != ext:
                 raise DatasetFileError(
                     f'test data: "{test_path}" is not same file type as train data'
                     f'(Expected: .{ext})')
 
             self._test_path = test_path
 
-        if ProblemDefKeys.STATIC_EXOGENOUS_PATH.value in clause:
+        self._static_path = None
+        if config.Keys.STATIC_EXOGENOUS_PATH.value in config.params:
             static_path = Path(
-                self._get(
-                    ProblemDefKeys.STATIC_EXOGENOUS_PATH)).expanduser().resolve()
+                config.params[config.Keys.STATIC_EXOGENOUS_PATH.value]).expanduser().resolve()
             static_ext = static_path.suffix[1:]
             if static_ext != ext:
                 raise DatasetFileError(
                     f'static data: "{static_path}" is not same file type as train data'
                     f'(Expected: .{ext})')
 
             self._static_path = static_path
 
-        self._read_roles()
-
-    def _load_dataframe(self, path: Path) -> Optional[pd.DataFrame]:
-        '''Load the file at path based on self._ext'''
-        retval = None
-
-        if self._ext == FileType.CSV.value:
-            retval = pd.read_csv(path)
-        elif self._ext == FileType.ARFF.value:
-            raw_data = loadarff(path)
-            retval = pd.DataFrame(raw_data[0])
-
-        if retval is None:
-            return None
-        return self._drop_unnamed_cols(retval)
+        super().__init__(config=config)
 
     def _drop_unnamed_cols(self, dataframe: pd.DataFrame) -> pd.DataFrame:
-        '''There are a few potential ways to do this.
+        '''Deal with pandas CSV loader loading the index as an unnamed column.
+
+        There are a few potential ways to do this.
         We choose to drop all cols called 'Unnamed: [int of any length]',
         as those were likely unnamed in the actual csv.'''
         # TODO(Merritt): warn user if we encounter this under certain circumstances
         # (for ex: not in first column
         # or the col is literally named 'Unnamed: [num]' in the csv)
         drop_cols = dataframe.filter(regex=r'^Unnamed: \d+$').columns
         retval = dataframe.drop(labels=drop_cols, axis=1)
         return retval
 
-    def _load_dataset(self, path: Path, path_type: str) -> Dataset:
-        retval = Dataset(metadata=self.metadata)
-        # TODO(Mujing/Merritt): move this try/except statement into _load_dataframe()
+    def _load_dataframe(self, path: Path) -> pd.DataFrame:
+        '''Load the file at path based on self._ext'''
+        retval = None
+
         try:
-            data = self._load_dataframe(path=path)
+            if self._ext == FileType.CSV.value:
+                retval = pd.read_csv(path)
+            elif self._ext == FileType.ARFF.value:
+                raw_data = loadarff(path)
+                retval = pd.DataFrame(raw_data[0])
         except FileNotFoundError as exc:
-            raise DatasetFileError(f'{path_type}_path: "{path}" not found') from exc
+            raise DatasetFileError(f'Unable to load file from "{path}".') from exc
 
-        if data is None:
+        if retval is None:
             raise DatasetFileError(f'Unsupported file type: {path}')
 
+        return self._drop_unnamed_cols(retval)
+
+    def _load_dataset(self, path: Path) -> Dataset:
+        '''Load a Dataset into a DataFrame from the provided Path'''
+        retval = Dataset(metadata=self._metadata)
+
+        data = self._load_dataframe(path=path)
+
         retval.dataframe = data
 
         # if this is a forecasting problem, load static exogenous data or create an empty key for it
-        if self._task and self._task.task_type == TaskType.FORECASTING:
+        # TODO(Piggy/Merritt): replace this with something that can be used by both memory and local
+        # to load additional data requested by a plugin
+        if self._metadata.task == TaskType.FORECASTING:
             if self._static_path is None:
                 retval[DatasetKeys.STATIC_EXOGENOUS.value] = None
-                logging.debug('Forecasting problem has no static exogenous table.')
+                logger.debug('Forecasting problem has no static exogenous table.')
             else:
-                try:
-                    static = self._load_dataframe(self._static_path)
-                except FileNotFoundError as exc:
-                    raise DatasetFileError(
-                        f'static_path "{self._static_path}" not found. '
-                        'This error should only appear in forecasting problems.') from exc
+                static = self._load_dataframe(self._static_path)
                 retval[DatasetKeys.STATIC_EXOGENOUS.value] = static
-            assert DatasetKeys.STATIC_EXOGENOUS.value in retval, (
-                'BUG: forecasting problem but no "static_exogenous" data')
 
         return retval
 
-    def load_train(self) -> Dataset:
-        assert self._train_path is not None, 'BUG: load() called when train_path is None'
+    def _load_train(self) -> Dataset:
         return self._load_dataset(
-            path=self._train_path,
-            path_type='train')
+            path=self._train_path)
 
-    def load_test(self) -> Optional[Dataset]:
+    def _load_test(self) -> Optional[Dataset]:
         if self._test_path is None:
             return None
 
         retval = self._load_dataset(
-            path=self._test_path,
-            path_type='test')
+            path=self._test_path)
 
-        return self._prune_target(retval)
+        return retval
 
     def dataset(self,
                 data: Any,
                 key: Union[DatasetKeys, str] = DatasetKeys.DATAFRAME,
                 cols: Optional[List[str]] = None,
                 roles: Optional[List[Union[RoleName, str]]] = None,
                 **kwargs) -> Dataset:
@@ -180,17 +160,10 @@
         if isinstance(data, (Path, str)):
             path = Path(data)
             data = self._load_dataframe(path=path)
 
         return super().dataset(data, key=key, cols=cols, roles=roles, **kwargs)
 
 
-class LocalDatasetFormat(DatasetFormat):
-    '''Used to load a local tabular dataset.'''
-    _builder = LocalDatasetConfig
-    _name = 'local'
-    _tags = {}
-
-
-def register(catalog: DatasetFormatCatalog, *args, **kwargs):
+def register(catalog: DataLoaderCatalog):
     '''Register all the objects in this file.'''
-    catalog.register(LocalDatasetFormat(*args, **kwargs))
+    catalog.register(LocalDataLoader)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/dataset_formats/memory_test.py` & `ngautonml-0.4.1b2/ngautonml/data_loaders/local_data_loader_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,178 @@
-""" Tests for MemoryDatasetConfig """
-from typing import Dict, Any
+'''Tests for local_data_loader.py'''
+from pathlib import Path
+from typing import Any, Dict, Optional
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import pandas as pd
 
-from .memory import MemoryDatasetConfig
-from ..problem_def.task import Task, TaskType
-from ..wrangler.dataset import RoleName
+from ..config_components.dataset_config import DatasetConfig
+from ..problem_def.problem_def import ProblemDefinition
+from ..problem_def.task import TaskType
+from ..wrangler.dataset import DatasetKeys, RoleName
+from .local_data_loader import LocalDataLoader
 
-# pylint: disable=missing-function-docstring
-
-CLAUSE = {
-    'config': 'memory',
-    'column_roles': {
-        'target': {
-            'name': 'a',
-            'pos_label': 1
-        }
-    }
-}
-TRAIN_DF = pd.DataFrame({'a': [1, 2], 'b': [3, 4]})
-
-
-def test_sunny_day():
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, clause=CLAUSE)
-    dut.validate()
-    result = dut.load_train()
-    got_train_df = result.dataframe
-
-    assert got_train_df.shape == (2, 2)
-    assert RoleName.TARGET in result.metadata.roles.keys()
-    assert len(result.metadata.roles[RoleName.TARGET]) == 1
-    assert result.metadata.roles[RoleName.TARGET][0].name == 'a'
 
+# pylint: disable=missing-function-docstring
 
-def test_attribute_role_default():
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, clause=CLAUSE)
-    dut.validate()
-    result = dut.cols_with_role(role=RoleName.ATTRIBUTE)
 
-    assert 1 == len(result)
-    assert result[0].name == 'b'
+def valid_data_path(filename: Optional[str] = None) -> str:
+    '''Returns a path (in the form of a string) to a valid csv file.'''
+    module_parent = Path(__file__).parents[2]
+    if filename is None:
+        filename = 'credit.csv'
+    path = module_parent / 'examples' / 'classification' / filename
+    return str(path)
 
 
-def test_no_target():
-    clause_without_target = {
-        'config': 'memory',
-        'column_roles': {}
+def make_dataset(train_path: str) -> Dict[str, Any]:
+    retval = {
+        'config': 'local',
+        'train_path': train_path,
+        'column_roles': {
+            'target': {
+                'name': 'class',
+                'pos_label': 'good'
+            }
+        },
     }
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, clause=clause_without_target)
-    dut.validate()
+    return retval
 
-    assert dut.target is None
 
+def test_load_simple_dataset() -> None:
+    clause = make_dataset(valid_data_path())
+    config = DatasetConfig(clause=clause)
+    dut = LocalDataLoader(config=config)
+    result = dut.load_train()
 
-def test_load_testdata() -> None:
-    test_df = pd.DataFrame({'a': [1, 2, 2], 'b': [30, 40, 500]})
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, clause=CLAUSE, test_df=test_df)
-    dut.validate()
-    result = dut.load_test()
-
-    assert result is not None   # needed to make pylint happy
-    got_test_df = result.dataframe
-
-    assert got_test_df.shape == (3, 1)
-    assert 'a' not in got_test_df.columns
-    assert 'b' in got_test_df.columns
-
-
-def test_load_nonexistent_testdata() -> None:
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, clause=CLAUSE)
-    dut.validate()
-    result = dut.load_test()
-
-    assert result is None
+    assert result is not None
+    train_df = result.dataframe
+    assert train_df.shape == (1000, 21)
+    assert train_df.columns[0] == 'checking_status'
+    assert train_df.columns[20] == 'class'
 
 
-FORECASTING_CLAUSE: Dict[str, Any] = {
-    'config': 'memory',
-    'column_roles': {
-        'target': {
-            'name': 'a'
+def test_no_target() -> None:
+    clause = {
+        'config': 'local',
+        'train_path': valid_data_path(),
+        'column_roles': {
+            'index': {
+                'id': 0
+            }
         }
-    },
-    'forecasting': {
-        'horizon': 1,
-        'input_size': 1,
-        'frequency': 'M'
     }
-}
+    config = DatasetConfig(clause=clause)
+    dut = LocalDataLoader(config=config)
+    dataset = dut.load_train()
+    assert dataset is not None
+    assert dataset.metadata.target is None
 
 
-FORECASTING_TASK_CLAUSE = {
-    'task': 'forecasting'
-}
-
-
-def test_load_testdata_forecasting() -> None:
-    """check that we don't drop the target column for forecasting test data"""
-    forecasting_clause = FORECASTING_CLAUSE.copy()
-    test_df = pd.DataFrame({'a': [1], 'b': [30]})
-
-    dut = MemoryDatasetConfig(
-        train_df=TRAIN_DF,
-        clause=forecasting_clause,
-        test_df=test_df,
-        task=Task(clause=FORECASTING_TASK_CLAUSE))
-    dut.validate()
-    test_data = dut.load_test()
-
-    assert test_data is not None
-    assert 'a' in test_data.dataframe.columns
-
-
-def test_forecasting_metadata() -> None:
-    forecasting_clause = {
-        'config': 'memory',
+def test_arff() -> None:
+    clause = {
+        'config': 'local',
+        'train_path': valid_data_path(filename='dataset_31_credit-g.arff'),
         'column_roles': {
             'target': {
-                'name': 'a'
+                'name': 'class'
             }
-        },
-        'forecasting': {
-            'horizon': 1,
-            'input_size': 3,
-            'frequency': 'M'
         }
     }
-    custom_train_df = pd.DataFrame({'a': [1, 2, 1, 2, 1], 'b': [3, 4, 5, 6, 7]})
+    config = DatasetConfig(clause=clause)
+    dut = LocalDataLoader(config=config)
+    got = dut.load_train()
+    assert got is not None
+    target = got.metadata.target
+    assert target is not None
+    assert 'class' == target.name
+
+    assert DatasetKeys.DATAFRAME.value in got
+
+    train_df = got.dataframe
+    assert isinstance(train_df, pd.DataFrame)
+    assert train_df.shape == (1000, 21)
+
+
+def test_load_test() -> None:
+    clause = {
+        'config': 'simple',
+        'train_path': valid_data_path(filename='credit-train.csv'),
+        'test_path': valid_data_path(filename='credit-test.csv'),
+        'column_roles': {
+            'target': {
+                'name': 'class'
+            }
+        },
+    }
+    config = DatasetConfig(clause=clause)
+    dut = LocalDataLoader(config=config)
+    result = dut.load_test()
+    assert result is not None
+    test_df = result.dataframe
+    assert test_df.shape == (200, 20)
+    assert 'class' not in test_df.columns
+    assert 'own_telephone' in test_df.columns
 
-    dut = MemoryDatasetConfig(
-        train_df=custom_train_df,
-        clause=forecasting_clause,
-        task=Task(clause=FORECASTING_TASK_CLAUSE))
-    dut.validate()
-    train_data = dut.load_train()
-
-    assert train_data.metadata.horizon == 1
-    assert train_data.metadata.input_size == 3
-    assert train_data.metadata.frequency == 'M'
-    assert train_data.metadata.step_size == 1
+
+def test_load_nonexistent_testdata() -> None:
+    '''If there is no test data, load_test() returns None'''
+    clause = make_dataset(valid_data_path())
+    config = DatasetConfig(clause=clause)
+    dut = LocalDataLoader(config=config)
+    result = dut.load_test()
+    assert result is None
 
 
 CLASSIFICATION_TASK_CLAUSE = {
-    'task': 'binary_classification'
+    'problem_type': {
+        'task': 'binary_classification'
+    },
+    'dataset': {
+        'config': 'ignore'
+    }
 }
 
 
 def test_task_in_metadata_with_load_train() -> None:
-    clause = CLAUSE.copy()
-    task = Task(clause=CLASSIFICATION_TASK_CLAUSE)
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, clause=clause, task=task)
-    dut.validate()
+    clause = make_dataset(valid_data_path())
+    problem_def_for_task = ProblemDefinition(CLASSIFICATION_TASK_CLAUSE)
+    config = DatasetConfig(clause=clause, problem_def=problem_def_for_task)
+    dut = LocalDataLoader(config=config)
     result = dut.load_train()
 
+    assert result is not None
     assert result.metadata.task == TaskType.BINARY_CLASSIFICATION
 
 
 def test_task_in_metadata_with_load_test() -> None:
-    clause = CLAUSE.copy()
-    test_df = pd.DataFrame({'a': [1], 'b': [30]})
-    task = Task(clause=CLASSIFICATION_TASK_CLAUSE)
-    dut = MemoryDatasetConfig(train_df=TRAIN_DF, test_df=test_df,
-                              clause=clause, task=task)
-    dut.validate()
+    clause = {
+        'config': 'local',
+        'train_path': valid_data_path(filename='credit-train.csv'),
+        'test_path': valid_data_path(filename='credit-test.csv'),
+        'column_roles': {
+            'target': {
+                'name': 'class'
+            }
+        },
+    }
+    problem_def_for_task = ProblemDefinition(CLASSIFICATION_TASK_CLAUSE)
+    config = DatasetConfig(clause=clause, problem_def=problem_def_for_task)
+    dut = LocalDataLoader(config=config)
     result = dut.load_test()
 
     assert result is not None
     assert result.metadata.task == TaskType.BINARY_CLASSIFICATION
+
+
+def test_load_arbitrary_csv() -> None:
+    clause = make_dataset(valid_data_path(filename='credit-train.csv'))
+    config = DatasetConfig(clause=clause)
+    dut = LocalDataLoader(config=config)
+
+    got = dut.dataset(data=valid_data_path(filename='credit-test.csv'),
+                      cols=['class', 'own_telephone'])
+    assert got.dataframe.shape == (200, 2)
+    assert set(got.dataframe.columns) == {'class', 'own_telephone'}
+    assert got.metadata.roles[RoleName.TARGET][0].name == 'class'
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/cucumber.py` & `ngautonml-0.4.1b2/ngautonml/executor/cucumber.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/cucumber_test.py` & `ngautonml-0.4.1b2/ngautonml/executor/cucumber_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/executor.py` & `ngautonml-0.4.1b2/ngautonml/executor/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''Executes executable pipelines and returns results'''
 import abc
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from .cucumber import JarOfCucumbers
 from .executor_kind import ExecutorKind
 from ..generator.designator import Designator
@@ -32,15 +32,15 @@
     @property
     def kind(self) -> ExecutorKind:
         '''Documents the kind of ExecutablePipeline we need.'''
         return self._kind
 
     @abc.abstractmethod
     def fit(self,
-            dataset: Dataset,
+            dataset: Optional[Dataset],
             pipelines: Dict[Designator, ExecutablePipeline]
             ) -> TrainedPipelineCollection:
         '''Train a list of pipelines on a dataset.'''
 
     @abc.abstractmethod
     def predict(self,
                 dataset: Dataset,
@@ -50,15 +50,15 @@
 
 
 class ExecutorStub(Executor):
     '''stub'''
     _kind = ExecutorKind('stub_executor_kind')
 
     def fit(self,
-            dataset: Dataset,
+            dataset: Optional[Dataset],
             pipelines: Dict[Designator, ExecutablePipeline]
             ) -> TrainedPipelineCollection:
         '''Train a list of pipelines on a dataset.'''
         return TrainedPipelineCollection()
 
     def predict(self,
                 dataset: Dataset,
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/executor_kind.py` & `ngautonml-0.4.1b2/ngautonml/executor/executor_kind.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_pipeline.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,44 +47,60 @@
         for step in self._steps:
             step.set_trained()
 
     def set_fit_error(self, err: FitError) -> None:
         '''Set this pipeline as throwing an error at fit time'''
         self._fit_error = err
 
-    def fit(self, dataset: Dataset) -> JarOfCucumbers:
+    def fit(self, dataset: Optional[Dataset]) -> JarOfCucumbers:
         '''Fit models to dataset.
 
         Args:
             dataset: The training dataset.
 
         Returns:
             A JarOfCucumbers
             (mapping from step designators to cucumbers for each step).
         '''
         # Pipelines set themselves as trained first, so that they are
         #   marked trained even if they throw an exception along the way
         self._trained = True
 
+        # If dataset is None, just call fit(None) on all the steps.
+        # This allows distributed pipelines to fit themselves with
+        # neighbor data.
+        result = None
         inp = dataset
         for step in self._steps:
             step.fit(dataset=inp)
-            result = step.predict(dataset=inp)
+            if inp is not None:
+                result = step.predict(dataset=inp)
             inp = result
-        return self.cucumberize_all()
+        if inp is not None:
+            return self.cucumberize_all()
+        return JarOfCucumbers()
 
-    def predict(self, dataset: Dataset) -> PipelineResult:
+    def predict(self, dataset: Optional[Dataset]) -> PipelineResult:
         '''Run prediction for a complete pipeline.'''
         if not self._trained:
             raise UntrainedError(f'pipeline "{self.name}" needs to be fit before it can predict')
-        inp = dataset.output()
+        if dataset is None:
+            inp = None
+        else:
+            inp = dataset.output()
         if self._fit_error is not None:
-            inp[DatasetKeys.ERROR.value] = self._fit_error
+            if inp is None:
+                inp = Dataset(metadata=None, **{DatasetKeys.ERROR.value: self._fit_error})
+            else:
+                inp[DatasetKeys.ERROR.value] = self._fit_error
         else:
-            inp.update(dataset)
+            if inp is not None and dataset is not None:
+                inp.update(dataset)
+            else:
+                inp = dataset
             for step in self._steps:
                 result = step.predict(dataset=inp)
                 inp = result
         return PipelineResult(executable_pipeline=self, prediction=inp)
 
     def cucumberize_all(self, parent_designator: Optional[Designator] = None) -> JarOfCucumbers:
         '''Cucumberize all steps that hold algorithms, and return the result.
@@ -100,9 +116,18 @@
                 f'pipeline "{self.name}" needs to be fit before it can cucumberize_all')
 
         models = JarOfCucumbers()
         for step in self._steps:
             models.update(
                 step.cucumberize_all(
                     parent_designator or self.designator))
-
         return models
+
+    def start(self) -> None:
+        '''Start the pipeline.'''
+        for step in self._steps:
+            step.start()
+
+    def stop(self) -> None:
+        '''Stop the pipeline.'''
+        for step in self._steps:
+            step.stop()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_pipeline_test.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_pipeline_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,20 +49,23 @@
         self._training_data = pickle.loads(serialized_model)
         return self
 
     def serialize(self) -> bytes:
         '''Return a serialized version of a trained model.'''
         return pickle.dumps(self._training_data, pickle.HIGHEST_PROTOCOL)
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         '''Fit a model based on train data.'''
-        self._training_data = Dataset(dataset.copy())
+        if dataset is not None:
+            self._training_data = Dataset(dataset.copy())
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         retval = dataset.output()
         retval.update(dataset)
         retval.update(self._hyperparams)
         return retval
 
 
 REFERENCE_DATASET = Dataset(
@@ -119,14 +122,15 @@
     # Connector will rename a key, FakeFitter will add a new key and value
     got_predict = dut.predict(dataset=REFERENCE_DATASET)
     want_predict = {
         'a_key_renamed': 'a_value',
         'another_key': 'another_value',
         'new_key': 'new_value'
     }
+    assert got_predict.prediction is not None
     assert set(got_predict.prediction.keys()) == set(want_predict.keys())
     assert set(got_predict.prediction.values()) == set(want_predict.values())
 
 
 def test_fit_must_precede_predict() -> None:
     pipe = BoundPipeline(name=Designator('foo'), tags={})
     fitter = FakeFitter()
@@ -166,15 +170,17 @@
 
     def __init__(self, parent: Algorithm, **hyperparams):
         super().__init__(parent)
         if 'random_seed' in hyperparams:
             # TODO(piggy): use generator instead of setting globally to avoid flakiness
             np.random.seed([hyperparams['random_seed']])
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         retval = dataset.output()
         retval['result'] = np.random.randint(0, 10, 5)
         return retval
 
 
 class RandomAlgorithm(Algorithm):
     def instantiate(self, **hyperparams) -> RandomAlgorithmInstance:
@@ -186,8 +192,9 @@
     pipe.step(model=RandomAlgorithm(random_seed=1234))
     dut = SimpleExecutablePipeline(pipeline=pipe)
 
     dut.fit(Dataset())
     got = dut.predict(Dataset())
 
     # For seed == 1234
+    assert got.prediction is not None
     assert (got.prediction['result'] == [2, 1, 9, 4, 2]).all()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_step.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                  bound_step: PipelineStep,
                  model: Optional[Algorithm] = None):
         super().__init__(
             model=model or bound_step._model,
             **bound_step.hyperparams())
         model = self._model
         self._bound_step = bound_step
+        self._overrides = bound_step._overrides
         self._name = bound_step.opt_name
         self._serial_number = bound_step.serial_number
         self._init_model()
 
     def _init_model(self):
         '''Provide a customization point for model handling.
 
@@ -68,22 +69,21 @@
 
         The default fit method does nothing.
         '''
         assert self._model_instance is not None
         if isinstance(self._model_instance, FittableAlgorithmInstance):
             self._model_instance.fit(*args, **kwargs)
 
-    def predict(self, *args, **kwargs) -> Dataset:
+    def predict(self, *args, **kwargs) -> Optional[Dataset]:
         '''Apply model to input dataset to create output.
 
         This may require that the model is fit (self.trained == True) before it is called.
         '''
         assert self._model_instance is not None
-        result = self._model_instance.predict(*args, **kwargs)
-        return result
+        return self._model_instance.predict(*args, **kwargs)
 
     def cucumberize_all(self, pipeline_designator: Designator) -> JarOfCucumbers:
         '''Make this step into a Cucumber and put it in a JarOfCucumbers.
 
         Parallel steps will override this, but in the non-parallel case,
             this step only contains one algorithm and thus yields a jar of
             1 cucumber.
@@ -104,7 +104,17 @@
 
     @property
     def trained(self) -> bool:
         '''Has this model been trained?'''
         if isinstance(self._model_instance, FittableAlgorithmInstance):
             return self._model_instance.trained
         return True
+
+    def start(self) -> None:
+        '''Start the model.'''
+        assert self._model_instance is not None
+        self._model_instance.start()
+
+    def stop(self) -> None:
+        '''Stop the model.'''
+        assert self._model_instance is not None
+        self._model_instance.stop()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executable_step_test.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executable_step_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executor.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''The "simple" executor'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import logging
-from typing import Dict
+from typing import Dict, Optional
 import traceback
 
 from .simple_executable_pipeline import SimpleExecutablePipeline
 from ..executor import Executor, ExecutorKind, TrainedPipelineCollection
 from ...generator.designator import Designator
 from ...instantiator.executable_pipeline import (ExecutablePipeline, PipelineResult,
                                                  FitError, PredictError)
@@ -16,15 +16,15 @@
 
 
 class SimpleExecutor(Executor):
     '''A simple implementation of an Executor'''
     _kind = ExecutorKind('simple')
 
     def fit(self,
-            dataset: Dataset,
+            dataset: Optional[Dataset],
             pipelines: Dict[Designator, ExecutablePipeline]
             ) -> TrainedPipelineCollection:
         '''Train a list of pipelines on a dataset.'''
         retval = TrainedPipelineCollection()
         for des, pipe in pipelines.items():
             assert isinstance(pipe, SimpleExecutablePipeline)
             try:
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_executor_test.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_executor_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''Tests for the "simple" executor'''
 import re
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import logging
 import pytest
 import numpy as np
@@ -173,16 +173,18 @@
 
     dut.fit(dataset=train,
             pipelines={fake_des: executable})
 
     got_predict = dut.predict(dataset=test,
                               pipelines={fake_des: executable})
 
-    got_connector = list(got_predict.values())[0].prediction['connector']
-    got_regression = list(got_predict.values())[0].prediction['regression']
+    got_result = list(got_predict.values())[0]
+    assert got_result.prediction is not None
+    got_connector = got_result.prediction['connector']
+    got_regression = got_result.prediction['regression']
 
     assert set(got_connector.keys()) == set(['new_key'])
     assert got_connector['new_key'].iat[0, 0] == pytest.approx(0.07786338762689, 1e-6)
     assert set(got_regression.keys()) == set(['result'])
     assert got_regression['result'].iat[0, 0] == pytest.approx(225.9732401, 1e-6)
 
 
@@ -197,31 +199,31 @@
             return BrokenPredictAlgInstance(parent=self, **hyperparams)
         raise NotImplementedError(f'Unimplemented kind: {hyperparams["kind"]}')
 
 
 class BrokenFitAlgInstance(FittableAlgorithmInstance):
     _name = 'fit is broken'
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         _ = 1 / 0
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         return dataset
 
 
 class BrokenPredictAlgInstance(FittableAlgorithmInstance):
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         # we need this condition because the model's predict() gets called as part
         #   of the pipeline's fit() call, however we only want to raise an error
         #   on the pipeline's predict() call
-        if 'hamster' in dataset:
+        if 'hamster' in (dataset or {}):
             raise NotImplementedError('hamster')
         return dataset
 
 
 def test_fit_error(caplog: pytest.LogCaptureFixture) -> None:
     pipe = BoundPipeline(name=Designator('broken_fit'))
     pipe.step(model=BrokenAlg(name='fit is broken', kind='fit'))
@@ -252,14 +254,15 @@
     pipes: Dict[Designator, ExecutablePipeline] = {des: executable}
     dut.fit(dataset=Dataset(), pipelines=pipes)
     with caplog.at_level(logging.WARNING):
         got = dut.predict(
             dataset=Dataset({'hamster': 'something'}),
             pipelines=pipes)
     got_pipe = got[des].prediction
+    assert got_pipe is not None
     assert isinstance(got_pipe['error'], PredictError)
     assert 'simple_executor_test.py' in str(got_pipe['error'])
     assert 'NotImplementedError' in str(got_pipe['error'])
     assert 'hamster' in str(got_pipe['error'])
     assert 'hamster' in caplog.text
     assert 'broken_predict' in caplog.text
 
@@ -279,10 +282,11 @@
     dut.fit(dataset=Dataset(),
             pipelines=pipes)
 
     got = dut.predict(dataset=Dataset(),
                       pipelines=pipes)
 
     got_pipe = got[des].prediction
+    assert got_pipe is not None
     assert isinstance(got_pipe['error'], FitError)
     assert 'simple_executor_test.py' in str(got_pipe['error'])
     assert 'ZeroDivisionError' in str(got_pipe['error'])
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_instantiator.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_instantiator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_instantiator_test.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_instantiator_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,8 +33,9 @@
     executable.fit(dataset=REFERENCE_DATASET)
 
     got_predict = executable.predict(dataset=REFERENCE_DATASET)
     want_predict = {
         'twice_transformed_key': 'a_value',
         'another_key': 'another_value',
     }
+    assert got_predict.prediction is not None
     assert set(got_predict.prediction) == set(want_predict)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/executor/simple/simple_parallel_executable_step.py` & `ngautonml-0.4.1b2/ngautonml/executor/simple/simple_parallel_executable_step.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/generator/bound_pipeline.py` & `ngautonml-0.4.1b2/ngautonml/generator/bound_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,42 @@
 
 
 class ValidationError(Error):
     '''The BoundPipeline object violates constraints.'''
 
 
 class BoundPipeline(PipelineTemplate):
-    '''Placeholder for Bound pipelines'''
+    '''A ``BoundPipeline`` is a ``PipelineTemplate`` with no query steps.
+
+    ``BoundPipeline``\\ s are outputs of the ``Generator``,
+    inputs and outputs of the ``Searcher``,
+    and inputs to the ``Instantiator``.
+    '''
     _frozen_overrides: Optional[FrozenOverrides] = None
 
     def __init__(self,
                  name: Optional[str] = None,
                  **kwargs):
         assert name is not None, (
             'BoundPipeline constructor requires a name or designator')
         super().__init__(name=name, **kwargs)
         self.validate()
 
     @property
+    def family_designator(self) -> Designator:
+        '''The name this bound pipeline shares when we ignore overrides.'''
+        components = [self.name]
+        components.extend(
+            step.pipeline_designator_component
+            for step in self.steps
+            if step.queried
+        )
+        return Designator('@'.join(components).lower())
+
+    @property
     def designator(self) -> Designator:
         '''The unique designator for this bound pipeline'''
         components = [self.name]
 
         for step in self.steps:
             has_overrides = (self._frozen_overrides is not None
                              and step.pipeline_designator_component in self._frozen_overrides)
@@ -55,15 +71,15 @@
             assert self._frozen_overrides is not None
             step_overrides = self._frozen_overrides[step.pipeline_designator_component]
             overrides_strs = sorted(
                 [f'{k}={v}' for k, v in step_overrides.items()])
             components.append(
                 f'{step.pipeline_designator_component}:{",".join(overrides_strs)}')
 
-        return Designator('@'.join(components))
+        return Designator('@'.join(components).lower())
 
     @property
     def _query_names(self) -> List[str]:
         '''A list of names of all steps that are from a query.
 
         We currently don't support query steps inside parallel steps.
         '''
```

### Comparing `ngautonml-0.4.1b1/ngautonml/generator/bound_pipeline_test.py` & `ngautonml-0.4.1b2/ngautonml/generator/bound_pipeline_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,7 +78,10 @@
     got = BoundPipelineStub.build(
         steps=dut.steps,
         template_name=Designator("new_template_name"),
         frozen_overrides=frozen_overrides)
 
     want = 'new_template_name@query1@query3:h=v@nonquery4:h1=v1,h2=v2'
     assert str(got.designator) == want
+
+    want_family = 'new_template_name@query1@query3'
+    assert str(got.family_designator) == want_family
```

### Comparing `ngautonml-0.4.1b1/ngautonml/generator/designator.py` & `ngautonml-0.4.1b2/ngautonml/generator/designator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/generator/generator.py` & `ngautonml-0.4.1b2/ngautonml/generator/generator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/generator/generator_test.py` & `ngautonml-0.4.1b2/ngautonml/generator/generator_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/executable_pipeline.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/executable_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,23 @@
 
 
 class PredictError(PipelineExecutionError):
     '''A pipeline threw an error during predict'''
 
 
 class ExecutablePipeline(metaclass=abc.ABCMeta):
-    '''Base class for all executable pipelines.'''
+    '''Base class for all executable pipelines.
+
+    An ``ExecutablePipeline`` can be executed by a specific kind of
+    ``Executor``, and is created from a ``BoundPipeline``
+    by the corresponding ``Instantiator``.
+
+    All algorithms and hyperparameters are bound to single values
+    (so no query steps or hyperparam search spaces).
+    '''
     _kind: ExecutorKind
     _pipeline: BoundPipeline
     _trained: bool = False
     _fit_error: Optional[FitError] = None
 
     @property
     def kind(self):
@@ -49,17 +57,17 @@
         '''The name of the underlying pipeline'''
         return self._pipeline.name
 
     @property
     def designator(self) -> Designator:
         '''The designator for this instance of an executable pipeline
 
-        Overriding classes should derive this from the bound pipeline.
+        Always the same as that of its bound pipeline
         '''
-        return Designator(self.name)  # TODO(piggy): This should be a .-separated path.
+        return self.bound.designator
 
     @property
     def bound(self) -> BoundPipeline:
         '''The bound pipeline this was compiled from'''
         return self._pipeline
 
     @property
@@ -90,14 +98,22 @@
     @abc.abstractmethod
     def cucumberize_all(self) -> JarOfCucumbers:
         '''Cucumberize all steps that hold algorithms, and return the result.
 
         This has the same output as fit() but requires the pipeline to be fit already.
         '''
 
+    @abc.abstractmethod
+    def start(self) -> None:
+        '''Start all pipeline threads.'''
+
+    @abc.abstractmethod
+    def stop(self) -> None:
+        '''Stop all pipeline threads.'''
+
     def __str__(self):
         return f'{{{self._pipeline.designator}, executor: {self.kind}}}'
 
 
 class ExecutablePipelineStub(ExecutablePipeline):
     '''stub'''
     _cucumbers: JarOfCucumbers
@@ -117,34 +133,40 @@
 
     def predict(self, dataset: Dataset) -> 'PipelineResult':
         return PipelineResult(prediction=dataset, executable_pipeline=self)
 
     def cucumberize_all(self) -> JarOfCucumbers:
         return self._cucumbers
 
+    def stop(self) -> None:
+        pass
+
+    def start(self) -> None:
+        pass
+
 
 class PipelineResultError(Exception):
     '''Base class for all errors associated with this file.'''
 
 
 # TODO(Merritt): put this in own file
 # (may need a separate InternalPipelineResult and ExternalPipelineResult)
 class PipelineResult(metaclass=abc.ABCMeta):
     '''Base class for objects that represent the result of a pipeline run.
 
     At a minimum contains a pipeline that was run and a dataset resulting from that run.
     Subclasses may contain additional information.
     '''
-    _prediction: Dataset
+    _prediction: Optional[Dataset]
     _bound_pipeline: Optional[BoundPipeline] = None
     _executable_pipeline: Optional[ExecutablePipeline] = None
     _split_dataset: Optional[SplitDataset] = None
 
     def __init__(self,
-                 prediction: Dataset,
+                 prediction: Optional[Dataset],
                  bound_pipeline: Optional[BoundPipeline] = None,
                  executable_pipeline: Optional[ExecutablePipeline] = None,
                  split_dataset: Optional[SplitDataset] = None):
 
         if bound_pipeline is None:
             assert executable_pipeline is not None, (
                 'BUG: both bound and executable pipelines are None'
@@ -152,21 +174,24 @@
 
         self._prediction = prediction
         self._bound_pipeline = bound_pipeline
         self._executable_pipeline = executable_pipeline
         self._split_dataset = split_dataset
         if (self._split_dataset is not None
             and self._split_dataset.ground_truth is not None
-                and DatasetKeys.PREDICTIONS.value in self._prediction):
+                and DatasetKeys.PREDICTIONS.value in (self._prediction or {})):
             self._add_ground_truth()
 
     def _add_ground_truth(self) -> None:
         '''Display ground truth next to train predictions.'''
         assert self._split_dataset is not None
         assert self._split_dataset.ground_truth is not None
+        assert self.prediction is not None, (
+            'BUG: attempt to add ground truth to a pipeline result with no prediction of None.'
+        )
         assert isinstance(self.prediction[DatasetKeys.PREDICTIONS.value], pd.DataFrame), (
             'BUG: can only add ground truth to predictions if predictions is a dataframe. '
             f'instead found f{self.prediction[DatasetKeys.PREDICTIONS.value]}')
 
         if OutputColName.GROUND_TRUTH.value in self.prediction.predictions.columns:
             # Predictions dataframe already contains ground truth
             return
@@ -181,19 +206,24 @@
         # Align the ground truth with the prediction dataframe.
         new_df.reset_index(inplace=True, drop=True)
         gt_df.reset_index(inplace=True, drop=True)
         new_df[OutputColName.GROUND_TRUTH.value] = gt_df[target.name]
         self.prediction.predictions = new_df
 
     @property
-    def prediction(self) -> Dataset:
+    def prediction(self) -> Optional[Dataset]:
         '''Dataset resulting from the pipeline run'''
         return self._prediction
 
     @property
+    def family_designator(self) -> Designator:
+        '''Family designator of BoundPipeline associated with this pipeline run'''
+        return self.bound_pipeline.family_designator
+
+    @property
     def bound_pipeline(self) -> BoundPipeline:
         '''Bound pipeline associated with this pipeline run.'''
         if self._executable_pipeline is not None:
             return self._executable_pipeline.bound
         assert self._bound_pipeline is not None, (
             'BUG: both bound and executable pipelines are None'
             ' in PipelineResult bound_pipeline property.')
@@ -227,15 +257,15 @@
         '''Attempts to infer ground truth using an arbitrary PipelineResult.'''
         split_dataset = self._some_result().split_dataset
         if split_dataset is not None:
             return split_dataset.ground_truth
         return None
 
     @property
-    def predictions(self) -> Dict[Designator, Dataset]:
+    def predictions(self) -> Dict[Designator, Optional[Dataset]]:
         '''Datasets resulting from the pipeline runs'''
         return {k: v.prediction for k, v in self.items()}
 
     @property
     def bound_pipelines(self) -> Dict[Designator, BoundPipeline]:
         '''Bound Pipelines associated with the pipeline runs'''
         return {k: v.bound_pipeline for k, v in self.items()}
```

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/executable_pipeline_test.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/executable_pipeline_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,13 +80,14 @@
         split_dataset=SplitDataset([
             Fold(
                 train=empty,
                 validate=empty,
                 ground_truth=gt
             )
         ]))
+    assert dut.prediction is not None
     got = dut.prediction.predictions
     want = pd.DataFrame({
         'a': [1, 2, 3],
         'ground truth': [4, 5, 6]
     })
     pd.testing.assert_frame_equal(got, want)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/instantiator.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/instantiator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/instantiator_factory.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/instantiator_factory.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/instantiator_test.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/instantiator_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/json_instantiator.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/json_instantiator.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/json_instantiator_test.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/json_instantiator_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/json_loader.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/json_loader.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/instantiator/json_loader_test.py` & `ngautonml-0.4.1b2/ngautonml/instantiator/json_loader_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_auto.py` & `ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_auto.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_auto_test.py` & `ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_auto_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_catalog.py` & `ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_catalog.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_catalog_test.py` & `ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_catalog_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/impl/metric_test.py` & `ngautonml-0.4.1b2/ngautonml/metrics/impl/metric_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/sklearn_metrics.py` & `ngautonml-0.4.1b2/ngautonml/metrics/sklearn_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,58 +5,56 @@
 
 from typing import Any, Callable, Dict, List, Optional
 
 import numpy as np
 import sklearn.metrics  # type: ignore[import]
 from sklearn.metrics import mean_squared_error  # type: ignore[import]
 
-from ..problem_def.task import TaskType
-from ..wrangler.constants import ProblemDefKeys
+from ..problem_def.task import Task, TaskType
 from ..wrangler.dataset import Dataset, DatasetKeyError, RoleName
 from .impl.metric import MetricInvalidDatasetError, SupervisedMetric
 from .impl.metric_catalog import MetricCatalog
 
 
 class SklearnMetric(SupervisedMetric):
     '''Wrapper for sklean.metrics'''
     _metric: Optional[Callable[..., float]] = None
 
     def __init__(self,
                  name: str,
                  metric: Optional[Callable[..., float]] = None,
                  tasks: Optional[List[TaskType]] = None,
                  high: bool = True,
-                 uses_proba: bool = False,
+                 needs_proba: bool = False,
                  needs_pos_label: bool = False):
-        # TODO(Merritt): high, uses_proba, needs_pos_label should be put in tags
         if metric is None:
             metric = getattr(sklearn.metrics, name, None)
         self._metric = metric
         if tasks is None:
             tasks = []
         self._tags = {
-            ProblemDefKeys.TASK_TYPE.value: [t.name.lower() for t in tasks],
+            Task.Keys.TASK_TYPE.value: [t.name.lower() for t in tasks],
         }
-        self._needs_pos_label = needs_pos_label
-        self._high = high
-        self._uses_proba = uses_proba
+        self._tags['needs_pos_label'] = [str(needs_pos_label).lower()]
+        self._tags['high'] = [str(high).lower()]
+        self._tags['needs_proba'] = [str(needs_proba).lower()]
         super().__init__(name=name)
 
     def calculate(self, pred: Dataset, ground_truth: Optional[Dataset] = None) -> float:
         # TODO(Merritt): should be able to accept hyperparams from problem def
         ground_truth = self.validate_input(pred, ground_truth)
         # validate_input is guaranteed to return ground truth Dataset rather than None.
         assert ground_truth.metadata.target is not None
         ground_truth_for_sklearn = list(
             ground_truth.ground_truth[ground_truth.metadata.target.name])
         assert pred.metadata.target is not None, (
             'BUG: calculate() called with no target info in metadata'
         )
 
-        if self.uses_proba:
+        if self.needs_proba:
             try:
                 pred_df = pred.probabilities
             except DatasetKeyError:
                 # We are not using 'from' because this error will be displayed
                 #   alongside metric scores as a explanation for why this score
                 #   cannot be calculated, thus we want it to be succint.
                 raise MetricInvalidDatasetError(   # pylint: disable=raise-missing-from
@@ -65,15 +63,15 @@
             pred_df = pred.predictions
 
         predictions_for_sklearn = list(
             pred_df[pred.metadata.target.name])
 
         assert self._metric is not None
 
-        if RoleName.TARGET in pred.metadata.pos_labels and self._needs_pos_label:
+        if RoleName.TARGET in pred.metadata.pos_labels and self.needs_pos_label:
             return self._metric(
                 ground_truth_for_sklearn,
                 predictions_for_sklearn,
                 pos_label=pred.metadata.pos_labels[RoleName.TARGET])
 
         return self._metric(ground_truth_for_sklearn, predictions_for_sklearn)
 
@@ -83,15 +81,15 @@
     return np.sqrt(mean_squared_error(*args, **kwargs))
 
 
 METRICS: List[Dict[str, Any]] = [
     {
         'name': 'roc_auc_score',
         'tasks': [TaskType.BINARY_CLASSIFICATION],
-        'uses_proba': True,
+        'needs_proba': True,
     },
     {
         'name': 'accuracy_score',
         'tasks': [TaskType.BINARY_CLASSIFICATION, TaskType.MULTICLASS_CLASSIFICATION],
     },
     {
         'name': 'f1_score',
```

### Comparing `ngautonml-0.4.1b1/ngautonml/metrics/sklearn_metrics_test.py` & `ngautonml-0.4.1b2/ngautonml/metrics/sklearn_metrics_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/aggregation_config.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/aggregation_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 '''Holds configuration information for aggregation.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from enum import Enum
 from typing import Any, Dict, List
 
-from ..wrangler.constants import ProblemDefKeys
-
-from .config_component import ConfigComponent, ConfigError
+from ..config_components.impl.config_component import ConfigComponent, ConfigError
 
 
 class AggregationError(ConfigError):
     '''Accummulating error for rank aggregation parsing.'''
 
     errors: List[ConfigError]
 
@@ -23,17 +22,21 @@
 class AggregationConfig(ConfigComponent):
     '''Holds configuration for rank aggregation.
 
     If this clause is missing, we do not do rank aggregation.
     '''
     _method: List[str]
 
+    class Keys(Enum):
+        '''Top-level clauses in aggregation component'''
+        METHOD = 'method'
+
     def __init__(self, clause: Dict[str, Any]):
         super().__init__(clause=clause)
-        method = self._get_with_default(ProblemDefKeys.METHOD, dflt=[])
+        method = self._get_with_default(self.Keys.METHOD, dflt=[])
         if method is not None:
             if not isinstance(method, list):
                 assert isinstance(method, str)
                 method = [method]
         self._method = method
         self.validate()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/config_component.py` & `ngautonml-0.4.1b2/ngautonml/config_components/impl/config_component.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 '''Base class for elements of the Problem Definition file'''
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-import abc
 import copy
-from typing import Any, Dict, List, Optional, Union
-from ..wrangler.constants import ProblemDefKeys
+from enum import Enum
+from typing import Any, Dict, List, Optional, Set, Union
 
 
 class ConfigError(BaseException):
     '''All errors thrown by problem definition modules'''
 
 
 class ConfigDirectoryError(ConfigError, NotADirectoryError):
@@ -50,46 +49,64 @@
 
     def __str__(self) -> str:
         retval_list1 = [str(arg) for arg in self.args]
         retval_list2 = [f'\t{repr(error)}' for error in self.errors]
         return '\n'.join(retval_list1 + retval_list2)
 
 
-class ConfigComponent(metaclass=abc.ABCMeta):
+class ConfigComponent():
     '''Base class for elements of the Problem Definition file
 
     This provides _get, _get_with_default, and _exists for
     use by config components.
     '''
     # pylint: disable=too-few-public-methods
+    # _parents is a path of ancestor clause names to reach this
+    # component, for use in error messages.
     _parents: List[str]
     _clause: Dict[str, Any]
 
-    def __init__(self, clause: Dict[str, Any], parents: Optional[List[str]] = None):
+    class Keys(Enum):
+        '''Child classes need to define this class with all their keys.'''
+
+    def __init__(self,
+                 clause: Dict[str, Any],
+                 parents: Optional[List[str]] = None,
+                 **unused_kwargs):
         if parents is None:
             parents = []
         self._parents = parents
         self._clause = clause
 
+    def allowed_keys(self) -> Set[str]:
+        '''Set of keys that are acceptable for this clause'''
+        return {key.value for key in list(self.Keys)}
+
+    # We default to no required keys.
+    def required_keys(self) -> Set[str]:
+        '''Subset of ALLOWED_KEYS that are required'''
+        return set()
+
     def _add_parent(self,
                     parents: Optional[List[str]],
                     new_parent: str) -> List[str]:
+        '''Keep track of where we are in the problem def for error messages.'''
         if parents is None:
             retval = []
         else:
             retval = parents.copy()
         retval.append(new_parent)
         return retval
 
-    def _get(self, *args: Union[int, str, ProblemDefKeys]):
+    def _get(self, *args: Union[int, str, Enum]):
         '''for ex: call _get('metric', 'name') to get metric name'''
         here = self._clause
         so_far = []
         for k in args:
-            if isinstance(k, ProblemDefKeys):
+            if isinstance(k, Enum):
                 k = k.value
             so_far.append(str(k))
             if isinstance(here, list):
                 if not isinstance(k, int):
                     raise ProblemDefTypeError(
                         f'found a list at {".".join(self._parents + so_far[:-1])}, '
                         f'expected an integer at {".".join(self._parents + so_far)}')
@@ -101,25 +118,25 @@
                                           f'{".".join(so_far)}')
                 assert isinstance(k, str), (
                     f'BUG: at _get {".".join(so_far)} we have a non-string key, {k!r} for {here!r}')
             here = here[k]
 
         return copy.deepcopy(here)
 
-    def _get_with_default(self, *args: Union[int, str, ProblemDefKeys], dflt: Any) -> Any:
+    def _get_with_default(self, *args: Union[int, str, Enum], dflt: Any) -> Any:
         if self._exists(*args):
             return self._get(*args)
         return dflt
 
-    def _exists(self, *args: Union[int, str, ProblemDefKeys]) -> bool:
+    def _exists(self, *args: Union[int, str, Enum]) -> bool:
         '''for ex: call _exists('metric', 'name') to see if metric.name exists'''
         here = self._clause
         so_far = []
         for k in args:
-            if isinstance(k, ProblemDefKeys):
+            if isinstance(k, Enum):
                 k = k.value
             so_far.append(str(k))
             if isinstance(here, list):
                 if not isinstance(k, int):
                     raise ProblemDefTypeError(
                         f'found a list at {".".join(self._parents + so_far[:-1])}, '
                         f'expected an integer at {".".join(self._parents + so_far)}')
@@ -130,10 +147,40 @@
                     return False
                 assert isinstance(k, str), (
                     f'BUG: at _exists {".".join(so_far)} we have a '
                     f'non-string key, {k!r} for {here!r}')
             here = here[k]
         return True
 
-    @abc.abstractmethod
     def validate(self, **kwargs) -> None:
-        '''Raise a ConfigError if something about the clause is invalid.'''
+        '''Raise a ConfigError if something about the clause is invalid.
+
+        The base class validate() checks only fotr required and allowed keys.
+
+        For ConfigComponents created by plugins, implementations must not raise an
+        error if the clause is an empty dict.
+        '''
+        _ = kwargs
+        errors: List[ConfigError] = []
+        if isinstance(self._clause, dict):
+            keys = set(self._clause.keys())
+            if not self.required_keys().issubset(keys):
+                errors.append(MissingKeyError(
+                    f'Required keys missing in {".".join(self._parents)} clause: '
+                    f'{self.required_keys().difference(keys)}'))
+
+            if not keys.issubset(self.allowed_keys()):
+                errors.append(InvalidKeyError(
+                    f'Invalid key(s) in {".".join(self._parents)} clause: '
+                    f'{keys.difference(self.allowed_keys())}. '
+                    f'Valid keys are {self.allowed_keys()}'))
+
+        if len(errors) > 0:
+            raise ValidationErrors(errors=errors)
+
+
+class ConfigComponentStub(ConfigComponent):
+    '''Config component for cases where we need a stub.'''
+    name = 'stub_config_component'
+
+    def validate(self, **kwargs) -> None:
+        pass
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/cross_validation_config.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/cross_validation_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 '''Holds configuration information for cross-validation.'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from enum import Enum
 from typing import Dict, Any, Optional, List
 
+from ..config_components.impl.config_component import ConfigComponent, InvalidValueError
 from ..wrangler.constants import ProblemDefKeys, Defaults
 
-from .config_component import ConfigComponent, InvalidValueError
-
 
 class CrossValidationConfig(ConfigComponent):
     '''
     Holds configuration information for cross-validation.
     '''
 
     def __init__(self, clause: Dict[str, Any], parents: Optional[List[str]] = None):
         parents = self._add_parent(parents, ProblemDefKeys.CROSS_VALIDATION.value)
         super().__init__(clause=clause, parents=parents)
 
+    class Constants(Enum):
+        '''Lower-level clauses in cross_validation component'''
+        N_SPLITS = 'n_splits'
+
+    class Keys(Enum):
+        '''Top-level clauses in cross_validation component'''
+        K = 'k'
+        SEED = 'seed'
+
     @property
     def k(self) -> Optional[int]:
         '''get k fold'''
-        field = self._get_with_default(
-            ProblemDefKeys.K.value,
-            dflt=None
-        )
+        field = self._get_with_default(self.Keys.K, dflt=None)
 
         return field
 
     @property
     def seed(self) -> int:
         '''Get default random seed or one set by'''
         field = self._get_with_default(
-            ProblemDefKeys.SEED.value,
+            self.Keys.SEED,
             dflt=Defaults.SEED
         )
         return field
 
     @property
     def splitter_hyperparams(self) -> Dict[str, Any]:
         '''get splitter hyperparams'''
         retval = {}
 
         if self.k:
-            retval['n_splits'] = self.k
+            retval[self.Constants.N_SPLITS.value] = self.k
 
         return retval
 
     def validate(self, **kwargs) -> None:
         if self.k is None:
             return
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/hyperparam_config.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/hyperparam_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
  instead of separate structures for each clause so that it is easier to do
  intelligent searches of hyperparameter overrides.
 '''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from enum import Enum
 from typing import Dict, Any, List, Union
 
+from ..config_components.impl.config_component import ConfigComponent, ConfigError
 from ..searcher.params import Overrides, Override, Selector, ParamRanges, ParamRange
-from ..wrangler.constants import (ProblemDefControl, ProblemDefKeys,
+from ..wrangler.constants import (ProblemDefControl,
                                   RangeMethod, Matcher, MATCHERS_TO_LOWERCASE)
 
-from .config_component import ConfigComponent, ConfigError
-
 
 class HyperparamError(ConfigError):
     '''Accummulating error for hyperparam parsing.'''
 
     errors: List[ConfigError]
 
     def __init__(self, errors: List[ConfigError]):
@@ -41,19 +41,27 @@
     We use a single data structure, HyperparamConfig, for all hyperparam clauses
     instead of separate structures for each clause so that it is easier to do
     intelligent searches of hyperparameter overrides.
     '''
     _control: List[str]
     _disable_grid_search = False
 
+    class Constants(Enum):
+        '''Keys below the top level.'''
+        HYPERPARAMS = 'hyperparams'
+        SELECT = 'select'
+        PARAMS = 'params'
+        DEFAULT = 'default'
+
     def __init__(self, clause: Dict[str, Any]):
         super().__init__(clause=clause)
         self._overrides = Overrides()
 
-        (overrides, control) = self._split_overrides_control(self._get(ProblemDefKeys.HYPERPARAMS))
+        (overrides, control) = self._split_overrides_control(
+            self._get(self.Constants.HYPERPARAMS))
         for override_clause in overrides:
             self._overrides.append(self._parse_override(override_clause))
         self._control = control
         self._parse_control()
 
         self.validate()
 
@@ -73,16 +81,16 @@
             elif isinstance(val, dict):
                 retval_overrides.append(val)
             else:
                 raise ControlError(f'Unexpected hyperparam type, {val}:{type(val)}')
         return (retval_overrides, retval_str)
 
     def _parse_override(self, subclause: Dict[str, Dict[str, Any]]) -> Override:
-        select_clause = subclause.pop(ProblemDefKeys.SELECT.value)
-        params_clause = subclause.pop(ProblemDefKeys.PARAMS.value)
+        select_clause = subclause.pop(self.Constants.SELECT.value)
+        params_clause = subclause.pop(self.Constants.PARAMS.value)
         if subclause:
             raise HyperparamTooManyClauses(f'Unexpected extra clauses: {subclause!r}')
         select = Selector()
         for matcher, arg in select_clause.items():
             matcher_enum = Matcher[matcher.upper()]
             if matcher_enum in MATCHERS_TO_LOWERCASE:
                 arg = arg.lower()
@@ -90,15 +98,15 @@
         params = ParamRanges()
         for name, hyperparam_param in params_clause.items():
             params[name] = self._parse_param(hyperparam_param)
 
         return Override(selector=select, params=params)
 
     def _parse_param(self, param: Dict[str, Any]) -> ParamRange:
-        default = param.pop(ProblemDefKeys.DEFAULT.value, None)
+        default = param.pop(self.Constants.DEFAULT.value, None)
         if len(param) != 1:
             raise HyperparamTooManyClauses(f'expecting 1 key, got {param!r}')
 
         for method, range_value in param.items():
             return ParamRange(method=RangeMethod[method.upper()],
                               prange=range_value,
                               default=default)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/hyperparam_config_test.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/hyperparam_config_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/metric_config.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/metric_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 '''Metric configuration'''
-from typing import Any, Dict, List, Optional
+from enum import Enum
+from typing import Any, Dict, List, Optional, Set
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from ..wrangler.constants import ProblemDefKeys
-from .config_component import ConfigComponent, ConfigError
+from ..config_components.impl.config_component import ConfigComponent, ConfigError
 
 
 class MetricConfigError(ConfigError):
     '''Base error for MetricConfig.'''
 
 
 class MetricConfig(ConfigComponent):
     '''Configured metrics'''
     _catalog_name: Optional[str] = None
 
+    class Constants(Enum):
+        '''Constants below and above top level.'''
+        CATALOG_NAME = 'catalog_name'
+        METRICS = 'metrics'
+
     def __init__(self, clause: Dict[str, Any], parents: Optional[List[str]] = None):
-        parents = self._add_parent(parents, ProblemDefKeys.METRICS.value)
+        parents = self._add_parent(parents, self.Constants.METRICS.value)
         super().__init__(clause=clause, parents=parents)
 
     def validate(self, **kwargs) -> None:
         '''Throw a MetricConfigError if the metric clause is invalid'''
         errors: List[MetricConfigError] = []
 
         if len(self._clause.keys()) != 1:
@@ -37,30 +42,42 @@
             self.catalog_name  # pylint: disable=pointless-statement
         except AssertionError as err:
             errors.append(MetricConfigError(str(err)))
 
         if len(errors) > 0:
             raise MetricConfigError(errors)
 
+    def allowed_keys(self) -> Set[str]:
+        return set(self._clause.keys())
+
     @property
     def name(self) -> str:
         '''The instance name for this metric.'''
         return list(self._clause.keys())[0]
 
     @property
     def hyperparams(self) -> Dict[str, Any]:
-        '''The hyperparams for this metric.'''
+        '''The hyperparams for this metric.
+
+        If you want more than one instance of a single metric
+        with different hyperparams, define each with its own
+        name and use the 'catalog_name' to specify the metric
+        in the catalog to use.
+        '''
         retval = dict(list(self._clause.values())[0])
-        if ProblemDefKeys.CATALOG_NAME.value in retval:
-            del retval[ProblemDefKeys.CATALOG_NAME.value]
+        if self.Constants.CATALOG_NAME.value in retval:
+            del retval[self.Constants.CATALOG_NAME.value]
         return retval
 
     @property
     def catalog_name(self) -> str:
         '''The metric catalog name for this metric.
 
+        We can have different metric entries with the same catalog_name,
+        but different hyperparams.
+
         Defaults to self.name.
         '''
         metric_info: Dict[str, Any] = list(self._clause.values())[0]
-        retval = metric_info.get(ProblemDefKeys.CATALOG_NAME.value, self.name)
+        retval = metric_info.get(self.Constants.CATALOG_NAME.value, self.name)
         assert isinstance(retval, str), f'catalog_name must be a str, not a {type(retval)}'
         return retval
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/output_config.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/output_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 '''Output configuration'''
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from enum import Enum
 from pathlib import Path
 from typing import Optional, Set, Dict, Any, List
 
-from .config_component import ConfigComponent, ConfigError
+from ..config_components.impl.config_component import ConfigComponent, ConfigError
 from ..wrangler.constants import FileType, Defaults, ProblemDefKeys
 from ..executor.executor_kind import ExecutorKind
 
 
 class OutputConfigError(ConfigError):
     '''Errors during building or validating OutputConfig.'''
 
 
 class OutputConfig(ConfigComponent):
     '''Output configuration'''
 
+    class Keys(Enum):
+        '''Top-level clauses in output component'''
+        OUTPUT_PATH = 'path'
+        FILE_TYPE = 'file_type'
+        INSTATIATIONS = 'instantiations'
+
     def __init__(self, clause: Dict[str, Any], parents: Optional[List[str]] = None):
         parents = self._add_parent(parents, ProblemDefKeys.OUTPUT.value)
         super().__init__(clause=clause, parents=parents)
 
     def validate(self, **kwargs) -> None:
         if self.path is not None:
             if self.path.exists() and not self.path.is_dir():
@@ -45,26 +52,26 @@
             _ = self.instantiations
         except NotImplementedError as err:
             raise OutputConfigError(err) from err
 
     @property
     def path(self) -> Optional[Path]:
         '''Path to the output folder specified in the problem def'''
-        if self._exists(ProblemDefKeys.OUTPUT_PATH):
-            return Path(self._get(ProblemDefKeys.OUTPUT_PATH)).resolve()
+        if self._exists(self.Keys.OUTPUT_PATH):
+            return Path(self._get(self.Keys.OUTPUT_PATH)).expanduser().resolve()
         return None
 
     @property
     def instantiations(self) -> Set[ExecutorKind]:
         '''Kinds of instantiations specified in the problem'''
         retval = self._get_with_default(
-            ProblemDefKeys.INSTATIATIONS, dflt=Defaults.INSTANTIANTIONS)
+            self.Keys.INSTATIATIONS, dflt=Defaults.INSTANTIANTIONS)
         return set(ExecutorKind(s) for s in retval)
 
     @property
     def file_type(self) -> FileType:
         '''Type of file for predictions to be saved in.'''
-        retval = self._get_with_default(ProblemDefKeys.FILE_TYPE.value, dflt=Defaults.FILE_TYPE)
+        retval = self._get_with_default(self.Keys.FILE_TYPE, dflt=Defaults.FILE_TYPE)
         try:
             return FileType[retval.upper()]
         except KeyError as exc:
             raise OutputConfigError(f'{retval} is not a valid file type') from exc
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/output_config_test.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/output_config_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/problem_def.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/problem_def.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,90 @@
 '''Contains ProblemDefinition'''
-import json
-import textwrap
-from typing import Any, Dict, List, Optional, Union
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-import pandas as pd
-from pandas import DataFrame
-
-from ..dataset_formats.impl.dataset_config import (DatasetConfig,
-                                                   DatasetFileError,
-                                                   DatasetConfigError)
-from ..dataset_formats.impl.dataset_format_catalog import (DatasetFormatCatalog,
-                                                           DatasetFormatCatalogAuto)
-from ..executor.executor_kind import ExecutorKind
-from ..wrangler.constants import ProblemDefKeys, ProblemDefKeySet, Defaults
-from ..wrangler.dataset import Metadata, RoleName
+from enum import Enum
+import json
+import textwrap
+from typing import Any, Dict, List, Optional, Set, Union
 
+from ..config_components.impl.config_component import (
+    ConfigComponent, ConfigError, InvalidKeyError,
+    MissingKeyError, ParsingErrors, ValidationErrors)
+from ..config_components.impl.config_component_catalog import ConfigComponentCatalog
+from ..config_components.impl.config_component_auto import ConfigComponentAuto
+from ..wrangler.constants import ProblemDefKeys
 from .aggregation_config import AggregationConfig, AggregationError
 from .cross_validation_config import CrossValidationConfig
-from .config_component import ConfigComponent, ConfigError, ParsingErrors
-from .config_component import MissingKeyError
-from .config_component import InvalidKeyError, ValidationErrors
-from .config_component import InvalidValueError, ProblemDefTypeError
 from .hyperparam_config import HyperparamConfig, HyperparamError
 from .metric_config import MetricConfig, MetricConfigError
 from .output_config import OutputConfig
-from .task import TaskType, Task
+from .problem_def_interface import ProblemDefInterface
+from .task import Task
 
 # pylint: disable=too-many-branches,too-many-statements
 
 
-class ProblemDefinition(ConfigComponent):
+class ProblemDefinition(ProblemDefInterface):
     '''Represents information needed to define an AutoML run'''
+    _catalog: Optional[ConfigComponentCatalog] = None
+    _plugin_components: Dict[str, ConfigComponent]
     _task: Optional[Task] = None
-
     _aggregation_config: Optional[AggregationConfig] = None
     _cross_validation_config: Optional[CrossValidationConfig] = None
-    _dataset_config: Optional[DatasetConfig] = None
     _metric_configs: Optional[Dict[str, MetricConfig]] = None
     _hyperparam_config: Optional[HyperparamConfig] = None
     _output_config: Optional[OutputConfig] = None
 
-    _data_formats_catalog: Optional[DatasetFormatCatalog] = None
+    def allowed_keys(self) -> Set[str]:
+        '''Set of keys that are acceptable for this clause'''
+        allowed = super().allowed_keys()
+        allowed.update(self._plugin_components.keys())
+        return allowed
+
+    def required_keys(self) -> Set[str]:
+        '''Subset of ALLOWED_KEYS that are required'''
+        return {self.Keys.TASK.value, self.Keys.DATASET.value}
 
     def __init__(self,
-                 problem_def: Union[str, Dict[str, Any]],
-                 train_df: Optional[DataFrame] = None,
-                 test_df: Optional[DataFrame] = None,
-                 data_formats_catalog: Optional[DatasetFormatCatalog] = None):
-
-        if isinstance(problem_def, str):
-            problem_def = self._parse_json(pdef=problem_def)
-        super().__init__(clause=remove_comments(problem_def))
-        self._data_formats_catalog = data_formats_catalog or DatasetFormatCatalogAuto()
+                 clause: Union[str, Dict[str, Any]]):
+
+        if self._catalog is None:
+            self._catalog = ConfigComponentAuto()
+
+        if isinstance(clause, str):
+            clause = self._parse_json(pdef=clause)
+        super().__init__(clause=remove_comments(clause))
 
         errors: List[ConfigError] = []
 
+        self._plugin_components = {}
+
+        for plugin_name, constructor in self._catalog.items():
+            try:
+                plugin_clause = self._get(plugin_name)
+            except MissingKeyError:
+                # We do not require all plugin clauses to be present.
+                plugin_clause = {}
+
+            try:
+                # But we still want to instantiate the plugin so that we can use its validator.
+                self._plugin_components[plugin_name] = (
+                    constructor(clause=plugin_clause, problem_def=self))
+            except ParsingErrors as err:
+                errors.extend(err.errors)
+
         try:
             self._task = Task(self._get(
                 ProblemDefKeys.TASK))
         except KeyError as err:
             errors.append(InvalidKeyError(err))
 
         try:
-            clause = self._get(ProblemDefKeys.DATASET)
-            self._dataset_config = self._data_formats_catalog.build(
-                clause=clause,
-                task=self._task,
-                train_df=train_df,
-                test_df=test_df
-            )
-        except (KeyError,  # Missing field names, bad column name, bad role name
-                FileNotFoundError,  # Missing csv
-                TypeError,  # Malformed json.
-                pd.errors.ParserError,  # Train file is not parsable.
-                IndexError  # Column id out of range.
-                ) as err:
-            errors.append(DatasetConfigError(err))
-        except DatasetConfigError as err:  # Train dataframe not provided for MemoryDatasetConfig
-            errors.append(err)
-
-        try:
             self._cross_validation_config = CrossValidationConfig(self._get_with_default(
                 ProblemDefKeys.CROSS_VALIDATION, dflt={}))
         except KeyError as err:
             errors.append(InvalidKeyError(err))
 
         try:
             metrics_clause = self._get_with_default(ProblemDefKeys.METRICS, dflt={})
@@ -141,111 +139,55 @@
 
         try:
             with open(pdef, 'r', encoding='utf8') as f:
                 retval = json.load(f)
             return retval
         except FileNotFoundError as err:
             errors.append(ConfigError(err))
+        except OSError as err:
+            errors.append(ConfigError(err))
         except json.decoder.JSONDecodeError as err:
             errors.append(ConfigError(err))
 
         errors.insert(0, ConfigError(
             'String provided could not be parsed as JSON or path to JSON file.'))
         raise ParsingErrors(errors=errors)
 
     def __str__(self):
         return textwrap.dedent(f'''
             problem_type={self.task}
-            dataset_config={self.dataset_config}
         ''')
 
     def validate(self, **kwargs) -> None:
-        errors: List[ConfigError] = []
-        keys = set(self._clause.keys())
-        if not ProblemDefKeySet.REQUIRED.issubset(keys):
-            errors.append(MissingKeyError(
-                'Required keys missing in problem definition: '
-                f'{ProblemDefKeySet.REQUIRED.difference(keys)}'))
-        if not keys.issubset(ProblemDefKeySet.ALLOWED):
-            errors.append(InvalidKeyError(
-                'Invalid key(s) in problem definition: '
-                f'{keys.difference(ProblemDefKeySet.ALLOWED)}'))
-
-        if self._task is not None:
-            try:
-                self.task.validate()
-            except ValidationErrors as err:
-                errors.extend(err.errors)
+        super().validate(**kwargs)  # all errors thrown by base class are fatal
 
-        if self._dataset_config is not None:
-            try:
-                self.dataset_config.validate()
-            except ValidationErrors as err:
-                errors.extend(err.errors)
+        errors: List[ConfigError] = []
 
-        if self._task is not None and self._dataset_config is not None:
-            try:
-                self._validate_task_dataset()
-            except ValidationErrors as err:
-                errors.extend(err.errors)
-            except ConfigError as err:
-                errors.append(err)
+        try:
+            self.task.validate()
+        except ValidationErrors as err:
+            # If task type is not provided, we cannot continue with validation
+            raise err
 
         if self._metric_configs is not None:
             for metric_config in self._metric_configs.values():
                 try:
                     metric_config.validate()
                 except MetricConfigError as err:
                     errors.append(err)
 
-        if self._cross_validation_config is not None \
-                and self._dataset_config is not None \
-                and self._task is not None:
-            # we need information about the dataset in order to sanity check
-            #   cross-validation settings (i.e., 0 < k <= total number of rows in dataframe)
+        for component in self._plugin_components.values():
             try:
-                pass
-                # train_df = self._dataset_config.load_train().dataframe
-                # self._cross_validation_config.validate(df_row_count=train_df.shape[0])
-            except ProblemDefTypeError as err:
-                errors.append(err)
-            except InvalidValueError as err:
-                errors.append(err)
+                component.validate(problem_def=self)
+            except ValidationErrors as errs:
+                errors.extend(errs.errors)
 
         if len(errors) > 0:
             raise ValidationErrors(errors)
 
-    def _validate_task_dataset(self) -> None:
-        errors: List[ConfigError] = []
-        if self.task.task_type == TaskType.FORECASTING:
-            if RoleName.TIME not in self.dataset_config.roles:
-                errors.append(
-                    DatasetFileError(
-                        'Dataset for forecasting problem must have a time column.\n'
-                        f'Found roles: {self.dataset_config.roles!r}'
-                    )
-                )
-
-            if self.dataset_config.forecasting is None:
-                errors.append(
-                    MissingKeyError(
-                        'Dataset config for forecasting problem must have a forecasting clause.'
-                    )
-                )
-
-        if len(errors) > 0:
-            raise ValidationErrors(errors=errors)
-
-    @property
-    def dataset_config(self) -> DatasetConfig:
-        '''The dataset description.'''
-        assert self._dataset_config is not None, (
-            'BUG: attempt to access dataset_config but it is None.')
-        return self._dataset_config
-
     @property
     def task(self) -> Task:
         '''Explains what kind of problem we're solving.
 
         This affects the selection of pipeline templates and models.
         '''
         assert self._task is not None, (
@@ -271,39 +213,22 @@
         assert self._cross_validation_config is not None, (
             'BUG: attempt to access cross_validation_config but it is None.'
         )
 
         return self._cross_validation_config
 
     @property
-    def instantiations(self) -> List[ExecutorKind]:
-        '''The user requests these kinds of output pipeline instantiations.
-
-        A missing instantions clause defaults to all available kinds.
-        An empty instantions clause disables instantiation.
-        '''
-        inst = self._get_with_default(ProblemDefKeys.OUTPUT, ProblemDefKeys.INSTATIATIONS,
-                                      dflt=Defaults.INSTANTIANTIONS)
-
-        return [ExecutorKind(i.lower()) for i in inst]
-
-    @property
     def output(self) -> OutputConfig:
         '''All the configuration about things to output.'''
         assert self._output_config is not None, (
             'BUG: empty output session should be handled in constructor.'
         )
         return self._output_config
 
     @property
-    def metadata(self) -> Metadata:
-        '''Package config metadata needed by some models.'''
-        return self.dataset_config.metadata
-
-    @property
     def hyperparams(self) -> HyperparamConfig:
         '''Configuration for all hyperparam overrides.'''
         assert self._hyperparam_config is not None, (
             'BUG: self._hyperparam_config is supposed to be set in __init__().')
         return self._hyperparam_config
 
     @property
@@ -314,14 +239,21 @@
         the catalog name of a rank aggregation method.
         See the top level "aggregators" directory.
         '''
         assert self._aggregation_config is not None, (
             'BUG: self._aggregation_config is supposed to be set in __init__().')
         return self._aggregation_config
 
+    def get_conf(self, config_name: Union[str, Enum]) -> ConfigComponent:
+        '''Get the plugin ConfigComponent for the config_name.'''
+        if isinstance(config_name, Enum):
+            config_name = config_name.value
+        assert isinstance(config_name, str)
+        return self._plugin_components[config_name]
+
 
 def remove_comments(entry: Any) -> Any:
     '''Remove '_comments' fields from every dict inside an anonymous object.'''
     if isinstance(entry, dict):
         retval = {
             k: remove_comments(v)
             for k, v in entry.items()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/problem_def_test.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/problem_def_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 '''Tests for problem_def.py'''
-from pathlib import Path
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from pathlib import Path
+import subprocess
+
 import pandas as pd
 import pytest
 
-from ..dataset_formats.local import LocalDatasetConfig
-from ..dataset_formats.memory import MemoryDatasetConfig
-from ..wrangler.dataset import RoleName, Column
-from .config_component import ParsingErrors
+from ..config_components.dataset_config import DatasetConfig
+from ..config_components.impl.config_component import ParsingErrors
 from .output_config import OutputConfigError
 from .problem_def import ProblemDefinition, Task, ValidationErrors
 
-
 # pylint: disable=missing-function-docstring,protected-access
 # pylint: disable=redefined-outer-name
 
 
 @pytest.fixture(scope="session")
 def tmp_path(tmp_path_factory: pytest.TempPathFactory) -> Path:
     return tmp_path_factory.mktemp("data")
@@ -29,15 +28,15 @@
     module_parent = pathobj.parents[2]
     return module_parent
 
 
 TEST_PROBLEM_DEF = '''{
     "_comments" : [
         "A json file fully encapsulating the problem definition",
-        "Specifically, an exmaple time series forecasting problem."
+        "Specifically, an exmaple regression problem."
     ],
     "dataset": {
         "config": "ignore",
         "column_roles": {}
     },
     "problem_type": {
         "task": "regression"
@@ -86,15 +85,17 @@
         },
         "problem_type": {
             "task": "regression"
         },
         "output": {}
     }
     dut = ProblemDefinition(pdef)
-    assert isinstance(dut.dataset_config, LocalDatasetConfig)
+    dataset_config = dut.get_conf(dut.Keys.DATASET)
+    assert isinstance(dataset_config, DatasetConfig)
+    assert 'local' == dataset_config.config
 
 
 MISSING_KEY = '''{
     "metrics" : {}
 }
 '''
 
@@ -165,40 +166,14 @@
 
 
 def test_no_metrics() -> None:
     dut = ProblemDefinition(TEST_PROBLEM_DEF)
     assert dut.metric_configs == {}
 
 
-OPTIONAL_FIELDS = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {}
-    },
-    "problem_type": {
-        "task": "regression"
-    },
-    "template_disable_list": {},
-    "template_enable_list": {},
-    "model_disable_list": {},
-    "model_enable_list": {},
-    "instantiations": [],
-    "hyperparam_search_space": {}
-}
-'''
-
-
-def test_optional_fields() -> None:
-    dut = ProblemDefinition(OPTIONAL_FIELDS)
-    assert set(dut._get().keys()).issuperset(set(
-        ["template_disable_list", "template_enable_list",
-         "model_disable_list", "model_enable_list",
-         "instantiations", "hyperparam_search_space"]))
-
-
 SUNNY_TASK = '''{
     "dataset": {
         "config": "ignore",
         "column_roles": {}
     },
     "problem_type": {
         "data_type": "text",
@@ -254,24 +229,25 @@
         "column_roles": {}
     },
     "problem_type": []
 }'''
 
 
 def test_problem_type_not_dict() -> None:
-    with pytest.raises(ValidationErrors, match=r'dict((.|\n)*)problem_type.task'):
+    with pytest.raises(ValidationErrors,
+                       match=r'(?i)problem_type.*dict'):
         ProblemDefinition(NON_DICT_PROBLEM_TYPE)
 
 
 _DEFAULT_INSTANTIATIONS = sorted(['simple', 'stub_executor_kind'])
 
 
 def test_instantiations_missing() -> None:
     dut = ProblemDefinition(TEST_PROBLEM_DEF)
-    instantiations = dut.instantiations
+    instantiations = dut.output.instantiations
     assert sorted(instantiations) == _DEFAULT_INSTANTIATIONS
 
 
 EMPTY_INSTANTIATIONS = '''{
     "dataset": {
         "config": "ignore",
         "column_roles": {}
@@ -283,16 +259,16 @@
         "instantiations": []
     }
 }'''
 
 
 def test_instantiations_disable() -> None:
     dut = ProblemDefinition(EMPTY_INSTANTIATIONS)
-    instantiations = dut.instantiations
-    assert instantiations == []
+    instantiations = dut.output.instantiations
+    assert not instantiations
 
 
 SIMPLE_INSTANTIATIONS = '''{
     "dataset": {
         "config": "ignore",
         "column_roles": {}
     },
@@ -306,15 +282,15 @@
         ]
     }
 }'''
 
 
 def test_instantiations_sunny_day() -> None:
     dut = ProblemDefinition(SIMPLE_INSTANTIATIONS)
-    instantiations = dut.instantiations
+    instantiations = dut.output.instantiations
     assert set(instantiations) == set({'simple', 'stub_executor_kind'})
 
 
 COMMENTS_PRESENT = '''{
     "metrics" : {},
     "dataset": {
         "config": "ignore",
@@ -359,38 +335,14 @@
 
 @pytest.mark.xfail
 def test_binary_classification_no_pos_label() -> None:
     with pytest.raises(ValidationErrors, match='binary_classification.*pos_label'):
         ProblemDefinition(BINARY_CLASSIFICATION_NO_POS_LABEL)
 
 
-BINARY_CLASSIFICATION_WITH_POS_LABEL = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {
-            "target": {
-                "name": "class",
-                "pos_label": "good"
-            }
-        }
-    },
-    "problem_type": {
-        "task": "binary_classification"
-    }
-}
-'''
-
-
-def test_metadata_binary_classification_with_pos_label() -> None:
-    dut = ProblemDefinition(BINARY_CLASSIFICATION_WITH_POS_LABEL)
-    data = dut.dataset_config.load_train()
-    assert data.roles[RoleName.TARGET] == [Column('class')]
-    assert data.metadata.pos_labels[RoleName.TARGET] == 'good'
-
-
 OUTPUT_DIR = '''{{
     "dataset": {{
         "config": "ignore",
         "column_roles": {{}}
     }},
     "problem_type": {{
         "task": "regression"
@@ -429,245 +381,79 @@
 def test_output_dir_parent_not_exist(tmp_path: Path) -> None:
     nonexistent_parent = tmp_path / 'nonexistent' / 'also_nonexistent'
     pdef_json = OUTPUT_DIR.format(output_path=str(nonexistent_parent))
     with pytest.raises(OutputConfigError):
         _ = ProblemDefinition(pdef_json)
 
 
-FORECASTING_NO_TIME = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {
-            "target": {
-                "name": "class"
-            }
-        },
-        "forecasting": {
-            "horizon": 5,
-            "input_size": 15
-        }
-    },
-    "problem_type": {
-        "task": "forecasting"
-    }
-}
-'''
-
-
-def test_forecasting_no_time() -> None:
-    with pytest.raises(ValidationErrors,
-                       match='(forecasting.*time)|(time.*forecasting)'):
-        ProblemDefinition(FORECASTING_NO_TIME)
-
-
-FORECASTING_NO_HORIZON = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {
-            "target": {
-                "name": "class"
-            },
-            "time": {
-                "name": "FOO"
-            }
-        },
-        "forecasting": {
-            "input_size": 15
-        }
-    },
-    "problem_type": {
-        "task": "forecasting"
-    }
-}
-'''
-
-
-def test_forecasting_no_horizon() -> None:
-    with pytest.raises(ValidationErrors,
-                       match='(forecasting.*horizon)|(horizon.*forecasting)'):
-        ProblemDefinition(FORECASTING_NO_HORIZON)
-
-
-FORECASTING_INVALID_FREQUENCY = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {
-            "target": {
-                "name": "class"
-            },
-            "time": {
-                "name": "FOO"
-            }
-        },
-        "forecasting": {
-            "horizon": 5,
-            "input_size": 15,
-            "frequency": "INVALID_FREQ_FOR_TEST"
-        }
-    },
-    "problem_type": {
-        "task": "forecasting"
-    }
-}
-'''
-
-
-def test_forecasting_invalid_frequency() -> None:
-    with pytest.raises(ValidationErrors,
-                       match='(forecasting.*frequency)|(frequency.*forecasting)'):
-        ProblemDefinition(FORECASTING_INVALID_FREQUENCY)
-
-
-FORECASTING_WITH_FREQUENCY = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {
-            "target": {
-                "name": "class"
-            },
-            "time": {
-                "name": "FOO"
-            }
-        },
-        "forecasting": {
-            "horizon": 5,
-            "input_size": 15,
-            "frequency": "D"
-        }
-    },
-    "problem_type": {
-        "task": "forecasting"
-    }
-}
-'''
-
-
-def test_forecasting_with_frequency() -> None:
-    dut = ProblemDefinition(FORECASTING_WITH_FREQUENCY)
-    got = dut._get('dataset', 'forecasting', 'frequency')
-    want = 'D'
-
-    assert got == want
-
-
-FORECASTING_WITH_DEFAULT_FREQUENCY = '''{
-    "dataset": {
-        "config": "ignore",
-        "column_roles": {
-            "target": {
-                "name": "class"
-            },
-            "time": {
-                "name": "FOO"
-            }
-        },
-        "forecasting": {
-            "horizon": 5,
-            "input_size": 15
-        }
-    },
-    "problem_type": {
-        "task": "forecasting"
-    }
-}
-'''
-
-
-def test_forecasting_with_default_frequency() -> None:
-    dut = ProblemDefinition(FORECASTING_WITH_DEFAULT_FREQUENCY)
-    assert dut.dataset_config.forecasting is not None
-    got = dut.dataset_config.forecasting['frequency']
-    want = 'M'
-
-    assert got == want
-
-
-MEMORY_PROBLEM_DEF = '''{
-    "dataset": {
-        "config": "memory",
-        "column_roles": {
-            "target": {
-                "name": "c"
-            }
-        }
-    },
-    "problem_type": {
-        "task": "binary_classification"
-    }
-}
-'''
-
-
-def test_memory_problem_def() -> None:
-    dataframe = pd.DataFrame(
-        {
-            'a': range(1, 15001),
-            'b': range(1, 15001),
-            'c': range(1, 15001)
-        }
-    )
-    dut = ProblemDefinition(MEMORY_PROBLEM_DEF, train_df=dataframe, test_df=dataframe)
-    dataset = dut.dataset_config.load_test()
-
-    assert isinstance(dut.dataset_config, MemoryDatasetConfig)
-    pd.testing.assert_frame_equal(dataframe, dut.dataset_config.load_train().dataframe)
-
-    assert dataset is not None
-    # drop the target column in the original dataframe because we expect
-    #   `load_test()` to drop the target column
-    pd.testing.assert_frame_equal(dataframe.drop('c', axis=1), dataset.dataframe)
-
-
-def test_missing_dataframe_memory_problem_def() -> None:
-    # expect error message in the exception has one of the following two patterns:
-    #   "memory ... dataframe"
-    #   "dataframe ... memory"
-    with pytest.raises(ValidationErrors, match=r'(memory.*dataframe)|(dataframe.*memory)/i'):
-        ProblemDefinition(MEMORY_PROBLEM_DEF)
-
-
 MEMORY_PROBLEM_DEF_WITH_K = '''{
     "dataset": {
         "config": "memory",
         "column_roles": {
             "target": {
                 "name": "c"
             }
+        },
+        "params": {
+            "train_data": "dataframe"
         }
     },
     "problem_type": {
         "task": "binary_classification"
     },
     "cross_validation": {
         "k": 10
     }
 }
 '''
 
 
 def test_memory_problem_def_with_k() -> None:
-    dataframe = pd.DataFrame(
+    dataframe = pd.DataFrame(  # noqa: F841 pylint: disable=unused-variable
         {
             'a': range(1, 15001),
             'b': range(1, 15001),
             'c': range(1, 15001)
         }
     )
-    dut = ProblemDefinition(MEMORY_PROBLEM_DEF_WITH_K, train_df=dataframe, test_df=dataframe)
+    dut = ProblemDefinition(MEMORY_PROBLEM_DEF_WITH_K)
 
     assert dut.cross_validation_config.k == 10
 
 
 # TODO(piggy): This test relies on validation that was removed to make image processing work.
 # The fix is to add a new catalog for problem defs.
 @pytest.mark.xfail
 def test_memory_problem_def_with_invalid_k() -> None:
-    dataframe = pd.DataFrame(
+    dataframe = pd.DataFrame(  # noqa: F841 pylint: disable=unused-variable
         {
             'a': range(1, 3),
             'b': range(1, 3),
             'c': range(1, 3)
         }
     )
 
     with pytest.raises(ValidationErrors, match=r'(k.*row)|(row.*k)/i'):
-        ProblemDefinition(MEMORY_PROBLEM_DEF_WITH_K, train_df=dataframe, test_df=dataframe)
+        ProblemDefinition(MEMORY_PROBLEM_DEF_WITH_K)
+
+
+def test_plugin_config_component() -> None:
+    '''Test that plugins can add comfig components.'''
+
+    pluginpath = (Path(__file__).parents[2] / 'plugins' / 'testproblemdef'
+                  / 'dist' / 'testproblemdef-0.0.1-py3-none-any.whl')
+    subprocess.run(['python', '-m', 'build'], cwd=pluginpath.parents[1], check=True)
+    subprocess.run(['pip', 'install', pluginpath], check=False)
+    try:
+        ProblemDefinition({
+            'dataset': {
+                'config': 'ignore'
+            },
+            'problem_type': {
+                'task': 'test_task'
+            },
+            'widget_config': {
+                'sprocket': 'sprocket_value'
+            }
+        })
+    finally:
+        subprocess.run(['pip', 'uninstall', '-y', 'testproblemdef'], check=False)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/problem_def/task.py` & `ngautonml-0.4.1b2/ngautonml/problem_def/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 '''Class representing problem type, which is a combination of data type and task.'''
-from typing import List, Optional, Dict, Any
-from enum import Enum, auto
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from .config_component import ConfigComponent, ConfigError
-from .config_component import InvalidKeyError, ValidationErrors, MissingKeyError
-from .config_component import InvalidValueError, ProblemDefTypeError
-from ..wrangler.constants import ProblemDefKeys, ProblemDefKeySet, Defaults
+from typing import Any, Dict, List, Optional, Set
+from enum import Enum, auto
+
+from ..config_components.impl.config_component import (
+    ConfigComponent, ConfigError, ValidationErrors,
+    InvalidValueError, ProblemDefTypeError)
+from ..wrangler.constants import ProblemDefKeys, Defaults
 
 
 class DataType(Enum):
     '''Possible input data types'''
     TABULAR = auto()
     IMAGE = auto()
     TIMESERIES = auto()
@@ -35,44 +36,50 @@
     REGRESSION = auto()
     FORECASTING = auto()
     TEST_TASK = auto()  # Only used in testing
 
     @staticmethod
     def validate(name: str) -> List[str]:
         '''Return an error message if task type is not in the list'''
+
+        # TODO(Merritt/Piggy): figure out how to deal with this without using forecasting
         errors: List[str] = []
         names = [member.name for member in TaskType]
         if name.upper() not in names:
             errors.append(f'"{name}" not among valid task types: f{names}')
         return errors
 
 
 class Task(ConfigComponent):
     '''Parsed form of the problem_type.'''
 
+    class Keys(Enum):
+        '''Top-level keys in Task component'''
+        DATA_TYPE = 'data_type'
+        TASK_TYPE = 'task'
+
+    def required_keys(self) -> Set[str]:
+        '''Subset of ALLOWED_KEYS that are required'''
+        return {self.Keys.TASK_TYPE.value}
+
     def __init__(self, clause: Dict[str, Any], parents: Optional[List[str]] = None):
         parents = self._add_parent(parents, ProblemDefKeys.TASK.value)
         super().__init__(clause=clause, parents=parents)
 
     @property
     def data_type(self) -> DataType:
         '''Data type'''
         return DataType[self._get_with_default(
-            ProblemDefKeys.DATA_TYPE.value,
+            self.Keys.DATA_TYPE,
             dflt=Defaults.DATA_TYPE).upper()]
 
     @property
-    def task_type(self) -> Optional[TaskType]:
+    def task_type(self) -> TaskType:
         '''ML task'''
-        field = self._get_with_default(
-            ProblemDefKeys.TASK_TYPE.value,
-            dflt=None
-        )
-        if field is None:
-            return None
+        field = self._get(self.Keys.TASK_TYPE)
         try:
             return TaskType[field.upper()]
         except KeyError as err:
             raise InvalidValueError(
                 f'task type {field} is not recognized.') from err
 
     def __str__(self) -> str:
@@ -89,35 +96,25 @@
         if isinstance(__value, Task):
             if __value.data_type == self.data_type and __value.task_type == self.task_type:
                 return True
         return False
 
     def validate(self, **kwargs) -> None:
         # test that problem_type maps to a dictionary containing exactly data_type and task_type
+        super().validate(**kwargs)
         errors: List[ConfigError] = []
 
         if isinstance(self._clause, dict):
-            task_keys = set(self._clause.keys())
-            if not ProblemDefKeySet.TASK.REQUIRED.issubset(task_keys):
-                errors.append(MissingKeyError(
-                    'Required keys missing in problem type: '
-                    f'{ProblemDefKeySet.TASK.REQUIRED.difference(task_keys)}'))
-
-            if not task_keys.issubset(ProblemDefKeySet.TASK.ALLOWED):
-                errors.append(InvalidKeyError(
-                    'Invalid key(s) in problem type: '
-                    f'{task_keys.difference(ProblemDefKeySet.TASK.ALLOWED)}'
-                ))
 
-            if ProblemDefKeys.DATA_TYPE.value in self._clause:
-                errmessages = DataType.validate(self._clause[ProblemDefKeys.DATA_TYPE.value])
+            if self.Keys.DATA_TYPE.value in self._clause:
+                errmessages = DataType.validate(self._clause[self.Keys.DATA_TYPE.value])
                 errors = errors + [InvalidValueError(err) for err in errmessages]
 
-            if ProblemDefKeys.TASK_TYPE.value in self._clause:
-                errmessages = TaskType.validate(self._clause[ProblemDefKeys.TASK_TYPE.value])
+            if self.Keys.TASK_TYPE.value in self._clause:
+                errmessages = TaskType.validate(self._clause[self.Keys.TASK_TYPE.value])
                 errors = errors + [InvalidValueError(err) for err in errmessages]
         else:
             errors.append(ProblemDefTypeError(
                 f'{ProblemDefKeys.TASK.value} must be a dict, '
                 f'instead found {type(self._clause)}'))
 
         if len(errors) > 0:
```

### Comparing `ngautonml-0.4.1b1/ngautonml/ranker/ranker.py` & `ngautonml-0.4.1b2/ngautonml/ranker/ranker.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
     @property
     def pipeline_des(self) -> Designator:
         '''Designator for the pipeline that produced this ScoredResult'''
         return self._result.bound_pipeline.designator
 
     @property
+    def family_des(self) -> Designator:
+        '''Family Designator of the pipeline that produced this ScoredResult'''
+        return self._result.bound_pipeline.family_designator
+
+    @property
     def metric(self) -> Metric:
         '''Metric used to evaulate this score'''
         return self._metric
 
     @property
     def result(self) -> PipelineResult:
         '''PipelineResult used to evaulate this score'''
@@ -101,58 +106,74 @@
             if self._unscorable_reason is None:
                 score_str = 'unscorable'
             else:
                 score_str = f'unscorable ({self._unscorable_reason})'
         else:
             score_str = f'{self._score:.4f}'
 
-        return (f'\tpipeline: {self._result.bound_pipeline!s},\n'
+        return (f'\tpipeline: {self._result.bound_pipeline!s}\n'
                 f'\tscore: {score_str}')
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, ScoredResult):
             return False
         return self._metric.name == other._metric.name and self._score == other._score
 
 
 class Ranking:
     '''Holds the result of applying a single metric to multiple ExecutorResult.'''
     _metric: Metric
     _results: PipelineResults
     _scores: List[ScoredResult]
+    _matriarch_scores: List[ScoredResult]
     _ground_truth: Optional[Dataset] = None
 
     def __init__(self,
                  metric: Metric,
                  results: PipelineResults,
                  ground_truth: Optional[Dataset] = None):
         self._metric = metric
         self._results = results
         self._scores = []  # List of ScoredResults, ordered from best to worst
+        self._matriarch_scores = []
         self._ground_truth = ground_truth
         self.score()
 
     def __str__(self):
         retval = f'--{self._metric}--\n'
-        for i, score in enumerate(self._scores):
+        for i, score in enumerate(self.scores()):
+            retval = f'{retval}{i+1}:\n{score}\n'
+        return retval
+
+    @property
+    def str_all_scores(self) -> str:
+        '''Create a string representation of all scores.'''
+        retval = f'--{self._metric}--\n'
+        for i, score in enumerate(self.scores(all_scores=True)):
             retval = f'{retval}{i+1}:\n{score}\n'
         return retval
 
     def score(self) -> None:
         '''Calculate the scores of all results.'''
         self._scores = []
+        family_designators = set()
         for res in self._results.values():
-            if DatasetKeys.ERROR.value in res.prediction:
+            family_designators.add(res.family_designator)
+            if DatasetKeys.ERROR.value in (res.prediction or {}):
+                assert res.prediction is not None, (
+                    'BUG: prediction is None but error is somehow present.')
                 self._scores.append(ScoredResult(
                     metric=self._metric,
                     result=res,
                     unscorable_reason=str(res.prediction[DatasetKeys.ERROR.value])
                 ))
                 continue
             try:
+                if res.prediction is None:
+                    raise MetricInvalidDatasetError('Prediction is None')
                 score = self._metric.calculate(
                     pred=res.prediction,
                     ground_truth=self._ground_truth)
                 scored_result = ScoredResult(
                     metric=self._metric,
                     result=res,
                     score=score)
@@ -164,51 +185,59 @@
             self._scores.append(scored_result)
 
         # We want the best scores first
         # __lt__ on a ScoredResult is defined so that higher=better
         # Thus we always reverse (sort from high to low)
         self._scores.sort(reverse=True)
 
+        # Pick out the highest scoring pipelines in each family,
+        # the "matriarchs".
+        for a_score in self._scores:
+            if a_score.family_des in family_designators:
+                self._matriarch_scores.append(a_score)
+                family_designators.remove(a_score.family_des)
+
     @property
     def metric(self) -> Metric:
         '''The metric used to evaulate this Ranking'''
         return self._metric
 
-    @property
-    def scores(self) -> List[ScoredResult]:
+    def scores(self, all_scores: bool = False) -> List[ScoredResult]:
         '''All ScoredResults, sorted from best to worst.'''
         if len(self._scores) != len(self._results):
             self.score()
-        return self._scores
+        if all_scores:
+            return self._scores
+        return self._matriarch_scores
 
-    @property
-    def scores_as_dict(self) -> Dict[Designator, ScoredResult]:
+    def scores_as_dict(self, all_scores: bool = False) -> Dict[Designator, ScoredResult]:
         '''All ScoredResults, in a dict keyed by their pipeline's Designator.'''
-        return {s.pipeline_des: s for s in self.scores}
+        return {s.pipeline_des: s for s in self.scores(all_scores)}
 
-    def as_dataframe(self) -> pd.DataFrame:
+    def as_dataframe(self, all_scores: bool = False) -> pd.DataFrame:
         '''Return ranking as a dataframe with 2 columns, pipeline designator and score.'''
+        scores = self.scores(all_scores)
         retval = pd.DataFrame()
-        retval[OutputColName.DESIGNATOR.value] = [str(s.pipeline_des) for s in self.scores]
-        retval[self.metric.name] = [s.score for s in self.scores]
+        retval[OutputColName.DESIGNATOR.value] = [str(s.pipeline_des) for s in scores]
+        retval[self.metric.name] = [s.score for s in scores]
         return retval
 
-    def best(self, num: int) -> List[ScoredResult]:
+    def best(self, num: int, all_scores: bool = False) -> List[ScoredResult]:
         '''Return best [num] ScoredResults, in order.'''
-        if num < 0 or num > len(self.scores):
+        if num < 0 or num > len(self.scores(all_scores=all_scores)):
             raise IndexError(
                 f'Cannot get best {num} scores.  '
-                f'Choose a number between 0 and {len(self.scores)}.')
-        return self.scores[:num]
+                f'Choose a number between 0 and {len(self.scores(all_scores=all_scores))}.')
+        return self.scores(all_scores=all_scores)[:num]
 
 
 class RankingStub(Ranking):
     '''stub'''
 
-    def best(self, num: int) -> List[ScoredResult]:
+    def best(self, num: int, all_scores: bool = False) -> List[ScoredResult]:
         return [ScoredResult(
             metric=self._metric,
             result=PipelineResult(
                 prediction=Dataset(),
                 bound_pipeline=BoundPipelineStub(name='stub'),
                 split_dataset=SplitDataset()),
             score=0.0)]
```

### Comparing `ngautonml-0.4.1b1/ngautonml/ranker/ranker_test.py` & `ngautonml-0.4.1b2/ngautonml/ranker/ranker_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 '''Tests for the Ranker class implementations'''
 import re
 from typing import Optional
 
 import pandas as pd
 import pytest
 
+from ..algorithms.connect import ConnectorModel
 from ..executor.executor import ExecutorKind
-from ..generator.bound_pipeline import BoundPipelineStub
+from ..generator.bound_pipeline import BoundPipelineStub, BoundPipeline
 from ..generator.designator import Designator
 from ..instantiator.executable_pipeline import (ExecutablePipelineStub,
                                                 PipelineResult,
                                                 PipelineResults)
 from ..metrics.impl.metric import MetricInvalidDatasetError
 from ..metrics.impl.metric_catalog import Metric
 from ..wrangler.dataset import Dataset
@@ -26,41 +27,41 @@
 # pylint: disable=too-few-public-methods
 # pylint: disable=redefined-outer-name
 
 
 class FakeMetricLow(Metric):
     '''Fake metric where lower is better'''
     _name = 'fake_metric_low'
-    _high = False
+    _tags = {'high': ['false']}
 
     def calculate(self,
                   pred: Dataset,
                   ground_truth: Optional[Dataset] = None) -> float:
         if 'column' not in pred:
             raise MetricInvalidDatasetError('hamster')
         return pred['column'][0]
 
 
 class FakeMetricHigh(Metric):
     '''Fake metric where higher is better'''
     _name = 'fake_metric_high'
-    _high = True
+    _tags = {'high': ['true']}
 
     def calculate(self,
                   pred: Dataset,
                   ground_truth: Optional[Dataset] = None) -> float:
         if 'column' not in pred:
             raise MetricInvalidDatasetError('hamster')
         return pred['column'][0]
 
 
 class FakeMetricAdd(Metric):
     '''Fake metric which adds .5 to whatever FakeMetricHigh returns'''
     _name = 'fake_metric_add'
-    _high = True
+    _tags = {'high': ['true']}
 
     def calculate(self,
                   pred: Dataset,
                   ground_truth: Optional[Dataset] = None) -> float:
         return FakeMetricHigh().calculate(pred, ground_truth) + 0.5
 
 
@@ -191,7 +192,48 @@
         'fake_metric_low': [1.0, 2.0, 'gerbil', 'hamster'],
         'fake_metric_add': [1.5, 2.5, 'gerbil', 'hamster'],
         'fake_metric_high': [1.0, 2.0, 'gerbil', 'hamster']
     })
     got_df = got.as_dataframe(order_metric='fake_metric_low')
     print(got_df)
     pd.testing.assert_frame_equal(want, got_df)
+
+
+def test_family_score() -> None:
+    # Create two pipelines in the same family, with different hyperparams
+    pipeline1 = BoundPipeline(name='base_pipeline')
+    pipeline1.step(model=ConnectorModel(name='model1', param1='some_value')).mark_queried()
+
+    pipeline2 = BoundPipeline(name='base_pipeline')
+    pipeline2.step(model=ConnectorModel(name='model1', param1='another_value')).mark_queried()
+
+    # Create another pipeline with 2 queried connector models
+    #   instead of one so it will not be in the same family
+    other_family_pipe = BoundPipeline(name='base_pipeline')
+    other_family_pipe.step(model=ConnectorModel(name='model1')).mark_queried()
+    other_family_pipe.step(model=ConnectorModel(name='model2')).mark_queried()
+
+    result1 = PipelineResult(
+        executable_pipeline=ExecutablePipelineStub(pipeline=pipeline1),
+        prediction=Dataset(column=[1.0]))
+
+    result2 = PipelineResult(
+        executable_pipeline=ExecutablePipelineStub(pipeline=pipeline2),
+        prediction=Dataset(column=[2.0]))
+
+    result_other_family = PipelineResult(
+        executable_pipeline=ExecutablePipelineStub(pipeline=other_family_pipe),
+        prediction=Dataset(column=[1.5]))
+
+    results = PipelineResults({
+        pipeline1.designator: result1,
+        pipeline2.designator: result2,
+        other_family_pipe.designator: result_other_family,
+    })
+
+    dut = RankerImpl()
+    got = dut.rank(results=results, metrics={'fake_metric_high': FakeMetricHigh()})
+    got_family_scores = got['fake_metric_high'].scores(all_scores=False)
+
+    assert len(got_family_scores) == 2
+    assert got_family_scores[0].pipeline_des == pipeline2.designator
+    assert got_family_scores[1].pipeline_des == other_family_pipe.designator
```

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/frozen_overrides.py` & `ngautonml-0.4.1b2/ngautonml/searcher/frozen_overrides.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/matchers.py` & `ngautonml-0.4.1b2/ngautonml/searcher/matchers.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/matchers_test.py` & `ngautonml-0.4.1b2/ngautonml/searcher/matchers_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 '''Tests for matchers.py'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
+from typing import Optional
 from ..algorithms.impl.algorithm import Algorithm
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
 from ..generator.bound_pipeline import BoundPipeline
 from ..wrangler.constants import Matcher
 from ..wrangler.dataset import Dataset
 
 from .matchers import MatcherFactory
 
-# pylint: disable=missing-class-docstring, missing-function-docstring
+# pylint: disable=missing-class-docstring, missing-function-docstring, duplicate-code
 
 
 class FakeAlgorithmInstance(AlgorithmInstance):
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         return Dataset(dataset.copy())
 
 
 class FakeAlgorithm(Algorithm):
     _name = 'fake_algorithm'
     _default_hyperparams = {
         'base_param': 'base_value',
```

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/param_range.py` & `ngautonml-0.4.1b2/ngautonml/searcher/param_range.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/params.py` & `ngautonml-0.4.1b2/ngautonml/searcher/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,19 @@
         return ','.join(retval)
 
 
 class Override(NamedTuple):
     '''Holds a Selector and its matching Params.'''
     selector: Selector
     params: ParamRanges
+    # This override should not be mentioned in designators.
+    no_show: bool = False
+
+    # TODO(Merritt): Consider a classmethod to simplify simpler
+    # use cases, e.g. Override.fixed_param(selector, name, value)
 
     def __str__(self) -> str:
         return f'Override({self.selector}, {self.params})'
 
 
 class Overrides():
     '''Holds a set of overrides.
@@ -73,20 +78,23 @@
 
     def __init__(self, value: Optional[Iterable[Override]] = None):
         self._value = []
         if value is not None:
             self._value = list(value)
 
     def __iter__(self) -> Generator[Override, None, None]:
-        for over in self._value:
-            yield over
+        yield from self._value
 
     def __len__(self) -> int:
         return len(self._value)
 
+    def copy(self) -> 'Overrides':
+        '''Return a shallow copy of this Overrides.'''
+        return Overrides(self._value)
+
     def append(self, value: Override):
         '''Add one Override.'''
         self._value.append(value)
 
     def extend(self, values: Iterable[Override]):
         '''Add a set of Overrides.'''
         self._value.extend(values)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/params_test.py` & `ngautonml-0.4.1b2/ngautonml/searcher/params_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/searcher.py` & `ngautonml-0.4.1b2/ngautonml/searcher/searcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 '''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import abc
 import logging
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
 from frozendict import frozendict
 
 from ..generator.bound_pipeline import BoundPipeline
 from ..generator.designator import Designator
 from ..problem_def.hyperparam_config import HyperparamConfig
 from ..templates.impl.pipeline_step import PipelineStep
@@ -26,20 +26,23 @@
 from .param_range import ParamRange
 
 
 class Searcher(metaclass=abc.ABCMeta):
     '''Generate new BoundPipelines based on hyperparam search spaces.'''
     _overrides: Overrides
     _disable_grid_search: bool
+    _inject: Optional[Dict[str, Any]]
 
     def __init__(
         self,
-        hyperparams: HyperparamConfig
+        hyperparams: HyperparamConfig,
+        inject: Optional[Overrides] = None
     ):
-        self._overrides = hyperparams.overrides
+        self._overrides = hyperparams.overrides.copy()
+        self._overrides.extend(inject or [])
         self._disable_grid_search = hyperparams.disable_grid_search
 
     @abc.abstractmethod
     def bind_hyperparams(self, pipeline: BoundPipeline) -> Dict[Designator, BoundPipeline]:
         '''Bind new BoundPipelines with revised hyperparameters.'''
 
     def bind_all(self,
@@ -72,31 +75,41 @@
         self._steps = {None: step}
         assert step.has_model(), (
             'BUG: attempt to bind hyperparams for step '
             f'({step.pipeline_designator_component}) with no algorithm')
         self._algorithm = step.model
         self._pipeline_designator_component = step.pipeline_designator_component
 
-    def multiply(self, hyperparam_name: str, param_range: ParamRange) -> 'StepSet':
+    def multiply(self,
+                 hyperparam_name: str,
+                 param_range: ParamRange,
+                 no_show: Set[str]) -> 'StepSet':
         '''Expand the set of steps by the number of values in param.'''
         new_steps: Dict[Optional[frozendict[str, str]], PipelineStep] = {}
         for old_bindings, old_step in self._steps.items():
             bindings: Dict[str, Any] = self._algorithm.bind(
                 hyperparam_name=hyperparam_name, param_range=param_range)
             for new_value_str, new_value in bindings.items():
 
                 new_step = old_step.clone(**{hyperparam_name: new_value})
                 assert new_step.filename is not None
 
-                if old_bindings is None:
-                    # step does not have any pre-existing overrides
-                    new_bindings = frozendict({hyperparam_name: new_value_str})
+                new_bindings: Optional[frozendict[str, str]] = frozendict()
+                if hyperparam_name in no_show:
+                    if old_bindings is not None:
+                        new_bindings = old_bindings
+                    else:
+                        new_bindings = None
                 else:
-                    # step has preexisting overrides
-                    new_bindings = old_bindings.set(hyperparam_name, new_value_str)
+                    if old_bindings is None:
+                        # step does not have any pre-existing overrides
+                        new_bindings = frozendict({hyperparam_name: new_value_str})
+                    else:
+                        # step has preexisting overrides
+                        new_bindings = old_bindings.set(hyperparam_name, new_value_str)
 
                 new_steps[new_bindings] = new_step
         self._steps = new_steps
         return self
 
     @property
     def steps(self) -> Dict[Optional[FrozenOverrides], PipelineStep]:
@@ -183,32 +196,37 @@
         builder = PipelineBuilder(pipeline.name)
         for step in reversed(pipeline.steps):
             default_alg_ranges = ParamRanges(
                 {k: p for k, p in step.hyperparams().items() if isinstance(p, ParamRange)}
             )
             overrides = Overrides(self._overrides)
 
+            no_show: Set[str] = set()  # These are overrides that should not be used in names.
             params = default_alg_ranges.copy()
             for override in overrides:
                 if override.selector.matches(step, pipeline):
                     logging.info('Matched: %s\n\tto step: %s\n\tin pipeline: %s\n',
                                  override,
                                  step.pipeline_designator_component,
                                  pipeline.designator)
                     params.update(override.params)
+                if override.no_show:
+                    no_show.update(override.params.keys())
 
             if len(params) > 0:
                 step_set = StepSet(step)
                 for hyperparam_name, param_range in params.items():
                     range_to_multiply = param_range
                     if self._disable_grid_search:
                         # Replace existing range with fixed range at default
                         range_to_multiply = ParamRange(
                             method=RangeMethod.FIXED,
                             prange=param_range.default)
-                    step_set.multiply(hyperparam_name, range_to_multiply)
+                    step_set.multiply(hyperparam_name=hyperparam_name,
+                                      param_range=range_to_multiply,
+                                      no_show=no_show)
 
                 builder.append(step_set)
             else:
                 builder.append_step(step)
 
         return builder.build()
```

### Comparing `ngautonml-0.4.1b1/ngautonml/searcher/searcher_test.py` & `ngautonml-0.4.1b2/ngautonml/searcher/searcher_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''Tests for searcher.py'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 from ..algorithms.connect import ConnectorModel
 from ..algorithms.impl.algorithm import Algorithm
 from ..algorithms.impl.algorithm_instance import AlgorithmInstance
 from ..generator.bound_pipeline import BoundPipeline
 from ..generator.designator import Designator
 from ..problem_def.hyperparam_config import HyperparamConfig
@@ -27,28 +27,30 @@
     step = PipelineStep(name='some_step',
                         model=ConnectorModel(overridable_param='overridable_value'))
     dut = StepSet(step=step)
 
     # 'multiply' binds all steps in the set.
     # it may increase the number of steps for RangeMethods other than FIXED,
     #   but that is not the case here.
-    dut.multiply('some_param', ParamRange(RangeMethod.FIXED, prange='some_value'))
+    dut.multiply('some_param', ParamRange(RangeMethod.FIXED, prange='some_value'),
+                 no_show=set())
     assert len(dut.steps) == 1
     new_step = list(dut.steps.values())[0]
     assert new_step.filename.endswith('@some_step:some_param=some_value')
     assert "connect_" in new_step.filename
     want_key = FrozenOverrides.freeze({
         new_step.pipeline_designator_component: {'some_param': 'some_value'}})
     assert dut.steps[want_key].hyperparams() == {
         'overridable_param': 'overridable_value',
         'some_param': 'some_value',
     }
 
     # Try another multiply and see that we get a new step.
-    dut.multiply('another_param', ParamRange(RangeMethod.FIXED, 'another_value'))
+    dut.multiply('another_param', ParamRange(RangeMethod.FIXED, 'another_value'),
+                 no_show=set())
     assert len(dut.steps) == 1
     new_step = list(dut.steps.values())[0]
     assert new_step.filename.endswith(
         '@some_step:another_param=another_value,some_param=some_value')
     assert "connect_" in new_step.filename
     want_key = FrozenOverrides.freeze({new_step.pipeline_designator_component: {
         'some_param': 'some_value',
@@ -63,20 +65,22 @@
 
 def test_step_set_filenames():
     PipelineStep.reset_serial_number()
     step = PipelineStep(name='some_step',
                         model=ConnectorModel(overridable_param='overridable_value'))
     dut = StepSet(step=step)
 
-    dut.multiply('some_param', ParamRange(RangeMethod.FIXED, prange='some_value'))
+    dut.multiply('some_param', ParamRange(RangeMethod.FIXED, prange='some_value'),
+                 no_show=set())
     key1 = FrozenOverrides.freeze({'some_step': {'some_param': 'some_value'}})
     assert dut.steps[key1].pipeline_designator_component == 'some_step'
     assert dut.steps[key1].filename == '@connect_1@some_step:some_param=some_value'
 
-    dut.multiply('overridable_param', ParamRange(RangeMethod.FIXED, prange='new_value'))
+    dut.multiply('overridable_param', ParamRange(RangeMethod.FIXED, prange='new_value'),
+                 no_show=set())
 
     key2 = FrozenOverrides.freeze({'some_step': {
         'some_param': 'some_value',
         'overridable_param': 'new_value'}})
     assert dut.steps[key2].pipeline_designator_component == 'some_step'
     assert (
         dut.steps[key2].filename
@@ -84,39 +88,42 @@
 
 
 def test_step_set_filenames_unnamed_step():
     PipelineStep.reset_serial_number()
     step = PipelineStep(model=ConnectorModel(overridable_param='overridable_value'))
     dut = StepSet(step=step)
 
-    dut.multiply('some_param', ParamRange(RangeMethod.FIXED, prange='some_value'))
+    dut.multiply('some_param', ParamRange(RangeMethod.FIXED, prange='some_value'),
+                 no_show=set())
 
     key1 = FrozenOverrides.freeze({
         'connect': {'some_param': 'some_value'}
     })
     assert dut.steps[key1].filename == '@connect_1@:some_param=some_value'
 
 
 def test_step_set_list_sunny_day():
     step = PipelineStep(model=ConnectorModel(overridable_param='overridable_value'),
                         name='some_step')
     dut = StepSet(step=step)
 
     # This is the test.
-    dut.multiply('some_param', ParamRange(RangeMethod.LIST, prange=['list_value1', 'list_value2']))
+    dut.multiply('some_param', ParamRange(RangeMethod.LIST, prange=['list_value1', 'list_value2']),
+                 no_show=set())
 
     key1 = FrozenOverrides.freeze({'some_step': {'some_param': 'list_value1'}})
     key2 = FrozenOverrides.freeze({'some_step': {'some_param': 'list_value2'}})
     assert set(dut.steps.keys()) == {key1, key2}
     assert dut.steps[key1].hyperparams() == {
         'overridable_param': 'overridable_value',
         'some_param': 'list_value1',
     }
     # Can we append a FIXED value to each of those?
-    dut.multiply('another_param', ParamRange(RangeMethod.FIXED, 'another_value'))
+    dut.multiply('another_param', ParamRange(RangeMethod.FIXED, 'another_value'),
+                 no_show=set())
     key3 = FrozenOverrides.freeze({'some_step': {
         'some_param': 'list_value2',
         'another_param': 'another_value'}})
     assert dut.steps[key3].hyperparams() == {
         'overridable_param': 'overridable_value',
         'some_param': 'list_value2',
         'another_param': 'another_value',
@@ -125,26 +132,28 @@
 
 def test_step_set_linear_sunny_day():
     step = PipelineStep(model=ConnectorModel(overridable_param='overridable_value'),
                         name='some_step')
     dut = StepSet(step=step)
 
     # This is the test.
-    dut.multiply('some_param', ParamRange(RangeMethod.LINEAR, prange=[1, 1, 3]))
+    dut.multiply('some_param', ParamRange(RangeMethod.LINEAR, prange=[1, 1, 3]),
+                 no_show=set())
 
     key1 = FrozenOverrides.freeze({'some_step': {'some_param': '1'}})
     key2 = FrozenOverrides.freeze({'some_step': {'some_param': '2'}})
     key3 = FrozenOverrides.freeze({'some_step': {'some_param': '3'}})
     assert set(dut.steps.keys()) == {key1, key2, key3}
     assert dut.steps[key3].hyperparams() == {
         'overridable_param': 'overridable_value',
         'some_param': 3,
     }
     # Can we append a FIXED value to each of those?
-    dut.multiply('another_param', ParamRange(RangeMethod.FIXED, 'another_value'))
+    dut.multiply('another_param', ParamRange(RangeMethod.FIXED, 'another_value'),
+                 no_show=set())
     key4 = FrozenOverrides.freeze({'some_step': {
         'some_param': '2',
         'another_param': 'another_value'}})
     assert dut.steps[key4].hyperparams() == {
         'overridable_param': 'overridable_value',
         'some_param': 2,
         'another_param': 'another_value',
@@ -160,15 +169,16 @@
     step = PipelineStep(model=ConnectorModel(overridable_param='overridable_value'),
                         name='some_step')
     dut = StepSet(step=step)
 
     # This is the test.
     dut.multiply('some_param',
                  ParamRange(method=RangeMethod.LINEAR,
-                            prange=[complex(1, 1), complex(1, 1), complex(3, 3)]))
+                            prange=[complex(1, 1), complex(1, 1), complex(3, 3)]),
+                 no_show=set())
 
     key1 = FrozenOverrides.freeze({'some_step': {'some_param': '(1+1j)'}})
     key2 = FrozenOverrides.freeze({'some_step': {'some_param': '(2+2j)'}})
     key3 = FrozenOverrides.freeze({'some_step': {'some_param': '(3+3j)'}})
     assert set(dut.steps.keys()) == {key1, key2, key3}
     assert dut.steps[key3].hyperparams() == {
         'overridable_param': 'overridable_value',
@@ -241,15 +251,17 @@
     want_des = Designator('some_template@step1')
     assert len(got) == 1
     assert want_des in got
     assert got[want_des].designator == want_des
 
 
 class FakeAlgorithmInstance(AlgorithmInstance):
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         return Dataset(dataset.copy())
 
 
 class FakeAlgorithm(Algorithm):
     _name = 'fake_algorithm'
     _default_hyperparams = {
         'base_param': ParamRange(RangeMethod.LIST, ['a', 'b']),
```

### Comparing `ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter.py` & `ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter_auto.py` & `ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter_auto.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter_auto_test.py` & `ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter_auto_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 '''Tests for splitter_auto.py'''
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from ...problem_def.cross_validation_config import CrossValidationConfig
 from ..k_fold_splitter import KFoldSplitter
-from ..single_fold_splitter import SingleFoldSplitter
 
 from .splitter_auto import SplitterCatalogAuto
 
 # pylint: disable=missing-function-docstring
 
 
 def test_sunny_day() -> None:
     dut = SplitterCatalogAuto(cv_config=CrossValidationConfig({}))
-    single_fold = dut.lookup_by_name('single_fold')
-    assert isinstance(single_fold, SingleFoldSplitter)
+    single_fold = dut.lookup_by_name('sklearn.model_selection.KFold')
+    assert isinstance(single_fold, KFoldSplitter)
 
 
 def test_lookup_by_task_defaults_properly() -> None:
     dut = SplitterCatalogAuto(cv_config=CrossValidationConfig({}))
     single_fold = dut.lookup_by_task('unknown')
     assert isinstance(single_fold, KFoldSplitter)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/splitters/impl/splitter_test.py` & `ngautonml-0.4.1b2/ngautonml/splitters/impl/splitter_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/splitters/k_fold_splitter.py` & `ngautonml-0.4.1b2/ngautonml/splitters/k_fold_splitter.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/splitters/k_fold_splitter_test.py` & `ngautonml-0.4.1b2/ngautonml/splitters/k_fold_splitter_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/parallel_step.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/parallel_step.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/parallel_step_test.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/parallel_step_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_step.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,18 @@
         overrides = {}
         if self._overrides is not None:
             overrides.update(self._overrides)
         bindings = sorted([
             f'{hyperparam}={str(value)}'
             for hyperparam, value in overrides.items()])
 
-        suffix = ''
-        if len(bindings) > 0:
-            suffix = f':{",".join(bindings)}'
+        suffix = f':{",".join(bindings)}' if len(bindings) > 0 else ''
         retval = f'@{self._model.name}_{self._serial_number}@{self._name or ""}{suffix}'
 
-        return StepDesignator(retval)
+        return StepDesignator(retval.lower())
 
     @property
     def serial_number(self) -> int:
         '''Serial number used to ensure that this step's designator is unique'''
         return self._serial_number
 
     def has_model(self) -> bool:
```

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_step_test.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_step_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_template.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_template.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,15 +21,28 @@
 
 
 class UndefinedError(Error):
     '''An undefined variable was referenced.'''
 
 
 class PipelineTemplate(CatalogElementMixin):
-    '''Holds a template for a group of pipelines
+    '''A template for a group of pipelines.
+
+    The :doc:`/_autosummary/ngautonml.generator.generator.Generator`
+    converts a template into several
+    :doc:`/_autosummary/ngautonml.generator.bound_pipeline.BoundPipeline`\\ s.
+
+    The ``Generator`` creates a new ``BoundPipeline`` for each combination of
+    algorithms returned by all the query steps in the template.
+
+    The ``Searcher`` creates new ``BoundPipeline``s out of those created
+    by the ``Generator``, using hyperparameter search.
+
+    Finally, the ``Instantiator`` turns all of these ``BoundPipelines``
+    into ``ExecutablePipelines`` to be run by the ``Executor``.
 
     :name: the unique primary key for this template in the template catalog.
 
     :tags: secondary keys for this template in the template catalog.
         If specified, they override all the tags in the declaration of the class.
 
     '''
@@ -74,36 +87,45 @@
         '''
         child = PipelineTemplate(name=f'{name}',
                                  algorithm_catalog=self._algorithm_catalog,
                                  generator=self._generator)
         return child
 
     def parallel(self, **pipelines: 'PipelineTemplate') -> PipelineStep:
-        '''Add a parallel step.
+        '''Add a parallel step, which contains 2 or more subpipelines.
 
-        Args:
-          A dictionary of output_variable: pipeline.
-          The pipelines should be generated from PipelineTemplate().new().
-        Returns:
-          The new step.
+        Parallel steps allow pipelines to do different things with different parts of the data.
+        For example, running preprocessors on the covariates but not the target column.
+
+        * ``**pipelines``: A dictionary of ``{output_key: pipeline}``.
+          The ``output_key`` for a subpipeline is where the parallel step stores
+          the results in the Dataset,
+          and can be any string, naming the subpipeline.
+          The pipelines should be generated from ``PipelineTemplate().new()``.
+
+        **Returns**: The new parallel step.
         '''
         retval = ParallelStep(model=None,
                               algorithm_catalog=self._algorithm_catalog,
                               generator=self._generator,
                               **pipelines)
         self._steps.append(retval)
         return retval
 
     def query(self, **tags: Union[str, Iterable[str]]) -> PipelineStep:
         '''Creates a query pipeline step and adds it to the template.
 
-        \\*\\*tags looks like::
-            tag_type = tag_value
-            OR
-            tag_type = (tag_value1, tag_value2)
+        A query step queries the ``AlgorithmCatalog`` by tag,
+        and returns a set of ``Algorithms``.
+        The ``Generator`` creates a new ``BoundPipeline``
+        for each element of the cartesian product of
+        all the query steps in the template.
+
+        * ``**tags``: looks like ``tag_type = tag_value`` or
+          ``tag_type = (tag_value1, tag_value2)``
 
         Queries for algorithms that match at least one specified tag value
         for all specified tag types.
         '''
         retval = QueryStep(algorithm_catalog=self._algorithm_catalog, **tags)
         self._steps.append(retval)
         return retval
```

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/pipeline_template_test.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/pipeline_template_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/query_step.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/query_step.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/query_step_test.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/query_step_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/template.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from typing import Dict, List, Union
 
 from ...catalog.catalog import CatalogError
 from ...catalog.memory_catalog import MemoryCatalog
-from ...wrangler.constants import ProblemDefKeys
+from ...problem_def.task import Task
 from .pipeline_template import PipelineTemplate
 
 
 class TemplateRegisterError(CatalogError):
     '''Template missing required keys for registration.'''
 
 
@@ -25,16 +25,16 @@
     def validate(self):
         '''Validate the catalog is capable of generating a pipeline.'''
         errors = []
 
         for obj in self.all_objects():
             final_tags = obj.tags
             # Check that at least one task and data type exists
-            tasks = final_tags[ProblemDefKeys.TASK_TYPE.value]
-            data_types = final_tags[ProblemDefKeys.DATA_TYPE.value]
+            tasks = final_tags[Task.Keys.TASK_TYPE.value]
+            data_types = final_tags[Task.Keys.DATA_TYPE.value]
 
             if 0 == len(tasks):
                 errors.append(TemplateRegisterError(
                     f'No task defined in Template Register for {obj.name}'))
 
             if 0 == len(data_types):
                 errors.append(TemplateRegisterError(
@@ -51,15 +51,15 @@
         tasks = task
 
         if isinstance(task, str):
             tasks = [task]
 
         for tas in tasks:
             results.update(
-                self.lookup_by_tag_and(**{ProblemDefKeys.TASK_TYPE.value: tas}))
+                self.lookup_by_tag_and(**{Task.Keys.TASK_TYPE.value: tas}))
 
         return results
 
     # TODO(piggy): Rewrite this in terms of DataType.
     def lookup_by_datatype(self, data_type: Union[str, List[str]]) -> Dict[str, PipelineTemplate]:
         '''Returns list of all templates that match at least one given task'''
         results: Dict[str, PipelineTemplate] = {}
@@ -67,15 +67,15 @@
         data_types = data_type
 
         if isinstance(data_type, str):
             data_types = [data_type]
 
         for dts in data_types:
             results.update(
-                self.lookup_by_tag_and(**{ProblemDefKeys.DATA_TYPE.value: dts}))
+                self.lookup_by_tag_and(**{Task.Keys.DATA_TYPE.value: dts}))
 
         return results
 
     # TODO(piggy): Rewrite this in terms of ProblemType.
     def lookup_by_both(self,
                        data_type: Union[str, List[str]],
                        task: Union[str, List[str]]
```

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/template_auto.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/template_auto.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/template_auto_test.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/template_auto_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/impl/template_test.py` & `ngautonml-0.4.1b2/ngautonml/templates/impl/template_test.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/tabular_classification.py` & `ngautonml-0.4.1b2/ngautonml/templates/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/templates/tabular_regression.py` & `ngautonml-0.4.1b2/ngautonml/templates/tabular_regression.py`

 * *Files identical despite different names*

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/dataset.py` & `ngautonml-0.4.1b2/ngautonml/data_loaders/impl/dataframe_loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,303 +1,255 @@
-'''Holds a dataset.'''
+'''Base class for loaders that create pandas dataframes.'''
 
-# Copyright (c) 2023 Carnegie Mellon University
+# Copyright (c) 2024 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
-from enum import Enum
-from typing import Any, Dict, List, Optional
+import abc
+import time
+from typing import Any, Dict, Optional, List, Union
 
 import pandas as pd
+from sklearn.model_selection import KFold  # type: ignore[import]
 
-from ..problem_def.task import DataType, TaskType
+from ...config_components.impl.config_component import (
+    ConfigError, ValidationErrors, ParsingErrors)
+from ...config_components.distributed_config import DistributedConfig
+from ...problem_def.task import TaskType
+from ...wrangler.constants import JSONKeys
+from ...wrangler.dataset import Dataset, Column, RoleName, DatasetKeys
+from ...config_components.dataset_config import DatasetFileError
+
+from .data_loader import DataLoader
 
 
 class Error(BaseException):
-    '''Base class for all model-related exceptions.'''
+    '''Base class for all errors in this file.'''
 
 
-class DatasetKeyError(Error, KeyError):
-    '''Raise when a fit() or predict() method is passed an input dataset
-    that is missing required keys.'''
-
-
-class DatasetValueError(Error, ValueError):
-    '''Raise when a dataset has the correct keys but invalid value(s)'''
-
-
-class RoleName(Enum):
-    '''Possible column roles'''
-    INDEX = 'index'
-    TARGET = 'target'
-    ATTRIBUTE = 'attribute'
-
-    # For testing only
-    TEST_ROLE = 'test_role'
-
-    # For time series only
-    TIME = 'time'
-    TIMESERIES_ID = 'timeseries_id'
-    PAST_EXOGENOUS = 'past_exogenous'
-    FUTURE_EXOGENOUS = 'future_exogenous'
-
-
-class Column():
-    '''Defines a column in a dataset'''
-    _name: str
-
-    def __init__(self,
-                 name: str):
-        self._name = name
-
-    @property
-    def name(self) -> str:
-        '''The column's name'''
-        return str(self._name)
-
-    def __eq__(self, other: Any):
-        if not isinstance(other, Column):
-            return False
-        return self.name == other.name
-
-    def __str__(self) -> str:
-        return f'Column({self.name})'
-
-    def __repr__(self) -> str:
-        return f'ngautonml.wrangler.dataset.Column ({self.name})'
-
-
-class DatasetKeys(Enum):
-    '''Standard keys used in the Dataset object passed between models'''
-    DATAFRAME = 'dataframe'
-    TARGET = 'target'
-    COVARIATES = 'covariates'
-    PREDICTIONS = 'predictions'
-    PROBABILITIES = 'probabilities'
-    TRAIN = 'train'
-    VALIDATE = 'validate'
-    GROUND_TRUTH = 'ground_truth'
-    ERROR = 'error'
-
-    # for time series forecasting only
-    STATIC_EXOGENOUS = 'static_exogenous'
-    DYNAMIC_EXOGENOUS = 'dynamic_exogenous'
-
-    # for keras image processing only
-    KERAS_DS = 'keras_ds'
-    KERAS_VALIDATE = 'keras_validate'
-
-
-class Metadata():
-    '''Metadata.'''
-    _roles: Dict[RoleName, List[Column]]
-    _pos_labels: Dict[RoleName, Any]
-    _task: Optional[TaskType]
-    _data_type: Optional[DataType]
-    # Forecast related metadata
-    _horizon: Optional[int]
-    _input_size: Optional[int]
-    _frequency: Optional[str]
-    _step_size: Optional[int]
-
-    def __init__(self,
-                 roles: Optional[Dict[RoleName, List[Column]]] = None,
-                 pos_labels: Optional[Dict[RoleName, Any]] = None,
-                 forecasting: Optional[Dict[str, Any]] = None,
-                 task: Optional[TaskType] = None,
-                 data_type: Optional[DataType] = None) -> None:
-        self._roles = roles or {}
-        self._pos_labels = pos_labels or {}
-        self._horizon = forecasting.get('horizon') if forecasting else None
-        self._input_size = forecasting.get('input_size') if forecasting else None
-        self._frequency = forecasting.get('frequency') if forecasting else None
-        self._step_size = forecasting.get('step_size') if forecasting else None
-        self._task = task
-        self._data_type = data_type
-
-    @property
-    def roles(self) -> Dict[RoleName, List[Column]]:
-        '''roles maps role names to lists of columns with that role.'''
-        return self._roles.copy()
-
-    @property
-    def task(self) -> Optional[TaskType]:
-        '''Data science task that is being approached with this dataset.'''
-        return self._task
-
-    @property
-    def data_type(self) -> Optional[DataType]:
-        '''Type of data contained in this dataset (image, tabular, etc)'''
-        return self._data_type
-
-    @property
-    def target(self) -> Optional[Column]:
-        '''Get name and index of target column if it exists.'''
-        if RoleName.TARGET not in self._roles or len(self._roles[RoleName.TARGET]) == 0:
-            return None
-        assert len(self._roles[RoleName.TARGET]) <= 1, 'Must have at most 1 target column'
-        return self._roles[RoleName.TARGET][0]
+class ColumnError(Error):
+    '''Attempt to select columns in a dataframe that don't exist.'''
+
+
+class DataframeLoader(DataLoader, metaclass=abc.ABCMeta):
+    '''Base class for loaders that create pandas dataframes.'''
+    _train_dataset: Dataset
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self._train_dataset = self._load_train()
+        self._update_roles()
+        self.validate(self._train_dataset)
+
+    def _update_roles(self) -> None:
+        '''Give all unassigned columns the Attribute role.'''
+        assigned_colnames: List[str] = []
+        errors: List[ConfigError] = []
+
+        if self._train_dataset is None:
+            return
+
+        for cols in self._metadata.roles.values():
+            for col in cols:
+                assigned_colnames.append(str(col.name))
+
+        unassigned_colnames = list(
+            set(self._train_dataset.dataframe.columns) - set(assigned_colnames))
+        unassigned_cols = []
+        for colname in unassigned_colnames:
+            unassigned_cols.append(Column(colname))
+
+        updated_roles = self._metadata.roles
+        if RoleName.ATTRIBUTE not in updated_roles:
+            updated_roles[RoleName.ATTRIBUTE] = []
+        updated_roles[RoleName.ATTRIBUTE].extend(unassigned_cols)
 
-    @property
-    def pos_labels(self) -> Dict[RoleName, Any]:
-        '''maps role names to a positive value for columns with that role'''
-        return self._pos_labels.copy()
-
-    @property
-    def horizon(self) -> Optional[int]:
-        '''Gives the forecast horizon (None if not a forecasting problem).'''
-        return self._horizon
-
-    @property
-    def input_size(self) -> Optional[int]:
-        '''Returns the input size of the data (None if not a forecasting problem).'''
-        return self._input_size
-
-    @property
-    def frequency(self) -> Optional[str]:
-        '''Returns the frequency of the data (None if not a forecasting problem).'''
-        return self._frequency
-
-    @property
-    def step_size(self) -> Optional[int]:
-        '''Returns the step_size of the data (None if not a forecasting problem).'''
-        return self._step_size
-
-    def override_roles(self, roles=Dict[RoleName, List[Column]]) -> 'Metadata':
-        '''Return a copy of metadata with new roles.'''
-        return self.__class__(
-            roles=roles,
-            pos_labels=self._pos_labels,
-            forecasting={'horizon': self._horizon,
-                         'input_size': self._input_size,
-                         'frequency': self._frequency})
-
-
-class Dataset(Dict[str, Any]):
-    '''Holds a dataset.
-    Allows for arbitrary keys and values as long as the keys are strings.
-
-    Standard keys: covariates, target, dataframe
-    '''
-    _metadata: Metadata
-
-    def __init__(self,
-                 *args,
-                 metadata: Optional[Metadata] = None,
-                 **kwargs):
-        super().__init__(*args, **kwargs)
-        if metadata is None:
-            metadata = Metadata(roles={}, pos_labels={})
-        self._metadata = metadata
-
-    @property
-    def roles(self) -> Dict[RoleName, List[Column]]:
-        '''Information about column roles in the dataset'''
-        return self._metadata.roles
-
-    @property
-    def metadata(self) -> Metadata:
-        '''Config metadata for use by models'''
-        return self._metadata
-
-    @property
-    def dataframe(self) -> pd.DataFrame:
-        '''Return the dataframe at DatasetKeys.DATAFRAME, or raise an error if it doesn't exist.'''
-
-        if DatasetKeys.DATAFRAME.value not in self:
-            raise DatasetKeyError(
-                f'Attempting to extract key "{DatasetKeys.DATAFRAME.value}" '
-                f'as input, instead found keys {list(self.keys())}.')
-        df_value = self[DatasetKeys.DATAFRAME.value]
-        if not isinstance(df_value, pd.DataFrame):
-            raise DatasetValueError(
-                f'Input key key {DatasetKeys.DATAFRAME.value} must point to '
-                f'a pandas.DataFrame, instead found a {type(df_value)}: '
-                f'{df_value}')
-        return pd.DataFrame(df_value)
-
-    @dataframe.setter
-    def dataframe(self, data: pd.DataFrame) -> None:
-        self[DatasetKeys.DATAFRAME.value] = data
-
-    @property
-    def ground_truth(self) -> pd.DataFrame:
-        '''Return the dataframe at DatasetKeys.GROUND_TRUTH
-
-        or raise an error if it doesn't exist.'''
-
-        if DatasetKeys.GROUND_TRUTH.value not in self:
-            raise DatasetKeyError(
-                f'Attempting to extract key "{DatasetKeys.GROUND_TRUTH.value}" '
-                f'as input, instead found keys {list(self.keys())}.')
-        df_value = self[DatasetKeys.GROUND_TRUTH.value]
-        if not isinstance(df_value, pd.DataFrame):
-            raise DatasetValueError(
-                f'Input key key {DatasetKeys.GROUND_TRUTH.value} must point to '
-                f'a pandas.DataFrame, instead found a {type(df_value)}: '
-                f'{df_value}')
-        return pd.DataFrame(df_value)
-
-    @ground_truth.setter
-    def ground_truth(self, data: pd.DataFrame) -> None:
-        self[DatasetKeys.GROUND_TRUTH.value] = data
-
-    @property
-    def predictions(self) -> pd.DataFrame:
-        '''Return the dataframe at DatasetKeys.PREDICTIONS
-        or raise an error if it doesn't exist.'''
-
-        if DatasetKeys.PREDICTIONS.value not in self:
-            raise DatasetKeyError(
-                f'Attempting to extract key "{DatasetKeys.PREDICTIONS.value}" '
-                f'as input, instead found keys {list(self.keys())}.')
-        df_value = self[DatasetKeys.PREDICTIONS.value]
-        if not isinstance(df_value, pd.DataFrame):
-            raise DatasetValueError(
-                f'Input key key {DatasetKeys.PREDICTIONS.value} must point to '
-                f'a pandas.DataFrame, instead found a {type(df_value)}: '
-                f'{df_value}')
-        return pd.DataFrame(df_value)
-
-    @predictions.setter
-    def predictions(self, data: pd.DataFrame) -> None:
-        self[DatasetKeys.PREDICTIONS.value] = data
+        self._metadata = self._metadata.override_roles(updated_roles)
 
-    @property
-    def probabilities(self) -> pd.DataFrame:
+        # Because train data is already loaded, we need to update its
+        # metadata separately.
+        self._train_dataset._metadata = self._metadata  # pylint: disable=protected-access
+
+        if len(errors) != 0:
+            raise ParsingErrors(errors)
+
+    def _prune_target(self, retval: Dataset) -> Dataset:
+        '''remove target col if it is in data
+
+        called by subclasses in load_test() since test data shouldn't have target
+
+        keep target for forecasting problems
         '''
-        Return the dataframe at `DatasetKeys.PROBABILITIES`
-        or raise an error if it doesn't exist.
+        # TODO(Merritt/Piggy): once we have a forecasting dataloader, we can
+        #   do something more elegant than checking the task type here.
+
+        if self._metadata.task != TaskType.FORECASTING:
+            target = self._metadata.target
+            if target is not None and target.name in retval.dataframe.columns:
+                new_data = retval.dataframe.drop(
+                    labels=target.name, axis=1)
+                retval.dataframe = new_data
+
+        return retval
+
+    def validate(self, dataset: Optional[Dataset]) -> None:
+        '''Raise a ValidationErrors if something about the dataset is inconsistent.'''
+        if dataset is None:
+            return  # A None dataset is valid.
+        if self._train_dataset is None:
+            return  # A None train dataset is valid.
+        errors: List[ConfigError] = []
+        for rolename, cols in self._metadata.roles.items():
+            for col in cols:
+                if col.name not in self._train_dataset.dataframe.columns:
+                    errors.append(DatasetFileError(
+                        f'Column {col.name} specified under role {rolename}'
+                        ' not found among columns in dataset. '
+                        f'Found: {self._train_dataset.dataframe.columns}'))
+        if len(errors) != 0:
+            raise ValidationErrors(errors)
+
+    def load_train(self) -> Optional[Dataset]:
+        self.validate(self._train_dataset)
+        return self._conditional_split(data=self._train_dataset)
+
+    @abc.abstractmethod
+    def _load_train(self) -> Optional[Dataset]:
+        ...
+
+    def load_test(self) -> Optional[Dataset]:
+        '''Load test data if it exists, otherwise None'''
+        retval = self._load_test()
+        if retval is None:
+            return None
+
+        retval = self._prune_target(retval)
+        self.validate(retval)
+        return self._conditional_split(data=retval)
+
+    @abc.abstractmethod
+    def _load_test(self) -> Optional[Dataset]:
+        ...
+
+    def _dataset(self,
+                 data: Any,
+                 key: Union[str, DatasetKeys] = DatasetKeys.DATAFRAME,
+                 cols: Optional[List[str]] = None,
+                 roles: Optional[List[Union[RoleName, str]]] = None,
+                 **kwargs) -> Dataset:
+        '''Load a Dataset object, by placing data at the supplied key.
+
+        As of 2023-12-04 we only know how to handle things we can turn into a pandas DataFrame.
+
+        Args:
+          data:
+            Dataframe or object that can be turned into one.
+          key:
+            The key for the data in the dataset. Defaults to "dataframe".
+          cols:
+            If set, only selects supplied column(s).
+            Will take union with roles if both are specified.
+          roles:
+            If set, only selects columns with supplied role(s).
+            Will take union with cols if both are specified.
         '''
 
-        if DatasetKeys.PROBABILITIES.value not in self:
-            raise DatasetKeyError(
-                f'Attempting to extract key "{DatasetKeys.PROBABILITIES.value}" '
-                f'as input, instead found keys {list(self.keys())}.'
-            )
-
-        df_value = self[DatasetKeys.PROBABILITIES.value]
-
-        if not isinstance(df_value, pd.DataFrame):
-            raise DatasetValueError(
-                f'Input key key {DatasetKeys.PROBABILITIES.value} must point to '
-                f'a pandas.DataFrame, instead found a {type(df_value)}: '
-                f'{df_value}'
-            )
-
-        return pd.DataFrame(df_value)
-
-    @probabilities.setter
-    def probabilities(self, data: pd.DataFrame) -> None:
-        self[DatasetKeys.PROBABILITIES.value] = data
+        retval = Dataset(metadata=self._metadata)
 
-    def output(self, override_metadata: Optional[Metadata] = None) -> 'Dataset':
-        '''Return a new dataset containing same metadata and nothing else.
+        data_df = pd.DataFrame(data)
 
-        Metadata can also be overriden, all preexisting metadata will be lost.
-        Generally called to create a new dataset to fill with a model's output.
-        '''
-        return self.__class__(metadata=override_metadata or self._metadata)
+        # Trim to selected columns if either cols or roles is set.
+        cols_to_select = set()
+        if cols is not None:
+            cols_to_select.update(cols)
+        if roles is not None:
+            for role in roles:
+                if isinstance(role, str):
+                    role = RoleName[role.upper()]
+                cols_to_select.update(
+                    c.name for c in self._metadata.roles[role])
+        if cols_to_select:
+            if cols_to_select.issubset(data_df.columns):
+                data_df = data_df[sorted(cols_to_select)]
+            else:
+                raise ColumnError(
+                    f'selecting columns {cols_to_select} from '
+                    f'dataframe with columns {data_df.columns};'
+                    'not all requested columns are present.'
+                )
+
+        if isinstance(key, str):
+            key = DatasetKeys[key.upper()]
+
+        retval[key.value] = data_df
+        return retval
+
+    def _conditional_split(self, data: Dataset) -> Dataset:
+        '''Split a dataset if we are in a distributed simulation, otherwise do nothing.'''
+        problem_def = self._config.metadata.problem_def
+        if problem_def is None:
+            return data
+
+        distributed = problem_def.get_conf('distributed')
+        assert isinstance(distributed, DistributedConfig), (
+            f'BUG: Expected distributed to be a DistributedConfig, '
+            f'got {type(distributed)} instead.'
+        )
+        distributed_split = distributed.split
+        if distributed_split is None:
+            return data
+
+        # split data for a distributed simulation
+        kfcv = KFold(
+            n_splits=distributed_split.num_nodes,
+            shuffle=True,
+            random_state=distributed_split.seed  # defaults to default seed
+        )
+
+        # 1-based: 1 <= my_id <= num_nodes.
+        n = distributed.my_id
+        # Choose nth split.
+        _, indices = next(
+            (x for i, x in enumerate(
+                kfcv.split(data.dataframe),
+                start=1
+            ) if i == n), (None, None))
+        assert indices is not None, (
+            f'BUG: Could not find {n}th split of {distributed_split.num_nodes} '
+            f'for node {distributed.my_id}'
+        )
+
+        split_df = data.dataframe.iloc[indices]
+        split_df.reset_index(inplace=True, drop=True)
+        retval = data.output()
+        retval.dataframe = split_df
+        return retval
+
+    def poll(self, timeout: Optional[float] = 0.0) -> Optional[Dataset]:
+        next_data = self._poll(timeout=timeout)
+        if next_data is None:
+            return None
+
+        self.validate(next_data)
 
-    def get_dataframe(self) -> pd.DataFrame:
-        '''Return the dataframe at DatasetKeys.DATAFRAME, or raise an error if it doesn't exist.'''
+        return self._conditional_split(data=next_data)
 
-        return self.dataframe
+    def _poll(self, timeout: Optional[float] = 0.0) -> Optional[Dataset]:
+        '''Return the latest unsplit dataset.'''
+        if timeout is not None:
+            time.sleep(timeout)
+        return self._load_train()
+
+    def build_dataset_from_json(self, json_data: Dict) -> Dataset:
+        '''Build a Dataset object from a JSON object.'''
+        retval = Dataset(metadata=self._metadata)
+        data = json_data[JSONKeys.DATA.value]
+        # fit() parameters
+        if DatasetKeys.COVARIATES.value in data and DatasetKeys.TARGET.value in data:
+            covariates = pd.DataFrame(data[DatasetKeys.COVARIATES.value])
+            retval[DatasetKeys.COVARIATES.value] = covariates
+            target = pd.DataFrame(data[DatasetKeys.TARGET.value])
+            retval[DatasetKeys.TARGET.value] = target
+        # predict() parameter
+        if DatasetKeys.DATAFRAME.value in data:
+            dataframe = pd.DataFrame(data[DatasetKeys.DATAFRAME.value])
+            retval[DatasetKeys.DATAFRAME.value] = dataframe
+        return retval
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/dataset_test.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/dataset_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,18 @@
     with pytest.raises(KeyError):
         got['some_key']
 
 
 def test_output_overrides_role():
     roles = {RoleName.TIME: Column('bug')}
     roles2 = {RoleName.TIME: Column('bugs')}
-    dut = Dataset(metadata=Metadata(roles=roles, forecasting={'horizon': 10}))
+    dut = Dataset(metadata=Metadata(roles=roles))
     dut['some_key'] = 'some_val'
     got = dut.output(override_metadata=dut.metadata.override_roles(roles=roles2))
     assert Column('bugs') == got.roles[RoleName.TIME]
-    assert got.metadata.horizon == 10
 
 
 def test_get_dataframe():
     dut = Dataset()
     dataframe = pd.DataFrame({'bug': [1, 2], 'bug2': ['a', 'b']})
     dut.dataframe = dataframe
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/examples_problem_def_test.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/examples_problem_def_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,35 +31,14 @@
     pd_paths_fixed = pd_paths_fixed.replace(
         'ngautonml/examples/regression/diabetes-output',
         str(tmp_path / 'output_dir')
     )
     ProblemDefinition(pd_paths_fixed)  # fails if example json is not valid
 
 
-def test_example_forecasting(tmp_path: Path) -> None:
-    path = module_path() / 'examples' / 'forecasting' / 'air-passengers.json'
-    csv_path = module_path() / 'examples' / 'forecasting' / 'air-passengers-train.csv'
-    test_csv_path = module_path() / 'examples' / 'forecasting' / 'air-passengers-test.csv'
-    with path.open() as file:
-        pd_str = file.read()
-    pd_paths_fixed = pd_str.replace(
-        'ngautonml/examples/forecasting/air-passengers-train.csv',
-        str(csv_path)
-    )
-    pd_paths_fixed = pd_paths_fixed.replace(
-        'ngautonml/examples/forecasting/air-passengers-test.csv',
-        str(test_csv_path)
-    )
-    pd_paths_fixed = pd_paths_fixed.replace(
-        'ngautonml/examples/forecasting/air-passengers-output',
-        str(tmp_path / 'output_dir')
-    )
-    ProblemDefinition(pd_paths_fixed)  # fails if example json is not valid
-
-
 def test_example_tabular_classification(tmp_path: Path):
     pd_path = module_path() / 'examples' / 'classification' / 'credit.json'
     csv_path = module_path() / 'examples' / 'classification' / 'credit-train.csv'
     test_csv_path = module_path() / 'examples' / 'classification' / 'credit-test.csv'
     with pd_path.open() as file:
         pd_str = file.read()
     pd_paths_fixed = pd_str.replace(
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/examples_test.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/examples_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,23 @@
     return module_parent
 
 
 def credit_problem_def():
     train_path = module_path() / 'examples' / 'classification' / 'credit-train.csv'
     pdef = {
         "dataset": {
-            "config": "local",
-            "train_path": train_path,
+            "input_format": "tabular_file",
+            "loaded_format": "pandas_dataframe",
             "column_roles": {
                 "target": {
                     "name": "class"
                 }
+            },
+            "params": {
+                "train_path": train_path,
             }
         },
         "problem_type": {
             "task": "binary_classification"
         },
         "cross_validation": {
             "k": 2
@@ -50,44 +53,41 @@
     dut = Wrangler(
         problem_definition=problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
     got = dut.fit_predict_rank()
 
     assert got.split_dataset.ground_truth is not None
     assert len(got.split_dataset.ground_truth.ground_truth) == 800
-
-    assert list(got.train_results.values())[0].prediction.predictions.shape == (800, 2)
+    got_train_result = list(got.train_results.values())[0].prediction
+    assert got_train_result is not None
+    assert got_train_result.predictions.shape == (800, 2)
 
     # For accuracy, we can't guarantee which pipe will be better, but
     #   we can check that both are present.
-    # We know accuracy will be the first Ranking because they are sorted
-    #   alphabetically by metric name.
     assert 'accuracy_score' in got.rankings
     pipes_included = {
         str(score.result.bound_pipeline.designator)
-        for score in got.rankings['accuracy_score'].scores}
+        for score in got.rankings['accuracy_score'].scores(all_scores=True)}
     assert len(pipes_included) == 18
     assert {
         'tabular_classification@sklearn.linear_model.logisticregression:c=100.0,class_weight=none',
         'tabular_classification@sklearn.svm.svc:c=0.01,class_weight=none'
     }.issubset(pipes_included)
 
     # For roc_auc, we know logistic regression is scorable and svc is unscorable
     #   (because svc cannot produce probabilities output.)
     # As a result, svc will always be ranked last and its score will be
     #   a str stating that it cannot be scored.
     assert 'roc_auc_score' in got.rankings
-    best_score = got.rankings['roc_auc_score'].scores[0]
+    best_score = got.rankings['roc_auc_score'].best(1, all_scores=True)[0]
     best_pipe = str(best_score.pipeline_des)
-    assert best_pipe == (
-        'tabular_classification@sklearn.linear_model.logisticregression:'
-        'c=1.0,class_weight=balanced')
+    assert best_pipe.startswith('tabular_classification@sklearn.linear_model.logisticregression:')
     assert isinstance(best_score.score, float)
 
-    worst_score = got.rankings['roc_auc_score'].scores[-1]
+    worst_score = got.rankings['roc_auc_score'].scores(all_scores=True)[-1]
     assert str(worst_score.pipeline_des) == (
         'tabular_classification@sklearn.svm.svc:c=100.0,class_weight=none')
     assert isinstance(worst_score.score, str)
 
 
 def iris_problem_def():
     train_path = module_path() / 'examples' / 'iris' / 'iris.csv'
@@ -116,24 +116,25 @@
     dut = Wrangler(
         problem_definition=problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
     got = dut.fit_predict_rank()
 
     assert got.split_dataset.ground_truth is not None
     assert len(got.split_dataset.ground_truth.ground_truth) == 150
-
-    assert list(got.train_results.values())[0].prediction.predictions.shape == (150, 2)
+    got_train_results = list(got.train_results.values())[0].prediction
+    assert got_train_results is not None
+    assert got_train_results.predictions.shape == (150, 2)
 
     # For accuracy, we can't guarantee which pipe will be better, but
     #   we can check that both are present.
     # We know accuracy will be the first Ranking because they are sorted
     #   alphabetically by metric name.
     pipes_included = {
         str(score.result.bound_pipeline.designator)
-        for score in got.rankings['accuracy_score'].scores}
+        for score in got.rankings['accuracy_score'].scores(all_scores=True)}
     assert len(pipes_included) == 18
     assert {
         'tabular_classification@sklearn.linear_model.logisticregression:c=100.0,class_weight=none',
         'tabular_classification@sklearn.svm.svc:c=0.01,class_weight=none'
     }.issubset(pipes_included)
 
     # TODO(Merritt): make roc_auc_score work for multiclass
@@ -171,8 +172,10 @@
         problem_definition=problem_definition,
         algorithm_catalog=FakeAlgorithmCatalogAuto
     )
     got = dut.fit_predict_rank()
 
     # there are 442 rows in examples/regression/diabetes.csv
     # we expect train predictions that cover all of them.
-    assert list(got.train_results.values())[0].prediction.predictions.shape == (442, 2)
+    got_train_results = list(got.train_results.values())[0].prediction
+    assert got_train_results is not None
+    assert got_train_results.predictions.shape == (442, 2)
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/saver.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/saver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 '''Save results.'''
 from pathlib import Path
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
-from typing import Dict
+from typing import Dict, Optional
 import pandas as pd
 
 from ..executor.executor_kind import ExecutorKind
 from ..generator.designator import Designator, StepDesignator
 from ..instantiator.executable_pipeline import ExecutablePipeline
 from ..instantiator.executable_pipeline import PipelineResult, PipelineResults
 from ..problem_def.output_config import OutputConfig
 
 from .constants import Filename, FileType, OutputFolder
 from .dataset import Dataset
 
 
-def save_csv(path: Path, filename: Filename, dataset: Dataset) -> None:
+def save_csv(path: Path, filename: Filename, dataset: Optional[Dataset]) -> None:
     '''Save the dataset as a csv at the specified path'''
+    if dataset is None:
+        raise NotImplementedError('Cannot save a None dataset.')
     for key, val in dataset.items():
         outfile = path / (f'{filename.value}_{key}.{FileType.CSV.value}')
         if not isinstance(val, pd.DataFrame):
             raise NotImplementedError(f'Cannot save a {type(val)}.')
         val.to_csv(outfile, index=False)
 
 
-def save_arff(path: Path, filename: Filename, dataset: Dataset) -> None:
+def save_arff(path: Path, filename: Filename, dataset: Optional[Dataset]) -> None:
     '''Save dataset as an arff file.'''
     raise NotImplementedError()
 
 
 Savers = {
     FileType.CSV: save_csv,
     FileType.ARFF: save_arff
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/saver_test.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/saver_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''Tests for the Saver object'''
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 from pathlib import Path
+from typing import Optional
 
 import pandas as pd
 import pytest
 
 from ..algorithms.connect import ConnectorModel
 from ..algorithms.impl.algorithm import Algorithm
 from ..algorithms.impl.fittable_algorithm_instance import FittableAlgorithmInstance
@@ -73,19 +74,19 @@
         return FakeAlgorithmInstance(parent=self, **hyperparams)
 
 
 class FakeAlgorithmInstance(FittableAlgorithmInstance):
     def serialize(self) -> bytes:
         return b'fake algorithm instance model\n'
 
-    def fit(self, dataset: Dataset) -> None:
+    def fit(self, dataset: Optional[Dataset]) -> None:
         _ = dataset
         self._trained = True
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
         return dataset
 
 
 DES1 = StepDesignator('a')
 DES2 = StepDesignator('b')
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/wrangler.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/wrangler_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,137 @@
-"""The wrangler is the central control object for all of AutonML."""
+'''Base class for Wranglers that can fit, predict and rank sets of pipelines.
+
+The Wrangler does the automl pieces, this base class does the rest.
+'''
+
+# Copyright (c) 2024 Carnegie Mellon University
+# This code is subject to the license terms contained in the LICENSE file.
+
+# pylint: disable=too-many-instance-attributes,too-many-arguments
+
+import abc
 import logging
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Type, Union
 
-from ..aggregators.impl.aggregate_ranker import AggregateRanker
 from ..aggregators.impl.aggregator_auto import AggregatorCatalogAuto
 from ..aggregators.impl.aggregator_catalog import AggregatorCatalog
 from ..algorithms.impl.algorithm import AlgorithmCatalog
 from ..algorithms.impl.algorithm_auto import AlgorithmCatalogAuto
 from ..catalog.catalog import Catalog
+from ..communicators.impl.communicator_auto import CommunicatorCatalogAuto
+from ..communicators.impl.communicator_catalog import CommunicatorCatalog
+from ..config_components.dataset_config import DatasetConfig
 from ..cross_validators.impl.cross_validator import CrossValidatorCatalog
 from ..cross_validators.impl.cross_validator_auto import \
     CrossValidatorCatalogAuto
+from ..data_loaders.impl.data_loader import DataLoader
+from ..data_loaders.impl.data_loader_auto import DataLoaderCatalogAuto
+from ..data_loaders.impl.data_loader_catalog import DataLoaderCatalog
+from ..discoverers.impl.discoverer_auto import DiscovererCatalogAuto
+from ..discoverers.impl.discoverer_catalog import DiscovererCatalog
 from ..executor.executor import Executor
 from ..executor.simple.simple_executor import SimpleExecutor
 from ..generator.bound_pipeline import BoundPipeline
 from ..generator.designator import Designator
 from ..generator.generator import Generator, GeneratorImpl
 from ..instantiator.executable_pipeline import (ExecutablePipeline,
-                                                PipelineResult,
                                                 PipelineResults)
 from ..instantiator.instantiator_factory import InstantiatorFactory
 from ..metrics.impl.metric import Metric
 from ..metrics.impl.metric_catalog import MetricCatalog
 from ..metrics.impl.metric_auto import MetricCatalogAuto
+from ..pipeline_loaders.impl.pipeline_loader_auto import PipelineLoaderCatalogAuto
+from ..pipeline_loaders.impl.pipeline_loader_catalog import PipelineLoaderCatalog
 from ..problem_def.problem_def import ProblemDefinition
 from ..ranker.ranker import Ranker, Rankings
 from ..ranker.ranker_impl import RankerImpl
 from ..searcher.searcher import Searcher, SearcherImpl
-from ..splitters.impl.splitter import SplitDataset, SplitterCatalog
+from ..splitters.impl.splitter import SplitterCatalog
 from ..splitters.impl.splitter_auto import SplitterCatalogAuto
 from ..templates.impl.pipeline_template import PipelineTemplate
 from ..templates.impl.template import TemplateCatalog
 from ..templates.impl.template_auto import TemplateCatalogAuto
+
 from .dataset import Dataset
 from .saver import Saver
 
-# Copyright (c) 2023 Carnegie Mellon University
-# This code is subject to the license terms contained in the LICENSE file.
-
-# pylint: disable=too-many-instance-attributes,too-many-arguments
-
 
 class Error(Exception):
     '''Base error for Wrangler.'''
 
 
 class WranglerFailure(Error):
     '''Wrangler can not procede.'''
 
 
 class ReassignmentError(Error):
     '''An attempt was made to assign a value more than once.'''
 
 
-class WranglerResult():
-    '''The results of Wrangler.wrangle.'''
-    _split_dataset: SplitDataset
-    _train_results: PipelineResults
-    _test_results: Optional[PipelineResults]
-    _rankings: Rankings
-
-    def __init__(self,
-                 split_dataset: SplitDataset,
-                 train_results: PipelineResults,
-                 test_results: Optional[PipelineResults],
-                 rankings: Rankings):
-        self._split_dataset = split_dataset
-        self._train_results = train_results
-        self._test_results = test_results
-        self._rankings = rankings
+class WranglerBase(metaclass=abc.ABCMeta):  # pylint: disable=too-many-public-methods
+    '''Base class for Wranglers that can fit, predict and rank sets of pipelines.
 
-    @property
-    def split_dataset(self) -> SplitDataset:
-        '''The ground truth and folds used to rank the pipelines.'''
-        return self._split_dataset
-
-    @property
-    def train_results(self) -> PipelineResults:
-        '''Predictions on train data, acquired using cross-validation.'''
-        return self._train_results
-
-    @property
-    def test_results(self) -> Optional[PipelineResults]:
-        '''Predictions on test data, if supplied in the problem definition.'''
-        return self._test_results
-
-    @property
-    def rankings(self) -> Rankings:
-        '''The rankings of all bound pipelines.'''
-        return self._rankings
-
-    @property
-    def executable_pipelines(self) -> Dict[Designator, ExecutablePipeline]:
-        '''Get all the executable pipelines.'''
-        return self._train_results.executable_pipelines
-
-
-class Wrangler():
-    '''The wrangler is the central control object for all of AutonML.'''
+    The Wrangler does the automl pieces, this base class does the rest.
+    '''
     _bound_pipelines: Optional[Dict[Designator, BoundPipeline]] = None
     # These are all pipelines identified during the first run.
-    _all_pipelines: Optional[Dict[Designator, ExecutablePipeline]] = None
+    _all_executable_pipelines: Optional[Dict[Designator, ExecutablePipeline]] = None
     # This is a subset of _all_pipelines which will be the default
     # for subsequent fit, predict, and rank methods.
-    _current_pipelines: Optional[Dict[Designator, ExecutablePipeline]] = None
+    _current_executable_pipelines: Optional[Dict[Designator, ExecutablePipeline]] = None
 
     def __init__(
         self,
         problem_definition: ProblemDefinition,
-        template_catalog: Optional[Type[TemplateCatalog]] = None,
-        metric_catalog: Optional[Type[MetricCatalog]] = None,
+        aggregator_catalog: Optional[Type[AggregatorCatalog]] = None,
         algorithm_catalog: Optional[Type[AlgorithmCatalog]] = None,
-        generator: Optional[Type[Generator]] = None,
-        searcher: Optional[Type[Searcher]] = None,
+        communicator_catalog: Optional[Type[CommunicatorCatalog]] = None,
+        dataloader_catalog: Optional[Type[DataLoaderCatalog]] = None,
+        discoverer_catalog: Optional[Type[DiscovererCatalog]] = None,
         executor: Optional[Type[Executor]] = None,
-        ranker: Optional[Type[Ranker]] = None,
+        generator: Optional[Type[Generator]] = None,
         instantiator_factory: Optional[Type[InstantiatorFactory]] = None,
-        splitter_catalog: Optional[Type[SplitterCatalog]] = None,
-        validator_catalog: Optional[Type[CrossValidatorCatalog]] = None,
+        metric_catalog: Optional[Type[MetricCatalog]] = None,
+        pipeline_loader_catalog: Optional[Type[PipelineLoaderCatalog]] = None,
+        ranker: Optional[Type[Ranker]] = None,
         saver: Optional[Type[Saver]] = None,
-        aggregator_catalog: Optional[Type[AggregatorCatalog]] = None,
+        searcher: Optional[Type[Searcher]] = None,
+        splitter_catalog: Optional[Type[SplitterCatalog]] = None,
+        template_catalog: Optional[Type[TemplateCatalog]] = None,
+        validator_catalog: Optional[Type[CrossValidatorCatalog]] = None
     ):
         # TODO(Merritt): initialize the logger
         # instantiate default components only if input is None
         self._pd = problem_definition
+
         self._metric_catalog = (metric_catalog or MetricCatalogAuto)()
-        self._algorithm_catalog = (algorithm_catalog or AlgorithmCatalogAuto)()
+        self._communicator_catalog = (communicator_catalog or CommunicatorCatalogAuto)()
+        self._discoverer_catalog = (discoverer_catalog or DiscovererCatalogAuto)()
+        self._algorithm_catalog = (algorithm_catalog or AlgorithmCatalogAuto)(
+            communicator_catalog=self._communicator_catalog,
+            discoverer_catalog=self._discoverer_catalog
+        )
         self._generator = (generator or GeneratorImpl)(
             algorithm_catalog=self._algorithm_catalog,
             problem_definition=self._pd)
         self._template_catalog = (template_catalog or TemplateCatalogAuto)(
             algorithm_catalog=self._algorithm_catalog,
             generator=self._generator
         )
+        self._pipeline_loader_catalog = (pipeline_loader_catalog or PipelineLoaderCatalogAuto)(
+            algorithm_catalog=self._algorithm_catalog,
+            template_catalog=self._template_catalog)
         self._searcher = (searcher or SearcherImpl)(hyperparams=self._pd.hyperparams)
         self._executor = (executor or SimpleExecutor)()
         self._ranker = (ranker or RankerImpl)()
         self._splitter_catalog = (splitter_catalog or SplitterCatalogAuto)(
             cv_config=self._pd.cross_validation_config)
+        self._dataloader_catalog = (dataloader_catalog or DataLoaderCatalogAuto)()
+        self._dataloader: Optional[DataLoader] = None
         self._validator_catalog = (validator_catalog or CrossValidatorCatalogAuto)()
         self._aggregator_catalog = (aggregator_catalog or AggregatorCatalogAuto)()
         self._saver = None
         # If there is no output path, we'll output no files.
         if self._pd.output.path is not None:
             self._saver = (saver or Saver)(self._pd.output)
         self._instantiator_factory = (
@@ -156,227 +145,145 @@
 
     @property
     def algorithm_catalog(self) -> AlgorithmCatalog:
         '''Query and register algorithms'''
         return self._algorithm_catalog
 
     @property
+    def bound_pipelines(self) -> Dict[Designator, BoundPipeline]:
+        '''The set of pipelines that have been bound.'''
+        assert self._bound_pipelines is not None, (
+            'BUG: bound_pipelines accessed before it is set.'
+        )
+        return self._bound_pipelines
+
+    @property
+    def communicator_catalog(self) -> CommunicatorCatalog:
+        '''Query and register communicators'''
+        return self._communicator_catalog
+
+    @property
+    def dataloader_catalog(self) -> DataLoaderCatalog:
+        '''Load data based on input and loaded types.'''
+        return self._dataloader_catalog
+
+    @property
+    def discoverer_catalog(self) -> DiscovererCatalog:
+        '''Query and register discoverers.'''
+        return self._discoverer_catalog
+
+    @property
     def metric_catalog(self) -> Catalog[Metric]:
-        '''Query and register metrics'''
+        '''Query and register metrics.'''
         return self._metric_catalog
 
     @property
+    def pipeline_loader_catalog(self) -> PipelineLoaderCatalog:
+        '''Query and register pipeline loaders.'''
+        return self._pipeline_loader_catalog
+
+    @property
+    def splitter_catalog(self) -> SplitterCatalog:
+        '''Query and register splitters.'''
+        return self._splitter_catalog
+
+    @property
     def template_catalog(self) -> TemplateCatalog:
-        '''Query and register templates'''
+        '''Query and register templates.'''
         return self._template_catalog
 
     @property
+    def validator_catalog(self) -> CrossValidatorCatalog:
+        '''Query and register cross validators.'''
+        return self._validator_catalog
+
+    @property
     def generator(self) -> Generator:
         '''Generates bound pipelines from templates.'''
         return self._generator
 
     @property
     def ranker(self) -> Ranker:
         '''Ranks the results of running pipelines.'''
         return self._ranker
 
-    def load_train_dataset(self) -> Dataset:
-        '''Load self._pd.dataset()'''
-        return self._pd.dataset_config.load_train()
+    def _find_data_loader(self) -> DataLoader:
+        if self._dataloader is not None:
+            return self._dataloader
+        dataset_config = self._pd.get_conf(self._pd.Keys.DATASET.value)
+        assert isinstance(dataset_config, DatasetConfig)
+        self._dataloader = self._dataloader_catalog.construct_instance(dataset_config)
+        return self._dataloader
+
+    def load_train_dataset(self) -> Optional[Dataset]:
+        '''Load this wrangler's train data'''
+        return self._find_data_loader().load_train()
 
     def load_test_dataset(self) -> Optional[Dataset]:
-        '''Load self._pd.dataset()'''
-        return self._pd.dataset_config.load_test()
+        '''Load this wrangler's test data'''
+        return self._find_data_loader().load_test()
 
     def dataset(self, data: Any, **kwargs) -> Dataset:
         '''Load in-memory data into a Dataset object, stored at key 'key'.'''
-        return self._pd.dataset_config.dataset(data, **kwargs)
-
-    def lookup_templates(self) -> Dict[str, PipelineTemplate]:
-        '''Look up the templates that match the problem definition.'''
-        task = self._pd.task
-        data_type = "None"
-        if task.data_type is not None:
-            data_type = task.data_type.name
-        task_type = "None"
-        if task.task_type is not None:
-            task_type = task.task_type.name
-
-        return self._template_catalog.lookup_by_both(
-            data_type=[data_type], task=[task_type])
-
-    def train_all_results(self,
-                          results: PipelineResults,
-                          dataset: Dataset) -> PipelineResults:
-        '''Instantiate and train all pipelines in results.
-
-        Note that we do NOT calculate new predictions.
-        '''
-        retval = PipelineResults()
-        pipelines: Dict[Designator, ExecutablePipeline] = {}
-
-        for des, result in results.items():
-            pipelines[des] = self._instantiator_factory.instantiate(
-                kind=self._executor.kind,
-                pipeline=result.bound_pipeline)
-
-        self._executor.fit(
-            dataset=dataset,
-            pipelines=pipelines)
-
-        for des, pipe in pipelines.items():
-            retval[des] = PipelineResult(
-                prediction=results[des].prediction,
-                split_dataset=results[des].split_dataset,
-                executable_pipeline=pipe)
+        return self._find_data_loader().dataset(data=data, **kwargs)
 
+    def save(self, train_results: PipelineResults) -> Dict[Designator, Path]:
+        '''Save all the models and all the pipelines.'''
+        assert self._saver is not None, 'BUG: Only call save if there is a saver.'
+        retval: Dict[Designator, Path] = {}
+        model_paths = self._saver.save_models(train_results.executable_pipelines)
+        for kind in self._pd.output.instantiations:
+            instantiatior = self._instantiator_factory.build(kind)
+            for des, result in train_results.items():
+                retval[des] = instantiatior.save(result.bound_pipeline, model_paths)
         return retval
 
-    def _predict_test_data(self,
-                           executable_pipelines: Dict[Designator, ExecutablePipeline]
-                           ) -> Optional[PipelineResults]:
-        '''Run the executor again on test data to get test predictions,
-            if test data is supplied in the problem definition.
-
-        (Currently runs all pipelines, may eventually run x best ones)'''
-        assert self._bound_pipelines is not None, (
-            'BUG: wrangle_test() called with no bound pipelines.')
-
-        test_dataset = self.load_test_dataset()
-
-        if test_dataset is None:
-            return None
-
-        test_predictions = self._executor.predict(
-            dataset=test_dataset,
-            pipelines=executable_pipelines)
-        return PipelineResults(test_predictions)
-
-    def fit_predict_rank(self) -> WranglerResult:
-        '''Do all the autoML things.'''
-        train_dataset = self.load_train_dataset()
-
+    def _build_pipelines(self) -> Dict[Designator, BoundPipeline]:
+        '''Build a set of pipelines to use for machine learning'''
         templates = self.lookup_templates()
         if len(templates) == 0:
             raise WranglerFailure(f'found no templates for {self._pd.task}')
         logging.info('Found %d templates', len(templates))
         print(f'Found {len(templates)} templates')
 
         gen_result = self._generator.generate_all(templates)
-        self._bound_pipelines = self._searcher.bind_all(gen_result)
-        logging.info('Generated %d bound pipelines', len(self._bound_pipelines))
-        print(f'Generated {len(self._bound_pipelines)} bound pipelines')
-
-        task = self._pd.task
-        assert task.task_type is not None, (
-            'BUG: missing task should have been caught in validation.')
-        splitters = self._splitter_catalog.lookup_by_tag_and(**{
-            'task': task.task_type.name,
-            'data_type': task.data_type.name,
-        })
-        if not splitters:
-            splitters = self._splitter_catalog.lookup_by_tag_and(**{
-                'default': 'true'
-            })
-        assert len(splitters) == 1, f'BUG: More than one splitter returned for {task}: {splitters}'
-        splitter = list(splitters.values())[0]
-        split_data = splitter.split(
-            dataset=train_dataset,
-            train_frac=self._pd.dataset_config.train_fraction,
-            **self._pd.cross_validation_config.splitter_hyperparams
-        )
-        logging.info('Split dataset into %d folds.', len(split_data.folds))
-        print(f'Split dataset into {len(split_data.folds)} folds.')
+        logging.info("Generated %d bound pipelines", len(gen_result))
+        print(f"Generated {len(gen_result)} bound pipelines")
 
-        cross_validator = self._validator_catalog.lookup_by_name('k_fold_cross_validator')
-        cross_validator_results = PipelineResults(cross_validator.validate_pipelines(
-            split_dataset=split_data,
-            bound_pipelines=self._bound_pipelines,
-            instantiator=self._instantiator_factory,
-            executor=self._executor))
-
-        metrics = self._metric_catalog.lookup_metrics(self._pd)
-        print(f'Got {len(metrics)} metrics.')
-        rankings = self._ranker.rank(
-            results=cross_validator_results,
-            metrics=metrics,
-            ground_truth=split_data.ground_truth)
-        logging.info('Rankings: %s', [str(rank) for rank in rankings])
-
-        methods = [self._aggregator_catalog.lookup_by_name(method)
-                   for method in self._pd.aggregation.method]
-        new_rankings = AggregateRanker(methods=methods,
-                                       rankings=rankings,
-                                       results=cross_validator_results)()
-        rankings.update(new_rankings)
-        print(f'Added {len(new_rankings)} aggregate rankings.')
-
-        train_results = self.train_all_results(
-            results=cross_validator_results,
-            dataset=train_dataset)
-
-        if self._all_pipelines is None:
-            self._all_pipelines = train_results.executable_pipelines
-            self._current_pipelines = self._all_pipelines
-
-        if self._saver is not None:
-            self.save(train_results)
-
-        test_results = self._predict_test_data(train_results.executable_pipelines)
-
-        return WranglerResult(
-            split_dataset=split_data,
-            train_results=train_results,
-            test_results=test_results,
-            rankings=rankings)
+        retval = self._searcher.bind_all(gen_result)
+        logging.info('Hyperparam searcher produced %d bound pipelines', len(retval))
+        print(f'Hyperparam searcher produced {len(retval)} bound pipelines')
 
-    def save(self, train_results: PipelineResults) -> Dict[Designator, Path]:
-        '''Save all the models and all the pipelines.'''
-        assert self._saver is not None, 'BUG: Only call save if there is a saver.'
-        retval: Dict[Designator, Path] = {}
-        model_paths = self._saver.save_models(train_results.executable_pipelines)
-        for kind in self._pd.instantiations:
-            instantiatior = self._instantiator_factory.build(kind)
-            for des, result in train_results.items():
-                retval[des] = instantiatior.save(result.bound_pipeline, model_paths)
         return retval
 
     def fit(self,
-            dataset: Dataset,
+            dataset: Optional[Dataset],
             pipelines: Optional[Dict[Designator, ExecutablePipeline]] = None
             ) -> Dict[Designator, ExecutablePipeline]:
         '''Fit the given pipelines with a new dataset.
 
         If no pipelines are specified, use the current set.
         '''
         if pipelines is None:
-            pipelines = self._current_pipelines
-
-        # Reinstantiate all the pipelines with clean models.
-        assert pipelines is not None, (
-            'BUG: fit called with None current pipelines'
-        )
-        for des, pipeline in pipelines.items():
-            pipelines[des] = self._instantiator_factory.instantiate(
-                kind=self._executor.kind,
-                pipeline=pipeline.bound)
+            pipelines = self._current_executable_pipelines
 
+        assert pipelines is not None
         self._executor.fit(
             dataset=dataset,
             pipelines=pipelines)
 
         return pipelines
 
     def predict(self,
                 new_data: Dataset,
                 trained_pipelines: Optional[
                     Dict[Designator, ExecutablePipeline]] = None) -> PipelineResults:
         '''Predict on new test data that was not supplied in the problem definition.'''
         if trained_pipelines is None:
-            trained_pipelines = self._current_pipelines
+            trained_pipelines = self._current_executable_pipelines
         assert trained_pipelines is not None, (
             'BUG: predict called with None current pipelines.'
         )
         pipeline_errors: List[str] = []
         for des, pipe in trained_pipelines.items():
             if pipe.kind != self._executor.kind:
                 pipeline_errors.append(
@@ -397,21 +304,21 @@
     def set_current(self, *args: str) -> None:
         '''Set the current set of pipelines to work with by name.
 
         If no arguments are given, reset to the full set of pipelines
         identified in the last fit_predict_rank.
         '''
         if len(args) == 0:
-            self._current_pipelines = self._all_pipelines
+            self._current_executable_pipelines = self._all_executable_pipelines
             return
-        if self._all_pipelines is None:
-            self._current_pipelines = None
+        if self._all_executable_pipelines is None:
+            self._current_executable_pipelines = None
             return
-        self._current_pipelines: Dict[Designator, ExecutablePipeline] = {
-            Designator(des): self._all_pipelines[Designator(des)]
+        self._current_executable_pipelines: Dict[Designator, ExecutablePipeline] = {
+            Designator(des): self._all_executable_pipelines[Designator(des)]
             for des in args
         }
 
     def rank(self,
              results: PipelineResults,
              metrics: Optional[Iterable[Union[str, Metric]]] = None,
              ground_truth: Optional[Dataset] = None) -> Rankings:
@@ -434,7 +341,11 @@
 
         if ground_truth is None:
             ground_truth = results.infer_ground_truth()
 
         return self.ranker.rank(results=results,
                                 metrics=metrics_for_ranker,
                                 ground_truth=ground_truth)
+
+    @abc.abstractmethod
+    def lookup_templates(self) -> Dict[str, PipelineTemplate]:
+        '''Look up the templates that match the problem definition.'''
```

### Comparing `ngautonml-0.4.1b1/ngautonml/wrangler/wrangler_test.py` & `ngautonml-0.4.1b2/ngautonml/wrangler/wrangler_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 '''Tests for wrangler.py'''
+
+# Copyright (c) 2024 Carnegie Mellon University
+# This code is subject to the license terms contained in the LICENSE file.
+
+# pylint: disable=missing-function-docstring,duplicate-code,protected-access,too-many-ancestors
+# pylint: disable=missing-class-docstring,redefined-outer-name,unused-variable
+
 import glob
 import json
 import os
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional, Tuple
 
 from numpy.random import RandomState
 import pandas as pd
 import pytest
 
 from ..aggregators.impl.aggregator import AggregatorStub
 from ..algorithms.impl.algorithm import Algorithm
@@ -23,22 +30,17 @@
                                                 PipelineResult)
 from ..problem_def.problem_def import ProblemDefinition
 from ..templates.impl.pipeline_step import PipelineStep
 from ..templates.impl.pipeline_template import PipelineTemplate
 from ..templates.impl.template import TemplateCatalog
 
 from .constants import Defaults
-from .dataset import Dataset, RoleName
-from .wrangler import Wrangler, WranglerFailure
-
-# Copyright (c) 2023 Carnegie Mellon University
-# This code is subject to the license terms contained in the LICENSE file.
-
-# pylint: disable=missing-function-docstring,duplicate-code,protected-access,too-many-ancestors
-# pylint: disable=missing-class-docstring,redefined-outer-name
+from .dataset import Column, Dataset, RoleName
+from .wrangler import Wrangler
+from .wrangler_base import WranglerFailure
 
 
 class FakeExecutor(ExecutorStub):
 
     def predict(self,
                 dataset: Dataset,
                 pipelines: Dict[Designator, ExecutablePipeline]
@@ -58,14 +60,18 @@
 {
     "dataset": {
         "config": "memory",
         "column_roles": {
             "target": {
                 "name": "c"
             }
+        },
+        "params": {
+            "train_data": "train_data",
+            "test_data": "test_data"
         }
     },
     "problem_type": {
         "task": "regression"
     },
     "cross_validation": {
         "k": 10
@@ -81,14 +87,18 @@
 {
     "dataset": {
         "config": "memory",
         "column_roles": {
             "target": {
                 "name": "c"
             }
+        },
+        "params": {
+            "train_data": "train_data",
+            "test_data": "test_data"
         }
     },
     "problem_type": {
         "task": "regression"
     },
     "cross_validation": {
         "k": 10
@@ -102,84 +112,83 @@
         "method": ["method1", "method2"]
     },
     "hyperparams": ["disable_grid_search"]
 }
 '''
 
 
-def memory_problem_def(has_test_data: bool = False,
-                       has_aggregation: bool = False) -> ProblemDefinition:
+def get_data() -> Tuple[pd.DataFrame, Optional[pd.DataFrame]]:
     data = pd.DataFrame(
         {
             'a': range(1, 21),
             'b': range(1, 21),
             'c': range(1, 21)
         }
     )
-    test_data = None
-    if has_test_data:
-        test_data = data
+    return (data, data)
+
 
+def memory_problem_def(has_aggregation: bool = False) -> ProblemDefinition:
     problem_def = MEMORY_PROBLEM_DEF
     if has_aggregation:
         problem_def = AGGREGATION_PROBLEM_DEF
 
-    return ProblemDefinition(
-        problem_def=problem_def,
-        train_df=data,
-        test_df=test_data)
+    return ProblemDefinition(clause=problem_def)
 
 
 def test_init_default() -> None:
     '''Test the components that wrangler defaults to.'''
+    (train_data, test_data) = get_data()  # noqa: F841
     dut = Wrangler(problem_definition=memory_problem_def())
     assert dut._generator.__class__.__name__ == "GeneratorImpl"
     assert dut._template_catalog.__class__.__name__ == "TemplateCatalogAuto"
 
 
 def test_init_custom() -> None:
     '''Test that overriding components when initializing the wrangler works.'''
+    (train_data, test_data) = get_data()  # noqa: F841
     dut = Wrangler(
         problem_definition=memory_problem_def(),
         executor=FakeExecutor,
         template_catalog=FakeTemplateCatalog)
     assert dut._executor.__class__.__name__ == "FakeExecutor"
     assert dut._template_catalog.__class__.__name__ == "FakeTemplateCatalog"
 
     # Testing that non-set arguments are still default
     assert dut._generator.__class__.__name__ == "GeneratorImpl"
 
 
 def test_wrangler_dataset() -> None:
     '''Test wrangler.dataset(), which takes a dataframe and returns a
     dataset containing the dataframe with metadata matching the problem definition.'''
+    (train_data, test_data) = get_data()  # noqa: F841 pylint: disable=unused-variable
     problem_def = memory_problem_def()
-    metadata = problem_def.metadata
-    data = {
+    new_data = {
         'a': range(1, 31),
         'b': range(1, 31),
         'c': range(1, 31),
     }
 
     dut = Wrangler(
         problem_definition=problem_def,
         executor=FakeExecutor)
 
-    got = dut.dataset(data)
+    got = dut.dataset(new_data)
 
     # Confirm that the dataframe matches
     pd.testing.assert_frame_equal(
         got.dataframe,
-        pd.DataFrame(data))
+        pd.DataFrame(new_data))
 
     # Confirm that at least part of the metadata matches.
-    assert got.metadata.roles == metadata.roles
+    assert set(got.metadata.roles[RoleName.ATTRIBUTE]) == {Column('a'), Column('b')}
 
 
 def test_wrangler_split() -> None:
+    (train_data, test_data) = get_data()  # noqa: F841
     problem_def = memory_problem_def()
     dut = Wrangler(
         problem_definition=problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto,
         executor=FakeExecutor)
 
     train_result = dut.fit_predict_rank()
@@ -198,48 +207,55 @@
     #    because it covers the whole dataset,
     #    and 1 col, because it only has the target.
     assert train_result.split_dataset.ground_truth is not None
     assert train_result.split_dataset.ground_truth.ground_truth.shape == (20, 1)
 
 
 def test_fit_predict_rank() -> None:
-    problem_def = memory_problem_def(has_test_data=True)
+    (train_data, test_data) = get_data()  # noqa: F841
+    problem_def = memory_problem_def()
 
     dut = Wrangler(
         problem_definition=problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
 
     got = dut.fit_predict_rank()
 
     # we expect pipelines to be named according to thier template (tabular regression)
     #    and the model that was chosen from thier query step.
     #    in the case of random forest regressor, wrangler will do grid search,
     #    and thus hyperparam values will also be in the designator.
     random_forest_des = Designator('tabular_regression@sklearn.ensemble.randomforestregressor:'
-                                   'max_depth=None,min_samples_split=2')
+                                   'max_depth=none,min_samples_split=2')
     linear_regression_des = Designator('tabular_regression@sklearn.linear_model.linearregression')
     assert {random_forest_des, linear_regression_des} == set(got.executable_pipelines.keys())
 
     assert len(got.train_results) == 2  # 2 pipelines
-    assert got.train_results.predictions[random_forest_des].predictions.shape == (20, 2)
+    got_result = got.train_results.predictions[random_forest_des]
+    assert got_result is not None
+    assert got_result.predictions is not None
+    assert got_result.predictions.shape == (20, 2)
 
     assert len(got.rankings) == 1  # 1 metric
     assert 'root_mean_squared_error' in got.rankings
 
     assert got.test_results is not None
     assert len(got.test_results) == 2  # 2 pipelines
 
     # executable pipelines associated with the test results should be identical
     assert set(got.executable_pipelines.keys()) == set(got.test_results.executable_pipelines.keys())
-
-    assert got.test_results.predictions[random_forest_des].predictions.shape == (20, 1)
+    got_result = got.test_results.predictions[random_forest_des]
+    assert got_result is not None
+    assert got_result.predictions is not None
+    assert got_result.predictions.shape == (20, 1)
 
 
 def test_fit_predict_rank_with_aggregation() -> None:
-    problem_def = memory_problem_def(has_test_data=True, has_aggregation=True)
+    (train_data, test_data) = get_data()  # noqa: F841
+    problem_def = memory_problem_def(has_aggregation=True)
 
     dut = Wrangler(
         problem_definition=problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
 
     dut.aggregator_catalog.register(AggregatorStub(name="method1"))
     dut.aggregator_catalog.register(AggregatorStub(name="method2"))
@@ -274,41 +290,46 @@
             'b': range(1, 21),
             'c': range(1, 21)
         }
     )
 
 
 def test_predict() -> None:
+    (train_data, test_data) = get_data()  # noqa: F841
     problem_def = memory_problem_def()
     executor = SimpleExecutor
     alg_catalog = FakeAlgorithmCatalogAuto
     dut = Wrangler(
         problem_definition=problem_def,
         executor=executor,
         algorithm_catalog=alg_catalog)
     got = dut.fit_predict_rank()
 
     fake_des = Designator('fake_des')
 
     testset = dut.dataset(memory_test_df())
-    result = list(got.train_results.values())[0]
-    pipeline = result.executable_pipeline
+    got_result = list(got.train_results.values())[0]
+    pipeline = got_result.executable_pipeline
     assert pipeline is not None
     test_got = dut.predict(
         new_data=testset,
         trained_pipelines={fake_des: pipeline})
-    prediction_df = test_got[fake_des].prediction.predictions
+    got_result = test_got[fake_des]
+    assert got_result is not None
+    assert got_result.prediction is not None
+    prediction_df = got_result.prediction.predictions
 
     # we expect 10 rows (length of test dataframe) and 1 col (target)
     assert prediction_df.shape == (10, 1)
     # we expect to be able to predict perfectly since test data is identical to train data.
     assert prediction_df['c'][9] == 10.0
 
 
 def test_predict_defaulted() -> None:
+    (train_data, test_data) = get_data()  # noqa: F841
     problem_def = memory_problem_def()
     executor = SimpleExecutor
     alg_catalog = FakeAlgorithmCatalogAuto
     dut = Wrangler(
         problem_definition=problem_def,
         executor=executor,
         algorithm_catalog=alg_catalog)
@@ -316,84 +337,87 @@
 
     testset = dut.dataset(memory_test_df())
     test_got = dut.predict(
         new_data=testset)
     assert {
         'tabular_regression@sklearn.linear_model.linearregression',
         'tabular_regression@sklearn.ensemble.randomforestregressor:'
-        'max_depth=None,min_samples_split=2',
+        'max_depth=none,min_samples_split=2',
     } == set(test_got.keys())
 
 
 def test_set_current_predict() -> None:
+    (train_data, test_data) = get_data()  # noqa: F841
     problem_def = memory_problem_def()
     executor = SimpleExecutor
     alg_catalog = FakeAlgorithmCatalogAuto
     dut = Wrangler(
         problem_definition=problem_def,
         executor=executor,
         algorithm_catalog=alg_catalog)
     _ = dut.fit_predict_rank()
 
     testset = dut.dataset(memory_test_df())
 
     # Pick one pipeline.
     dut.set_current('tabular_regression@sklearn.ensemble.randomforestregressor:'
-                    'max_depth=None,min_samples_split=2')
+                    'max_depth=none,min_samples_split=2')
     test_got = dut.predict(new_data=testset)
     assert set(test_got.keys()) == {
         'tabular_regression@sklearn.ensemble.randomforestregressor:'
-        'max_depth=None,min_samples_split=2',
+        'max_depth=none,min_samples_split=2',
     }
 
     # Reset to all known pipelines.
     dut.set_current()
 
     test_got = dut.predict(new_data=testset)
     assert {
         'tabular_regression@sklearn.linear_model.linearregression',
         'tabular_regression@sklearn.ensemble.randomforestregressor:'
-        'max_depth=None,min_samples_split=2',
+        'max_depth=none,min_samples_split=2',
     } == set(test_got.keys())
 
 
 def test_set_current_fit() -> None:
+    (train_data, test_data) = get_data()
     problem_def = memory_problem_def()
     executor = SimpleExecutor
     alg_catalog = FakeAlgorithmCatalogAuto
     dut = Wrangler(
         problem_definition=problem_def,
         executor=executor,
         algorithm_catalog=alg_catalog)
     _ = dut.fit_predict_rank()
 
     testset = dut.dataset(memory_train_df())
 
     # Pick one pipeline.
     dut.set_current('tabular_regression@sklearn.ensemble.randomforestregressor:'
-                    'max_depth=None,min_samples_split=2')
+                    'max_depth=none,min_samples_split=2')
 
     test_got = dut.fit(dataset=testset)
     assert set(test_got.keys()) == {
         'tabular_regression@sklearn.ensemble.randomforestregressor:'
-        'max_depth=None,min_samples_split=2',
+        'max_depth=none,min_samples_split=2',
     }
 
     # Reset to all known pipelines.
     dut.set_current()
 
     test_got = dut.fit(dataset=testset)
     assert {
         'tabular_regression@sklearn.linear_model.linearregression',
         'tabular_regression@sklearn.ensemble.randomforestregressor:'
-        'max_depth=None,min_samples_split=2',
+        'max_depth=none,min_samples_split=2',
     } == set(test_got.keys())
 
 
 def test_predict_bad_executor_kind() -> None:
+    (train_data, test_data) = get_data()
     problem_def = memory_problem_def()
     executor = SimpleExecutor
     dut = Wrangler(
         problem_definition=problem_def,
         executor=executor)
 
     fake_des = Designator('fake_des')
@@ -402,14 +426,15 @@
     with pytest.raises(WranglerFailure, match=r'(fake_des.*simple)|(simple.*fake_des)/i'):
         dut.predict(
             new_data=Dataset(),
             trained_pipelines={fake_des: stub_pipeline})
 
 
 def test_predict_untrained_pipeline() -> None:
+    (train_data, test_data) = get_data()
     problem_def = memory_problem_def()
     executor = FakeExecutor  # executor kind is 'stub_executor_kind', should match stub pipeline.
     dut = Wrangler(
         problem_definition=problem_def,
         executor=executor)
 
     fake_des = Designator('fake_des')
@@ -429,14 +454,18 @@
     config = {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "task": "regression"
         },
         "cross_validation": {
             "k": 10
@@ -449,29 +478,21 @@
             "instantiations": [
                 "json"
             ],
             "file_type": "csv"
         },
         "hyperparams": ["disable_grid_search"]
     }
-    data = pd.DataFrame(
-        {
-            'a': range(1, 21),
-            'b': range(1, 21),
-            'c': range(1, 21)
-        }
-    )
 
-    return ProblemDefinition(
-        problem_def=config,
-        train_df=data)
+    return ProblemDefinition(clause=config)
 
 
 def test_save_filesystem(saver_problem_def: ProblemDefinition) -> None:
     PipelineStep.reset_serial_number()
+    (train_data, test_data) = get_data()
     dut = Wrangler(
         problem_definition=saver_problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
     _ = dut.fit_predict_rank()
 
     path = saver_problem_def.output.path
     assert path is not None
@@ -503,14 +524,18 @@
     {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "task": "regression"
         },
         "cross_validation": {
             "k": 2
@@ -528,28 +553,21 @@
                         "list": [100, 200]
                     }
                 }
             }
         ]
     }
     '''
-    data = pd.DataFrame(
-        {
-            'a': range(1, 21),
-            'b': range(1, 21),
-            'c': range(1, 21)
-        }
-    )
 
     return ProblemDefinition(
-        problem_def=config,
-        train_df=data)
+        clause=config)
 
 
 def test_hyperparam_search(search_problem_def: ProblemDefinition) -> None:
+    (train_data, test_data) = get_data()
     dut = Wrangler(
         problem_definition=search_problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
     got = dut.fit_predict_rank()
     assert len(got.executable_pipelines) == 25
     assert {
         'tabular_regression@sklearn.linear_model.linearregression',
@@ -566,44 +584,41 @@
     {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "task": "test_task"
         },
         "cross_validation": {
             "k": 3
         },
         "metrics" : {
             "root_mean_squared_error" : {}
         },
         "hyperparams": ["disable_grid_search"]
     }
     '''
-    data = pd.DataFrame(
-        {
-            'a': range(1, 22),
-            'b': range(1, 22),
-            'c': range(2, 23)
-        }
-    )
 
-    return ProblemDefinition(
-        problem_def=config,
-        train_df=data)
+    return ProblemDefinition(clause=config)
 
 
 class FakeInst(FakeInstance):
     '''The instance of a fake algorithm for order tests.'''
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         retval = dataset.output()
         df = pd.DataFrame({'c': dataset.dataframe['a'] + 1})
         retval.predictions = df
         return retval
 
 
 class FakeAlg(Algorithm):
@@ -611,29 +626,40 @@
     _name = 'fake_algorithm'
 
     def instantiate(self, **hyperparams) -> 'FakeInstance':
         return FakeInst(parent=self, **hyperparams)
 
 
 def test_order(order_problem_def) -> None:
+    train_data = pd.DataFrame(
+        {
+            'a': range(1, 22),
+            'b': range(1, 22),
+            'c': range(2, 23)
+        }
+    )
+    test_data = train_data  # noqa: F841 pylint: disable=unused-variable
     dut = Wrangler(
         problem_definition=order_problem_def)
 
     fake_template = PipelineTemplate(
         name='test_template',
         tags={
             'task': ['test_task'],
             'data_type': ['tabular']},
         generator=dut.generator
     )
     fake_template.step(model=FakeAlg())
     dut.template_catalog.register(fake_template)
 
     got = dut.fit_predict_rank()
-    predict_df = got.train_results.predictions[Designator('test_template')].predictions
+    results = got.train_results.predictions[Designator('test_template')]
+    assert results is not None
+    assert results.predictions is not None
+    predict_df = results.predictions
     assert got.split_dataset.ground_truth is not None
     ground_truth_df = got.split_dataset.ground_truth.ground_truth
     pd.testing.assert_frame_equal(predict_df[['c']], ground_truth_df)
     assert all(predict_df['c'] == predict_df['ground truth'])
 
 
 def non_seeded_problem_def() -> ProblemDefinition:
@@ -641,49 +667,55 @@
     {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "task": "test_task"
         },
         "cross_validation": {
             "k": 2
         },
         "metrics" : {
             "root_mean_squared_error" : {}
         },
         "hyperparams": ["disable_grid_search"]
     }
     '''
-    data = pd.DataFrame(
+    train_data = pd.DataFrame(  # noqa: F841 pylint: disable=unused-variable
         {
             'a': range(1, 21),
             'b': range(1, 21),
             'c': range(2, 22)
         }
     )
 
-    return ProblemDefinition(
-        problem_def=config,
-        train_df=data)
+    return ProblemDefinition(clause=config)
 
 
 def seeded_problem_def(seed: int) -> ProblemDefinition:
     config = {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "task": "test_task"
         },
         "cross_validation": {
             "k": 2
@@ -703,36 +735,36 @@
                     "random_seed": {
                         "fixed": seed
                     }
                 }
             }
         ]
     }
-    data = pd.DataFrame(
+    train_data = pd.DataFrame(  # noqa: F841 pylint: disable=unused-variable
         {
             'a': range(1, 21),
             'b': range(1, 21),
             'c': range(2, 22)
         }
     )
 
-    return ProblemDefinition(
-        problem_def=config,
-        train_df=data)
+    return ProblemDefinition(clause=config)
 
 
 class RandomAlgorithmInstance(AlgorithmInstance):
     _rng: RandomState
 
     def __init__(self, parent: Algorithm, **hyperparams):
         super().__init__(parent)
         if 'random_seed' in hyperparams:
             self._rng = RandomState(hyperparams['random_seed'])
 
-    def predict(self, dataset: Dataset) -> Dataset:
+    def predict(self, dataset: Optional[Dataset]) -> Optional[Dataset]:
+        if dataset is None:
+            return None
         retval = dataset.output()
         retval['predictions'] = pd.DataFrame({
             'c': list(self._rng.randint(0, 10, len(dataset.dataframe)))
         }).reset_index(drop=True)
         return retval
 
 
@@ -748,14 +780,15 @@
     }
 
     def instantiate(self, **hyperparams) -> RandomAlgorithmInstance:
         return RandomAlgorithmInstance(parent=self, **self.hyperparams(**hyperparams))
 
 
 def test_set_seed() -> None:
+    (train_data, test_data) = get_data()
     dut_def = Wrangler(problem_definition=non_seeded_problem_def())
     dut5678 = Wrangler(problem_definition=seeded_problem_def(5678))
 
     pipe_def = PipelineTemplate(
         name='test_template',
         tags={
             'task': ['test_task'],
@@ -777,16 +810,22 @@
 
     got_def = dut_def.fit_predict_rank()
     got5678 = dut5678.fit_predict_rank()
 
     des_def = Designator('test_template')
     des5678 = Designator('test_template@random_algorithm:random_seed=5678')
 
-    predictions_def = got_def.train_results[des_def].prediction.predictions[['c']]
-    predictions5678 = got5678.train_results[des5678].prediction.predictions[['c']]
+    got_def_train_results_des_def = got_def.train_results[des_def]
+    got5678_train_results_des5678 = got5678.train_results[des5678]
+
+    assert got_def_train_results_des_def.prediction is not None
+    assert got5678_train_results_des5678.prediction is not None
+
+    predictions_def = got_def_train_results_des_def.prediction.predictions[['c']]
+    predictions5678 = got5678_train_results_des5678.prediction.predictions[['c']]
 
     # The k-fold-cross-validator instantiates the algorithm separately
     # for each fold, so in this special case, we expect to see the same
     # sequence twice.
 
     want_def = pd.DataFrame({'c': [3, 3, 6, 2, 1, 8, 5, 1, 7, 3, 3, 3, 6, 2, 1, 8, 5, 1, 7, 3]})
     want5678 = pd.DataFrame({'c': [5, 3, 6, 9, 3, 3, 9, 8, 3, 3, 5, 3, 6, 9, 3, 3, 9, 8, 3, 3]})
@@ -800,14 +839,18 @@
     {
         "dataset": {
             "config": "memory",
             "column_roles": {
                 "target": {
                     "name": "c"
                 }
+            },
+            "params": {
+                "train_data": "train_data",
+                "test_data": "test_data"
             }
         },
         "problem_type": {
             "task": "regression"
         },
         "cross_validation": {
             "k": 2
@@ -828,30 +871,22 @@
                     }
                 }
             }
         ],
         "output": {}
     }
     '''
-    data = pd.DataFrame(
-        {
-            'a': range(1, 21),
-            'b': range(1, 21),
-            'c': range(1, 21)
-        }
-    )
 
-    return ProblemDefinition(
-        problem_def=config,
-        train_df=data)
+    return ProblemDefinition(clause=config)
 
 
 def test_disable_grid_search(disable_grid_search_problem_def: ProblemDefinition) -> None:
+    (train_data, test_data) = get_data()
     dut = Wrangler(
         problem_definition=disable_grid_search_problem_def,
         algorithm_catalog=FakeAlgorithmCatalogAuto)
     got = dut.fit_predict_rank()
     assert {
         'tabular_regression@sklearn.linear_model.linearregression',
         'tabular_regression@sklearn.ensemble.randomforestregressor'
-        ':max_depth=None,min_samples_split=2,n_estimators=100'
+        ':max_depth=none,min_samples_split=2,n_estimators=100'
     } == set(got.executable_pipelines.keys())
```

### Comparing `ngautonml-0.4.1b1/picard.py` & `ngautonml-0.4.1b2/picard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/python
+#!/bin/env python
 """Main for AutonML."""
 
 # Copyright (c) 2023 Carnegie Mellon University
 # This code is subject to the license terms contained in the LICENSE file.
 
 import argparse
 import logging
@@ -15,14 +15,15 @@
 from ngautonml.generator.generator import GeneratorImpl
 from ngautonml.instantiator.instantiator_factory import InstantiatorFactory
 from ngautonml.metrics.impl.metric_auto import MetricCatalogAuto
 from ngautonml.problem_def.problem_def import ProblemDefinition
 from ngautonml.ranker.ranker_impl import RankerImpl
 from ngautonml.templates.impl.template_auto import TemplateCatalogAuto
 from ngautonml.wrangler.wrangler import Wrangler
+from ngautonml.wrangler.distributed_wrangler import DistributedWrangler
 
 logging.basicConfig(level=logging.ERROR)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 def wrangle(args: argparse.Namespace):
@@ -50,14 +51,25 @@
     """Instantiate one or more pipelines.
 
     Optionally includes a trained model in the instantiated pipeline.
     """
     print(f'Instantiate: {args!r}')
 
 
+def distributed(args: argparse.Namespace):
+    """Stand up a distributed node."""
+    with open(args.problem_definition, 'r', encoding='utf8') as _f:
+        problem_definition = ProblemDefinition(_f.read())
+    logging.info('%s', problem_definition)
+    wrangler = DistributedWrangler(
+        problem_definition=problem_definition,
+        my_id=args.my_id)
+    wrangler.server(host=args.host, port=args.port)()
+
+
 def usage(parser: argparse.ArgumentParser) -> Callable[
         [argparse.Namespace], None]:
     """Returns a function that prints the usage message."""
     def _f(_args: argparse.Namespace):
         parser.print_usage(sys.stderr)
     return _f
 
@@ -104,13 +116,42 @@
     parser_instantiate.add_argument(
         '-m', '--trained_model',
         action='append',
         help='optional path to the trained model to instantiate. '
         'May be repeated.'
     )
 
+    parser_distributed = sub_parsers.add_parser('distributed',
+                                                help='Start up a server running '
+                                                'a set of distributed algorithms.')
+    parser_distributed.set_defaults(func=distributed)
+    parser_distributed.add_argument(
+        '-d', '--problem_definition',
+        type=str,
+        help='path to problem definition JSON file',
+        required=True)
+    parser_distributed.add_argument(
+        '-i', '--my_id',
+        type=int,
+        help='Node number of the server',
+        required=False,
+        default=1
+    )
+    parser_distributed.add_argument(
+        '-H', '--host',
+        type=str,
+        help='Host name or IP address of web API',
+        default='localhost',
+    )
+    parser_distributed.add_argument(
+        '-P', '--port',
+        type=int,
+        help='Port number of web API',
+        default=60080,
+    )
+
     a = parser_global.parse_args()
     a.func(a)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ngautonml-0.4.1b1/pyproject.toml` & `ngautonml-0.4.1b2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "ngautonml"
-version = "0.4.1b01"
+version = "0.4.1b02"
 description = "Automated Machine Learning Pipeline Generation"
 authors = [
     "L.H. Piggy Yarroll <piggy@cmu.edu>",
     "Merritt Kowaleski <merrittk@cmu.edu>",
     "Andrew Williams <awillia2@andrew.cmu.edu>",
-    "Jieshi Chen <jieshic@andrew.cmu.edu>"
+    "Jieshi Chen <jieshic@andrew.cmu.edu>",
+    "Dan Howarth <howarth@cmu.edu>"
 ]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
     "picard.py",
     "*.ipynb",
 ]
```

### Comparing `ngautonml-0.4.1b1/PKG-INFO` & `ngautonml-0.4.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngautonml
-Version: 0.4.1b1
+Version: 0.4.1b2
 Summary: Automated Machine Learning Pipeline Generation
 Home-page: https://gitlab.com/autonlab/ngautonml
 License: Apache-2.0
 Keywords: machine learning
 Author: L.H. Piggy Yarroll
 Author-email: piggy@cmu.edu
 Requires-Python: >=3.9,<4.0
```

