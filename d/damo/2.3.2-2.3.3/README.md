# Comparing `tmp/damo-2.3.2.tar.gz` & `tmp/damo-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.3.2.tar", last modified: Mon Apr 22 18:43:59 2024, max compression
+gzip compressed data, was "damo-2.3.3.tar", last modified: Mon Apr 29 19:56:34 2024, max compression
```

## Comparing `damo-2.3.2.tar` & `damo-2.3.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-22 18:43:59.558561 damo-2.3.2/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-22 18:43:59.558561 damo-2.3.2/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-22 18:43:56.000000 damo-2.3.2/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.2/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-22 18:43:59.558561 damo-2.3.2/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.3.2/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-22 18:43:59.546561 damo-2.3.2/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-22 18:43:59.558561 damo-2.3.2/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-22 18:43:56.000000 damo-2.3.2/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.3.2/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.3.2/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.3.2/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.3.2/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.3.2/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-04-18 21:22:30.000000 damo-2.3.2/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.3.2/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.3.2/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44958 2024-04-21 16:55:34.000000 damo-2.3.2/src/damo/_damo_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.3.2/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47012 2024-04-16 16:12:10.000000 damo-2.3.2/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    22289 2024-04-14 15:18:46.000000 damo-2.3.2/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.3.2/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.3.2/src/damo/_damon_sysfs.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-04-20 20:06:09.000000 damo-2.3.2/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-04-06 16:27:42.000000 damo-2.3.2/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-04-06 16:27:57.000000 damo-2.3.2/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.3.2/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.3.2/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-04-06 16:21:28.000000 damo-2.3.2/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.3.2/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.3.2/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-04-06 16:21:33.000000 damo-2.3.2/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.3.2/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5116 2024-04-14 16:27:26.000000 damo-2.3.2/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-04-06 16:21:42.000000 damo-2.3.2/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-04-06 16:21:46.000000 damo-2.3.2/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-04-14 17:07:12.000000 damo-2.3.2/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-04-21 16:55:34.000000 damo-2.3.2/src/damo/damo_report_footprint.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-04-06 16:21:52.000000 damo-2.3.2/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-04-06 16:21:55.000000 damo-2.3.2/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-04-06 16:21:59.000000 damo-2.3.2/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.3.2/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-04-06 16:22:07.000000 damo-2.3.2/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.3.2/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.3.2/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.3.2/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-04-14 15:16:45.000000 damo-2.3.2/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-04-06 16:22:11.000000 damo-2.3.2/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-22 18:43:51.000000 damo-2.3.2/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5998 2024-04-16 16:46:36.000000 damo-2.3.2/src/damo/damo_wss.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-22 18:43:59.558561 damo-2.3.2/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-22 18:43:59.000000 damo-2.3.2/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1277 2024-04-22 18:43:59.000000 damo-2.3.2/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-22 18:43:59.000000 damo-2.3.2/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-22 18:43:59.000000 damo-2.3.2/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-22 18:43:59.000000 damo-2.3.2/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.077430 damo-2.3.3/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-29 19:56:34.077430 damo-2.3.3/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-29 19:56:30.000000 damo-2.3.3/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.3/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-29 19:56:34.077430 damo-2.3.3/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.3.3/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.065430 damo-2.3.3/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.077430 damo-2.3.3/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:30.000000 damo-2.3.3/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.3.3/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.3.3/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.3.3/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.3.3/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.3.3/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-04-18 21:22:30.000000 damo-2.3.3/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.3.3/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.3.3/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44940 2024-04-27 18:41:30.000000 damo-2.3.3/src/damo/_damo_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.3.3/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-04-27 18:53:46.000000 damo-2.3.3/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    22388 2024-04-27 19:00:02.000000 damo-2.3.3/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.3.3/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.3.3/src/damo/_damon_sysfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      256 2024-04-27 18:18:15.000000 damo-2.3.3/src/damo/abc.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-04-20 20:06:09.000000 damo-2.3.3/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-04-06 16:27:42.000000 damo-2.3.3/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-04-06 16:27:57.000000 damo-2.3.3/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.3.3/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.3.3/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-04-06 16:21:28.000000 damo-2.3.3/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.3.3/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.3.3/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-04-06 16:21:33.000000 damo-2.3.3/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.3.3/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5330 2024-04-28 19:08:50.000000 damo-2.3.3/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-04-06 16:21:42.000000 damo-2.3.3/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-04-06 16:21:46.000000 damo-2.3.3/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-04-14 17:07:12.000000 damo-2.3.3/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-04-21 16:55:34.000000 damo-2.3.3/src/damo/damo_report_footprint.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-04-06 16:21:52.000000 damo-2.3.3/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-04-06 16:21:55.000000 damo-2.3.3/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-04-06 16:21:59.000000 damo-2.3.3/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.3.3/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-04-06 16:22:07.000000 damo-2.3.3/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.3.3/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.3.3/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.3.3/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-04-14 15:16:45.000000 damo-2.3.3/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-04-06 16:22:11.000000 damo-2.3.3/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-29 19:56:20.000000 damo-2.3.3/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-04-28 19:04:36.000000 damo-2.3.3/src/damo/damo_wss.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.077430 damo-2.3.3/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1293 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.3.2/PKG-INFO` & `damo-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.2
+Version: 2.3.3
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.2/README.md` & `damo-2.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,29 +75,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.2/setup.py` & `damo-2.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_ascii_color.py` & `damo-2.3.3/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_deprecated.py` & `damo-2.3.3/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_deprecation_notice.py` & `damo-2.3.3/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_dist.py` & `damo-2.3.3/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_fmt_str.py` & `damo-2.3.3/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_fs.py` & `damo-2.3.3/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_paddr_layout.py` & `damo-2.3.3/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_print.py` & `damo-2.3.3/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damo_records.py` & `damo-2.3.3/src/damo/_damo_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -667,18 +667,16 @@
 
 def all_targets_terminated(targets):
     for target in targets:
         if pid_running('%s' % target.pid):
             return False
     return True
 
