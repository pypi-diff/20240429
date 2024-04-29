# Comparing `tmp/biapy-3.4.0.tar.gz` & `tmp/biapy-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biapy-3.4.0.tar", last modified: Sun Apr 28 18:08:37 2024, max compression
+gzip compressed data, was "biapy-3.4.1.tar", last modified: Mon Apr 29 07:14:32 2024, max compression
```

## Comparing `biapy-3.4.0.tar` & `biapy-3.4.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.395937 biapy-3.4.0/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1079 2023-10-17 15:21:29.000000 biapy-3.4.0/LICENSE.md
--rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23460 2024-04-28 18:08:37.395937 biapy-3.4.0/PKG-INFO
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    20933 2024-02-13 08:45:05.000000 biapy-3.4.0/README.md
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.387937 biapy-3.4.0/biapy/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2097 2024-04-28 17:54:13.000000 biapy-3.4.0/biapy/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19820 2024-04-10 10:46:29.000000 biapy-3.4.0/biapy/_biapy.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.387937 biapy-3.4.0/biapy/config/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       22 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/config/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    75069 2024-04-17 17:01:31.000000 biapy-3.4.0/biapy/config/config.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.387937 biapy-3.4.0/biapy/data/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        0 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/data/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    41275 2024-04-17 17:47:14.000000 biapy-3.4.0/biapy/data/data_2D_manipulation.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    62136 2024-04-10 10:46:29.000000 biapy-3.4.0/biapy/data/data_3D_manipulation.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.387937 biapy-3.4.0/biapy/data/generators/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    27729 2024-04-17 17:30:50.000000 biapy-3.4.0/biapy/data/generators/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66739 2024-04-14 17:29:53.000000 biapy-3.4.0/biapy/data/generators/augmentors.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    69342 2024-04-17 17:47:56.000000 biapy-3.4.0/biapy/data/generators/pair_base_data_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5531 2024-04-10 07:02:56.000000 biapy-3.4.0/biapy/data/generators/pair_data_2D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7767 2024-04-11 11:49:07.000000 biapy-3.4.0/biapy/data/generators/pair_data_3D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21839 2024-04-17 17:50:54.000000 biapy-3.4.0/biapy/data/generators/single_base_data_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1612 2024-01-10 14:40:34.000000 biapy-3.4.0/biapy/data/generators/single_data_2D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2864 2024-04-10 07:26:02.000000 biapy-3.4.0/biapy/data/generators/single_data_3D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18735 2024-04-17 17:33:33.000000 biapy-3.4.0/biapy/data/generators/test_pair_data_generators.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10205 2024-04-17 17:33:22.000000 biapy-3.4.0/biapy/data/generators/test_single_data_generator.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.387937 biapy-3.4.0/biapy/data/post_processing/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3028 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/data/post_processing/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    76121 2024-02-25 18:30:55.000000 biapy-3.4.0/biapy/data/post_processing/post_processing.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10434 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/data/post_processing/smooth_tiled_predictions.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    59239 2024-04-17 17:29:25.000000 biapy-3.4.0/biapy/data/pre_processing.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.391937 biapy-3.4.0/biapy/engine/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2606 2024-02-23 08:04:46.000000 biapy-3.4.0/biapy/engine/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    92000 2024-04-14 15:50:07.000000 biapy-3.4.0/biapy/engine/base_workflow.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    60824 2024-04-16 06:30:21.000000 biapy-3.4.0/biapy/engine/check_configuration.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    15050 2024-04-10 10:46:29.000000 biapy-3.4.0/biapy/engine/classification.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22609 2024-04-10 11:22:44.000000 biapy-3.4.0/biapy/engine/denoising.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    53161 2024-04-10 11:27:47.000000 biapy-3.4.0/biapy/engine/detection.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13410 2024-04-14 15:24:09.000000 biapy-3.4.0/biapy/engine/image_to_image.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    48257 2024-04-10 10:46:29.000000 biapy-3.4.0/biapy/engine/instance_seg.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    25026 2024-04-14 10:22:07.000000 biapy-3.4.0/biapy/engine/metrics.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.391937 biapy-3.4.0/biapy/engine/schedulers/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      956 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/engine/schedulers/warmup_cosine_decay.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21105 2024-04-10 11:29:23.000000 biapy-3.4.0/biapy/engine/self_supervised.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11246 2024-04-14 15:53:50.000000 biapy-3.4.0/biapy/engine/semantic_seg.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13055 2024-04-10 10:46:29.000000 biapy-3.4.0/biapy/engine/super_resolution.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4664 2024-04-10 06:46:00.000000 biapy-3.4.0/biapy/engine/train_engine.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.391937 biapy-3.4.0/biapy/models/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11931 2024-04-10 06:46:00.000000 biapy-3.4.0/biapy/models/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7576 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/attention_unet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    17636 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/models/blocks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3637 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/dfcan.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3305 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/edsr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1221 2024-02-05 08:46:05.000000 biapy-3.4.0/biapy/models/efficientnet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18737 2024-04-10 06:46:00.000000 biapy-3.4.0/biapy/models/mae.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13552 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/multiresunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2732 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/rcan.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     9139 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/resunet++.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7451 2024-03-06 11:13:09.000000 biapy-3.4.0/biapy/models/resunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7231 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/seunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2998 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/models/simple_cnn.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1734 2024-02-26 12:21:55.000000 biapy-3.4.0/biapy/models/tr_layers.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7186 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/unet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10300 2024-04-10 06:46:00.000000 biapy-3.4.0/biapy/models/unetr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3592 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/models/vit.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2982 2024-02-25 11:08:42.000000 biapy-3.4.0/biapy/models/wdsr.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.391937 biapy-3.4.0/biapy/utils/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4243 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/callbacks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    12958 2024-04-14 08:44:02.000000 biapy-3.4.0/biapy/utils/matching.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    14861 2024-03-01 08:53:49.000000 biapy-3.4.0/biapy/utils/misc.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.395937 biapy-3.4.0/biapy/utils/scripts/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3617 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/calculate_detection_metrics.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5803 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/calculate_metrics_3D.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5021 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/create_probability_csv.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1808 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/crop_2D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1171 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/crop_3D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1828 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/crop_and_discard_3D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1726 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/detection_plots.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4873 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/detection_probs_to_points.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2374 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/fill_holes_in_seg_masks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3864 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/filter_close_points.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1895 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/from_class_csv_to_folders.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      674 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/h5_to_tif.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1212 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/h5_to_zarr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2328 2024-04-22 08:23:08.000000 biapy-3.4.0/biapy/utils/scripts/lightmycell_data_preparation.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      920 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/merge_dataset_channels.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2538 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/order_axes.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      966 2024-01-08 16:04:47.000000 biapy-3.4.0/biapy/utils/scripts/tif_to_h5.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    57739 2024-04-14 16:12:07.000000 biapy-3.4.0/biapy/utils/util.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-28 18:08:37.395937 biapy-3.4.0/biapy.egg-info/
--rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23460 2024-04-28 18:08:37.000000 biapy-3.4.0/biapy.egg-info/PKG-INFO
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2703 2024-04-28 18:08:37.000000 biapy-3.4.0/biapy.egg-info/SOURCES.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        1 2024-04-28 18:08:37.000000 biapy-3.4.0/biapy.egg-info/dependency_links.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       37 2024-04-28 18:08:37.000000 biapy-3.4.0/biapy.egg-info/entry_points.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      323 2024-04-28 18:08:37.000000 biapy-3.4.0/biapy.egg-info/requires.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        6 2024-04-28 18:08:37.000000 biapy-3.4.0/biapy.egg-info/top_level.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1399 2024-04-28 18:08:22.000000 biapy-3.4.0/pyproject.toml
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       38 2024-04-28 18:08:37.395937 biapy-3.4.0/setup.cfg
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.041028 biapy-3.4.1/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1079 2023-10-17 15:21:29.000000 biapy-3.4.1/LICENSE.md
+-rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23491 2024-04-29 07:14:32.041028 biapy-3.4.1/PKG-INFO
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    20933 2024-02-13 08:45:05.000000 biapy-3.4.1/README.md
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.033028 biapy-3.4.1/biapy/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2097 2024-04-28 17:54:13.000000 biapy-3.4.1/biapy/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19820 2024-04-10 10:46:29.000000 biapy-3.4.1/biapy/_biapy.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.037028 biapy-3.4.1/biapy/config/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       22 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/config/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    75069 2024-04-17 17:01:31.000000 biapy-3.4.1/biapy/config/config.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.037028 biapy-3.4.1/biapy/data/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        0 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/data/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    41275 2024-04-17 17:47:14.000000 biapy-3.4.1/biapy/data/data_2D_manipulation.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    62136 2024-04-10 10:46:29.000000 biapy-3.4.1/biapy/data/data_3D_manipulation.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.037028 biapy-3.4.1/biapy/data/generators/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    27729 2024-04-17 17:30:50.000000 biapy-3.4.1/biapy/data/generators/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66739 2024-04-14 17:29:53.000000 biapy-3.4.1/biapy/data/generators/augmentors.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    69342 2024-04-17 17:47:56.000000 biapy-3.4.1/biapy/data/generators/pair_base_data_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5531 2024-04-10 07:02:56.000000 biapy-3.4.1/biapy/data/generators/pair_data_2D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7767 2024-04-11 11:49:07.000000 biapy-3.4.1/biapy/data/generators/pair_data_3D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21839 2024-04-17 17:50:54.000000 biapy-3.4.1/biapy/data/generators/single_base_data_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1612 2024-01-10 14:40:34.000000 biapy-3.4.1/biapy/data/generators/single_data_2D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2864 2024-04-10 07:26:02.000000 biapy-3.4.1/biapy/data/generators/single_data_3D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18735 2024-04-17 17:33:33.000000 biapy-3.4.1/biapy/data/generators/test_pair_data_generators.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10205 2024-04-17 17:33:22.000000 biapy-3.4.1/biapy/data/generators/test_single_data_generator.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.037028 biapy-3.4.1/biapy/data/post_processing/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3028 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/data/post_processing/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    76121 2024-02-25 18:30:55.000000 biapy-3.4.1/biapy/data/post_processing/post_processing.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10434 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/data/post_processing/smooth_tiled_predictions.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    59239 2024-04-17 17:29:25.000000 biapy-3.4.1/biapy/data/pre_processing.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.037028 biapy-3.4.1/biapy/engine/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2606 2024-02-23 08:04:46.000000 biapy-3.4.1/biapy/engine/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    92000 2024-04-14 15:50:07.000000 biapy-3.4.1/biapy/engine/base_workflow.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    60824 2024-04-16 06:30:21.000000 biapy-3.4.1/biapy/engine/check_configuration.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    15050 2024-04-10 10:46:29.000000 biapy-3.4.1/biapy/engine/classification.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22609 2024-04-10 11:22:44.000000 biapy-3.4.1/biapy/engine/denoising.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    53161 2024-04-10 11:27:47.000000 biapy-3.4.1/biapy/engine/detection.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13410 2024-04-14 15:24:09.000000 biapy-3.4.1/biapy/engine/image_to_image.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    48257 2024-04-10 10:46:29.000000 biapy-3.4.1/biapy/engine/instance_seg.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    25026 2024-04-14 10:22:07.000000 biapy-3.4.1/biapy/engine/metrics.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.037028 biapy-3.4.1/biapy/engine/schedulers/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      956 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/engine/schedulers/warmup_cosine_decay.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21105 2024-04-10 11:29:23.000000 biapy-3.4.1/biapy/engine/self_supervised.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11246 2024-04-14 15:53:50.000000 biapy-3.4.1/biapy/engine/semantic_seg.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13055 2024-04-10 10:46:29.000000 biapy-3.4.1/biapy/engine/super_resolution.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4664 2024-04-10 06:46:00.000000 biapy-3.4.1/biapy/engine/train_engine.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.041028 biapy-3.4.1/biapy/models/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11931 2024-04-10 06:46:00.000000 biapy-3.4.1/biapy/models/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7576 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/attention_unet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    17636 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/models/blocks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3637 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/dfcan.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3305 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/edsr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1221 2024-02-05 08:46:05.000000 biapy-3.4.1/biapy/models/efficientnet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18737 2024-04-10 06:46:00.000000 biapy-3.4.1/biapy/models/mae.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13552 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/multiresunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2732 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/rcan.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     9139 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/resunet++.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7451 2024-03-06 11:13:09.000000 biapy-3.4.1/biapy/models/resunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7231 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/seunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2998 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/models/simple_cnn.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1734 2024-02-26 12:21:55.000000 biapy-3.4.1/biapy/models/tr_layers.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7186 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/unet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10300 2024-04-10 06:46:00.000000 biapy-3.4.1/biapy/models/unetr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3592 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/models/vit.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2982 2024-02-25 11:08:42.000000 biapy-3.4.1/biapy/models/wdsr.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.041028 biapy-3.4.1/biapy/utils/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4243 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/callbacks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    12958 2024-04-14 08:44:02.000000 biapy-3.4.1/biapy/utils/matching.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    14861 2024-03-01 08:53:49.000000 biapy-3.4.1/biapy/utils/misc.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.041028 biapy-3.4.1/biapy/utils/scripts/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3617 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/calculate_detection_metrics.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5803 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/calculate_metrics_3D.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5021 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/create_probability_csv.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1808 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/crop_2D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1171 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/crop_3D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1828 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/crop_and_discard_3D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1726 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/detection_plots.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4873 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/detection_probs_to_points.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2374 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/fill_holes_in_seg_masks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3864 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/filter_close_points.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1895 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/from_class_csv_to_folders.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      674 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/h5_to_tif.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1212 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/h5_to_zarr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2328 2024-04-22 08:23:08.000000 biapy-3.4.1/biapy/utils/scripts/lightmycell_data_preparation.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      920 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/merge_dataset_channels.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2538 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/order_axes.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      966 2024-01-08 16:04:47.000000 biapy-3.4.1/biapy/utils/scripts/tif_to_h5.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    57739 2024-04-14 16:12:07.000000 biapy-3.4.1/biapy/utils/util.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 07:14:32.041028 biapy-3.4.1/biapy.egg-info/
+-rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23491 2024-04-29 07:14:32.000000 biapy-3.4.1/biapy.egg-info/PKG-INFO
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2703 2024-04-29 07:14:32.000000 biapy-3.4.1/biapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        1 2024-04-29 07:14:32.000000 biapy-3.4.1/biapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       37 2024-04-29 07:14:32.000000 biapy-3.4.1/biapy.egg-info/entry_points.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      339 2024-04-29 07:14:32.000000 biapy-3.4.1/biapy.egg-info/requires.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        6 2024-04-29 07:14:32.000000 biapy-3.4.1/biapy.egg-info/top_level.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1422 2024-04-29 07:13:37.000000 biapy-3.4.1/pyproject.toml
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       38 2024-04-29 07:14:32.041028 biapy-3.4.1/setup.cfg
```

### Comparing `biapy-3.4.0/LICENSE.md` & `biapy-3.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/PKG-INFO` & `biapy-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biapy
-Version: 3.4.0
+Version: 3.4.1
 Summary: BiaPy: Bioimage analysis pipelines in Python
 Author-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 Maintainer-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 License: MIT License
         
         Copyright (c) 2022 Daniel Franco-Barranco
         
