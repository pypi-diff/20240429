# Comparing `tmp/pybaseutils-1.0.5.tar.gz` & `tmp/pybaseutils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaseutils-1.0.5.tar", last modified: Wed Apr 17 03:54:49 2024, max compression
+gzip compressed data, was "pybaseutils-1.0.6.tar", last modified: Mon Apr 29 03:16:55 2024, max compression
```

## Comparing `pybaseutils-1.0.5.tar` & `pybaseutils-1.0.6.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.540737 pybaseutils-1.0.5/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.5/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3944 2024-04-17 03:54:49.540398 pybaseutils-1.0.5/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.5/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.409094 pybaseutils-1.0.5/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-04-17 03:54:45.000000 pybaseutils-1.0.5/pybaseutils/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.414853 pybaseutils-1.0.5/pybaseutils/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.5/pybaseutils/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.5/pybaseutils/audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.5/pybaseutils/audio/pyaudio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.5/pybaseutils/audio/vad_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/base64_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.5/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.416692 pybaseutils-1.0.5/pybaseutils/build_utils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.5/pybaseutils/build_utils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.5/pybaseutils/build_utils/cython_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.5/pybaseutils/build_utils/pyarmor_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.419394 pybaseutils-1.0.5/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.5/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.5/pybaseutils/config_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.429336 pybaseutils-1.0.5/pybaseutils/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.5/pybaseutils/converter/build_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.5/pybaseutils/converter/build_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.5/pybaseutils/converter/build_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.5/pybaseutils/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_coco2labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.5/pybaseutils/converter/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.5/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.432421 pybaseutils-1.0.5/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.5/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10572 2024-03-01 02:06:03.000000 pybaseutils-1.0.5/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.5/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.5/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.440160 pybaseutils-1.0.5/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.5/pybaseutils/dataloader/base_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7634 2024-03-18 07:07:15.000000 pybaseutils-1.0.5/pybaseutils/dataloader/base_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_det.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7946 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_ins.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_kps.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17642 2024-04-17 03:54:20.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17629 2024-03-18 07:11:47.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.0.5/pybaseutils/dataloader/parser_yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.5/pybaseutils/dataloader/voc_seg_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39284 2024-03-15 09:42:00.000000 pybaseutils-1.0.5/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.444848 pybaseutils-1.0.5/pybaseutils/filter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/filter/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/filter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.5/pybaseutils/filter/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/filter/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.5/pybaseutils/filter/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.5/pybaseutils/filter/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.5/pybaseutils/filter/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.445546 pybaseutils-1.0.5/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.5/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.5/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)   103608 2024-03-27 03:34:35.000000 pybaseutils-1.0.5/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4480 2023-08-11 03:00:05.000000 pybaseutils-1.0.5/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.5/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.449630 pybaseutils-1.0.5/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.5/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.5/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.452516 pybaseutils-1.0.5/pybaseutils/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.5/pybaseutils/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.5/pybaseutils/pose/bones_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.5/pybaseutils/pose/human_pose.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.5/pybaseutils/pose/pose_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.454237 pybaseutils-1.0.5/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.5/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.5/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/pycpp/main.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.455515 pybaseutils-1.0.5/pybaseutils/server/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.5/pybaseutils/server/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.5/pybaseutils/server/apm_server.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.5/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.5/pybaseutils/singleton_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.5/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.5/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.460516 pybaseutils-1.0.5/pybaseutils/tracking/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/tracking/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/tracking/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.5/pybaseutils/tracking/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.5/pybaseutils/tracking/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.5/pybaseutils/tracking/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.5/pybaseutils/tracking/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.5/pybaseutils/tracking/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.463908 pybaseutils-1.0.5/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.5/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5104 2024-02-05 11:42:05.000000 pybaseutils-1.0.5/pybaseutils/transforms/face_alignment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5150 2024-02-21 06:07:01.000000 pybaseutils-1.0.5/pybaseutils/transforms/transform_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.5/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.5/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.5/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.412339 pybaseutils-1.0.5/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3944 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6937 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.5/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-04-17 03:54:49.000000 pybaseutils-1.0.5/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-04-17 03:54:49.540829 pybaseutils-1.0.5/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.5/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.487275 pybaseutils-1.0.5/test_py/
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.489146 pybaseutils-1.0.5/test_py/WebCrawler/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.5/test_py/WebCrawler/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.5/test_py/WebCrawler/search_image.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.5/test_py/WebCrawler/search_image_for_baidu.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.499144 pybaseutils-1.0.5/test_py/aije/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.5/test_py/aije/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.5/test_py/aije/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.0.5/test_py/aije/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.0.5/test_py/aije/copy_move.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.0.5/test_py/aije/demo_video_aije.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.5/test_py/aije/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.0.5/test_py/aije/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.5/test_py/aije/video_demo.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.503572 pybaseutils-1.0.5/test_py/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.5/test_py/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.5/test_py/audio/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.5/test_py/audio/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.5/test_py/audio/main_read.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.5/test_py/audio/segment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.5/test_py/audio/speechbrain_asr_indoor_prod.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.5/test_py/audio/speechbrain_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.5/test_py/class_attribute.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.5/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.519943 pybaseutils-1.0.5/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.5/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.5/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.5/test_py/converter/FL3D_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.5/test_py/converter/FreiHAND2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.5/test_py/converter/MTFL2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2718 2024-02-21 06:07:01.000000 pybaseutils-1.0.5/test_py/converter/WaterMeters.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.5/test_py/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.5/test_py/converter/convert_gesture2hand.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.5/test_py/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.5/test_py/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.5/test_py/converter/fatigue_driving.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/fdd_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.5/test_py/converter/handpose2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.5/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.0.5/test_py/converter/voc_sbd2labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.525220 pybaseutils-1.0.5/test_py/cython_build/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.5/test_py/cython_build/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.5/test_py/cython_build/build_cython.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.5/test_py/cython_build/build_pyarmor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.5/test_py/cython_build/cryptography_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.5/test_py/cython_build/fun_sum.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.5/test_py/cython_build/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.5/test_py/cython_build/model_des_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.5/test_py/cython_build/model_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2614 2024-02-21 01:59:28.000000 pybaseutils-1.0.5/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.5/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.5/test_py/demo3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.5/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.5/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.5/test_py/demo_coco_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.5/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.5/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.5/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.5/test_py/demo_for_pair_file.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.5/test_py/demo_for_polygon.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.5/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.5/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.5/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.5/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.5/test_py/demo_image_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.5/test_py/demo_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.5/test_py/demo_nii.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.5/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.5/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1049 2024-04-15 12:43:54.000000 pybaseutils-1.0.5/test_py/demo_rename.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.5/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.5/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.5/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.5/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.5/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.5/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.5/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.527489 pybaseutils-1.0.5/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.5/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.5/test_py/detector/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.5/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.5/test_py/detector/predet_labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.530223 pybaseutils-1.0.5/test_py/edit_distance/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.5/test_py/edit_distance/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.5/test_py/edit_distance/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.5/test_py/edit_distance/text_matching.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.5/test_py/edit_distance/text_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.531903 pybaseutils-1.0.5/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.5/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.5/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.5/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.534708 pybaseutils-1.0.5/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.5/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.5/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.5/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.5/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.5/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.5/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.5/test_py/performance.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.536208 pybaseutils-1.0.5/test_py/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.5/test_py/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.5/test_py/pose/human_pose.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-17 03:54:49.539663 pybaseutils-1.0.5/test_py/registry/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.5/test_py/registry/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.5/test_py/registry/base.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.5/test_py/registry/component.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.5/test_py/registry/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.5/test_py/registry/register.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.097719 pybaseutils-1.0.6/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.6/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-29 03:16:55.097348 pybaseutils-1.0.6/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.6/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.965375 pybaseutils-1.0.6/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-04-29 03:16:31.000000 pybaseutils-1.0.6/pybaseutils/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.970428 pybaseutils-1.0.6/pybaseutils/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.6/pybaseutils/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.6/pybaseutils/audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.6/pybaseutils/audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.6/pybaseutils/audio/vad_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/base64_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.6/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.972337 pybaseutils-1.0.6/pybaseutils/build_utils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.6/pybaseutils/build_utils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.6/pybaseutils/build_utils/cython_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.6/pybaseutils/build_utils/pyarmor_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.975096 pybaseutils-1.0.6/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.6/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.6/pybaseutils/config_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.985195 pybaseutils-1.0.6/pybaseutils/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.6/pybaseutils/converter/build_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.6/pybaseutils/converter/build_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.6/pybaseutils/converter/build_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.6/pybaseutils/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_coco2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_labelme2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_voc2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_voc2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.6/pybaseutils/converter/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.6/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.990458 pybaseutils-1.0.6/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.6/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10928 2024-04-28 11:36:44.000000 pybaseutils-1.0.6/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.6/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.6/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.998094 pybaseutils-1.0.6/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.6/pybaseutils/dataloader/base_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7634 2024-03-18 07:07:15.000000 pybaseutils-1.0.6/pybaseutils/dataloader/base_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.0.6/pybaseutils/dataloader/parser_coco_det.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7946 2024-03-18 07:53:24.000000 pybaseutils-1.0.6/pybaseutils/dataloader/parser_coco_ins.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.0.6/pybaseutils/dataloader/parser_coco_kps.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17737 2024-04-17 06:17:13.000000 pybaseutils-1.0.6/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17629 2024-03-18 07:11:47.000000 pybaseutils-1.0.6/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.0.6/pybaseutils/dataloader/parser_yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.6/pybaseutils/dataloader/voc_seg_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39284 2024-03-15 09:42:00.000000 pybaseutils-1.0.6/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.003356 pybaseutils-1.0.6/pybaseutils/filter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.6/pybaseutils/filter/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.6/pybaseutils/filter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.6/pybaseutils/filter/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.6/pybaseutils/filter/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.6/pybaseutils/filter/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.6/pybaseutils/filter/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.6/pybaseutils/filter/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.004691 pybaseutils-1.0.6/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.6/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.6/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)   103608 2024-03-27 03:34:35.000000 pybaseutils-1.0.6/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4480 2023-08-11 03:00:05.000000 pybaseutils-1.0.6/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.6/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.009143 pybaseutils-1.0.6/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.6/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.6/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.011989 pybaseutils-1.0.6/pybaseutils/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.6/pybaseutils/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.6/pybaseutils/pose/bones_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.6/pybaseutils/pose/human_pose.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.6/pybaseutils/pose/pose_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.013962 pybaseutils-1.0.6/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.6/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.6/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/pycpp/main.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.015262 pybaseutils-1.0.6/pybaseutils/server/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.6/pybaseutils/server/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.6/pybaseutils/server/apm_server.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.6/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.6/pybaseutils/singleton_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.6/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.6/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.020002 pybaseutils-1.0.6/pybaseutils/tracking/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.6/pybaseutils/tracking/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.6/pybaseutils/tracking/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.6/pybaseutils/tracking/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.6/pybaseutils/tracking/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.6/pybaseutils/tracking/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.6/pybaseutils/tracking/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.6/pybaseutils/tracking/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.022808 pybaseutils-1.0.6/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.6/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5112 2024-04-28 11:41:39.000000 pybaseutils-1.0.6/pybaseutils/transforms/face_alignment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7103 2024-04-29 02:20:17.000000 pybaseutils-1.0.6/pybaseutils/transforms/transform_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.6/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.6/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.6/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:54.967944 pybaseutils-1.0.6/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-29 03:16:54.000000 pybaseutils-1.0.6/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6937 2024-04-29 03:16:54.000000 pybaseutils-1.0.6/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-04-29 03:16:54.000000 pybaseutils-1.0.6/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.6/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-04-29 03:16:54.000000 pybaseutils-1.0.6/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-04-29 03:16:55.097823 pybaseutils-1.0.6/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.6/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.046597 pybaseutils-1.0.6/test_py/
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.048642 pybaseutils-1.0.6/test_py/WebCrawler/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.6/test_py/WebCrawler/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.6/test_py/WebCrawler/search_image.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.6/test_py/WebCrawler/search_image_for_baidu.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/test_py/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.054022 pybaseutils-1.0.6/test_py/aije/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.6/test_py/aije/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.6/test_py/aije/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.0.6/test_py/aije/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.0.6/test_py/aije/copy_move.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.0.6/test_py/aije/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.6/test_py/aije/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.0.6/test_py/aije/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.6/test_py/aije/video_demo.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.058887 pybaseutils-1.0.6/test_py/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.6/test_py/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.6/test_py/audio/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.6/test_py/audio/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.6/test_py/audio/main_read.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.6/test_py/audio/segment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.6/test_py/audio/speechbrain_asr_indoor_prod.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.6/test_py/audio/speechbrain_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.6/test_py/class_attribute.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.6/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.075783 pybaseutils-1.0.6/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.6/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.6/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.6/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.6/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.6/test_py/converter/FL3D_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.6/test_py/converter/FreiHAND2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.6/test_py/converter/MTFL2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.6/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2723 2024-04-28 11:46:31.000000 pybaseutils-1.0.6/test_py/converter/WaterMeters.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/test_py/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.6/test_py/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.6/test_py/converter/convert_gesture2hand.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.6/test_py/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.6/test_py/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.6/test_py/converter/fatigue_driving.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/test_py/converter/fdd_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.6/test_py/converter/handpose2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.6/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.6/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.0.6/test_py/converter/voc_sbd2labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.081065 pybaseutils-1.0.6/test_py/cython_build/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.6/test_py/cython_build/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.6/test_py/cython_build/build_cython.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.6/test_py/cython_build/build_pyarmor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.6/test_py/cython_build/cryptography_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.6/test_py/cython_build/fun_sum.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.6/test_py/cython_build/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.6/test_py/cython_build/model_des_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.6/test_py/cython_build/model_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1088 2024-04-28 12:11:12.000000 pybaseutils-1.0.6/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.6/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.6/test_py/demo3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.6/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.6/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.6/test_py/demo_coco_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.6/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.6/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.6/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.6/test_py/demo_for_pair_file.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.6/test_py/demo_for_polygon.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.6/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.6/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.6/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.6/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.6/test_py/demo_image_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.6/test_py/demo_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.6/test_py/demo_nii.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.6/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.6/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1056 2024-04-19 09:16:57.000000 pybaseutils-1.0.6/test_py/demo_rename.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.6/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.6/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.6/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.6/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.6/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.6/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.6/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.083853 pybaseutils-1.0.6/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.6/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.6/test_py/detector/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.6/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.6/test_py/detector/predet_labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.086528 pybaseutils-1.0.6/test_py/edit_distance/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.6/test_py/edit_distance/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.6/test_py/edit_distance/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.6/test_py/edit_distance/text_matching.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.6/test_py/edit_distance/text_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.088574 pybaseutils-1.0.6/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.6/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.6/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.6/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.091594 pybaseutils-1.0.6/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.6/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.6/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.6/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.6/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.6/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.6/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.6/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.092930 pybaseutils-1.0.6/test_py/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.6/test_py/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.6/test_py/pose/human_pose.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:16:55.096584 pybaseutils-1.0.6/test_py/registry/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.6/test_py/registry/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.6/test_py/registry/base.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.6/test_py/registry/component.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.6/test_py/registry/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.6/test_py/registry/register.py
```

### Comparing `pybaseutils-1.0.5/LICENCE` & `pybaseutils-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/PKG-INFO` & `pybaseutils-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.5
+Version: 1.0.6
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
+Platform: UNKNOWN
 License-File: LICENCE
 
 base-utils
 ==========
 
 -  开源不易,麻烦给个【Star】
 -  源码 ： https://github.com/PanJinquan/base-utils