-def __poll_target_pids(handle):
+def __poll_target_pids(kdamonds, add_childs):
     '''Return if polling should continued'''
-    kdamonds = handle.kdamonds
-    add_childs = handle.poll_add_child_tasks
 
     current_targets = kdamonds[0].contexts[0].targets
     if all_targets_terminated(current_targets):
         return False
     if not add_childs:
         return True
 
@@ -713,30 +711,27 @@
         err = _damon.commit(kdamonds)
         if err != None:
             # this might be not a problem; some of processes might
             # finished meanwhile
             return False
     return True
 
-def poll_target_pids(handle):
+def poll_target_pids(kdamonds, add_childs):
     has_pid_target = False
-    if handle.kdamonds:
-        for kdamond in handle.kdamonds:
+    if kdamonds:
+        for kdamond in kdamonds:
             for ctx in kdamond.contexts:
                 if _damon.target_has_pid(ctx.ops):
                     has_pid_target = True
                     break
             if has_pid_target:
                 break
     if has_pid_target is False:
         return False
-    rc = __poll_target_pids(handle)
-    if rc is True and handle.mem_footprint_snapshots is not None:
-        record_mem_footprint(handle.kdamonds, handle.mem_footprint_snapshots)
-    return rc
+    return __poll_target_pids(kdamonds, add_childs)
 
 # for recording
 
 class RecordingHandle:
     # for tracepoint recording
     tracepoint = None
     file_path = None
@@ -747,45 +742,48 @@
 
     # for CPU clock event recording
     do_profile = None
     perf_profile_pipe = None
 
     # for adding child tasks and memory footprint recording
     kdamonds = None
-    poll_add_child_tasks = None
+    add_child_tasks = None
     mem_footprint_snapshots = None
 
     def __init__(self, tracepoint, file_path, file_format, file_permission,
                  monitoring_intervals,
                  do_profile,
-                 kdamonds, poll_add_child_tasks, poll_add_mem_footprint):
+                 kdamonds, add_child_tasks, record_mem_footprint):
         self.tracepoint = tracepoint
         self.file_path = file_path
         self.file_format = file_format
         self.file_permission = file_permission
         self.monitoring_intervals = monitoring_intervals
 
         self.do_profile = do_profile
 
         self.kdamonds = kdamonds
-        self.poll_add_child_tasks = poll_add_child_tasks
-        if poll_add_mem_footprint is True:
+        self.add_child_tasks = add_child_tasks
+        if record_mem_footprint is True:
             self.mem_footprint_snapshots = []
 
 def start_recording(handle):
     if handle.tracepoint is not None:
         handle.perf_pipe = subprocess.Popen(
                 [PERF, 'record', '-a', '-e', handle.tracepoint,
                  '-o', handle.file_path])
     if handle.do_profile:
         cmd = [PERF, 'record', '-o', '%s.profile' % handle.file_path]
         handle.perf_profile_pipe = subprocess.Popen(cmd)