@@ -32,15 +32,14 @@
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: imgaug>=0.4.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: pydot>=1.4.2
 Requires-Dist: yacs>=0.1.8
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: scikit-image>=0.22.0
 Requires-Dist: edt>=2.3.2
@@ -50,15 +49,17 @@
 Requires-Dist: torchinfo>=1.8.0
 Requires-Dist: tensorboardX>=2.6.2.2
 Requires-Dist: h5py>=3.9.0
 Requires-Dist: zarr>=2.16.1
 Requires-Dist: bioimageio.core==0.5.9
 Requires-Dist: imagecodecs>=2024.1.1
 Requires-Dist: pytorch-msssim>=1.0.0
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: numpy>=1.25.2
+Requires-Dist: imageio>=2.31.6
+Requires-Dist: imgaug>=0.4.0
 
 ![BiaPy logo](https://raw.githubusercontent.com/BiaPyX/BiaPy/master/img/biapy_logo.png)
 
 # BiaPy: Bioimage analysis pipelines in Python
 
 <p align="left">
     <a href="https://www.python.org/">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biapy Version: 3.4.0 Summary: BiaPy: Bioimage
+Metadata-Version: 2.1 Name: biapy Version: 3.4.1 Summary: BiaPy: Bioimage
 analysis pipelines in Python Author-email: Daniel Franco-Barranco
 dipc.org> Maintainer-email: Daniel Franco-Barranco
 dipc.org> License: MIT License Copyright (c) 2022 Daniel Franco-Barranco
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -17,24 +17,25 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://biapyx.github.io
 Project-URL: Source, https://github.com/BiaPyX/BiaPy Project-URL: Forum, https:
 //forum.image.sc/tag/biapy Keywords: feed,reader,tutorial Classifier: License
 :: OSI Approved :: MIT License Classifier: Environment :: GPU :: NVIDIA CUDA ::
 11.8 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-imgaug>=0.4.0 Requires-Dist: matplotlib>=3.7.1 Requires-Dist: scikit-
-learn>=1.4.0 Requires-Dist: pydot>=1.4.2 Requires-Dist: yacs>=0.1.8 Requires-
-Dist: tqdm>=4.66.1 Requires-Dist: scikit-image>=0.22.0 Requires-Dist:
-edt>=2.3.2 Requires-Dist: fill-voids>=2.0.6 Requires-Dist: opencv-
-python>=4.8.0.76 Requires-Dist: pandas>=1.5.3 Requires-Dist: torchinfo>=1.8.0
-Requires-Dist: tensorboardX>=2.6.2.2 Requires-Dist: h5py>=3.9.0 Requires-Dist:
-zarr>=2.16.1 Requires-Dist: bioimageio.core==0.5.9 Requires-Dist:
-imagecodecs>=2024.1.1 Requires-Dist: pytorch-msssim>=1.0.0 Requires-Dist:
-numpy>=1.26.4 ![BiaPy logo](https://raw.githubusercontent.com/BiaPyX/BiaPy/
-master/img/biapy_logo.png) # BiaPy: Bioimage analysis pipelines in Python
+matplotlib>=3.7.1 Requires-Dist: scikit-learn>=1.4.0 Requires-Dist:
+pydot>=1.4.2 Requires-Dist: yacs>=0.1.8 Requires-Dist: tqdm>=4.66.1 Requires-
+Dist: scikit-image>=0.22.0 Requires-Dist: edt>=2.3.2 Requires-Dist: fill-
+voids>=2.0.6 Requires-Dist: opencv-python>=4.8.0.76 Requires-Dist:
+pandas>=1.5.3 Requires-Dist: torchinfo>=1.8.0 Requires-Dist:
+tensorboardX>=2.6.2.2 Requires-Dist: h5py>=3.9.0 Requires-Dist: zarr>=2.16.1
+Requires-Dist: bioimageio.core==0.5.9 Requires-Dist: imagecodecs>=2024.1.1
+Requires-Dist: pytorch-msssim>=1.0.0 Requires-Dist: numpy>=1.25.2 Requires-
+Dist: imageio>=2.31.6 Requires-Dist: imgaug>=0.4.0 ![BiaPy logo](https://
+raw.githubusercontent.com/BiaPyX/BiaPy/master/img/biapy_logo.png) # BiaPy:
+Bioimage analysis pipelines in Python
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._1_0_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_P_y_T_o_r_c_h_-_2_._2_-_o_r_a_n_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
 _b_i_a_p_y_._s_v_g_?_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_-_L_a_t_e_s_t_-_2_B_A_F_2_B_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_b_i_o_R_x_i_v_-_P_a_p_e_r_-_b_d_2_6_3_5_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_I_E_E_E_-_P_a_p_e_r_-
 _0_0_6_2_9_B_._s_v_g_]
 ð¥**NEWS**ð¥: We have a new **preprint**! Check it out at bioRxiv: https://