@@ -134,7 +135,9 @@
        DEBUG_TIME(t2);
        LOGI("rum time:%3.3fms", RUN_TIME(t2 - t1));
        cv::waitKey(0);
        DEBUG_IMSHOW("image", image);
        return 0;
    }
 
+
+
```

### Comparing `pybaseutils-1.0.5/README.md` & `pybaseutils-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/audio/audio_utils.py` & `pybaseutils-1.0.6/pybaseutils/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/audio/pyaudio_utils.py` & `pybaseutils-1.0.6/pybaseutils/audio/pyaudio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/audio/vad_utils.py` & `pybaseutils-1.0.6/pybaseutils/audio/vad_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/base64_utils.py` & `pybaseutils-1.0.6/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/batch_utils.py` & `pybaseutils-1.0.6/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/build_utils/cython_utils.py` & `pybaseutils-1.0.6/pybaseutils/build_utils/cython_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/build_utils/pyarmor_utils.py` & `pybaseutils-1.0.6/pybaseutils/build_utils/pyarmor_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/cluster/kmean.py` & `pybaseutils-1.0.6/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-1.0.6/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/cluster/similarity.py` & `pybaseutils-1.0.6/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/color_utils.py` & `pybaseutils-1.0.6/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/config_utils.py` & `pybaseutils-1.0.6/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/build_coco.py` & `pybaseutils-1.0.6/pybaseutils/converter/build_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/build_labelme.py` & `pybaseutils-1.0.6/pybaseutils/converter/build_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/build_voc.py` & `pybaseutils-1.0.6/pybaseutils/converter/build_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/concat_coco.py` & `pybaseutils-1.0.6/pybaseutils/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_coco2labelme.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_coco2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_coco2voc.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2coco.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2voc.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_labelme2yolo.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_labelme2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2coco.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_voc2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2labelme.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_voc2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2voc.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_voc2yolo.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/converter/convert_yolo2voc.py` & `pybaseutils-1.0.6/pybaseutils/converter/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/coords_utils.py` & `pybaseutils-1.0.6/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-1.0.6/pybaseutils/cvutils/corner_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,49 +36,56 @@
         corners = cv2.approxPolyDP(contour, epsilon, closed=True)
         corners = corners.reshape(-1, 2)
         k += 1
         if log: print(f"k={k},corners={len(corners)},epsilon={epsilon}")
     return corners
 
 