-    while poll_target_pids(handle):
+    while (poll_target_pids(handle.kdamonds, handle.add_child_tasks) or
+           _damon.any_kdamond_running()):
+        if handle.mem_footprint_snapshots is not None:
+            record_mem_footprint(handle.kdamonds,
+                                 handle.mem_footprint_snapshots)
         time.sleep(1)
-    _damon.wait_kdamonds_turned_off()
 
 def finish_recording(handle):
     try:
         handle.perf_pipe.send_signal(signal.SIGINT)
         handle.perf_pipe.wait()
     except:
         # perf might already finished
```

### Comparing `damo-2.3.2/src/damo/_damo_subcmds.py` & `damo-2.3.3/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damon.py` & `damo-2.3.3/src/damo/_damon.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,24 +404,30 @@
     def effectively_equal(self, other, intervals):
         return (
                 self.converted_for_units(
                     unit_samples, unit_aggr_intervals, intervals) ==
                 other.converted_for_units(
                     unit_samples, unit_aggr_intervals, intervals))
 
+qgoal_user_input = 'user_input'
+qgoal_some_mem_psi_us = 'some_mem_psi_us'
+qgoal_metrics = [qgoal_user_input, qgoal_some_mem_psi_us]
+
 class DamosQuotaGoal:
     metric = None
     target_value = None
     current_value = None
     quotas = None
 
-    def __init__(self, metric='user_input',
+    def __init__(self, metric=qgoal_user_input,
                  target_value='0', current_value='0'):
+        if not metric in qgoal_metrics:
+            raise Exception('unsupported DAMOS quota goal metric')
         self.metric = metric
-        if metric == 'some_mem_psi_us':
+        if metric == qgoal_some_mem_psi_us:
             self.target_value = _damo_fmt_str.text_to_us(target_value)
         else:
             self.target_value = _damo_fmt_str.text_to_nr(target_value)
         self.current_value = _damo_fmt_str.text_to_nr(current_value)
 
     def to_str(self, raw):
         return 'metric %s target %s current %s' % (
```

### Comparing `damo-2.3.2/src/damo/_damon_args.py` & `damo-2.3.3/src/damo/_damon_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,16 +525,19 @@
             help=' '.join([
             'damos quotas (<time (ms)> [<size (bytes)> [<reset interval (ms)>',
                 '[<size priority weight (permil)>',
                 '[<access rate priority weight> (permil)',
                 '[<age priority weight> (permil)]]]]])']))
     parser.add_argument('--damos_quota_goal', nargs='+', action='append',
             default=[],
-            metavar='<metric or target value or current value>',
-            help='damos quota goal (<metric> <target value> [current value])')
+            metavar='<metric or value>',
+            help=' '.join([
+                'damos quota goal (<metric> <target value> [current value]).',
+                '<metric> shoule be {%s}.' %
+                ','.join(_damon.qgoal_metrics)]))
     parser.add_argument('--damos_nr_quota_goals', type=int, nargs='+',
             default=[], metavar='<integer>',
             help='number of quota goals for each scheme (in order)')
     parser.add_argument('--damos_wmarks', nargs=5, action='append', default=[],
             metavar=('<metric (none|free_mem_rate)>', '<interval (us)>',
                 '<high mark (permil)>', '<mid mark (permil)>',
                 '<low mark (permil)>'),
```

### Comparing `damo-2.3.2/src/damo/_damon_dbgfs.py` & `damo-2.3.3/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/_damon_sysfs.py` & `damo-2.3.3/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo.py` & `damo-2.3.3/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_adjust.py` & `damo-2.3.3/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_convert_record_format.py` & `damo-2.3.3/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_features.py` & `damo-2.3.3/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_fmt_json.py` & `damo-2.3.3/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_heats.py` & `damo-2.3.3/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_lru_sort.py` & `damo-2.3.3/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_monitor.py` & `damo-2.3.3/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_nr_regions.py` & `damo-2.3.3/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_reclaim.py` & `damo-2.3.3/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_record.py` & `damo-2.3.3/src/damo/damo_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         if not _damon.any_kdamond_running():
             print('DAMON is not turned on')
             exit(1)
 
         # TODO: Support multiple kdamonds, multiple contexts
         monitoring_intervals = data_for_cleanup.orig_kdamonds[
                 0].contexts[0].intervals
-        kdamonds = None
+        kdamonds = data_for_cleanup.orig_kdamonds
 
     if args.schemes_target_regions == False:
         tracepoint = _damo_records.perf_event_damon_aggregated
     else:
         tracepoint = _damo_records.perf_event_damos_before_apply
 
     record_handle = _damo_records.RecordingHandle(
@@ -114,16 +114,16 @@
             tracepoint=tracepoint, file_path=args.out,
             file_format=args.output_type,
             file_permission=args.output_permission,
             monitoring_intervals=monitoring_intervals,
             # for perf profile
             do_profile=args.profile is True,
             # for childs recording and memory footprint
-            kdamonds=kdamonds, poll_add_child_tasks=args.include_child_tasks,
-            poll_add_mem_footprint=args.footprint)
+            kdamonds=kdamonds, add_child_tasks=args.include_child_tasks,
+            record_mem_footprint=args.footprint)
     data_for_cleanup.record_handle = record_handle
 
     print('Press Ctrl+C to stop')
     _damo_records.start_recording(record_handle)
     cleanup_exit(0)
 
 def set_argparser(parser):