```

### Comparing `biapy-3.4.0/README.md` & `biapy-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/__init__.py` & `biapy-3.4.1/biapy/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/_biapy.py` & `biapy-3.4.1/biapy/_biapy.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/config/config.py` & `biapy-3.4.1/biapy/config/config.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/data_2D_manipulation.py` & `biapy-3.4.1/biapy/data/data_2D_manipulation.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/data_3D_manipulation.py` & `biapy-3.4.1/biapy/data/data_3D_manipulation.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/__init__.py` & `biapy-3.4.1/biapy/data/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/augmentors.py` & `biapy-3.4.1/biapy/data/generators/augmentors.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/pair_base_data_generator.py` & `biapy-3.4.1/biapy/data/generators/pair_base_data_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/pair_data_2D_generator.py` & `biapy-3.4.1/biapy/data/generators/pair_data_2D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/pair_data_3D_generator.py` & `biapy-3.4.1/biapy/data/generators/pair_data_3D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/single_base_data_generator.py` & `biapy-3.4.1/biapy/data/generators/single_base_data_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/single_data_2D_generator.py` & `biapy-3.4.1/biapy/data/generators/single_data_2D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/single_data_3D_generator.py` & `biapy-3.4.1/biapy/data/generators/single_data_3D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/test_pair_data_generators.py` & `biapy-3.4.1/biapy/data/generators/test_pair_data_generators.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/generators/test_single_data_generator.py` & `biapy-3.4.1/biapy/data/generators/test_single_data_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/post_processing/__init__.py` & `biapy-3.4.1/biapy/data/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/post_processing/post_processing.py` & `biapy-3.4.1/biapy/data/post_processing/post_processing.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/post_processing/smooth_tiled_predictions.py` & `biapy-3.4.1/biapy/data/post_processing/smooth_tiled_predictions.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/data/pre_processing.py` & `biapy-3.4.1/biapy/data/pre_processing.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/__init__.py` & `biapy-3.4.1/biapy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/base_workflow.py` & `biapy-3.4.1/biapy/engine/base_workflow.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/check_configuration.py` & `biapy-3.4.1/biapy/engine/check_configuration.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/classification.py` & `biapy-3.4.1/biapy/engine/classification.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/denoising.py` & `biapy-3.4.1/biapy/engine/denoising.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/detection.py` & `biapy-3.4.1/biapy/engine/detection.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/image_to_image.py` & `biapy-3.4.1/biapy/engine/image_to_image.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/instance_seg.py` & `biapy-3.4.1/biapy/engine/instance_seg.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/metrics.py` & `biapy-3.4.1/biapy/engine/metrics.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/schedulers/warmup_cosine_decay.py` & `biapy-3.4.1/biapy/engine/schedulers/warmup_cosine_decay.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/self_supervised.py` & `biapy-3.4.1/biapy/engine/self_supervised.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/semantic_seg.py` & `biapy-3.4.1/biapy/engine/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/super_resolution.py` & `biapy-3.4.1/biapy/engine/super_resolution.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/engine/train_engine.py` & `biapy-3.4.1/biapy/engine/train_engine.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/__init__.py` & `biapy-3.4.1/biapy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/attention_unet.py` & `biapy-3.4.1/biapy/models/attention_unet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/blocks.py` & `biapy-3.4.1/biapy/models/blocks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/dfcan.py` & `biapy-3.4.1/biapy/models/dfcan.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/edsr.py` & `biapy-3.4.1/biapy/models/edsr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/efficientnet.py` & `biapy-3.4.1/biapy/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/mae.py` & `biapy-3.4.1/biapy/models/mae.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/multiresunet.py` & `biapy-3.4.1/biapy/models/multiresunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/rcan.py` & `biapy-3.4.1/biapy/models/rcan.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/resunet++.py` & `biapy-3.4.1/biapy/models/resunet++.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/resunet.py` & `biapy-3.4.1/biapy/models/resunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/seunet.py` & `biapy-3.4.1/biapy/models/seunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/simple_cnn.py` & `biapy-3.4.1/biapy/models/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/tr_layers.py` & `biapy-3.4.1/biapy/models/tr_layers.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/unet.py` & `biapy-3.4.1/biapy/models/unet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/unetr.py` & `biapy-3.4.1/biapy/models/unetr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/vit.py` & `biapy-3.4.1/biapy/models/vit.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/models/wdsr.py` & `biapy-3.4.1/biapy/models/wdsr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/callbacks.py` & `biapy-3.4.1/biapy/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/matching.py` & `biapy-3.4.1/biapy/utils/matching.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/misc.py` & `biapy-3.4.1/biapy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/calculate_detection_metrics.py` & `biapy-3.4.1/biapy/utils/scripts/calculate_detection_metrics.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/calculate_metrics_3D.py` & `biapy-3.4.1/biapy/utils/scripts/calculate_metrics_3D.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/create_probability_csv.py` & `biapy-3.4.1/biapy/utils/scripts/create_probability_csv.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/crop_2D_dataset.py` & `biapy-3.4.1/biapy/utils/scripts/crop_2D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/crop_3D_dataset.py` & `biapy-3.4.1/biapy/utils/scripts/crop_3D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/crop_and_discard_3D_dataset.py` & `biapy-3.4.1/biapy/utils/scripts/crop_and_discard_3D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/detection_plots.py` & `biapy-3.4.1/biapy/utils/scripts/detection_plots.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/detection_probs_to_points.py` & `biapy-3.4.1/biapy/utils/scripts/detection_probs_to_points.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/fill_holes_in_seg_masks.py` & `biapy-3.4.1/biapy/utils/scripts/fill_holes_in_seg_masks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/filter_close_points.py` & `biapy-3.4.1/biapy/utils/scripts/filter_close_points.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/from_class_csv_to_folders.py` & `biapy-3.4.1/biapy/utils/scripts/from_class_csv_to_folders.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/h5_to_tif.py` & `biapy-3.4.1/biapy/utils/scripts/h5_to_tif.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/h5_to_zarr.py` & `biapy-3.4.1/biapy/utils/scripts/h5_to_zarr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/lightmycell_data_preparation.py` & `biapy-3.4.1/biapy/utils/scripts/lightmycell_data_preparation.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/merge_dataset_channels.py` & `biapy-3.4.1/biapy/utils/scripts/merge_dataset_channels.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/order_axes.py` & `biapy-3.4.1/biapy/utils/scripts/order_axes.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/scripts/tif_to_h5.py` & `biapy-3.4.1/biapy/utils/scripts/tif_to_h5.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy/utils/util.py` & `biapy-3.4.1/biapy/utils/util.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/biapy.egg-info/PKG-INFO` & `biapy-3.4.1/biapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biapy
-Version: 3.4.0
+Version: 3.4.1
 Summary: BiaPy: Bioimage analysis pipelines in Python
 Author-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 Maintainer-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 License: MIT License
         
         Copyright (c) 2022 Daniel Franco-Barranco
         