-def get_target_points(src_pts: np.ndarray):
+def get_target_points(src_pts: np.ndarray, diagonal=True):
     """
     根据输入的四个角点，计算其矫正后的目标四个角点,src_pts四个点分布：
         0--(w01)---1
         |          |
       (h03)      (h21)
         |          |
         3--(w23)---2
     :param src_pts:
+    :param diagonal: 是否使用对角线
     :return:
     """
     # 计算四个角点的边长
     w01 = np.sum(np.square(src_pts[0] - src_pts[1]), axis=0)
     h03 = np.sum(np.square(src_pts[0] - src_pts[3]), axis=0)
     h21 = np.sum(np.square(src_pts[2] - src_pts[1]), axis=0)
     w23 = np.sum(np.square(src_pts[2] - src_pts[3]), axis=0)
-    xmin, ymin = 0, 0
-    if h03 > w01:
-        xmax = np.sqrt(np.mean([w01, w23]))
-        ymax = np.sqrt(np.mean([h03, h21]))
-    else:
-        xmax = np.sqrt(np.mean([w01, w23]))
-        ymax = np.sqrt(np.mean([h03, h21]))
+    xmin, ymin, xmax, ymax = 0, 0, (w01 + w23) / 2, (h03 + h21) / 2
+    if diagonal:
+        if h03 > w01:
+            xmax = np.sqrt(np.mean([w01, w23]))
+            ymax = np.sqrt(np.mean([h03, h21]))
+        else:
+            xmax = np.sqrt(np.mean([w01, w23]))
+            ymax = np.sqrt(np.mean([h03, h21]))
     dst_pts = [[xmin, ymin], [xmax, ymin], [xmax, ymax], [xmin, ymax]]
     dst_pts = np.asarray(dst_pts)
     return dst_pts
 
 
 def get_order_points(pts_src):
     """
     对4个点按顺时针方向进行排序:[top-left, top-right, bottom-right, bottom-left]
     top-left    ：对应y+x之和的最小点
     bottom-right：对应y+x之和的最大点
     top-right   ：对应y-x之差的最小点
     bottom-left ：对应y-x之差的最大点
+         0(top-left)----(w10)----1(top-right)
+            |                       |
+          (h30)                    (h21)
+            |                       |
+        3(bottom-left)--(w23)---2(bottom-right)
     :param pts_src: pts_dst [top-left, top-right, bottom-right, bottom-left]
     :return:
     """
     pts_src = np.array(pts_src)
     pts_dst = np.zeros(shape=(4, 2), dtype=np.float32)
     s = pts_src.sum(axis=1)
     # Top-left point will have the smallest sum.