@@ -132,14 +132,17 @@
                         choices=_damo_records.file_types,
                         default=_damo_records.file_type_json_compressed,
                         help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
                         help='permission of the output file')
     parser.add_argument('--perf_path', type=str, default='perf',
                         help='path of perf tool ')
+    parser.add_argument('--exclude_child_tasks', action='store_false',
+                        dest='include_child_tasks',
+                        help='do not record access of child processes')
     parser.add_argument('--include_child_tasks', action='store_true',
                         help='record accesses of child processes')
     parser.add_argument('--schemes_target_regions', action='store_true',
                         help='record schemes tried to be applied regions')
     parser.add_argument('--profile', action='store_true',
                         help='record profiling information together')
     parser.add_argument('--footprint', action='store_true',
```

### Comparing `damo-2.3.2/src/damo/damo_record_info.py` & `damo-2.3.3/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_replay.py` & `damo-2.3.3/src/damo/damo_replay.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_report.py` & `damo-2.3.3/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_report_footprint.py` & `damo-2.3.3/src/damo/damo_report_footprint.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_report_profile.py` & `damo-2.3.3/src/damo/damo_report_profile.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_report_raw.py` & `damo-2.3.3/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_report_times.py` & `damo-2.3.3/src/damo/damo_report_times.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_schemes.py` & `damo-2.3.3/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_show.py` & `damo-2.3.3/src/damo/damo_show.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_start.py` & `damo-2.3.3/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_status.py` & `damo-2.3.3/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_stop.py` & `damo-2.3.3/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_tune.py` & `damo-2.3.3/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_validate.py` & `damo-2.3.3/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.2/src/damo/damo_wss.py` & `damo-2.3.3/src/damo/damo_wss.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,17 @@
     parser.add_argument('--nr_cols_bar', type=int, metavar='<num>',
             default=59,
             help='number of columns that is reserved for wss visualization')
     parser.add_argument('--raw_number', action='store_true',
             help='use machine-friendly raw numbers')
     parser.add_argument('--all_wss', action='store_true',
             help='Do not print percentile but all calculated wss')
+    parser.add_argument('--per_target', action='store_false',
+                        dest='collapse_targets',
+                        help='Report workingset size per monitoring target')
     parser.add_argument('--collapse_targets', action='store_true',
                         help='Collapse targets in the record into one')
     parser.description = 'Show distribution of working set size'
 
 def main(args):
     file_path = args.input
     percentiles = range(args.range[0], args.range[1], args.range[2])
```

### Comparing `damo-2.3.2/src/damo.egg-info/PKG-INFO` & `damo-2.3.3/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.2
+Version: 2.3.3
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.2/src/damo.egg-info/SOURCES.txt` & `damo-2.3.3/src/damo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/damo/_damo_print.py
 src/damo/_damo_records.py
 src/damo/_damo_subcmds.py
 src/damo/_damon.py
 src/damo/_damon_args.py
 src/damo/_damon_dbgfs.py
 src/damo/_damon_sysfs.py
+src/damo/abc.py
 src/damo/damo.py
 src/damo/damo_adjust.py
 src/damo/damo_convert_record_format.py
 src/damo/damo_features.py
 src/damo/damo_fmt_json.py
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
```