@@ -32,15 +32,14 @@
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: imgaug>=0.4.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: pydot>=1.4.2
 Requires-Dist: yacs>=0.1.8
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: scikit-image>=0.22.0
 Requires-Dist: edt>=2.3.2
@@ -50,15 +49,17 @@
 Requires-Dist: torchinfo>=1.8.0
 Requires-Dist: tensorboardX>=2.6.2.2
 Requires-Dist: h5py>=3.9.0
 Requires-Dist: zarr>=2.16.1
 Requires-Dist: bioimageio.core==0.5.9
 Requires-Dist: imagecodecs>=2024.1.1
 Requires-Dist: pytorch-msssim>=1.0.0
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: numpy>=1.25.2
+Requires-Dist: imageio>=2.31.6
+Requires-Dist: imgaug>=0.4.0
 
 ![BiaPy logo](https://raw.githubusercontent.com/BiaPyX/BiaPy/master/img/biapy_logo.png)
 
 # BiaPy: Bioimage analysis pipelines in Python
 
 <p align="left">
     <a href="https://www.python.org/">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biapy Version: 3.4.0 Summary: BiaPy: Bioimage
+Metadata-Version: 2.1 Name: biapy Version: 3.4.1 Summary: BiaPy: Bioimage
 analysis pipelines in Python Author-email: Daniel Franco-Barranco
 dipc.org> Maintainer-email: Daniel Franco-Barranco
 dipc.org> License: MIT License Copyright (c) 2022 Daniel Franco-Barranco
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -17,24 +17,25 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://biapyx.github.io
 Project-URL: Source, https://github.com/BiaPyX/BiaPy Project-URL: Forum, https:
 //forum.image.sc/tag/biapy Keywords: feed,reader,tutorial Classifier: License
 :: OSI Approved :: MIT License Classifier: Environment :: GPU :: NVIDIA CUDA ::
 11.8 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-imgaug>=0.4.0 Requires-Dist: matplotlib>=3.7.1 Requires-Dist: scikit-
-learn>=1.4.0 Requires-Dist: pydot>=1.4.2 Requires-Dist: yacs>=0.1.8 Requires-
-Dist: tqdm>=4.66.1 Requires-Dist: scikit-image>=0.22.0 Requires-Dist:
-edt>=2.3.2 Requires-Dist: fill-voids>=2.0.6 Requires-Dist: opencv-
-python>=4.8.0.76 Requires-Dist: pandas>=1.5.3 Requires-Dist: torchinfo>=1.8.0
-Requires-Dist: tensorboardX>=2.6.2.2 Requires-Dist: h5py>=3.9.0 Requires-Dist:
-zarr>=2.16.1 Requires-Dist: bioimageio.core==0.5.9 Requires-Dist:
-imagecodecs>=2024.1.1 Requires-Dist: pytorch-msssim>=1.0.0 Requires-Dist:
-numpy>=1.26.4 ![BiaPy logo](https://raw.githubusercontent.com/BiaPyX/BiaPy/
-master/img/biapy_logo.png) # BiaPy: Bioimage analysis pipelines in Python
+matplotlib>=3.7.1 Requires-Dist: scikit-learn>=1.4.0 Requires-Dist:
+pydot>=1.4.2 Requires-Dist: yacs>=0.1.8 Requires-Dist: tqdm>=4.66.1 Requires-
+Dist: scikit-image>=0.22.0 Requires-Dist: edt>=2.3.2 Requires-Dist: fill-
+voids>=2.0.6 Requires-Dist: opencv-python>=4.8.0.76 Requires-Dist:
+pandas>=1.5.3 Requires-Dist: torchinfo>=1.8.0 Requires-Dist:
+tensorboardX>=2.6.2.2 Requires-Dist: h5py>=3.9.0 Requires-Dist: zarr>=2.16.1
+Requires-Dist: bioimageio.core==0.5.9 Requires-Dist: imagecodecs>=2024.1.1
+Requires-Dist: pytorch-msssim>=1.0.0 Requires-Dist: numpy>=1.25.2 Requires-
+Dist: imageio>=2.31.6 Requires-Dist: imgaug>=0.4.0 ![BiaPy logo](https://
+raw.githubusercontent.com/BiaPyX/BiaPy/master/img/biapy_logo.png) # BiaPy:
+Bioimage analysis pipelines in Python
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._1_0_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_P_y_T_o_r_c_h_-_2_._2_-_o_r_a_n_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
 _b_i_a_p_y_._s_v_g_?_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_-_L_a_t_e_s_t_-_2_B_A_F_2_B_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_b_i_o_R_x_i_v_-_P_a_p_e_r_-_b_d_2_6_3_5_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_I_E_E_E_-_P_a_p_e_r_-
 _0_0_6_2_9_B_._s_v_g_]
 ð¥**NEWS**ð¥: We have a new **preprint**! Check it out at bioRxiv: https://