```

### Comparing `pybaseutils-1.0.5/pybaseutils/cvutils/monitor.py` & `pybaseutils-1.0.6/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-1.0.6/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/cvutils/video_utils.py` & `pybaseutils-1.0.6/pybaseutils/cvutils/video_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/base_coco.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/base_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/base_dataset.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/base_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_det.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/parser_coco_det.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_ins.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/parser_coco_ins.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/parser_coco_kps.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/parser_coco_kps.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/parser_labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,17 +408,18 @@
 
 
 if __name__ == "__main__":
     from pybaseutils.converter import build_labelme
 
     anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v1/json"
     anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v7/json"
-    anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-outdoor-det/dataset-test/json"
+    anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/使用钳形电流表测量低压线路电流/dataset-v1/json"
     # anno_dir = [anno_dir, anno_dir]
-    names = None
+    # names = None
+    names = ['A相电线','B相电线','C相电线','N相电线']
     dataset = LabelMeDatasets(filename=None,
                               data_root=None,
                               anno_dir=anno_dir,
                               image_dir=None,
                               class_name=names,
                               check=False,
                               phase="val",
```

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/parser_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/parser_yolo.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/parser_yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/dataloader/voc_seg_utils.py` & `pybaseutils-1.0.6/pybaseutils/dataloader/voc_seg_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/file_utils.py` & `pybaseutils-1.0.6/pybaseutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/filter/QueueTable.py` & `pybaseutils-1.0.6/pybaseutils/filter/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/filter/demo.py` & `pybaseutils-1.0.6/pybaseutils/filter/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/filter/kalman_filter.py` & `pybaseutils-1.0.6/pybaseutils/filter/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/filter/mean_filter.py` & `pybaseutils-1.0.6/pybaseutils/filter/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/filter/motion_filter.py` & `pybaseutils-1.0.6/pybaseutils/filter/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/filter/pose_filter.py` & `pybaseutils-1.0.6/pybaseutils/filter/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/font_style/__init__.py` & `pybaseutils-1.0.6/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/font_utils.py` & `pybaseutils-1.0.6/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/geometry_tools.py` & `pybaseutils-1.0.6/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/heatmap_utils.py` & `pybaseutils-1.0.6/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/image_utils.py` & `pybaseutils-1.0.6/pybaseutils/image_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/json_utils.py` & `pybaseutils-1.0.6/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/log.py` & `pybaseutils-1.0.6/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/logger.py` & `pybaseutils-1.0.6/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/metrics/accuracy.py` & `pybaseutils-1.0.6/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/metrics/average_meter.py` & `pybaseutils-1.0.6/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/metrics/class_report.py` & `pybaseutils-1.0.6/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/metrics/plot_pr.py` & `pybaseutils-1.0.6/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/metrics/plot_roc.py` & `pybaseutils-1.0.6/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/numpy_utils.py` & `pybaseutils-1.0.6/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/pandas_utils.py` & `pybaseutils-1.0.6/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/plot_utils.py` & `pybaseutils-1.0.6/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/pose/bones_utils.py` & `pybaseutils-1.0.6/pybaseutils/pose/bones_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/pose/human_pose.py` & `pybaseutils-1.0.6/pybaseutils/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/pose/pose_utils.py` & `pybaseutils-1.0.6/pybaseutils/pose/pose_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/pycpp/demo.py` & `pybaseutils-1.0.6/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/pycpp/main.py` & `pybaseutils-1.0.6/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/server/apm_server.py` & `pybaseutils-1.0.6/pybaseutils/server/apm_server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/setup_config.py` & `pybaseutils-1.0.6/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/singleton_utils.py` & `pybaseutils-1.0.6/pybaseutils/singleton_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/thread_utils.py` & `pybaseutils-1.0.6/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/time_utils.py` & `pybaseutils-1.0.6/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracemalloc_utils.py` & `pybaseutils-1.0.6/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-1.0.6/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracking/QueueTable.py` & `pybaseutils-1.0.6/pybaseutils/tracking/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracking/demo.py` & `pybaseutils-1.0.6/pybaseutils/tracking/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracking/kalman_filter.py` & `pybaseutils-1.0.6/pybaseutils/tracking/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracking/mean_filter.py` & `pybaseutils-1.0.6/pybaseutils/tracking/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracking/motion_filter.py` & `pybaseutils-1.0.6/pybaseutils/tracking/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/tracking/pose_filter.py` & `pybaseutils-1.0.6/pybaseutils/tracking/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/transforms/affine_transform.py` & `pybaseutils-1.0.6/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/transforms/face_alignment.py` & `pybaseutils-1.0.6/pybaseutils/transforms/face_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,19 +99,19 @@
     :param method: lstsq,estimate,affine,homo
     :return:  align_image 对齐后的图像
               M           S->D的变换矩阵(2×3)
               Minv        D->S的逆变换矩阵(2×3)
     """
     if extend:
         dst_pts, out_size = get_facial_points(out_size=out_size, extend=extend, square=True, vis=False)
-        align_face, M, Minv = image_alignment(image, src_pts, dst_pts, out_size, method="lstsq")
+        align_face, M, Minv = get_image_alignment(image, src_pts, dst_pts, out_size, method="lstsq")
     else:
         # 获得标准人脸关键点
         dst_pts = get_reference_facial_points(out_size=out_size, square=True, vis=False)
-        align_face, M, Minv = image_alignment(image, src_pts, dst_pts, out_size, method=method)
+        align_face, M, Minv = get_image_alignment(image, src_pts, dst_pts, out_size, method=method)
     return align_face, M, Minv
 
 
 if __name__ == "__main__":
     from pybaseutils import image_utils
 
     image_file = "test.jpg"
```

### Comparing `pybaseutils-1.0.5/pybaseutils/transforms/transform_utils.py` & `pybaseutils-1.0.6/pybaseutils/transforms/transform_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,58 +6,96 @@
     @Brief  :
 """
 import cv2
 import numpy as np
 from pybaseutils.cvutils import corner_utils
 
 
-def get_target_corner_points(src_pts: np.ndarray):
+def get_target_corner_points(src_pts: np.ndarray, diagonal=True):
     """
     根据输入的四个角点，计算其矫正后的目标四个角点,src_pts四个点分布：
         0--(w01)---1
         |          |
       (h03)      (h21)
         |          |
         3--(w23)---2
-    :param src_pts: 原始4个角点
-    :return: 目标4个角点
+    :param src_pts:
+    :param diagonal: 是否使用对角线
+    :return:
     """
-    return corner_utils.get_target_points(src_pts=src_pts)
+    return corner_utils.get_target_points(src_pts=src_pts, diagonal=diagonal)
 
 
-def image_alignment(image, src_pts, dst_pts, out_size=None, method="lstsq"):
+def get_image_alignment(image, src_pts, dst_pts, dsize=None, method="lstsq"):
     """
     apply affine transform实现对齐图像
     D=M*S or D=H*S
     :param image: input image
     :param src_pts: 原始点S集合(n×2)
     :param dst_pts: 目标点D集合(n×2)
-    :param out_size: 变换后输出图像大小
+    :param dsize: 变换后输出图像大小
     :param method: lstsq,estimate,affine,homo
     :return:  align_image 对齐后的图像
               M           S->D的变换矩阵(2×3)
               Minv        D->S的逆变换矩阵(2×3)
     """
-    if out_size is None:
+    if dsize is None:
         xmax = int(max(dst_pts[:, 0]))
         ymax = int(max(dst_pts[:, 1]))
-        out_size = (xmax, ymax)
+        dsize = (xmax, ymax)
     M = get_transform(src_pts, dst_pts, method=method)
     # 进行仿射变换
     if M.size == 6:  # 如果M是2×3的变换矩阵
-        align_image = cv2.warpAffine(image, M=M, dsize=tuple(out_size))
+        align_image = cv2.warpAffine(image, M=M, dsize=tuple(dsize))
         # Minv = get_transform(dst_pts, src_pts, method=method)
         Minv = get_inverse_matrix(M)
         # Minv = cv2.invertAffineTransform(M)
     else:  # 如果M是3×3的单应矩阵
-        align_image = cv2.warpPerspective(image, M, dsize=tuple(out_size))
+        align_image = cv2.warpPerspective(image, M, dsize=tuple(dsize))
         Minv = get_transform(dst_pts, src_pts, method=method)
     return align_image, M, Minv
 
 
+def image_alignment(image: np.ndarray, src_pts, dst_pts=None, dsize=(-1, -1), scale=(1.0, 1.0), method="lstsq"):
+    """
+    apply affine transform实现对齐图像
+    :param image:
+    :param src_pts:
+    :param dst_pts:
+    :param dsize:
+    :param scale:
+    :param method:
+    :return:
+    """
+    h, w = image.shape[:2]
+    if dst_pts is None:
+        dst_pts = get_target_corner_points(src_pts)
+        xmin = min(dst_pts[:, 0])
+        ymin = min(dst_pts[:, 1])
+        xmax = max(dst_pts[:, 0])
+        ymax = max(dst_pts[:, 1])
+        tsize = (xmax - xmin, ymax - ymin)
+    else:
+        tsize = (w, h)
+    if dsize[0] < 0 or dsize[1] < 0:
+        dsize = tsize
+    # 映射居中
+    tsize = np.array(tsize)
+    dsize = np.array(dsize)
+    dst_pts = np.array(dst_pts)
+    diff = dsize - tsize
+    dst_pts = dst_pts + diff / 2.
+    # 缩放大小
+    diff = dsize * scale - dsize
+    dsize = np.array(dsize * scale, dtype=np.int32)
+    dst_pts = dst_pts + diff / 2
+    dst, M, Minv = get_image_alignment(image, src_pts=src_pts, dst_pts=dst_pts, dsize=tuple(dsize), method=method)
+    return dst, dst_pts, M, Minv
+
+
 def solve_lstsq(src_pts: np.ndarray, dst_pts: np.ndarray):
     """
     通过最小二乘法计算变换矩阵
     np.linalg.lstsq() <==>  cv2.solve()
     :param src_pts:
     :param dst_pts:
     :return: M
@@ -134,7 +172,26 @@
     """
     Minv = np.zeros((3, 3))
     Minv[0:2, :] = M
     Minv[2, 2] = 1
     Minv = np.linalg.pinv(Minv)
     Minv = Minv[0:2, :]
     return Minv
+
+
+def test_transform(image_file):
+    from pybaseutils import image_utils
+    src = cv2.imread(image_file)
+    mask = image_utils.get_image_mask(src)
+    contours = image_utils.find_mask_contours(mask)
+    src_pts = image_utils.find_minAreaRect(contours, order=True)[0]
+    dst, dst_pts, M, Minv = image_alignment(src, src_pts, dsize=(400, 500), scale=(1.2, 1.2))
+    src = image_utils.draw_image_contours(src, contours)
+    src = image_utils.draw_landmark(src, [src_pts], color=(255, 0, 0), vis_id=True)
+    dst = image_utils.draw_landmark(dst, [dst_pts], color=(0, 255, 0), vis_id=True)
+    image_utils.cv_show_image("src", src, delay=10)
+    image_utils.cv_show_image("dst", dst, delay=0)
+
+
+if __name__ == '__main__':
+    image_file = "../../data/mask/mask5.jpg"
+    test_transform(image_file)
```

### Comparing `pybaseutils-1.0.5/pybaseutils/word_utils.py` & `pybaseutils-1.0.6/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/worker.py` & `pybaseutils-1.0.6/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils/yaml_utils.py` & `pybaseutils-1.0.6/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-1.0.6/pybaseutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.5
+Version: 1.0.6
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
+Platform: UNKNOWN
 License-File: LICENCE
 
 base-utils
 ==========
 
 -  开源不易,麻烦给个【Star】
 -  源码 ： https://github.com/PanJinquan/base-utils
@@ -134,7 +135,9 @@
        DEBUG_TIME(t2);
        LOGI("rum time:%3.3fms", RUN_TIME(t2 - t1));
        cv::waitKey(0);
        DEBUG_IMSHOW("image", image);
        return 0;
    }
 
+
+
```

### Comparing `pybaseutils-1.0.5/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-1.0.6/pybaseutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/setup.py` & `pybaseutils-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/WebCrawler/search_image.py` & `pybaseutils-1.0.6/test_py/WebCrawler/search_image.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/WebCrawler/search_image_for_baidu.py` & `pybaseutils-1.0.6/test_py/WebCrawler/search_image_for_baidu.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/convert_labelme2coco.py` & `pybaseutils-1.0.6/test_py/aije/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/convert_labelme2voc.py` & `pybaseutils-1.0.6/test_py/aije/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/copy_move.py` & `pybaseutils-1.0.6/test_py/aije/copy_move.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/demo_video_aije.py` & `pybaseutils-1.0.6/test_py/aije/demo_video_aije.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/demo_voc_crop.py` & `pybaseutils-1.0.6/test_py/aije/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/demo_voc_vis.py` & `pybaseutils-1.0.6/test_py/aije/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/aije/video_demo.py` & `pybaseutils-1.0.6/test_py/aije/video_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/audio/demo.py` & `pybaseutils-1.0.6/test_py/audio/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/audio/main.py` & `pybaseutils-1.0.6/test_py/audio/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/audio/main_read.py` & `pybaseutils-1.0.6/test_py/audio/main_read.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/audio/segment.py` & `pybaseutils-1.0.6/test_py/audio/segment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/audio/speechbrain_asr_indoor_prod.py` & `pybaseutils-1.0.6/test_py/audio/speechbrain_asr_indoor_prod.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/audio/speechbrain_demo.py` & `pybaseutils-1.0.6/test_py/audio/speechbrain_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/class_attribute.py` & `pybaseutils-1.0.6/test_py/class_attribute.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/class_names.py` & `pybaseutils-1.0.6/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/AffectNet.py` & `pybaseutils-1.0.6/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/AsianMovie.py` & `pybaseutils-1.0.6/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/BITVehicle2voc.py` & `pybaseutils-1.0.6/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/BSTLD2voc.py` & `pybaseutils-1.0.6/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/CCPD.py` & `pybaseutils-1.0.6/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/CCPD2voc.py` & `pybaseutils-1.0.6/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/FL3D_dataset.py` & `pybaseutils-1.0.6/test_py/converter/FL3D_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/MTFL2voc.py` & `pybaseutils-1.0.6/test_py/converter/MTFL2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/TT100K.py` & `pybaseutils-1.0.6/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/WaterMeters.py` & `pybaseutils-1.0.6/test_py/converter/WaterMeters.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         postfix = image_name.split(".")[-1]
         lable_name = image_name.replace(f".{postfix}", ".txt")
         image_file = os.path.join(image_dir, image_name)
         lable_file = os.path.join(label_dir, lable_name)
         image, point, label, boxes = load_annotation(image_file, lable_file)
         if use_align:
             dst_pts = transform_utils.get_target_corner_points(point)
-            crop, M, Minv = transform_utils.image_alignment(image, src_pts=point, dst_pts=dst_pts, out_size=None,
-                                                            method="lstsq")
+            crop, M, Minv = transform_utils.get_image_alignment(image, src_pts=point, dst_pts=dst_pts, dsize=None,
+                                                                method="lstsq")
             crop_file = os.path.join(out_root, "{}_{:0=5d}_alignment.jpg".format(label, i))
             cv2.imwrite(crop_file, crop)
         else:
             crop = image_utils.get_bbox_crop(image, bbox=boxes[0])
             crop_file = os.path.join(out_root, "{}_{:0=5d}_crop.jpg".format(label, i))
             h, w = crop.shape[:2]
             if w > 3 * h: cv2.imwrite(crop_file, crop)
```

### Comparing `pybaseutils-1.0.5/test_py/converter/concat_coco.py` & `pybaseutils-1.0.6/test_py/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/convert_coco2voc.py` & `pybaseutils-1.0.6/test_py/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/convert_gesture2hand.py` & `pybaseutils-1.0.6/test_py/converter/convert_gesture2hand.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/convert_labelme2coco.py` & `pybaseutils-1.0.6/test_py/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/convert_labelme2voc.py` & `pybaseutils-1.0.6/test_py/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/fatigue_driving.py` & `pybaseutils-1.0.6/test_py/converter/fatigue_driving.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/fdd_dataset.py` & `pybaseutils-1.0.6/test_py/converter/fdd_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/handpose2coco.py` & `pybaseutils-1.0.6/test_py/converter/handpose2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-1.0.6/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/tt100k_utils.py` & `pybaseutils-1.0.6/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/ua_detrac2voc.py` & `pybaseutils-1.0.6/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/converter/voc_sbd2labelme.py` & `pybaseutils-1.0.6/test_py/converter/voc_sbd2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/cython_build/build_cython.py` & `pybaseutils-1.0.6/test_py/cython_build/build_cython.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/cython_build/build_pyarmor.py` & `pybaseutils-1.0.6/test_py/cython_build/build_pyarmor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/cython_build/cryptography_demo.py` & `pybaseutils-1.0.6/test_py/cython_build/cryptography_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/cython_build/model_des_enctypt.py` & `pybaseutils-1.0.6/test_py/cython_build/model_des_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/cython_build/model_enctypt.py` & `pybaseutils-1.0.6/test_py/cython_build/model_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo1.py` & `pybaseutils-1.0.6/test_py/demo_pandas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,48 @@
 # -*-coding: utf-8 -*-
 """
-    @Author : PKing
-    @E-mail :
-    @Date   : 2024-02-05 18:19:18
+    @Author : Pan
+    @E-mail : 390737991@qq.com
+    @Date   : 2022-10-13 18:14:53
     @Brief  :
 """
 import os
-import cv2
 import numpy as np
-from tqdm import tqdm
-from pybaseutils import image_utils, file_utils
-from pybaseutils.transforms import transform_utils
+import cv2
+from pybaseutils import pandas_utils, image_utils, file_utils
 from pybaseutils.converter import build_voc
 
-
-def load_annotation(image_file, lable_file):
-    image = image_utils.read_image(image_file)
-    annos = file_utils.read_data(lable_file, split=" ", convertNum=False)
-    annos = annos[0]
-    point = [int(i) for i in annos[0:8]]
-    point = np.asarray(point).reshape(-1, 2)
-    label = annos[8]
-    boxes = image_utils.polygons2boxes([point])
-    return image, point, label, boxes
-
-
-def WaterMeters(image_dir, label_dir, out_root, use_align=False, vis=True):
-    if out_root: file_utils.create_dir(out_root)
-    file_list = file_utils.get_files_lists(image_dir, sub=True)
-    contents = []
-    for i, image_name in tqdm(enumerate(file_list)):
-        postfix = image_name.split(".")[-1]
-        lable_name = image_name.replace(f".{postfix}", ".txt")
+if __name__ == "__main__":
+    image_dir = "/home/dm/nasdata/dataset/csdn/helmet/Helmet_Dataset(kaggle)/helmet_dataset/JPEGImages"
+    out_xml_dir = "/home/dm/nasdata/dataset/csdn/helmet/Helmet_Dataset(kaggle)/helmet_dataset/Annotations"
+    file = "/home/dm/nasdata/dataset/csdn/helmet/Helmet_Dataset(kaggle)/helmet_dataset/train_labels.csv"
+    df = pandas_utils.read_csv(file)
+    content = pandas_utils.df2list(df)
+    class_name = {'head': 0, "helmet": 1}
+    vis = True
+    for item in content:
+        if not len(item) == 2:
+            continue
+        image_name, info = item
+        print(image_name, info)
+        info = info.lstrip().rstrip().split(" ")
+        image_name = image_name.lstrip().rstrip()
+        image_id, format = image_name.split(".")
+        image_id = "{:0=5d}".format(int(image_id))
+        image_name = "{}.{}".format(image_id, format)
+        info = np.asarray(info).reshape(-1, 5)
+        bboxes = np.asarray(info[:, 0:4], dtype=np.int32)
+        labels_ = info[:, 4:5].reshape(-1).tolist()
+        labels = []
+        for name in labels_:
+            name = "head" if name == "none" else "helmet"
+            labels.append(name)
         image_file = os.path.join(image_dir, image_name)
-        lable_file = os.path.join(label_dir, "gt_" + lable_name)
-        if os.path.exists(image_file) and os.path.exists(lable_file):
-            item = file_utils.get_sub_list([image_file, lable_file], out_root)
-            contents.append(item)
-        else:
-            print("not exists:{}".format(image_file))
-    filename = os.path.join(out_root, "lable.txt")
-    file_utils.write_data(filename, contents, split="\t")
-    # image, point, label, boxes = load_annotation(image_file, lable_file)
-    # if use_align:
-    #     dst_pts = transform_utils.get_target_points(point)
-    #     crop, M, Minv = transform_utils.image_alignment(image, src_pts=point, dst_pts=dst_pts, out_size=None,
-    #                                                     method="lstsq")
-    #     crop_file = os.path.join(out_root, "{}_{:0=5d}_alignment.jpg".format(label, i))
-    #     cv2.imwrite(crop_file, crop)
-    # else:
-    #     crop = image_utils.get_bbox_crop(image, bbox=boxes[0])
-    #     crop_file = os.path.join(out_root, "{}_{:0=5d}_crop.jpg".format(label, i))
-    #     h, w = crop.shape[:2]
-    #     if w > 3 * h: cv2.imwrite(crop_file, crop)
-    # if vis:
-    #     image = image_utils.draw_image_bboxes_text(image, boxes, boxes_name=[label])
-    #     image = image_utils.draw_key_point_in_image(image, [point], vis_id=True)
-    #     image_utils.cv_show_image("crop", crop, delay=10)
-    #     image_utils.cv_show_image("image", image)
-    return
-
-
-if __name__ == '__main__':
-    pass
+        image = cv2.imread(image_file)
+        image_shape = image.shape
+        xml_path = file_utils.create_dir(out_xml_dir, None, "{}.xml".format(image_id))
+        objects = build_voc.create_objects(bboxes, labels, keypoints=None, class_name=None)
+        build_voc.write_voc_xml_objects(image_name, image_shape, objects, xml_path)
+        if vis:
+            labels = [class_name[l] for l in labels]
+            image = image_utils.draw_image_bboxes_labels(image, bboxes, labels, thickness=2, fontScale=0.5)
+            image_utils.cv_show_image("image", image, use_rgb=False, delay=1)
```

### Comparing `pybaseutils-1.0.5/test_py/demo2.py` & `pybaseutils-1.0.6/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo3.py` & `pybaseutils-1.0.6/test_py/demo3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_async_await2.py` & `pybaseutils-1.0.6/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_coco_vis.py` & `pybaseutils-1.0.6/test_py/demo_coco_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_copy_files.py` & `pybaseutils-1.0.6/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_copy_files_for_voc.py` & `pybaseutils-1.0.6/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_ffmpy.py` & `pybaseutils-1.0.6/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_for_pair_file.py` & `pybaseutils-1.0.6/test_py/demo_for_pair_file.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_for_polygon.py` & `pybaseutils-1.0.6/test_py/demo_for_polygon.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_get_file_list.py` & `pybaseutils-1.0.6/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_gif.py` & `pybaseutils-1.0.6/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_gif_video.py` & `pybaseutils-1.0.6/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_image_crop.py` & `pybaseutils-1.0.6/test_py/demo_image_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_labelme.py` & `pybaseutils-1.0.6/test_py/demo_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_metrics.py` & `pybaseutils-1.0.6/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_mouse.py` & `pybaseutils-1.0.6/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_nii.py` & `pybaseutils-1.0.6/test_py/demo_nii.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_plot.py` & `pybaseutils-1.0.6/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_rename.py` & `pybaseutils-1.0.6/test_py/demo_rename.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,10 +20,10 @@
         name = "{}_{:0=4d}.{}".format(name, i, postfix)
         new = os.path.join(output, name)
         file_utils.copy_file(old, new)
 
 
 if __name__ == '__main__':
 
-    image_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/使用钳形电流表测量低压线路电流/天河数据/2024-04-12-1-2-train"
-    output = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/使用钳形电流表测量低压线路电流/天河数据/2024-04-12-1-2-train2"
-    rename_image_file(image_dir, output, prefix="南沙")
+    image_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/室内考题/天河视频/20240419_天河训练视频/室内考题-天河数据1"
+    output = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/室内考题/天河视频/20240419_天河训练视频/室内考题-天河数据1-train"
+    rename_image_file(image_dir, output, prefix="天河")
```

### Comparing `pybaseutils-1.0.5/test_py/demo_standard_image .py` & `pybaseutils-1.0.6/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_standard_video .py` & `pybaseutils-1.0.6/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_taichi.py` & `pybaseutils-1.0.6/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_video.py` & `pybaseutils-1.0.6/test_py/demo_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_voc_crop.py` & `pybaseutils-1.0.6/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_voc_vis.py` & `pybaseutils-1.0.6/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_word_similar.py` & `pybaseutils-1.0.6/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_worker1.py` & `pybaseutils-1.0.6/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/demo_worker2.py` & `pybaseutils-1.0.6/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/detector/demo.py` & `pybaseutils-1.0.6/test_py/detector/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/detector/detect_face_person.py` & `pybaseutils-1.0.6/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/detector/predet_labelme.py` & `pybaseutils-1.0.6/test_py/detector/predet_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/edit_distance/demo.py` & `pybaseutils-1.0.6/test_py/edit_distance/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/edit_distance/text_matching.py` & `pybaseutils-1.0.6/test_py/edit_distance/text_matching.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/edit_distance/text_utils.py` & `pybaseutils-1.0.6/test_py/edit_distance/text_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/flask_demo/server.py` & `pybaseutils-1.0.6/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-1.0.6/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-1.0.6/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-1.0.6/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/kafka_worker.py` & `pybaseutils-1.0.6/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/men_tracemalloc.py` & `pybaseutils-1.0.6/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/performance.py` & `pybaseutils-1.0.6/test_py/performance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/pose/human_pose.py` & `pybaseutils-1.0.6/test_py/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/registry/base.py` & `pybaseutils-1.0.6/test_py/registry/base.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/registry/component.py` & `pybaseutils-1.0.6/test_py/registry/component.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/registry/main.py` & `pybaseutils-1.0.6/test_py/registry/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.5/test_py/registry/register.py` & `pybaseutils-1.0.6/test_py/registry/register.py`

 * *Files identical despite different names*

