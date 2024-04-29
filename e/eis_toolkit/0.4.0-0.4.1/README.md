# Comparing `tmp/eis_toolkit-0.4.0.tar.gz` & `tmp/eis_toolkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis_toolkit-0.4.0.tar", max compression
+gzip compressed data, was "eis_toolkit-0.4.1.tar", max compression
```

## Comparing `eis_toolkit-0.4.0.tar` & `eis_toolkit-0.4.1.tar`

### file list

```diff
@@ -1,102 +1,104 @@
--rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.4.0/LICENSE
--rwxr-xr-x   0        0        0     5397 2024-03-06 08:49:18.301086 eis_toolkit-0.4.0/README.md
--rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.4.0/eis_toolkit/__init__.py
--rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.4.0/eis_toolkit/__main__.py
--rw-r--r--   0        0        0    97345 2024-04-17 10:08:54.947934 eis_toolkit-0.4.0/eis_toolkit/cli.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/conversions/__init__.py
--rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.4.0/eis_toolkit/conversions/csv_to_geodataframe.py
--rw-r--r--   0        0        0     1784 2024-04-09 09:00:19.128132 eis_toolkit-0.4.0/eis_toolkit/conversions/raster_to_dataframe.py
--rw-r--r--   0        0        0     2643 2024-02-22 09:12:29.156927 eis_toolkit-0.4.0/eis_toolkit/exceptions.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/__init__.py
--rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
--rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/chi_square_test.py
--rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/correlation_matrix.py
--rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/covariance_matrix.py
--rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/dbscan.py
--rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/descriptive_statistics.py
--rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/feature_importance.py
--rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/k_means_cluster.py
--rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/local_morans_i.py
--rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/normality_test.py
--rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/parallel_coordinates.py
--rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/pca.py
--rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/plot_utils.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/prediction/__init__.py
--rw-r--r--   0        0        0     5228 2024-04-17 10:08:54.947934 eis_toolkit-0.4.0/eis_toolkit/prediction/fuzzy_overlay.py
--rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.4.0/eis_toolkit/prediction/gradient_boosting.py
--rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.4.0/eis_toolkit/prediction/logistic_regression.py
--rw-r--r--   0        0        0    17660 2024-04-16 07:29:55.248116 eis_toolkit-0.4.0/eis_toolkit/prediction/machine_learning_general.py
--rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.4.0/eis_toolkit/prediction/mlp.py
--rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.4.0/eis_toolkit/prediction/random_forests.py
--rw-r--r--   0        0        0    17398 2024-03-04 07:36:07.783856 eis_toolkit-0.4.0/eis_toolkit/prediction/weights_of_evidence.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/raster_processing/__init__.py
--rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/clipping.py
--rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/create_constant_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/__init__.py
--rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/classification.py
--rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/parameters.py
--rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
--rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/utilities.py
--rw-r--r--   0        0        0    10167 2024-04-03 09:32:00.769041 eis_toolkit-0.4.0/eis_toolkit/raster_processing/distance_to_anomaly.py
--rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/extract_values_from_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/__init__.py
--rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/focal.py
--rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/kernels.py
--rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/speckle.py
--rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/utilities.py
--rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.4.0/eis_toolkit/raster_processing/reclassify.py
--rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.4.0/eis_toolkit/raster_processing/reprojecting.py
--rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.4.0/eis_toolkit/raster_processing/resampling.py
--rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.4.0/eis_toolkit/raster_processing/snapping.py
--rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.4.0/eis_toolkit/raster_processing/unifying.py
--rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/raster_processing/unique_combinations.py
--rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.4.0/eis_toolkit/raster_processing/windowing.py
--rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/training_data_tools/__init__.py
--rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.4.0/eis_toolkit/training_data_tools/class_balancing.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/transformations/__init__.py
--rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.4.0/eis_toolkit/transformations/binarize.py
--rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/clip.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/transformations/coda/__init__.py
--rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/coda/alr.py
--rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/coda/clr.py
--rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/coda/ilr.py
--rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/coda/pairwise.py
--rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/coda/plr.py
--rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/linear.py
--rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/logarithmic.py
--rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/one_hot_encoding.py
--rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/transformations/sigmoid.py
--rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.4.0/eis_toolkit/transformations/winsorize.py
--rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.4.0/eis_toolkit/utilities/__init__.py
--rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.4.0/eis_toolkit/utilities/aitchison_geometry.py
--rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/utilities/checks/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.4.0/eis_toolkit/utilities/checks/compositional.py
--rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/utilities/checks/dataframe.py
--rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/utilities/checks/geometry.py
--rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/utilities/checks/parameter.py
--rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.4.0/eis_toolkit/utilities/checks/raster.py
--rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/utilities/conversions.py
--rw-r--r--   0        0        0     8640 2024-04-17 10:08:54.947934 eis_toolkit-0.4.0/eis_toolkit/utilities/file_io.py
--rw-r--r--   0        0        0    12203 2024-04-17 10:08:54.947934 eis_toolkit-0.4.0/eis_toolkit/utilities/miscellaneous.py
--rw-r--r--   0        0        0     4947 2024-04-17 10:08:54.951934 eis_toolkit-0.4.0/eis_toolkit/utilities/nodata.py
--rw-r--r--   0        0        0     4082 2024-04-17 10:08:54.951934 eis_toolkit-0.4.0/eis_toolkit/utilities/raster.py
--rwxr-xr-x   0        0        0        0 2022-09-27 06:51:57.621043 eis_toolkit-0.4.0/eis_toolkit/validation/__init__.py
--rw-r--r--   0        0        0     1415 2024-04-16 07:29:55.252116 eis_toolkit-0.4.0/eis_toolkit/validation/calculate_auc.py
--rw-r--r--   0        0        0     4577 2024-02-22 09:12:29.164927 eis_toolkit-0.4.0/eis_toolkit/validation/calculate_base_metrics.py
--rw-r--r--   0        0        0     2484 2024-04-16 07:29:55.252116 eis_toolkit-0.4.0/eis_toolkit/validation/get_pa_intersection.py
--rw-r--r--   0        0        0     1794 2024-04-16 07:29:55.252116 eis_toolkit-0.4.0/eis_toolkit/validation/plot_confusion_matrix.py
--rw-r--r--   0        0        0     2644 2024-04-15 11:24:32.422063 eis_toolkit-0.4.0/eis_toolkit/validation/plot_nn_model_performance.py
--rw-r--r--   0        0        0     3289 2024-04-16 07:29:55.252116 eis_toolkit-0.4.0/eis_toolkit/validation/plot_prediction_area_curves.py
--rw-r--r--   0        0        0     2682 2024-04-16 07:29:55.252116 eis_toolkit-0.4.0/eis_toolkit/validation/plot_rate_curve.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.0/eis_toolkit/vector_processing/__init__.py
--rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.4.0/eis_toolkit/vector_processing/calculate_geometry.py
--rw-r--r--   0        0        0    22658 2024-02-22 09:12:29.168927 eis_toolkit-0.4.0/eis_toolkit/vector_processing/cell_based_association.py
--rw-r--r--   0        0        0     2543 2024-04-03 09:32:00.769041 eis_toolkit-0.4.0/eis_toolkit/vector_processing/distance_computation.py
--rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.4.0/eis_toolkit/vector_processing/extract_shared_lines.py
--rw-r--r--   0        0        0     3742 2024-03-12 15:53:06.759589 eis_toolkit-0.4.0/eis_toolkit/vector_processing/idw_interpolation.py
--rw-r--r--   0        0        0     4080 2023-12-06 09:22:12.535287 eis_toolkit-0.4.0/eis_toolkit/vector_processing/kriging_interpolation.py
--rw-r--r--   0        0        0     6502 2024-02-22 09:12:29.168927 eis_toolkit-0.4.0/eis_toolkit/vector_processing/rasterize_vector.py
--rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.4.0/eis_toolkit/vector_processing/reproject_vector.py
--rw-r--r--   0        0        0     1778 2023-12-06 09:22:12.535287 eis_toolkit-0.4.0/eis_toolkit/vector_processing/vector_density.py
--rwxr-xr-x   0        0        0     1778 2024-03-06 08:46:40.214906 eis_toolkit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 eis_toolkit-0.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.4.1/LICENSE
+-rwxr-xr-x   0        0        0     5864 2024-04-24 11:26:53.983156 eis_toolkit-0.4.1/README.md
+-rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.4.1/eis_toolkit/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.4.1/eis_toolkit/__main__.py
+-rw-r--r--   0        0        0   101955 2024-04-29 07:18:52.216497 eis_toolkit-0.4.1/eis_toolkit/cli.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/conversions/__init__.py
+-rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.4.1/eis_toolkit/conversions/csv_to_geodataframe.py
+-rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-0.4.1/eis_toolkit/conversions/raster_to_dataframe.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/__init__.py
+-rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/calculate_base_metrics.py
+-rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/classification_label_evaluation.py
+-rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/classification_probability_evaluation.py
+-rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_confusion_matrix.py
+-rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_nn_model_performance.py
+-rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_prediction_area_curves.py
+-rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_rate_curve.py
+-rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-0.4.1/eis_toolkit/evaluation/scoring.py
+-rw-r--r--   0        0        0     2643 2024-02-22 09:12:29.156927 eis_toolkit-0.4.1/eis_toolkit/exceptions.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/__init__.py
+-rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
+-rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/chi_square_test.py
+-rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/correlation_matrix.py
+-rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/covariance_matrix.py
+-rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/dbscan.py
+-rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py
+-rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/feature_importance.py
+-rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/k_means_cluster.py
+-rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/local_morans_i.py
+-rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/normality_test.py
+-rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py
+-rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/pca.py
+-rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/plot_utils.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/prediction/__init__.py
+-rw-r--r--   0        0        0     5228 2024-04-29 06:12:57.053049 eis_toolkit-0.4.1/eis_toolkit/prediction/fuzzy_overlay.py
+-rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.4.1/eis_toolkit/prediction/gradient_boosting.py
+-rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.4.1/eis_toolkit/prediction/logistic_regression.py
+-rw-r--r--   0        0        0    13336 2024-04-29 05:55:02.267130 eis_toolkit-0.4.1/eis_toolkit/prediction/machine_learning_general.py
+-rw-r--r--   0        0        0     1837 2024-04-25 10:25:47.565371 eis_toolkit-0.4.1/eis_toolkit/prediction/machine_learning_predict.py
+-rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.4.1/eis_toolkit/prediction/mlp.py
+-rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.4.1/eis_toolkit/prediction/random_forests.py
+-rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-0.4.1/eis_toolkit/prediction/weights_of_evidence.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/raster_processing/__init__.py
+-rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/clipping.py
+-rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/create_constant_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/__init__.py
+-rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/classification.py
+-rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/parameters.py
+-rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
+-rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/utilities.py
+-rw-r--r--   0        0        0    10388 2024-04-29 07:18:52.216497 eis_toolkit-0.4.1/eis_toolkit/raster_processing/distance_to_anomaly.py
+-rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/extract_values_from_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/__init__.py
+-rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/focal.py
+-rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/kernels.py
+-rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/speckle.py
+-rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/utilities.py
+-rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.4.1/eis_toolkit/raster_processing/reclassify.py
+-rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/raster_processing/reprojecting.py
+-rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/raster_processing/resampling.py
+-rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.4.1/eis_toolkit/raster_processing/snapping.py
+-rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/raster_processing/unifying.py
+-rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/raster_processing/unique_combinations.py
+-rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.4.1/eis_toolkit/raster_processing/windowing.py
+-rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/training_data_tools/__init__.py
+-rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.4.1/eis_toolkit/training_data_tools/class_balancing.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/transformations/__init__.py
+-rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.4.1/eis_toolkit/transformations/binarize.py
+-rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/clip.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/__init__.py
+-rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/alr.py
+-rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/clr.py
+-rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/ilr.py
+-rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/pairwise.py
+-rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/coda/plr.py
+-rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/linear.py
+-rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/logarithmic.py
+-rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/one_hot_encoding.py
+-rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/transformations/sigmoid.py
+-rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.4.1/eis_toolkit/transformations/winsorize.py
+-rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.4.1/eis_toolkit/utilities/__init__.py
+-rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.4.1/eis_toolkit/utilities/aitchison_geometry.py
+-rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/compositional.py
+-rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/dataframe.py
+-rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/geometry.py
+-rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/parameter.py
+-rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.4.1/eis_toolkit/utilities/checks/raster.py
+-rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.4.1/eis_toolkit/utilities/conversions.py
+-rw-r--r--   0        0        0     8640 2024-04-24 06:18:14.118407 eis_toolkit-0.4.1/eis_toolkit/utilities/file_io.py
+-rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-0.4.1/eis_toolkit/utilities/miscellaneous.py
+-rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-0.4.1/eis_toolkit/utilities/nodata.py
+-rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-0.4.1/eis_toolkit/utilities/raster.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.4.1/eis_toolkit/vector_processing/__init__.py
+-rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.4.1/eis_toolkit/vector_processing/calculate_geometry.py
+-rw-r--r--   0        0        0    22658 2024-02-22 09:12:29.168927 eis_toolkit-0.4.1/eis_toolkit/vector_processing/cell_based_association.py
+-rw-r--r--   0        0        0     3240 2024-04-29 07:18:52.216497 eis_toolkit-0.4.1/eis_toolkit/vector_processing/distance_computation.py
+-rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.4.1/eis_toolkit/vector_processing/extract_shared_lines.py
+-rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-0.4.1/eis_toolkit/vector_processing/idw_interpolation.py
+-rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-0.4.1/eis_toolkit/vector_processing/kriging_interpolation.py
+-rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-0.4.1/eis_toolkit/vector_processing/rasterize_vector.py
+-rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.4.1/eis_toolkit/vector_processing/reproject_vector.py
+-rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-0.4.1/eis_toolkit/vector_processing/vector_density.py
+-rwxr-xr-x   0        0        0     1778 2024-04-29 07:41:48.254374 eis_toolkit-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 eis_toolkit-0.4.1/PKG-INFO
```

### Comparing `eis_toolkit-0.4.0/LICENSE` & `eis_toolkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/README.md` & `eis_toolkit-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,24 +34,34 @@
 EIS Toolkit is a comprehensive Python package for mineral prospectivity mapping and analysis. EIS Toolkit is developed as part of [EIS Horizon EU project](https://eis-he.eu/), which aims to aid EU's efforts in the green transition by securing critical raw materials. EIS Toolkit serves both as a standalone library that brings together and implements relevant tools for mineral prospectivity mapping and as a computational backend for [EIS QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin).
 
 > [!NOTE]  
 > This repository is still in development. Check the [wiki page of EIS Toolkit](https://github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap](#roadmap) for more details about the project.
 
 
 ## Installation
-You can find the latest release of EIS Toolkit in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) as a Python wheel. To install EIS Toolkit, download the wheel and install with pip
+We recommend installing EIS Toolkit in an empty virtual environment to ensure compatibility between package versions. 
+
+EIS Toolkit is available in conda-forge and PyPI and can be installed with one of the following commands.
 
 ```console
-pip install eis_toolkit-0.4.0-py3-none-any.whl
+pip install eis_toolkit
+```
+
+```console
+conda-install -c conda-forge eis_toolkit
 ```
 
-We recommend installing EIS Toolkit in an empty virtual environment to ensure compatibility between package versions.
+You can find the latest release of EIS Toolkit also in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a Python wheel. Just download the wheel and install with pip
+
+```console
+pip install eis_toolkit-0.4.0-py3-none-any.whl
+```
 
-> [!NOTE]
-> EIS Toolkit has not yet been released in PyPi or Conda, but will be at a later stage.
+> [!TIP]
+> GDAL installation can cause issues on various platforms, especially on Windows. If you have trouble installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
 
 
 ## Usage
 EIS Toolkit can be used in Python scripts, Jupyter notebooks or via the CLI. At the moment, most tools have their own module and are imported like this:
 ```python
 # In general
 from eis_toolkit.category.module import module_function
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_g0980_xp_/tmp5pt9o707_TarContainer/0/1.md", line 6, column 35: Levels of opening and closing headings don't match*

```diff
@@ -11,57 +11,62 @@
 (https://eis-he.eu/), which aims to aid EU's efforts in the green transition by
 securing critical raw materials. EIS Toolkit serves both as a standalone
 library that brings together and implements relevant tools for mineral
 prospectivity mapping and as a computational backend for [EIS QGIS Plugin]
 (https://github.com/GispoCoding/eis_qgis_plugin). > [!NOTE] > This repository
 is still in development. Check the [wiki page of EIS Toolkit](https://
 github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap]
-(#roadmap) for more details about the project. ## Installation You can find the
-latest release of EIS Toolkit in the [releases page](https://github.com/
-GispoCoding/eis_toolkit/releases) as a Python wheel. To install EIS Toolkit,
-download the wheel and install with pip ```console pip install eis_toolkit-
-0.4.0-py3-none-any.whl ``` We recommend installing EIS Toolkit in an empty
-virtual environment to ensure compatibility between package versions. > [!NOTE]
-> EIS Toolkit has not yet been released in PyPi or Conda, but will be at a
-later stage. ## Usage EIS Toolkit can be used in Python scripts, Jupyter
-notebooks or via the CLI. At the moment, most tools have their own module and
-are imported like this: ```python # In general from eis_toolkit.category.module
-import module_function # Some examples from
-eis_toolkit.raster_processing.reprojecting import reproject_raster from
-eis_toolkit.exploratory_analyses.pca import compute_pca ``` You can find
-several Jupyter notebooks in this repostiory that demonstrate how tools of EIS
-Toolkit can be used. The documentation of EIS Toolkit can be read [here](https:
-//gispocoding.github.io/eis_toolkit/). ### EIS QGIS Plugin For those that
-prefer using tools of EIS Toolkit via a graphical user interface, check [EIS
-QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin
-includes the main GUI application called EIS Wizard and all individual EIS
-Toolkit tools as QGIS processing algorithms. The plugin is developed by the
-same core team that develops EIS Toolkit. ### CLI EIS Toolkit includes a
-[Typer](https://typer.tiangolo.com/) command-line interface that serves as a
-common interface for integrating the toolkit with external applications, such
-as QGIS. However, it can be used directly too. To use the CLI, simply use the
-command ```console eis ``` or ```console eis --help ``` to get started.
-However, please note that the CLI has been primarily designed to communicate
-with external programs and may feel clunky in direct use. ## Roadmap -
-Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the
-basic funtionalities required for a full MPM workflow. Official testing phase
-begins. The plugin will be still under active development. - Milestone 2:
-**Release 1.0** (April 2024). All features should be incorporated at this time
-and the toolkit useful for actual MPM work. Testing will continue, potential
-bugs will be fixed and the user experience refined. ## Contributing We welcome
-contributions to EIS Toolkit in various forms: - â¨ Developing new tools -
-ð Fixing bugs in the code - ð Bug and other reporting - ð¡ Feature
-suggestions To contribute with code or documentation, you'll need a local
-development environment and a copy of the repository. Please refer to the **For
-developers** section below for detailed setup instructions. If you're
-interested in bug reporting or making feature suggestions, you can familiarize
-yourself with the toolkit and test it as described in the **Usage** section.
-When you encounter bugs or have ideas for new features, you can create an issue
-in this repository. ### For developers All contributing developers need Git and
-a copy of the repository. ```console git clone https://github.com/GispoCoding/
-eis_toolkit.git ``` After this you have three options for setting up your local
-development environment. 1. Docker - [instructions](./instructions/
-dev_setup_with_docker.md) 2. Poetry - [instructions](./instructions/
-dev_setup_without_docker.md) 3. Conda - [instructions](./instructions/
-dev_setup_without_docker_with_conda.md) *For general contributing guidelines,
-see [CONTRIBUTING](./CONTRIBUTING.md).* ## License Licensed under the EUPL-1.2
-or later.
+(#roadmap) for more details about the project. ## Installation We recommend
+installing EIS Toolkit in an empty virtual environment to ensure compatibility
+between package versions. EIS Toolkit is available in conda-forge and PyPI and
+can be installed with one of the following commands. ```console pip install
+eis_toolkit ``` ```console conda-install -c conda-forge eis_toolkit ``` You can
+find the latest release of EIS Toolkit also in the [releases page](https://
+github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a
+Python wheel. Just download the wheel and install with pip ```console pip
+install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL installation can
+cause issues on various platforms, especially on Windows. If you have trouble
+installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel
+(for example from [this repository](https://github.com/cgohlke/geospatial-
+wheels/releases)), install it first, and then attempt to install EIS Toolkit
+again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter notebooks or
+via the CLI. At the moment, most tools have their own module and are imported
+like this: ```python # In general from eis_toolkit.category.module import
+module_function # Some examples from eis_toolkit.raster_processing.reprojecting
+import reproject_raster from eis_toolkit.exploratory_analyses.pca import
+compute_pca ``` You can find several Jupyter notebooks in this repostiory that
+demonstrate how tools of EIS Toolkit can be used. The documentation of EIS
+Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/). ### EIS
+QGIS Plugin For those that prefer using tools of EIS Toolkit via a graphical
+user interface, check [EIS QGIS Plugin](https://github.com/GispoCoding/
+eis_qgis_plugin). The plugin includes the main GUI application called EIS
+Wizard and all individual EIS Toolkit tools as QGIS processing algorithms. The
+plugin is developed by the same core team that develops EIS Toolkit. ### CLI
+EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line
+interface that serves as a common interface for integrating the toolkit with
+external applications, such as QGIS. However, it can be used directly too. To
+use the CLI, simply use the command ```console eis ``` or ```console eis --help
+``` to get started. However, please note that the CLI has been primarily
+designed to communicate with external programs and may feel clunky in direct
+use. ## Roadmap - Milestone 1: **Beta release 0.1** (November 2023). The
+toolkit should have the basic funtionalities required for a full MPM workflow.
+Official testing phase begins. The plugin will be still under active
+development. - Milestone 2: **Release 1.0** (April 2024). All features should
+be incorporated at this time and the toolkit useful for actual MPM work.
+Testing will continue, potential bugs will be fixed and the user experience
+refined. ## Contributing We welcome contributions to EIS Toolkit in various
+forms: - â¨ Developing new tools - ð Fixing bugs in the code - ð Bug and
+other reporting - ð¡ Feature suggestions To contribute with code or
+documentation, you'll need a local development environment and a copy of the
+repository. Please refer to the **For developers** section below for detailed
+setup instructions. If you're interested in bug reporting or making feature
+suggestions, you can familiarize yourself with the toolkit and test it as
+described in the **Usage** section. When you encounter bugs or have ideas for
+new features, you can create an issue in this repository. ### For developers
+All contributing developers need Git and a copy of the repository. ```console
+git clone https://github.com/GispoCoding/eis_toolkit.git ``` After this you
+have three options for setting up your local development environment. 1. Docker
+- [instructions](./instructions/dev_setup_with_docker.md) 2. Poetry -
+[instructions](./instructions/dev_setup_without_docker.md) 3. Conda -
+[instructions](./instructions/dev_setup_without_docker_with_conda.md) *For
+general contributing guidelines, see [CONTRIBUTING](./CONTRIBUTING.md).* ##
+License Licensed under the EUPL-1.2 or later.
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/cli.py` & `eis_toolkit-0.4.1/eis_toolkit/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,14 +248,23 @@
 
     squared_error = "squared_error"
     absolute_error = "absolute_error"
     friedman_mse = "friedman_mse"
     poisson = "poisson"
 
 
+class ThresholdCriteria(str, Enum):
+    """Threshold criteria for distance to anomaly."""
+
+    lower = "lower"
+    higher = "higher"
+    in_between = "in_between"
+    outside = "outside"
+
+
 INPUT_FILE_OPTION = Annotated[
     Path,
     typer.Option(
         exists=True,
         file_okay=True,
         dir_okay=False,
         writable=False,
@@ -1173,14 +1182,57 @@
     with rasterio.open(output_raster, "w", **out_meta) as dest:
         dest.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Creating constant raster completed, writing raster to {output_raster}.")
 
 
+# DISTANCE TO ANOMALY
+@app.command()
+def distance_to_anomaly_cli(
+    input_raster: INPUT_FILE_OPTION,
+    output_raster: OUTPUT_FILE_OPTION,
+    threshold_criteria: Annotated[ThresholdCriteria, typer.Option(case_sensitive=False)],
+    first_threshold_criteria_value: float = typer.Option(),
+    second_threshold_criteria_value: float = None,
+    max_distance: float = None,
+):
+    """
+    Calculate distance from each raster cell to nearest anomaly cell.
+
+    Uses only the first band of the raster.
+    """
+    from eis_toolkit.raster_processing.distance_to_anomaly import distance_to_anomaly
+
+    typer.echo("Progress: 10%")
+
+    if second_threshold_criteria_value is not None:
+        threshold_criteria_value = (first_threshold_criteria_value, second_threshold_criteria_value)
+    else:
+        threshold_criteria_value = first_threshold_criteria_value
+
+    with rasterio.open(input_raster) as raster:
+        typer.echo("Progress: 25%")
+        out_image, out_meta = distance_to_anomaly(
+            anomaly_raster_profile=raster.profile,
+            anomaly_raster_data=raster.read(1),
+            threshold_criteria_value=threshold_criteria_value,
+            threshold_criteria=get_enum_values(threshold_criteria),
+            max_distance=max_distance,
+        )
+
+    typer.echo("Progress: 75%")
+
+    with rasterio.open(output_raster, "w", **out_meta) as dest:
+        dest.write(out_image, 1)
+    typer.echo("Progress: 100%")
+
+    typer.echo(f"Computing distance to anomaly completed, writing raster to {output_raster}.")
+
+
 # EXTRACT VALUES FROM RASTER
 @app.command()
 def extract_values_from_raster_cli(
     input_raster: INPUT_FILE_OPTION,
     geometries: INPUT_FILE_OPTION,
     output_vector: OUTPUT_FILE_OPTION,
 ):
@@ -1681,156 +1733,166 @@
 
 
 # IDW INTERPOLATION
 @app.command()
 def idw_interpolation_cli(
     input_vector: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
+    base_raster: INPUT_FILE_OPTION = None,
     target_column: str = typer.Option(),
-    resolution: float = typer.Option(),
+    pixel_size: float = None,
+    extent: Tuple[float, float, float, float] = (None, None, None, None),
     power: float = 2.0,
-    extent: Tuple[float, float, float, float] = (None, None, None, None),  # TODO Change this
 ):
     """Apply inverse distance weighting (IDW) interpolation to input vector file."""
+    from eis_toolkit.exceptions import InvalidParameterValueException
+    from eis_toolkit.utilities.raster import profile_from_extent_and_pixel_size
     from eis_toolkit.vector_processing.idw_interpolation import idw
 
     typer.echo("Progress: 10%")
 
-    if extent == (None, None, None, None):
-        extent = None
-
     geodataframe = gpd.read_file(input_vector)
     typer.echo("Progress: 25%")
 
-    out_image, out_meta = idw(
-        geodataframe=geodataframe,
-        target_column=target_column,
-        resolution=(resolution, resolution),
-        extent=extent,
-        power=power,
-    )
-    typer.echo("Progress: 75%")
+    if base_raster is None or base_raster == "":
+        if any(bound is None for bound in extent) or pixel_size is None or pixel_size <= 0:
+            raise InvalidParameterValueException(
+                "Expected positive pixel size and defined extent in absence of base raster. "
+                + f"Pixel size: {pixel_size}, extent: {extent}."
+            )
+        profile = profile_from_extent_and_pixel_size(extent, (pixel_size, pixel_size))
+        profile["crs"] = geodataframe.crs
+        profile["driver"] = "GTiff"
+        profile["dtype"] = "float32"
+    else:
+        with rasterio.open(base_raster) as raster:
+            profile = raster.profile.copy()
 
-    out_meta.update(
-        {
-            "count": 1,
-            "driver": "GTiff",
-            "dtype": "float32",
-        }
-    )
+    out_image = idw(geodataframe=geodataframe, target_column=target_column, raster_profile=profile, power=power)
+    typer.echo("Progress: 75%")
 
-    with rasterio.open(output_raster, "w", **out_meta) as dst:
+    profile["count"] = 1
+    with rasterio.open(output_raster, "w", **profile) as dst:
         dst.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"IDW interpolation completed, writing raster to {output_raster}.")
 
 
 # KRIGING INTERPOLATION
 @app.command()
 def kriging_interpolation_cli(
     input_vector: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
+    base_raster: INPUT_FILE_OPTION = None,
     target_column: str = typer.Option(),
-    resolution: float = typer.Option(),
-    extent: Tuple[float, float, float, float] = (None, None, None, None),  # TODO Change this
+    pixel_size: float = None,
+    extent: Tuple[float, float, float, float] = (None, None, None, None),
     variogram_model: Annotated[VariogramModel, typer.Option(case_sensitive=False)] = VariogramModel.linear,
     coordinates_type: Annotated[CoordinatesType, typer.Option(case_sensitive=False)] = CoordinatesType.geographic,
     method: Annotated[KrigingMethod, typer.Option(case_sensitive=False)] = KrigingMethod.ordinary,
 ):
     """Apply kriging interpolation to input vector file."""
+    from eis_toolkit.exceptions import InvalidParameterValueException
+    from eis_toolkit.utilities.raster import profile_from_extent_and_pixel_size
     from eis_toolkit.vector_processing.kriging_interpolation import kriging
 
     typer.echo("Progress: 10%")
 
-    if extent == (None, None, None, None):
-        extent = None
-
     geodataframe = gpd.read_file(input_vector)
     typer.echo("Progress: 25%")
 
-    out_image, out_meta = kriging(
-        data=geodataframe,
+    if base_raster is None or base_raster == "":
+        if any(bound is None for bound in extent) or pixel_size is None or pixel_size <= 0:
+            raise InvalidParameterValueException(
+                "Expected positive pixel size and defined extent in absence of base raster. "
+                + f"Pixel size: {pixel_size}, extent: {extent}."
+            )
+        profile = profile_from_extent_and_pixel_size(extent, (pixel_size, pixel_size))
+        profile["crs"] = geodataframe.crs
+        profile["driver"] = "GTiff"
+        profile["dtype"] = "float32"
+    else:
+        with rasterio.open(base_raster) as raster:
+            profile = raster.profile.copy()
+
+    out_image = kriging(
+        geodataframe=geodataframe,
         target_column=target_column,
-        resolution=(resolution, resolution),
-        extent=extent,
+        raster_profile=profile,
         variogram_model=get_enum_values(variogram_model),
         coordinates_type=get_enum_values(coordinates_type),
         method=get_enum_values(method),
     )
     typer.echo("Progress: 75%")
 
-    out_meta.update(
-        {
-            "count": 1,
-            "driver": "GTiff",
-            "dtype": "float32",
-        }
-    )
-
-    with rasterio.open(output_raster, "w", **out_meta) as dst:
+    profile["count"] = 1
+    with rasterio.open(output_raster, "w", **profile) as dst:
         dst.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Kriging interpolation completed, writing raster to {output_raster}.")
 
 
 # RASTERIZE
 @app.command()
 def rasterize_cli(
     input_vector: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
-    resolution: float = None,
+    base_raster: INPUT_FILE_OPTION = None,
     value_column: str = None,
+    pixel_size: float = None,
+    extent: Tuple[float, float, float, float] = (None, None, None, None),
     default_value: float = 1.0,
     fill_value: float = 0.0,
-    base_raster_profile_raster: INPUT_FILE_OPTION = None,
     buffer_value: float = None,
     merge_strategy: Annotated[MergeStrategy, typer.Option(case_sensitive=False)] = MergeStrategy.replace,
 ):
     """
     Rasterize input vector.
 
-    Either resolution or base-raster-profile-raster must be provided.
+    Either base raster or pixel size + extent must be provided.
     """
+    from eis_toolkit.exceptions import InvalidParameterValueException
+    from eis_toolkit.utilities.raster import profile_from_extent_and_pixel_size
     from eis_toolkit.vector_processing.rasterize_vector import rasterize_vector
 
     typer.echo("Progress: 10%")
 
     geodataframe = gpd.read_file(input_vector)
+    typer.echo("Progress: 25%")
 
-    if base_raster_profile_raster is not None:
-        with rasterio.open(base_raster_profile_raster) as raster:
-            base_raster_profile = raster.profile
+    if base_raster is None or base_raster == "":
+        if any(bound is None for bound in extent) or pixel_size is None or pixel_size <= 0:
+            raise InvalidParameterValueException(
+                "Expected positive pixel size and defined extent in absence of base raster. "
+                + f"Pixel size: {pixel_size}, extent: {extent}."
+            )
+        profile = profile_from_extent_and_pixel_size(extent, (pixel_size, pixel_size))
+        profile["crs"] = geodataframe.crs
+        profile["driver"] = "GTiff"
+        profile["dtype"] = "float32"
     else:
-        base_raster_profile = base_raster_profile_raster
-    typer.echo("Progress: 25%")
+        with rasterio.open(base_raster) as raster:
+            profile = raster.profile.copy()
 
-    out_image, out_meta = rasterize_vector(
+    out_image = rasterize_vector(
         geodataframe,
-        resolution,
+        profile,
         value_column,
         default_value,
         fill_value,
-        base_raster_profile,
         buffer_value,
         get_enum_values(merge_strategy),
     )
     typer.echo("Progress: 75%")
 
-    out_meta.update(
-        {
-            "count": 1,
-            "dtype": base_raster_profile["dtype"] if base_raster_profile_raster else "float32",  # TODO change this
-        }
-    )
-
-    with rasterio.open(output_raster, "w", **out_meta) as dst:
-        for band_n in range(1, out_meta["count"]):
-            dst.write(out_image, band_n)
+    profile["count"] = 1
+    with rasterio.open(output_raster, "w", **profile) as dst:
+        dst.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Rasterizing completed, writing raster to {output_raster}.")
 
 
 # REPROJECT VECTOR
 @app.command()
@@ -1857,84 +1919,104 @@
 
 
 # VECTOR DENSITY
 @app.command()
 def vector_density_cli(
     input_vector: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
-    resolution: float = None,
-    base_raster_profile_raster: INPUT_FILE_OPTION = None,
+    base_raster: INPUT_FILE_OPTION = None,
+    pixel_size: float = None,
+    extent: Tuple[float, float, float, float] = (None, None, None, None),
     buffer_value: float = None,
     statistic: Annotated[VectorDensityStatistic, typer.Option(case_sensitive=False)] = VectorDensityStatistic.density,
 ):
     """
     Compute density of geometries within raster.
 
-    Either resolution or base_raster_profile_raster must be provided.
+    Either base raster or pixel size + extent must be provided.
     """
+    from eis_toolkit.exceptions import InvalidParameterValueException
+    from eis_toolkit.utilities.raster import profile_from_extent_and_pixel_size
     from eis_toolkit.vector_processing.vector_density import vector_density
 
     typer.echo("Progress: 10%")
 
     geodataframe = gpd.read_file(input_vector)
+    typer.echo("Progress: 25%")
 
-    if base_raster_profile_raster is not None:
-        with rasterio.open(base_raster_profile_raster) as raster:
-            base_raster_profile = raster.profile
+    if base_raster is None or base_raster == "":
+        if any(bound is None for bound in extent) or pixel_size is None or pixel_size <= 0:
+            raise InvalidParameterValueException(
+                "Expected positive pixel size and defined extent in absence of base raster. "
+                + f"Pixel size: {pixel_size}, extent: {extent}."
+            )
+        profile = profile_from_extent_and_pixel_size(extent, (pixel_size, pixel_size))
+        profile["crs"] = geodataframe.crs
+        profile["driver"] = "GTiff"
+        profile["dtype"] = "float32"
     else:
-        base_raster_profile = base_raster_profile_raster
-    typer.echo("Progress: 25%")
+        with rasterio.open(base_raster) as raster:
+            profile = raster.profile.copy()
 
-    out_image, out_meta = vector_density(
+    out_image = vector_density(
         geodataframe=geodataframe,
-        resolution=resolution,
-        base_raster_profile=base_raster_profile,
+        raster_profile=profile,
         buffer_value=buffer_value,
         statistic=get_enum_values(statistic),
     )
     typer.echo("Progress: 75%")
 
-    out_meta.update(
-        {
-            "count": 1,
-            "dtype": base_raster_profile["dtype"] if base_raster_profile_raster else "float32",  # TODO change this
-        }
-    )
-
-    with rasterio.open(output_raster, "w", **out_meta) as dst:
-        for band_n in range(1, out_meta["count"]):
-            dst.write(out_image, band_n)
+    profile["count"] = 1
+    with rasterio.open(output_raster, "w", **profile) as dst:
+        dst.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Vector density computation completed, writing raster to {output_raster}.")
 
 
 # DISTANCE COMPUTATION
 @app.command()
 def distance_computation_cli(
-    input_raster: INPUT_FILE_OPTION,
-    geometries: INPUT_FILE_OPTION,
+    input_vector: INPUT_FILE_OPTION,
     output_raster: OUTPUT_FILE_OPTION,
+    base_raster: INPUT_FILE_OPTION = None,
+    pixel_size: float = None,
+    extent: Tuple[float, float, float, float] = (None, None, None, None),
+    max_distance: float = None,
 ):
     """Calculate distance from raster cell to nearest geometry."""
+    from eis_toolkit.exceptions import InvalidParameterValueException
+    from eis_toolkit.utilities.raster import profile_from_extent_and_pixel_size
     from eis_toolkit.vector_processing.distance_computation import distance_computation
 
     typer.echo("Progress: 10%")
 
-    with rasterio.open(input_raster) as raster:
-        profile = raster.profile
-
-    geodataframe = gpd.read_file(geometries)
+    geodataframe = gpd.read_file(input_vector)
     typer.echo("Progress: 25%")
 
-    out_image = distance_computation(profile, geodataframe)
+    if base_raster is None or base_raster == "":
+        if any(bound is None for bound in extent) or pixel_size is None or pixel_size <= 0:
+            raise InvalidParameterValueException(
+                "Expected positive pixel size and defined extent in absence of base raster. "
+                + f"Pixel size: {pixel_size}, extent: {extent}."
+            )
+        profile = profile_from_extent_and_pixel_size(extent, (pixel_size, pixel_size))
+        profile["crs"] = geodataframe.crs
+        profile["driver"] = "GTiff"
+        profile["dtype"] = "float32"
+    else:
+        with rasterio.open(base_raster) as raster:
+            profile = raster.profile.copy()
+
+    out_image = distance_computation(geodataframe=geodataframe, raster_profile=profile, max_distance=max_distance)
+    profile["count"] = 1
     typer.echo("Progress: 75%")
 
     with rasterio.open(output_raster, "w", **profile) as dst:
-        dst.write(out_image, profile["count"])
+        dst.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Distance computation completed, writing raster to {output_raster}.")
 
 
 # CBA
 # TODO
@@ -2880,15 +2962,15 @@
     with rasterio.open(output_raster, "w", **out_meta) as dst:
         dst.write(out_image)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Winsorize transform completed, writing raster to {output_raster}.")
 
 
-# ---VALIDATION ---
+# ---EVALUATION ---
 # TODO
 
 
 # --- UTILITIES ---
 @app.command()
 def split_raster_bands_cli(input_raster: INPUT_FILE_OPTION, output_dir: OUTPUT_DIR_OPTION):  # CHECK
     """Split multiband raster into singleband rasters."""
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/conversions/csv_to_geodataframe.py` & `eis_toolkit-0.4.1/eis_toolkit/conversions/csv_to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exceptions.py` & `eis_toolkit-0.4.1/eis_toolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/chi_square_test.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/chi_square_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/correlation_matrix.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/covariance_matrix.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/dbscan.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/dbscan.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/descriptive_statistics.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/feature_importance.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/feature_importance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/k_means_cluster.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/k_means_cluster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/local_morans_i.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/local_morans_i.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/normality_test.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/normality_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/parallel_coordinates.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/exploratory_analyses/pca.py` & `eis_toolkit-0.4.1/eis_toolkit/exploratory_analyses/pca.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/fuzzy_overlay.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/fuzzy_overlay.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/gradient_boosting.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/logistic_regression.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/machine_learning_general.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/machine_learning_general.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,29 +4,20 @@
 
 import geopandas as gpd
 import joblib
 import numpy as np
 import pandas as pd
 import rasterio
 from beartype import beartype
-from beartype.typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union
+from beartype.typing import Any, List, Literal, Optional, Sequence, Tuple, Union
 from scipy import sparse
-from sklearn.base import BaseEstimator, is_classifier, is_regressor
-from sklearn.metrics import (
-    accuracy_score,
-    f1_score,
-    mean_absolute_error,
-    mean_squared_error,
-    precision_score,
-    r2_score,
-    recall_score,
-)
+from sklearn.base import BaseEstimator
 from sklearn.model_selection import KFold, LeaveOneOut, StratifiedKFold, train_test_split
-from tensorflow import keras
 
+from eis_toolkit.evaluation.scoring import score_predictions
 from eis_toolkit.exceptions import (
     InvalidParameterValueException,
     NonMatchingParameterLengthsException,
     NonMatchingRasterMetadataException,
 )
 from eis_toolkit.utilities.checks.raster import check_raster_grids
 from eis_toolkit.vector_processing.rasterize_vector import rasterize_vector
@@ -96,70 +87,14 @@
 
     split_data = train_test_split(*data, test_size=split_size, random_state=random_state, shuffle=shuffle)
 
     return split_data
 
 
 @beartype
-def evaluate_model(
-    X_test: Union[np.ndarray, pd.DataFrame],
-    y_test: Union[np.ndarray, pd.Series],
-    model: Union[BaseEstimator, keras.Model],
-    metrics: Optional[Sequence[Literal["mse", "rmse", "mae", "r2", "accuracy", "precision", "recall", "f1"]]] = None,
-) -> Tuple[np.ndarray, Dict[str, Number]]:
-    """
-    Evaluate/score a trained model with test data.
-
-    Predicts with the given test data and evaluates the predictions.
-
-    Args:
-        X_test: Test data.
-        y_test: Target labels for test data.
-        model: Trained Sklearn classifier or regressor.
-        metrics: Metrics to use for scoring the model. Defaults to "accuracy" for a classifier
-            and to "mse" for a regressor.
-
-    Returns:
-        Predictions and metric scores as a dictionary.
-    """
-    x_size = X_test.index.size if isinstance(X_test, pd.DataFrame) else X_test.shape[0]
-    if x_size != y_test.size:
-        raise NonMatchingParameterLengthsException(f"X and y must have the length {x_size} != {y_test.size}.")
-
-    if metrics is None:
-        metrics = ["accuracy"] if is_classifier(model) else ["mse"]
-
-    y_pred = model.predict(X_test)
-
-    out_metrics = {}
-    for metric in metrics:
-        score = _score_model(model, y_test, y_pred, metric)
-        out_metrics[metric] = score
-
-    return y_pred, out_metrics
-
-
-@beartype
-def predict(data: Union[np.ndarray, pd.DataFrame], model: Union[BaseEstimator, keras.Model]) -> np.ndarray:
-    """
-    Predict with a trained model.
-
-    Args:
-        data: Data used to make predictions.
-        model: Trained classifier or regressor. Can be any machine learning model trained with
-            EIS Toolkit (Sklearn and Keras models).
-
-    Returns:
-        Predictions.
-    """
-    result = model.predict(data)
-    return result
-
-
-@beartype
 def reshape_predictions(
     predictions: np.ndarray, height: int, width: int, nodata_mask: Optional[np.ndarray] = None
 ) -> np.ndarray:
     """
     Reshape 1D prediction ouputs into 2D Numpy array.
 
     The output is ready to be visualized and saved as a raster.
@@ -245,15 +180,15 @@
 
     if label_file is not None:
         # Check label file type and process accordingly
         file_extension = os.path.splitext(label_file)[1].lower()
 
         # Labels/deposits in vector format
         if file_extension in [".shp", ".geojson", ".json", ".gpkg"]:
-            y, _ = rasterize_vector(geodataframe=gpd.read_file(label_file), base_raster_profile=reference_profile)
+            y = rasterize_vector(geodataframe=gpd.read_file(label_file), raster_profile=reference_profile)
 
         # Labels/deposits in raster format
         else:
             with rasterio.open(label_file) as label_raster:
                 y = label_raster.read(1)  # Assuming labels are in the first band
                 label_nodata = label_raster.nodata
 
@@ -331,15 +266,15 @@
             X, y, split_size=split_size, random_state=random_state, shuffle=shuffle
         )
         model.fit(X_train, y_train)
         y_pred = model.predict(X_valid)
 
         out_metrics = {}
         for metric in metrics:
-            score = _score_model(model, y_valid, y_pred, metric)
+            score = score_predictions(y_valid, y_pred, metric)
             out_metrics[metric] = score
 
     # Validation approach 3: Cross-validation
     elif validation_method in [KFOLD_CV, SKFOLD_CV, LOO_CV]:
         cv = _get_cross_validator(validation_method, cv_folds, shuffle, random_state)
 
         # Initialize output metrics dictionary
@@ -350,15 +285,15 @@
 
         # Loop over cross-validation folds and save metric scores
         for train_index, valid_index in cv.split(X, y):
             model.fit(X[train_index], y[train_index])
             y_pred = model.predict(X[valid_index])
 
             for metric in metrics:
-                score = _score_model(model, y[valid_index], y_pred, metric)
+                score = score_predictions(y[valid_index], y_pred, metric)
                 all_scores = out_metrics[metric][f"{metric}_all"]
                 all_scores.append(score)
 
         # Calculate mean and standard deviation for all metrics
         for metric in metrics:
             scores = out_metrics[metric][f"{metric}_all"]
             out_metrics[metric][f"{metric}_mean"] = np.mean(scores)
@@ -374,76 +309,14 @@
     else:
         raise InvalidParameterValueException(f"Unrecognized validation method: {validation_method}")
 
     return model, out_metrics
 
 
 @beartype
-def _score_model(
-    model: BaseEstimator,
-    y_true: Union[np.ndarray, pd.Series],
-    y_pred: Union[np.ndarray, pd.Series],
-    metric: Literal["mse", "rmse", "mae", "r2", "accuracy", "precision", "recall", "f1"],
-) -> float:
-    """
-    Score predictions of Sklearn model using the selected metric.
-
-    Args:
-        model: Sklearn model used to produce the predictions. Used only to identify the type
-            of model (regressor or classifier).
-        y_true: Target values ("ground truth") against which scoring is performed.
-        y_pred: Predicted values generated by the model.
-        metric: The scoring metric. Different options for regressor and classifier.
-
-    Returns:
-        The prediction score.
-
-    Raises:
-        InvalidParameterValueException: If model type is invalid for the given metric or metric was not recognized.
-    """
-    if metric in ["mae", "mse", "rmse", "r2"] and not is_regressor(model):
-        raise InvalidParameterValueException(
-            f"Chosen metric ({metric}) is not applicable for given model type (classifier)."
-        )
-    if metric in ["accuracy", "precision", "recall", "f1"] and not is_classifier(model):
-        raise InvalidParameterValueException(
-            f"Chosen metric ({metric}) is not applicable for given model type (regressor)."
-        )
-
-    if is_classifier(model):
-        # Multiclass classification
-        if len(y_true) > 2:
-            average_method = "micro"
-        # Binary classification
-        else:
-            average_method = "binary"
-
-    if metric == "mae":
-        score = mean_absolute_error(y_true, y_pred)
-    elif metric == "mse":
-        score = mean_squared_error(y_true, y_pred)
-    elif metric == "rmse":
-        score = mean_squared_error(y_true, y_pred, squared=False)
-    elif metric == "r2":
-        score = r2_score(y_true, y_pred)
-    elif metric == "accuracy":
-        score = accuracy_score(y_true, y_pred)
-    elif metric == "precision":
-        score = precision_score(y_true, y_pred, average=average_method)
-    elif metric == "recall":
-        score = recall_score(y_true, y_pred, average=average_method)
-    elif metric == "f1":
-        score = f1_score(y_true, y_pred, average=average_method)
-    else:
-        raise InvalidParameterValueException(f"Unrecognized metric: {metric}")
-
-    return score
-
-
-@beartype
 def _get_cross_validator(
     cv: Literal["kfold_cv", "skfold_cv", "loo_cv"], folds: int, shuffle: bool, random_state: Optional[int]
 ) -> Union[KFold, StratifiedKFold, LeaveOneOut]:
     """
     Create a Sklearn cross-validator.
 
     Args:
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/mlp.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/mlp.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/random_forests.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/random_forests.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/prediction/weights_of_evidence.py` & `eis_toolkit-0.4.1/eis_toolkit/prediction/weights_of_evidence.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,16 +297,16 @@
         metrics_to_arrays = arrays_to_generate.copy()
 
     # 1. Preprocess data
     evidence_array = _read_and_preprocess_evidence(evidential_raster, raster_nodata)
     raster_meta = evidential_raster.meta
 
     # Rasterize deposits
-    deposit_array, _ = rasterize_vector(
-        geodataframe=deposits, default_value=1.0, base_raster_profile=raster_meta, fill_value=0.0
+    deposit_array = rasterize_vector(
+        geodataframe=deposits, raster_profile=raster_meta, default_value=1.0, fill_value=0.0
     )
 
     # Mask NaN out of the array
     nodata_mask = np.isnan(evidence_array)
     masked_evidence_array = evidence_array[~nodata_mask]
     masked_deposit_array = deposit_array[~nodata_mask]
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/clipping.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/clipping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/create_constant_raster.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/create_constant_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/classification.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/classification.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/parameters.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/parameters.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/partial_derivatives.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/derivatives/utilities.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/derivatives/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/distance_to_anomaly.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/distance_to_anomaly.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 @beartype
 def distance_to_anomaly(
     anomaly_raster_profile: Union[profiles.Profile, dict],
     anomaly_raster_data: np.ndarray,
     threshold_criteria_value: Union[Tuple[Number, Number], Number],
     threshold_criteria: Literal["lower", "higher", "in_between", "outside"],
+    max_distance: Optional[Number] = None,
 ) -> Tuple[np.ndarray, Union[profiles.Profile, dict]]:
     """Calculate distance from raster cell to nearest anomaly.
 
     The criteria for what is anomalous can be defined as a single number and
     criteria text of "higher" or "lower". Alternatively, the definition can be
     a range where values inside (criteria text of "within") or outside are
     marked as anomalous (criteria text of "outside"). If anomaly_raster_profile does
@@ -55,14 +56,15 @@
         anomaly_raster_data: The raster data in which the distances
             to the nearest anomalous value are determined.
         threshold_criteria_value: Value(s) used to define anomalous.
             If the threshold criteria requires a tuple of values,
             the first value should be the minimum and the second
             the maximum value.
         threshold_criteria: Method to define anomalous.
+        max_distance: The maximum distance in the output array.
 
     Returns:
         A 2D numpy array with the distances to anomalies computed
         and the original anomaly raster profile.
 
     """
     check_raster_profile(raster_profile=anomaly_raster_profile)
@@ -71,14 +73,15 @@
     )
 
     out_image = _distance_to_anomaly(
         anomaly_raster_profile=anomaly_raster_profile,
         anomaly_raster_data=anomaly_raster_data,
         threshold_criteria=threshold_criteria,
         threshold_criteria_value=threshold_criteria_value,
+        max_distance=max_distance,
     )
     return out_image, anomaly_raster_profile
 
 
 @beartype
 def distance_to_anomaly_gdal(
     anomaly_raster_profile: Union[profiles.Profile, dict],
@@ -197,14 +200,15 @@
 
 
 def _distance_to_anomaly(
     anomaly_raster_profile: Union[profiles.Profile, dict],
     anomaly_raster_data: np.ndarray,
     threshold_criteria_value: Union[Tuple[Number, Number], Number],
     threshold_criteria: Literal["lower", "higher", "in_between", "outside"],
+    max_distance: Optional[Number],
 ) -> np.ndarray:
     data_fits_criteria = _fits_criteria(
         threshold_criteria=threshold_criteria,
         threshold_criteria_value=threshold_criteria_value,
         anomaly_raster_data=anomaly_raster_data,
         nodata_value=anomaly_raster_profile.get("nodata"),
     )
@@ -226,10 +230,12 @@
     all_points_by_rows = [
         row_points(row=row, cols=cols[data_fits_criteria[row]], raster_transform=anomaly_raster_profile["transform"])
         for row in rows
     ]
     all_points = list(chain(*all_points_by_rows))
     all_points_gdf = gpd.GeoDataFrame(geometry=all_points, crs=anomaly_raster_profile["crs"])
 
-    distance_array = distance_computation(raster_profile=anomaly_raster_profile, geometries=all_points_gdf)
+    distance_array = distance_computation(
+        raster_profile=anomaly_raster_profile, geodataframe=all_points_gdf, max_distance=max_distance
+    )
 
     return distance_array
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/extract_values_from_raster.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/extract_values_from_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/focal.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/focal.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/kernels.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/kernels.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/speckle.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/speckle.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/filters/utilities.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/filters/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/reclassify.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/reclassify.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/reprojecting.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/reprojecting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/resampling.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/resampling.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/snapping.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/snapping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/unifying.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/unifying.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/unique_combinations.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/unique_combinations.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/raster_processing/windowing.py` & `eis_toolkit-0.4.1/eis_toolkit/raster_processing/windowing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/training_data_tools/class_balancing.py` & `eis_toolkit-0.4.1/eis_toolkit/training_data_tools/class_balancing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/binarize.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/binarize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/clip.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/clip.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/coda/alr.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/alr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/coda/clr.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/clr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/coda/ilr.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/ilr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/coda/pairwise.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/pairwise.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/coda/plr.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/coda/plr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/linear.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/linear.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/logarithmic.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/logarithmic.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/one_hot_encoding.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/sigmoid.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/transformations/winsorize.py` & `eis_toolkit-0.4.1/eis_toolkit/transformations/winsorize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/aitchison_geometry.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/aitchison_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/checks/compositional.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/compositional.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/checks/dataframe.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/checks/geometry.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/checks/parameter.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/parameter.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/checks/raster.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/checks/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/conversions.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/conversions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/file_io.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/file_io.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/miscellaneous.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/utilities/nodata.py` & `eis_toolkit-0.4.1/eis_toolkit/utilities/nodata.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/validation/calculate_base_metrics.py` & `eis_toolkit-0.4.1/eis_toolkit/evaluation/calculate_base_metrics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/validation/get_pa_intersection.py` & `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_prediction_area_curves.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,96 @@
+import matplotlib
 import numpy as np
 import pandas as pd
 from beartype import beartype
 from beartype.typing import Tuple, Union
+from matplotlib import pyplot as plt
 from shapely.geometry import LineString
-from shapely.geometry.point import Point
 
 from eis_toolkit.exceptions import InvalidParameterValueException
 
 
 def _get_pa_intersection(
     true_positive_rate_values: Union[np.ndarray, pd.Series],
     proportion_of_area_values: Union[np.ndarray, pd.Series],
     threshold_values: Union[np.ndarray, pd.Series],
-) -> Point:
+) -> Tuple[float, float]:
     true_positive_area_curve = LineString(np.column_stack((threshold_values, true_positive_rate_values)))
     proportion_of_area_values_curve = LineString(np.column_stack((threshold_values, 1 - proportion_of_area_values)))
     intersection = true_positive_area_curve.intersection(proportion_of_area_values_curve)
 
-    return intersection
+    return intersection.x, intersection.y
+
+
+def _plot_prediction_area_curves(
+    true_positive_rate_values: Union[np.ndarray, pd.Series],
+    proportion_of_area_values: Union[np.ndarray, pd.Series],
+    threshold_values: Union[np.ndarray, pd.Series],
+) -> matplotlib.figure.Figure:
+    x, y = _get_pa_intersection(true_positive_rate_values, proportion_of_area_values, threshold_values)
+
+    fig = plt.figure(figsize=(10, 7))
+    ax1 = fig.add_subplot(111)
+    ax2 = ax1.twinx()
+    ax1.plot(threshold_values, true_positive_rate_values, "r-", label="Prediction rate")
+
+    ax2.plot(threshold_values, proportion_of_area_values, "b-", label="Area")
+    ax2.plot(x, 1 - y, " o", markersize=7, c="black", label="Intersection point")
+    ax1.set_ylim(0, 1.01)
+    ax2.set_ylim(-0.01, 1)
+    ax2.invert_yaxis()
+    ax1.set_xlabel("Threshold")
+    ax1.set_ylabel("True positive rate", color="r")
+    ax2.set_ylabel("Proportion of area", color="b")
+    ax1.annotate(
+        text="TPR:" + str(round(y, 2)),
+        xy=(x, y),
+        xytext=(x + threshold_values.max() / 10, y),
+        arrowprops=dict(facecolor="black", shrink=0.09, width=0.3),
+        verticalalignment="center",
+    )
+    fig.legend(bbox_to_anchor=(0.3, 0.6), bbox_transform=ax1.transAxes)
+    plt.title("Prediction-area plot")
+
+    return fig
 
 
 @beartype
-def get_pa_intersection(
+def plot_prediction_area_curves(
     true_positive_rate_values: Union[np.ndarray, pd.Series],
     proportion_of_area_values: Union[np.ndarray, pd.Series],
     threshold_values: Union[np.ndarray, pd.Series],
-) -> Tuple[float, float]:
-    """Calculate the intersection point for prediction rate and area curves in (P-A plot).
+) -> matplotlib.figure.Figure:
+    """Plot prediction-area (P-A) plot.
+
+    Plots prediction area plot that can be used to evaluate mineral prospectivity maps and evidential layers. See e.g.,
+    Yousefi and Carranza (2015).
 
-    Threshold_values values act as x-axis for both curves. Prediction rate curve uses true positive rate for y-axis.
-    Area curve uses inverted proportion of area as y-axis.
+    The inputs needed for this tool can be obtained with calculate_base_metrics() tool.
 
     Args:
-        true_positive_rate_values: True positive rate values, values should be within range 0-1.
-        proportion_of_area_values: Proportion of area values, values should be within range 0-1.
-        threshold_values: Threshold values that were used to calculate true positive rate and proportion of area.
+        true_positive_rate_values: True positive rate values.
+        proportion_of_area_values: Proportion of area values.
+        threshold_values: Threshold values.
 
     Returns:
-        X and y coordinates of the intersection point.
+        P-A plot figure object.
 
     Raises:
         InvalidParameterValueException: true_positive_rate_values or proportion_of_area_values values are out of bounds.
+
+    References:
+        Yousefi, Mahyar, and Emmanuel John M. Carranza. "Fuzzification of continuous-value spatial evidence for mineral
+        prospectivity mapping." Computers & Geosciences 74 (2015): 97-109.
     """
     if true_positive_rate_values.max() > 1 or true_positive_rate_values.min() < 0:
-        raise InvalidParameterValueException("true_positive_rate_values values should be within range 0-1")
+        raise InvalidParameterValueException("true_positive_rate values should be within range 0-1")
 
     if proportion_of_area_values.max() > 1 or proportion_of_area_values.min() < 0:
-        raise InvalidParameterValueException("proportion_of_area_values values should be within range 0-1")
+        raise InvalidParameterValueException("proportion_of_area values should be within range 0-1")
 
-    intersection = _get_pa_intersection(
+    fig = _plot_prediction_area_curves(
         true_positive_rate_values=true_positive_rate_values,
         proportion_of_area_values=proportion_of_area_values,
         threshold_values=threshold_values,
     )
-
-    return intersection.x, intersection.y
+    return fig
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/validation/plot_confusion_matrix.py` & `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_confusion_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 from matplotlib.colors import Colormap
 
 from eis_toolkit.exceptions import InvalidDataShapeException
 
 
 @beartype
 def plot_confusion_matrix(
-    confusion_matrix: np.ndarray, cmap: Optional[Union[str, Colormap, Sequence]] = None
+    confusion_matrix: np.ndarray,
+    cmap: Optional[Union[str, Colormap, Sequence]] = None,
+    plot_title: str = "Confusion matrix",
+    ax: Optional[plt.Axes] = None,
+    **kwargs,
 ) -> plt.Axes:
     """Plot confusion matrix to visualize classification results.
 
     Args:
         confusion_matrix: The confusion matrix as 2D Numpy array. Expects the first element
             (upper-left corner) to have True negatives.
         cmap: Colormap name, matploltib colormap objects or list of colors for coloring the plot.
             Optional parameter.
+        plot_title: Title for the plot. Defaults to "Confusion matrix".
+        ax: An existing Axes in which to draw the plot. Defaults to None.
+        **kwargs: Additional keyword arguments passed to sns.heatmap.
 
     Returns:
         Matplotlib axes containing the plot.
 
     Raises:
         InvalidDataShapeException: Raised if input confusion matrix is not square.
     """
@@ -36,11 +43,11 @@
 
     if shape == (2, 2):  # Binary classificaiton
         names = ["True Neg", "False Pos", "False Neg", "True Pos"]
         labels = np.asarray([f"{v1}\n{v2}\n{v3}" for v1, v2, v3 in zip(names, counts, percentages)]).reshape(shape)
     else:
         labels = np.asarray([f"{v1}\n{v2}" for v1, v2 in zip(counts, percentages)]).reshape(shape)
 
-    ax = sns.heatmap(confusion_matrix, annot=labels, fmt="", cmap=cmap)
-    ax.set(xlabel="Predicted label", ylabel="True label")
+    out_ax = sns.heatmap(confusion_matrix, annot=labels, fmt="", cmap=cmap, ax=ax, **kwargs)
+    out_ax.set(xlabel="Predicted label", ylabel="True label", title=plot_title)
 
-    return ax
+    return out_ax
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/validation/plot_nn_model_performance.py` & `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_nn_model_performance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/validation/plot_rate_curve.py` & `eis_toolkit-0.4.1/eis_toolkit/evaluation/plot_rate_curve.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,61 @@
 import matplotlib
 import numpy as np
 import pandas as pd
 from beartype import beartype
-from beartype.typing import Literal, Union
+from beartype.typing import Union
 from matplotlib import pyplot as plt
+from sklearn.metrics import auc
 
 from eis_toolkit.exceptions import InvalidParameterValueException
-from eis_toolkit.validation.calculate_auc import calculate_auc
 
 
 def _plot_rate_curve(
     x_values: Union[np.ndarray, pd.Series], y_values: Union[np.ndarray, pd.Series], label: str, xlab: str
 ) -> matplotlib.figure.Figure:
     fig = plt.figure(figsize=(10, 7))
     plt.plot(x_values, y_values, label=label)
     plt.xlim(-0.01, 1)
     plt.ylim(0, 1.01)
     plt.xlabel(xlab)
     plt.ylabel("True positive rate")
     plt.plot([0, 1], [0, 1], "--", label="Random baseline")
     auc_bbox = dict(boxstyle="round", facecolor="grey", alpha=0.2)
-    auc = str(round(calculate_auc(x_values, y_values), 2))
-    plt.text(0.8, 0.2, "AUC: " + auc, bbox=auc_bbox)
+    auc_value = str(round(auc(x_values, y_values), 2))
+    plt.text(0.8, 0.2, "AUC: " + auc_value, bbox=auc_bbox)
     plt.title(label)
     fig.legend(bbox_to_anchor=(0.85, 0.4))
 
     return fig
 
 
 @beartype
 def plot_rate_curve(
     x_values: Union[np.ndarray, pd.Series],
     y_values: Union[np.ndarray, pd.Series],
-    plot_type: Literal["success_rate", "prediction_rate", "roc"] = "success_rate",
+    plot_title: str = "success_rate",
 ) -> matplotlib.figure.Figure:
-    """Plot success rate, prediction rate or ROC curve.
+    """Plot success rate.
 
-    Plot type depends on plot_type argument. Y-axis is always true positive rate, while x-axis can be either false
-    positive rate (roc) or proportion of area (success and prediction rate) depending on plot type.
+    Y-axis is true positive rate and x-axis is proportion of area.
 
     Args:
-        x_values: False positive rate values or proportion of area values.
+        x_values: Proportion of area values.
         y_values: True positive rate values.
-        plot_type: Plot type. Can be either: "success_rate", "prediction_rate" or "roc".
+        plot_title: Success rate
 
     Returns:
-        Success rate, prediction rate or ROC plot figure object.
+        Matplotlib figure containing the produced plot.
 
     Raises:
         InvalidParameterValueException: Invalid plot type.
         InvalidParameterValueException: x_values or y_values are out of bounds.
     """
-    if plot_type == "success_rate":
-        label = "Success rate"
-        xlab = "Proportion of area"
-    elif plot_type == "prediction_rate":
-        label = "Prediction rate"
-        xlab = "Proportion of area"
-    elif plot_type == "roc":
-        label = "ROC"
-        xlab = "False positive rate"
-    else:
-        raise InvalidParameterValueException("Invalid plot type")
+    label = plot_title
+    xlab = "Proportion of area"
 
     if x_values.max() > 1 or x_values.min() < 0:
         raise InvalidParameterValueException("x_values should be within range 0-1")
 
     if y_values.max() > 1 or y_values.min() < 0:
         raise InvalidParameterValueException("y_values should be within range 0-1")
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/calculate_geometry.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/calculate_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/cell_based_association.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/cell_based_association.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/distance_computation.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/distance_computation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,63 @@
+from numbers import Number
+
 import geopandas as gpd
 import numpy as np
 from beartype import beartype
-from beartype.typing import Union
+from beartype.typing import Optional, Union
 from rasterio import profiles, transform
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
-from eis_toolkit.exceptions import EmptyDataFrameException, NonMatchingCrsException
+from eis_toolkit.exceptions import EmptyDataFrameException, NonMatchingCrsException, NumericValueSignException
 from eis_toolkit.utilities.checks.raster import check_raster_profile
 from eis_toolkit.utilities.miscellaneous import row_points
 
 
 @beartype
-def distance_computation(raster_profile: Union[profiles.Profile, dict], geometries: gpd.GeoDataFrame) -> np.ndarray:
+def distance_computation(
+    geodataframe: gpd.GeoDataFrame, raster_profile: Union[profiles.Profile, dict], max_distance: Optional[Number] = None
+) -> np.ndarray:
     """Calculate distance from raster cell to nearest geometry.
 
     Args:
+        geodataframe: The GeoDataFrame with geometries to determine distance to.
         raster_profile: The raster profile of the raster in which the distances
             to the nearest geometry are determined.
-        geometries: The geometries to determine distance to.
+        max_distance: The maximum distance in the output array.
 
     Returns:
         A 2D numpy array with the distances computed.
 
+    Raises:
+        NonMatchingCrsException: The input raster profile and geodataframe have mismatching CRS.
+        EmptyDataFrameException: The input geodataframe is empty.
     """
-    if raster_profile.get("crs") != geometries.crs:
-        raise NonMatchingCrsException("Expected coordinate systems to match between raster and geometries. ")
-    if geometries.shape[0] == 0:
+    if raster_profile.get("crs") != geodataframe.crs:
+        raise NonMatchingCrsException("Expected coordinate systems to match between raster and GeoDataFrame.")
+    if geodataframe.shape[0] == 0:
         raise EmptyDataFrameException("Expected GeoDataFrame to not be empty.")
+    if max_distance is not None and max_distance <= 0:
+        raise NumericValueSignException("Expected max distance to be a positive number.")
 
     check_raster_profile(raster_profile=raster_profile)
 
     raster_width = raster_profile.get("width")
     raster_height = raster_profile.get("height")
     raster_transform = raster_profile.get("transform")
 
-    return _distance_computation(
-        raster_width=raster_width, raster_height=raster_height, raster_transform=raster_transform, geometries=geometries
+    distance_matrix = _distance_computation(
+        raster_width=raster_width,
+        raster_height=raster_height,
+        raster_transform=raster_transform,
+        geodataframe=geodataframe,
     )
+    if max_distance is not None:
+        distance_matrix[distance_matrix > max_distance] = max_distance
+
+    return distance_matrix
 
 
 def _calculate_row_distances(
     row: int,
     cols: np.ndarray,
     raster_transform: transform.Affine,
     geometries_unary_union: Union[BaseGeometry, BaseMultipartGeometry],
@@ -51,21 +68,21 @@
             for point in row_points(row=row, cols=cols, raster_transform=raster_transform)
         ]
     )
     return row_distances
 
 
 def _distance_computation(
-    raster_width: int, raster_height: int, raster_transform: transform.Affine, geometries: gpd.GeoDataFrame
+    raster_width: int, raster_height: int, raster_transform: transform.Affine, geodataframe: gpd.GeoDataFrame
 ) -> np.ndarray:
 
     cols = np.arange(raster_width)
     rows = np.arange(raster_height)
 
-    geometries_unary_union = geometries.geometry.unary_union
+    geometries_unary_union = geodataframe.geometry.unary_union
 
     distance_matrix = np.array(
         [
             _calculate_row_distances(
                 row=row, cols=cols, raster_transform=raster_transform, geometries_unary_union=geometries_unary_union
             )
             for row in rows
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/extract_shared_lines.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/extract_shared_lines.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/kriging_interpolation.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/kriging_interpolation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,105 @@
-from numbers import Number
-
 import geopandas as gpd
 import numpy as np
 from beartype import beartype
-from beartype.typing import Literal, Optional, Tuple
+from beartype.typing import Literal, Union
 from pykrige.ok import OrdinaryKriging
 from pykrige.uk import UniversalKriging
-from rasterio import transform
+from rasterio import profiles, transform
 
-from eis_toolkit.exceptions import EmptyDataFrameException, InvalidParameterValueException
+from eis_toolkit.exceptions import EmptyDataFrameException, InvalidParameterValueException, NonMatchingCrsException
+from eis_toolkit.utilities.checks.raster import check_raster_profile
 
 
 def _kriging(
     data: gpd.GeoDataFrame,
     target_column: str,
-    resolution: Tuple[Number, Number],
-    extent: Optional[Tuple[Number, Number, Number, Number]],
-    variogram_model: Literal,
-    coordinates_type: Literal,
-    method: Literal,
-) -> Tuple[np.ndarray, dict]:
+    raster_width: int,
+    raster_height: int,
+    raster_transform: transform.Affine,
+    variogram_model: Literal["linear", "power", "gaussian", "spherical", "exponential"],
+    coordinates_type: Literal["euclidean", "geographic"],
+    method: Literal["ordinary", "universal"],
+) -> np.ndarray:
 
     x = data.geometry.x
     y = data.geometry.y
     z = data[target_column].values
 
-    if extent is None:
-        grid_x_min = data.geometry.total_bounds[0]
-        grid_x_max = data.geometry.total_bounds[2]
-        grid_y_min = data.geometry.total_bounds[1]
-        grid_y_max = data.geometry.total_bounds[3]
-
-    else:
-        grid_x_min, grid_x_max, grid_y_min, grid_y_max = extent
+    pixel_size_x = raster_transform.a
+    pixel_size_y = abs(raster_transform.e)
+    grid_x_min = raster_transform.xoff
+    grid_x_max = grid_x_min + raster_width * pixel_size_x
+    grid_y_max = raster_transform.yoff
+    grid_y_min = grid_y_max - raster_height * pixel_size_y
 
-    grid_x = np.arange(grid_x_min, grid_x_max + resolution[0], resolution[0])
-    grid_y = np.arange(grid_y_min, grid_y_max + resolution[1], resolution[1])
+    grid_x = np.arange(grid_x_min, grid_x_max, pixel_size_x)
+    grid_y = np.arange(grid_y_min, grid_y_max, pixel_size_y)
 
     if method == "universal":
-        universal_kriging = UniversalKriging(x, y, z, variogram_model=variogram_model, drift_terms=["regional_linear"])
-        z_interpolated, _ = universal_kriging.execute("grid", grid_x, grid_y)
-
-    if method == "ordinary":
-        ordinary_kriging = OrdinaryKriging(x, y, z, variogram_model=variogram_model, coordinates_type=coordinates_type)
-        z_interpolated, _ = ordinary_kriging.execute("grid", grid_x, grid_y)
-
-    out_meta = {
-        "crs": data.crs,
-        "width": len(grid_x),
-        "height": len(grid_y),
-        "transform": transform.from_bounds(grid_x_min, grid_y_min, grid_x_max, grid_y_max, len(grid_x), len(grid_y)),
-    }
+        kriging_method = UniversalKriging(x, y, z, variogram_model=variogram_model, drift_terms=["regional_linear"])
+    elif method == "ordinary":
+        kriging_method = OrdinaryKriging(x, y, z, variogram_model=variogram_model, coordinates_type=coordinates_type)
+    z_interpolated, _ = kriging_method.execute("grid", grid_x, grid_y)
 
-    return z_interpolated, out_meta
+    return z_interpolated
 
 
 @beartype
 def kriging(
-    data: gpd.GeoDataFrame,
+    geodataframe: gpd.GeoDataFrame,
     target_column: str,
-    resolution: Tuple[Number, Number],
-    extent: Optional[Tuple[Number, Number, Number, Number]] = None,
+    raster_profile: Union[profiles.Profile, dict],
     variogram_model: Literal["linear", "power", "gaussian", "spherical", "exponential"] = "linear",
     coordinates_type: Literal["euclidean", "geographic"] = "geographic",
     method: Literal["ordinary", "universal"] = "ordinary",
-) -> Tuple[np.ndarray, dict]:
+) -> np.ndarray:
     """
     Perform Kriging interpolation on the input data.
 
     Args:
-        data: GeoDataFrame containing the input data.
+        geodataframe: GeoDataFrame containing the input data.
         target_column: The column name with values for each geometry.
-        resolution: The resolution i.e. cell size of the output raster as (pixel_size_x, pixel_size_y).
-        extent: The extent of the output raster as (x_min, x_max, y_min, y_max).
-            If None, calculate extent from the input vector data.
-        variogram_model: Variogram model to be used.
-            Either 'linear', 'power', 'gaussian', 'spherical' or 'exponential'. Defaults to 'linear'.
+        raster_profile: The raster profile used for output grid properties. Needs to include at least
+            crs, transform, width and height.
+        variogram_model: Variogram model to be used. Either 'linear', 'power', 'gaussian', 'spherical'
+            or 'exponential'. Defaults to 'linear'.
         coordinates_type: Determines are coordinates on a plane ('euclidean') or a sphere ('geographic').
             Used only in ordinary kriging. Defaults to 'geographic'.
         method: Ordinary or universal kriging. Defaults to 'ordinary'.
 
     Returns:
-        Grid containing the interpolated values and metadata.
+        Numpy array containing the interpolated values.
 
     Raises:
         EmptyDataFrameException: The input GeoDataFrame is empty.
         InvalidParameterValueException: Target column name is invalid or resolution is not greater than zero.
+        NonMatchingCrsException: The input GeoDataFrame and raster profile have mismatching CRS.
     """
 
-    if data.empty:
-        raise EmptyDataFrameException("The input GeoDataFrame is empty.")
-
-    if target_column not in data.columns:
+    if geodataframe.empty:
+        raise EmptyDataFrameException("Expected GeoDataFrame to not be empty.")
+    if raster_profile.get("crs") != geodataframe.crs:
+        raise NonMatchingCrsException("Expected coordinate systems to match between raster and GeoDataFrame.")
+    if target_column not in geodataframe.columns:
         raise InvalidParameterValueException(
-            f"Expected target_column ({target_column}) to be contained in geodataframe columns."
+            f"Expected target_column ({target_column}) to be contained in GeoDataFrame columns."
         )
 
-    if resolution[0] <= 0 or resolution[1] <= 0:
-        raise InvalidParameterValueException("The resolution must be greater than zero.")
+    check_raster_profile(raster_profile)
 
-    data_interpolated, out_meta = _kriging(
-        data, target_column, resolution, extent, variogram_model, coordinates_type, method
+    raster_width = raster_profile.get("width")
+    raster_height = raster_profile.get("height")
+    raster_transform = raster_profile.get("transform")
+
+    data_interpolated = _kriging(
+        geodataframe,
+        target_column,
+        raster_width,
+        raster_height,
+        raster_transform,
+        variogram_model,
+        coordinates_type,
+        method,
     )
 
-    return data_interpolated, out_meta
+    return data_interpolated
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/rasterize_vector.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/rasterize_vector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,116 @@
 import geopandas as gpd
 import numpy as np
 from beartype import beartype
-from beartype.typing import Literal, Optional, Tuple, Union
+from beartype.typing import Literal, Optional, Union
 from rasterio import features, profiles, transform
 from rasterio.enums import MergeAlg
 
 from eis_toolkit.exceptions import (
     EmptyDataFrameException,
     InvalidColumnException,
-    InvalidParameterValueException,
+    NonMatchingCrsException,
     NumericValueSignException,
 )
+from eis_toolkit.utilities.checks.raster import check_raster_profile
 
 
 @beartype
 def rasterize_vector(
     geodataframe: gpd.GeoDataFrame,
-    resolution: Optional[float] = None,
+    raster_profile: Union[profiles.Profile, dict],
     value_column: Optional[str] = None,
     default_value: float = 1.0,
     fill_value: float = 0.0,
-    base_raster_profile: Optional[Union[profiles.Profile, dict]] = None,
     buffer_value: Optional[float] = None,
     merge_strategy: Literal["replace", "add"] = "replace",
-) -> Tuple[np.ndarray, dict]:
+) -> np.ndarray:
     """Transform vector data into raster data.
 
     Args:
         geodataframe: The vector dataframe to be rasterized.
-        resolution: The resolution i.e. cell size of the output raster.
-            Optional if base_raster_profile is given.
+        raster_profile: The raster profile used for output grid properties.
+            Needs to include at least CRS, transform, width and height.
         value_column: The column name with values for each geometry.
             If None, then default_value is used for all geometries.
         default_value: Default value burned into raster cells based on geometries.
-        base_raster_profile: Base raster profile
-            to be used for determining the grid on which vectors are
-            burned in. If None, the geometries and provided resolution
-            value are used to compute grid.
         fill_value: Value used outside the burned/rasterized geometry cells.
-        buffer_value: For adding a buffer around passed
-            geometries before rasterization.
+        buffer_value: For adding a buffer around passed geometries before rasterization.
         merge_strategy: How to handle overlapping geometries.
             "add" causes overlapping geometries to add together the
             values while "replace" does not. Adding them together is the
             basis for density computations where the density can be
             calculated by using a default value of 1.0 and the sum in
             each cell is the count of intersecting geometries.
 
     Returns:
-        Rasterized vector data and metadata.
+        Rasterized vector data..
 
     Raises:
         EmptyDataFrameException: The geodataframe does not contain geometries.
         InvalidColumnException: Given value_column is not in the input geodataframe.
-        InvalidParameterValueException: No resolution or base_raster_profile is given,
-            or base_raster_profile has the wrong type.
+        NonMatchingCrsException: The input GeoDataFrame and raster profile have mismatching CRS.
         NumericValueSignException: Input resolution value is zero or negative, or input
             buffer_value is negative.
     """
-
-    if geodataframe.shape[0] == 0:
+    if geodataframe.empty:
         raise EmptyDataFrameException("Expected geodataframe to contain geometries.")
-
-    if resolution is None and base_raster_profile is None:
-        raise InvalidParameterValueException("Expected either resolution or base_raster_profile to be given.")
-
-    if resolution is not None and resolution <= 0:
-        raise NumericValueSignException(f"Expected a positive resolution value ({dict(resolution=resolution)})")
-
+    if raster_profile.get("crs") != geodataframe.crs:
+        raise NonMatchingCrsException("Expected coordinate systems to match between raster and GeoDataFrame.")
     if value_column is not None and value_column not in geodataframe.columns:
         raise InvalidColumnException(f"Expected value_column ({value_column}) to be contained in geodataframe columns.")
-
-    if buffer_value is not None and buffer_value < 0:
-        raise NumericValueSignException(f"Expected a positive buffer_value ({dict(buffer_value=buffer_value)})")
-
-    if base_raster_profile is not None and not isinstance(base_raster_profile, (profiles.Profile, dict)):
-        raise InvalidParameterValueException(
-            f"Expected base_raster_profile ({type(base_raster_profile)}) to be dict or rasterio.profiles.Profile."
-        )
+    check_raster_profile(raster_profile)
 
     if buffer_value is not None:
+        if buffer_value < 0:
+            raise NumericValueSignException(f"Expected a positive buffer_value ({dict(buffer_value=buffer_value)})")
+
         geodataframe = geodataframe.copy()
         geodataframe["geometry"] = geodataframe["geometry"].apply(lambda geom: geom.buffer(buffer_value))
 
-    return _rasterize_vector(
+    raster_width = raster_profile.get("width")
+    raster_height = raster_profile.get("height")
+    raster_transform = raster_profile.get("transform")
+
+    out_image = _rasterize_vector(
         geodataframe=geodataframe,
+        raster_width=raster_width,
+        raster_height=raster_height,
+        raster_transform=raster_transform,
         value_column=value_column,
         default_value=default_value,
         fill_value=fill_value,
-        base_raster_profile=base_raster_profile,
-        resolution=resolution,
         merge_alg=getattr(MergeAlg, merge_strategy),
     )
-
-
-def _transform_from_geometries(
-    geodataframe: gpd.GeoDataFrame, resolution: float
-) -> Tuple[float, float, transform.Affine]:
-    """Determine transform from the input geometries.
-
-    Returns:
-        Width, height and transform of the raster in a tuple.
-    """
-    min_x, min_y, max_x, max_y = geodataframe.total_bounds
-    width = (max_x - min_x) / resolution
-    height = (max_y - min_y) / resolution
-
-    out_transform = transform.from_bounds(min_x, min_y, max_x, max_y, width=width, height=height)
-    return width, height, out_transform
+    return out_image
 
 
 def _rasterize_vector(
     geodataframe: gpd.GeoDataFrame,
+    raster_width: int,
+    raster_height: int,
+    raster_transform: transform.Affine,
     value_column: Optional[str],
     default_value: float,
     fill_value: float,
-    base_raster_profile: Optional[Union[profiles.Profile, dict]],
-    resolution: Optional[float],
     merge_alg: MergeAlg,
-) -> Tuple[np.ndarray, dict]:
+) -> np.ndarray:
     # rasterio.features.rasterize expects a shapes parameter which is
     # an iterable of tuples where the first value is a geometry and
     # the other a value for the geometry
     # Alternatively, if there are not values for each geometry,
     # an iterable of geometries can be passed
+
     geometries = geodataframe["geometry"].values
     values = geodataframe[value_column].values if value_column is not None else None
     geometry_value_pairs = list(geometries) if values is None else list(zip(geometries, values))
 
-    if base_raster_profile is None and resolution is not None:
-        width, height, out_transform = _transform_from_geometries(geodataframe=geodataframe, resolution=resolution)
-    elif base_raster_profile is not None:
-        width, height, out_transform = (
-            base_raster_profile["width"],
-            base_raster_profile["height"],
-            base_raster_profile["transform"],
-        )
-    else:
-        raise InvalidParameterValueException("Expected resolution or base_raster_profile to be given.")
-
     out_raster_array = features.rasterize(
         shapes=geometry_value_pairs,
         # fill and default_value can be floats even though typing claims otherwise
         fill=fill_value,
         default_value=default_value,
-        transform=out_transform,
-        out_shape=(round(height), round(width)),
+        transform=raster_transform,
+        out_shape=(raster_height, raster_width),
         merge_alg=merge_alg,
     )
-    return out_raster_array, dict(transform=out_transform, height=height, width=width)
+    return out_raster_array
```

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/reproject_vector.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/reproject_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.4.0/eis_toolkit/vector_processing/vector_density.py` & `eis_toolkit-0.4.1/eis_toolkit/vector_processing/vector_density.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import geopandas as gpd
 import numpy as np
 from beartype import beartype
-from beartype.typing import Literal, Optional, Tuple, Union
+from beartype.typing import Literal, Optional, Union
 from rasterio import profiles
 
 from eis_toolkit.vector_processing.rasterize_vector import rasterize_vector
 
 
 @beartype
 def vector_density(
     geodataframe: gpd.GeoDataFrame,
-    resolution: Optional[float] = None,
-    base_raster_profile: Optional[Union[profiles.Profile, dict]] = None,
+    raster_profile: Union[profiles.Profile, dict],
     buffer_value: Optional[float] = None,
     statistic: Literal["density", "count"] = "density",
-) -> Tuple[np.ndarray, dict]:
+) -> np.ndarray:
     """Compute density of geometries within raster.
 
     Args:
-        geodataframe: The dataframe with vectors
-            of which density is computed.
-        resolution: The resolution i.e. cell size of the output raster.
-            Optional if base_raster_profile is given.
-        base_raster_profile: Base raster profile
-            to be used for determining the grid on which vectors are
-            burned in. If None, the geometries and provided resolution
-            value are used to compute grid.
-        buffer_value: For adding a buffer around passed
-            geometries before computing density.
+        geodataframe: The dataframe with vectors of which density is computed.
+        base_raster_profile: Base raster profile to be used for determining
+            the grid on which vectors are burned in. If None, the geometries
+            and provided resolution value are used to compute grid.
+        buffer_value: For adding a buffer around passed geometries before computing density.
+        statistic: The statistic to use in density computation. Defaults to "density".
 
     Returns:
-        Computed density of vector data and metadata.
+        Computed density of vector data.
     """
-    out_raster_array, out_metadata = rasterize_vector(
+    out_raster_array = rasterize_vector(
         geodataframe=geodataframe,
-        resolution=resolution,
-        base_raster_profile=base_raster_profile,
+        raster_profile=raster_profile,
         buffer_value=buffer_value,
         value_column=None,
         default_value=1.0,
         fill_value=0.0,
         merge_strategy="add",
     )
     max_count = np.max(out_raster_array)
     if statistic == "count" or np.isclose(max_count, 0.0):
-        return out_raster_array, out_metadata
+        return out_raster_array
     else:
-        return (out_raster_array / max_count), out_metadata
+        return out_raster_array / max_count
```

### Comparing `eis_toolkit-0.4.0/pyproject.toml` & `eis_toolkit-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eis_toolkit"
-version = "0.4.0"
+version = "0.4.1"
 description = "EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union."
 authors = []
 maintainers = ["Gispo Ltd. <info@gispo.fi>"]
 license = "EUPL-1.2"
 readme = "README.md"
 homepage = "https://eis-he.eu"
 repository = "https://github.com/GispoCoding/eis_toolkit"
```

### Comparing `eis_toolkit-0.4.0/PKG-INFO` & `eis_toolkit-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis_toolkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union.
 Home-page: https://eis-he.eu
 License: EUPL-1.2
 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/Engineering :: GIS,Programming Language :: Python :: 3 :: Only
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 Requires-Python: >=3.9,<3.11
@@ -69,24 +69,34 @@
 EIS Toolkit is a comprehensive Python package for mineral prospectivity mapping and analysis. EIS Toolkit is developed as part of [EIS Horizon EU project](https://eis-he.eu/), which aims to aid EU's efforts in the green transition by securing critical raw materials. EIS Toolkit serves both as a standalone library that brings together and implements relevant tools for mineral prospectivity mapping and as a computational backend for [EIS QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin).
 
 > [!NOTE]  
 > This repository is still in development. Check the [wiki page of EIS Toolkit](https://github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap](#roadmap) for more details about the project.
 
 
 ## Installation
-You can find the latest release of EIS Toolkit in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) as a Python wheel. To install EIS Toolkit, download the wheel and install with pip
+We recommend installing EIS Toolkit in an empty virtual environment to ensure compatibility between package versions. 
+
+EIS Toolkit is available in conda-forge and PyPI and can be installed with one of the following commands.
 
 ```console
-pip install eis_toolkit-0.4.0-py3-none-any.whl
+pip install eis_toolkit
+```
+
+```console
+conda-install -c conda-forge eis_toolkit
 ```
 
-We recommend installing EIS Toolkit in an empty virtual environment to ensure compatibility between package versions.
+You can find the latest release of EIS Toolkit also in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a Python wheel. Just download the wheel and install with pip
+
+```console
+pip install eis_toolkit-0.4.0-py3-none-any.whl
+```
 
-> [!NOTE]
-> EIS Toolkit has not yet been released in PyPi or Conda, but will be at a later stage.
+> [!TIP]
+> GDAL installation can cause issues on various platforms, especially on Windows. If you have trouble installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
 
 
 ## Usage
 EIS Toolkit can be used in Python scripts, Jupyter notebooks or via the CLI. At the moment, most tools have their own module and are imported like this:
 ```python
 # In general
 from eis_toolkit.category.module import module_function
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_g0980_xp_/tmp5pt9o707_TarContainer/0/101", line 41, column 35: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eis_toolkit Version: 0.4.0 Summary: EIS Toolkit is
+Metadata-Version: 2.1 Name: eis_toolkit Version: 0.4.1 Summary: EIS Toolkit is
 a comprehensive collection of tools suitable for mineral prospectivity mapping.
 This toolkit has been developed as part of the Exploration Information System
 project which has been funded by European Union. Home-page: https://eis-he.eu
 License: EUPL-1.2 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/
 Engineering :: GIS,Programming Language :: Python :: 3 :: Only Maintainer:
 Gispo Ltd. Maintainer-email: info@gispo.fi Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL
@@ -33,57 +33,62 @@
 (https://eis-he.eu/), which aims to aid EU's efforts in the green transition by
 securing critical raw materials. EIS Toolkit serves both as a standalone
 library that brings together and implements relevant tools for mineral
 prospectivity mapping and as a computational backend for [EIS QGIS Plugin]
 (https://github.com/GispoCoding/eis_qgis_plugin). > [!NOTE] > This repository
 is still in development. Check the [wiki page of EIS Toolkit](https://
 github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap]
-(#roadmap) for more details about the project. ## Installation You can find the
-latest release of EIS Toolkit in the [releases page](https://github.com/
-GispoCoding/eis_toolkit/releases) as a Python wheel. To install EIS Toolkit,
-download the wheel and install with pip ```console pip install eis_toolkit-
-0.4.0-py3-none-any.whl ``` We recommend installing EIS Toolkit in an empty
-virtual environment to ensure compatibility between package versions. > [!NOTE]
-> EIS Toolkit has not yet been released in PyPi or Conda, but will be at a
-later stage. ## Usage EIS Toolkit can be used in Python scripts, Jupyter
-notebooks or via the CLI. At the moment, most tools have their own module and
-are imported like this: ```python # In general from eis_toolkit.category.module
-import module_function # Some examples from
-eis_toolkit.raster_processing.reprojecting import reproject_raster from
-eis_toolkit.exploratory_analyses.pca import compute_pca ``` You can find
-several Jupyter notebooks in this repostiory that demonstrate how tools of EIS
-Toolkit can be used. The documentation of EIS Toolkit can be read [here](https:
-//gispocoding.github.io/eis_toolkit/). ### EIS QGIS Plugin For those that
-prefer using tools of EIS Toolkit via a graphical user interface, check [EIS
-QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin
-includes the main GUI application called EIS Wizard and all individual EIS
-Toolkit tools as QGIS processing algorithms. The plugin is developed by the
-same core team that develops EIS Toolkit. ### CLI EIS Toolkit includes a
-[Typer](https://typer.tiangolo.com/) command-line interface that serves as a
-common interface for integrating the toolkit with external applications, such
-as QGIS. However, it can be used directly too. To use the CLI, simply use the
-command ```console eis ``` or ```console eis --help ``` to get started.
-However, please note that the CLI has been primarily designed to communicate
-with external programs and may feel clunky in direct use. ## Roadmap -
-Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the
-basic funtionalities required for a full MPM workflow. Official testing phase
-begins. The plugin will be still under active development. - Milestone 2:
-**Release 1.0** (April 2024). All features should be incorporated at this time
-and the toolkit useful for actual MPM work. Testing will continue, potential
-bugs will be fixed and the user experience refined. ## Contributing We welcome
-contributions to EIS Toolkit in various forms: - â¨ Developing new tools -
-ð Fixing bugs in the code - ð Bug and other reporting - ð¡ Feature
-suggestions To contribute with code or documentation, you'll need a local
-development environment and a copy of the repository. Please refer to the **For
-developers** section below for detailed setup instructions. If you're
-interested in bug reporting or making feature suggestions, you can familiarize
-yourself with the toolkit and test it as described in the **Usage** section.
-When you encounter bugs or have ideas for new features, you can create an issue
-in this repository. ### For developers All contributing developers need Git and
-a copy of the repository. ```console git clone https://github.com/GispoCoding/
-eis_toolkit.git ``` After this you have three options for setting up your local
-development environment. 1. Docker - [instructions](./instructions/
-dev_setup_with_docker.md) 2. Poetry - [instructions](./instructions/
-dev_setup_without_docker.md) 3. Conda - [instructions](./instructions/
-dev_setup_without_docker_with_conda.md) *For general contributing guidelines,
-see [CONTRIBUTING](./CONTRIBUTING.md).* ## License Licensed under the EUPL-1.2
-or later.
+(#roadmap) for more details about the project. ## Installation We recommend
+installing EIS Toolkit in an empty virtual environment to ensure compatibility
+between package versions. EIS Toolkit is available in conda-forge and PyPI and
+can be installed with one of the following commands. ```console pip install
+eis_toolkit ``` ```console conda-install -c conda-forge eis_toolkit ``` You can
+find the latest release of EIS Toolkit also in the [releases page](https://
+github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a
+Python wheel. Just download the wheel and install with pip ```console pip
+install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL installation can
+cause issues on various platforms, especially on Windows. If you have trouble
+installing EIS Toolkit in a venv due to GDAL, download a compatible GDAL wheel
+(for example from [this repository](https://github.com/cgohlke/geospatial-
+wheels/releases)), install it first, and then attempt to install EIS Toolkit
+again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter notebooks or
+via the CLI. At the moment, most tools have their own module and are imported
+like this: ```python # In general from eis_toolkit.category.module import
+module_function # Some examples from eis_toolkit.raster_processing.reprojecting
+import reproject_raster from eis_toolkit.exploratory_analyses.pca import
+compute_pca ``` You can find several Jupyter notebooks in this repostiory that
+demonstrate how tools of EIS Toolkit can be used. The documentation of EIS
+Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/). ### EIS
+QGIS Plugin For those that prefer using tools of EIS Toolkit via a graphical
+user interface, check [EIS QGIS Plugin](https://github.com/GispoCoding/
+eis_qgis_plugin). The plugin includes the main GUI application called EIS
+Wizard and all individual EIS Toolkit tools as QGIS processing algorithms. The
+plugin is developed by the same core team that develops EIS Toolkit. ### CLI
+EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line
+interface that serves as a common interface for integrating the toolkit with
+external applications, such as QGIS. However, it can be used directly too. To
+use the CLI, simply use the command ```console eis ``` or ```console eis --help
+``` to get started. However, please note that the CLI has been primarily
+designed to communicate with external programs and may feel clunky in direct
+use. ## Roadmap - Milestone 1: **Beta release 0.1** (November 2023). The
+toolkit should have the basic funtionalities required for a full MPM workflow.
+Official testing phase begins. The plugin will be still under active
+development. - Milestone 2: **Release 1.0** (April 2024). All features should
+be incorporated at this time and the toolkit useful for actual MPM work.
+Testing will continue, potential bugs will be fixed and the user experience
+refined. ## Contributing We welcome contributions to EIS Toolkit in various
+forms: - â¨ Developing new tools - ð Fixing bugs in the code - ð Bug and
+other reporting - ð¡ Feature suggestions To contribute with code or
+documentation, you'll need a local development environment and a copy of the
+repository. Please refer to the **For developers** section below for detailed
+setup instructions. If you're interested in bug reporting or making feature
+suggestions, you can familiarize yourself with the toolkit and test it as
+described in the **Usage** section. When you encounter bugs or have ideas for
+new features, you can create an issue in this repository. ### For developers
+All contributing developers need Git and a copy of the repository. ```console
+git clone https://github.com/GispoCoding/eis_toolkit.git ``` After this you
+have three options for setting up your local development environment. 1. Docker
+- [instructions](./instructions/dev_setup_with_docker.md) 2. Poetry -
+[instructions](./instructions/dev_setup_without_docker.md) 3. Conda -
+[instructions](./instructions/dev_setup_without_docker_with_conda.md) *For
+general contributing guidelines, see [CONTRIBUTING](./CONTRIBUTING.md).* ##
+License Licensed under the EUPL-1.2 or later.
```