```

### Comparing `biapy-3.4.0/biapy.egg-info/SOURCES.txt` & `biapy-3.4.1/biapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biapy-3.4.0/pyproject.toml` & `biapy-3.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biapy"
-version = "3.4.0"
+version = "3.4.1"
 description = "BiaPy: Bioimage analysis pipelines in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{ name = "Daniel Franco-Barranco", email = "daniel.franco@dipc.org" }]
 maintainers = [{ name = "Daniel Franco-Barranco", email = "daniel.franco@dipc.org" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Environment :: GPU :: NVIDIA CUDA :: 11.8",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["feed", "reader", "tutorial"]
 dependencies = [
-    "imgaug>=0.4.0",
     "matplotlib>=3.7.1",
     "scikit-learn>=1.4.0",
     "pydot>=1.4.2",
     "yacs>=0.1.8",
     "tqdm>=4.66.1",
     "scikit-image>=0.22.0",
     "edt>=2.3.2",
@@ -32,15 +31,17 @@
     "torchinfo>=1.8.0",
     "tensorboardX>=2.6.2.2",
     "h5py>=3.9.0",
     "zarr>=2.16.1",
     "bioimageio.core==0.5.9",
     "imagecodecs>=2024.1.1",
     "pytorch-msssim>=1.0.0",
-    "numpy>=1.26.4",
+    "numpy>=1.25.2",
+    "imageio>=2.31.6",
+    "imgaug>=0.4.0",
 ]
 
 [project.scripts]
 biapy = "biapy:main"
 
 [project.urls]
 "Homepage" = "https://biapyx.github.io"
```

