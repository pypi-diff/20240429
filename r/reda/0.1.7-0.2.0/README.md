# Comparing `tmp/reda-0.1.7.tar.gz` & `tmp/reda-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reda-0.1.7.tar", last modified: Tue Feb 27 11:15:52 2024, max compression
+gzip compressed data, was "reda-0.2.0.tar", last modified: Mon Apr 29 07:15:57 2024, max compression
```

## Comparing `reda-0.1.7.tar` & `reda-0.2.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1158 2017-11-13 07:45:48.000000 reda-0.1.7/COPYING
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3194 2024-02-27 11:15:52.000000 reda-0.1.7/PKG-INFO
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2690 2024-02-27 11:15:26.000000 reda-0.1.7/README.md
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1257 2024-02-27 10:05:25.000000 reda-0.1.7/lib/reda/__init__.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/configs/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2018-02-20 09:09:06.000000 reda-0.1.7/lib/reda/configs/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    40312 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/configs/configManager.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/containers/
--rw-r--r--   0 mweigand   (545) geophysik   (128)    25259 2024-02-27 09:17:55.000000 reda-0.1.7/lib/reda/containers/BaseContainer.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     5486 2021-03-29 07:38:44.000000 reda-0.1.7/lib/reda/containers/CR.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    12616 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/containers/ERT.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     6376 2020-08-21 06:23:46.000000 reda-0.1.7/lib/reda/containers/SIP.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    14167 2021-03-29 07:38:44.000000 reda-0.1.7/lib/reda/containers/TDIP.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)       52 2018-08-22 11:56:13.000000 reda-0.1.7/lib/reda/containers/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    32821 2024-02-27 09:19:53.000000 reda-0.1.7/lib/reda/containers/sEIT.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/eis/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2018-08-04 17:12:28.000000 reda-0.1.7/lib/reda/eis/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     8082 2018-08-22 11:56:13.000000 reda-0.1.7/lib/reda/eis/convert.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    20165 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/eis/plots.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     5991 2020-03-20 15:50:00.000000 reda-0.1.7/lib/reda/eis/test_convert.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2516 2020-03-20 15:50:00.000000 reda-0.1.7/lib/reda/eis/units.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/exporters/
--rw-r--r--   0 mweigand   (545) geophysik   (128)       60 2018-08-22 11:56:13.000000 reda-0.1.7/lib/reda/exporters/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2833 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/exporters/bert.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3289 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/exporters/crtomo.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1628 2017-11-13 07:45:48.000000 reda-0.1.7/lib/reda/exporters/syscal.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     9902 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/exporters/tsert_export.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/importers/
--rw-r--r--   0 mweigand   (545) geophysik   (128)       52 2018-08-22 11:56:13.000000 reda-0.1.7/lib/reda/importers/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3799 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/bert.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3968 2024-02-27 09:20:29.000000 reda-0.1.7/lib/reda/importers/crtomo.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    23701 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/eit_fzj.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     6156 2020-03-20 15:50:00.000000 reda-0.1.7/lib/reda/importers/eit_version_2010.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     7377 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/eit_version_2013.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    15536 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/eit_version_2017.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    15395 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/eit_version_2018a.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    15172 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/importers/eit_version_20200609.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    24609 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/fzj_readbin.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2471 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/importers/geotom.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    20378 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/importers/iris_syscal_pro.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/importers/legacy/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2018-11-22 07:49:12.000000 reda-0.1.7/lib/reda/importers/legacy/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    14001 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/importers/legacy/eit160.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    11796 2019-11-29 11:55:34.000000 reda-0.1.7/lib/reda/importers/legacy/eit40.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    17057 2020-03-27 19:24:55.000000 reda-0.1.7/lib/reda/importers/mpt_das1.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    13951 2020-03-27 19:24:55.000000 reda-0.1.7/lib/reda/importers/radic_sip256c.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     4389 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/importers/res2dinv.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    14753 2020-09-29 14:18:54.000000 reda-0.1.7/lib/reda/importers/sip04.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     8265 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/importers/tsert_import.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/importers/utils/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2018-12-03 10:26:36.000000 reda-0.1.7/lib/reda/importers/utils/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1153 2018-12-03 10:26:36.000000 reda-0.1.7/lib/reda/importers/utils/decorators.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1301 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/importers/utils/transforms.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/main/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2017-11-13 07:45:48.000000 reda-0.1.7/lib/reda/main/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2703 2020-08-21 06:23:46.000000 reda-0.1.7/lib/reda/main/logger.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2279 2019-10-17 06:50:57.000000 reda-0.1.7/lib/reda/main/units.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/plotters/
--rw-r--r--   0 mweigand   (545) geophysik   (128)      161 2018-08-22 11:56:13.000000 reda-0.1.7/lib/reda/plotters/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    11515 2024-02-21 15:20:33.000000 reda-0.1.7/lib/reda/plotters/histograms.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    15302 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/plotters/plots2d.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    18329 2024-02-21 15:12:46.000000 reda-0.1.7/lib/reda/plotters/pseudoplots.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     4197 2024-02-19 13:09:55.000000 reda-0.1.7/lib/reda/plotters/pseudoplots_type_3_crtomo.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2643 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/plotters/time_series.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/tdip/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2020-03-27 19:24:55.000000 reda-0.1.7/lib/reda/tdip/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)      190 2020-03-27 19:24:55.000000 reda-0.1.7/lib/reda/tdip/decay_curve.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/testing/
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2211 2024-02-21 14:12:26.000000 reda-0.1.7/lib/reda/testing/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1636 2024-02-21 14:55:51.000000 reda-0.1.7/lib/reda/testing/containers.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/testing/data/
--rw-r--r--   0 mweigand   (545) geophysik   (128)   866312 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/testing/data/seit_test_data.zip
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/testing/ert_container/
--rw-r--r--   0 mweigand   (545) geophysik   (128)        0 2019-12-02 10:07:41.000000 reda-0.1.7/lib/reda/testing/ert_container/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2066 2019-12-02 10:30:34.000000 reda-0.1.7/lib/reda/testing/ert_container/test_K_computation.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2832 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/testing/fzj_readbin.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1707 2021-11-16 15:07:58.000000 reda-0.1.7/lib/reda/testing/test_container_ert.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2955 2024-02-27 11:09:28.000000 reda-0.1.7/lib/reda/testing/test_container_seit.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2135 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/testing/test_crtomo_import.py
--rwxr-xr-x   0 mweigand   (545) geophysik   (128)    20897 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/testing/test_electrode_manager.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda/utils/
--rw-r--r--   0 mweigand   (545) geophysik   (128)      148 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/utils/__init__.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1760 2018-08-04 17:12:28.000000 reda-0.1.7/lib/reda/utils/data.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2396 2024-02-21 15:25:06.000000 reda-0.1.7/lib/reda/utils/decorators_and_managers.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    19556 2024-01-23 10:25:28.000000 reda-0.1.7/lib/reda/utils/eit_fzj_utils.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    24882 2024-01-23 10:16:15.000000 reda-0.1.7/lib/reda/utils/electrode_manager.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)      784 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/utils/enter_directory.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     7124 2018-08-22 11:56:13.000000 reda-0.1.7/lib/reda/utils/filter_config_types.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     4012 2019-12-02 10:16:00.000000 reda-0.1.7/lib/reda/utils/fix_sign_with_K.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     6671 2024-01-23 10:16:21.000000 reda-0.1.7/lib/reda/utils/geom_fac_crtomo.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3647 2024-01-23 10:16:21.000000 reda-0.1.7/lib/reda/utils/geometric_factors.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3032 2019-06-06 19:41:13.000000 reda-0.1.7/lib/reda/utils/helper_functions.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)     4368 2024-02-19 13:21:44.000000 reda-0.1.7/lib/reda/utils/mpl.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)    16915 2024-02-27 09:01:41.000000 reda-0.1.7/lib/reda/utils/norrec.py
--rw-r--r--   0 mweigand   (545) geophysik   (128)      875 2019-11-29 11:54:43.000000 reda-0.1.7/lib/reda/utils/pseudo_positions.py
-drwxr-xr-x   0 mweigand   (545) geophysik   (128)        0 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda.egg-info/
--rw-r--r--   0 mweigand   (545) geophysik   (128)     3194 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda.egg-info/PKG-INFO
--rw-r--r--   0 mweigand   (545) geophysik   (128)     2725 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda.egg-info/SOURCES.txt
--rw-r--r--   0 mweigand   (545) geophysik   (128)        1 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda.egg-info/dependency_links.txt
--rw-r--r--   0 mweigand   (545) geophysik   (128)       65 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda.egg-info/requires.txt
--rw-r--r--   0 mweigand   (545) geophysik   (128)        5 2024-02-27 11:15:52.000000 reda-0.1.7/lib/reda.egg-info/top_level.txt
--rw-r--r--   0 mweigand   (545) geophysik   (128)       38 2024-02-27 11:15:52.000000 reda-0.1.7/setup.cfg
--rw-r--r--   0 mweigand   (545) geophysik   (128)     1381 2024-02-27 11:14:55.000000 reda-0.1.7/setup.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.434293 reda-0.2.0/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1158 2019-11-07 13:45:16.000000 reda-0.2.0/COPYING
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3179 2024-04-29 07:15:57.430293 reda-0.2.0/PKG-INFO
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2690 2024-04-29 07:10:59.000000 reda-0.2.0/README.md
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.406293 reda-0.2.0/lib/
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.406293 reda-0.2.0/lib/reda/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1257 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/__init__.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.410293 reda-0.2.0/lib/reda/configs/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/configs/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    41606 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/configs/configManager.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.410293 reda-0.2.0/lib/reda/containers/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    25523 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/containers/BaseContainer.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5486 2021-06-12 11:40:09.000000 reda-0.2.0/lib/reda/containers/CR.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    12616 2022-04-08 07:55:36.000000 reda-0.2.0/lib/reda/containers/ERT.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     6376 2020-08-20 17:40:33.000000 reda-0.2.0/lib/reda/containers/SIP.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    14167 2021-06-12 11:40:09.000000 reda-0.2.0/lib/reda/containers/TDIP.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       52 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/containers/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    32821 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/containers/sEIT.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.414293 reda-0.2.0/lib/reda/eis/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/eis/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8082 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/eis/convert.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    20165 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/eis/plots.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5991 2020-03-20 07:47:33.000000 reda-0.2.0/lib/reda/eis/test_convert.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2516 2020-03-20 07:47:33.000000 reda-0.2.0/lib/reda/eis/units.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.414293 reda-0.2.0/lib/reda/exporters/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       60 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/exporters/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2838 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/exporters/bert.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3289 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/exporters/crtomo.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1628 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/exporters/syscal.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    10345 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/exporters/tsert_export.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.418293 reda-0.2.0/lib/reda/importers/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       52 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/importers/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3799 2021-06-12 11:40:09.000000 reda-0.2.0/lib/reda/importers/bert.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3990 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/importers/crtomo.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    23701 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/importers/eit_fzj.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     6156 2020-03-20 07:47:33.000000 reda-0.2.0/lib/reda/importers/eit_version_2010.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     7377 2021-06-12 11:40:09.000000 reda-0.2.0/lib/reda/importers/eit_version_2013.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    15536 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/importers/eit_version_2017.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    15395 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/importers/eit_version_2018a.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    15194 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/importers/eit_version_20200609.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    24609 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/importers/fzj_readbin.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2471 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/importers/geotom.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    20764 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/importers/iris_syscal_pro.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.418293 reda-0.2.0/lib/reda/importers/legacy/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/importers/legacy/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    14001 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/importers/legacy/eit160.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    11796 2019-12-02 07:59:13.000000 reda-0.2.0/lib/reda/importers/legacy/eit40.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    17105 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/importers/mpt_das1.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    13951 2020-03-23 09:52:50.000000 reda-0.2.0/lib/reda/importers/radic_sip256c.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4389 2022-04-08 07:55:36.000000 reda-0.2.0/lib/reda/importers/res2dinv.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    14753 2020-10-30 08:52:47.000000 reda-0.2.0/lib/reda/importers/sip04.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8131 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/importers/tsert_import.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.418293 reda-0.2.0/lib/reda/importers/utils/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/importers/utils/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1153 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/importers/utils/decorators.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1301 2021-06-12 11:40:09.000000 reda-0.2.0/lib/reda/importers/utils/transforms.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.418293 reda-0.2.0/lib/reda/main/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/main/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2703 2020-08-20 17:18:58.000000 reda-0.2.0/lib/reda/main/logger.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2279 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/main/units.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.422293 reda-0.2.0/lib/reda/plotters/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      161 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/plotters/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    11515 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/plotters/histograms.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    15302 2022-04-08 07:55:36.000000 reda-0.2.0/lib/reda/plotters/plots2d.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18329 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/plotters/pseudoplots.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4197 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/plotters/pseudoplots_type_3_crtomo.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2643 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/plotters/time_series.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.422293 reda-0.2.0/lib/reda/tdip/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2020-04-13 07:34:05.000000 reda-0.2.0/lib/reda/tdip/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      190 2020-04-13 07:34:05.000000 reda-0.2.0/lib/reda/tdip/decay_curve.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.422293 reda-0.2.0/lib/reda/testing/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2211 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/testing/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1636 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/testing/containers.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.422293 reda-0.2.0/lib/reda/testing/data/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)   866312 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/testing/data/seit_test_data.zip
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.426293 reda-0.2.0/lib/reda/testing/ert_container/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2019-12-02 08:51:23.000000 reda-0.2.0/lib/reda/testing/ert_container/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2066 2020-01-10 10:52:12.000000 reda-0.2.0/lib/reda/testing/ert_container/test_K_computation.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2832 2021-11-16 14:47:56.000000 reda-0.2.0/lib/reda/testing/fzj_readbin.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1707 2021-06-12 11:40:09.000000 reda-0.2.0/lib/reda/testing/test_container_ert.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2995 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/testing/test_container_seit.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2135 2022-04-08 07:55:36.000000 reda-0.2.0/lib/reda/testing/test_crtomo_import.py
+-rwxr-xr-x   0 mweigand  (1001) mweigand  (1001)    20897 2022-04-08 07:55:36.000000 reda-0.2.0/lib/reda/testing/test_electrode_manager.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.430293 reda-0.2.0/lib/reda/utils/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      148 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/utils/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1760 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/utils/data.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      517 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/datetimes.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2396 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/decorators_and_managers.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    19556 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/eit_fzj_utils.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    24882 2022-04-08 07:55:36.000000 reda-0.2.0/lib/reda/utils/electrode_manager.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      784 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/utils/enter_directory.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     7124 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/utils/filter_config_types.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4012 2020-01-10 10:52:12.000000 reda-0.2.0/lib/reda/utils/fix_sign_with_K.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     6671 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/geom_fac_crtomo.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3647 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/geometric_factors.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3032 2019-11-07 13:45:16.000000 reda-0.2.0/lib/reda/utils/helper_functions.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4368 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/mpl.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    16915 2024-04-29 07:10:59.000000 reda-0.2.0/lib/reda/utils/norrec.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      875 2019-12-02 07:59:13.000000 reda-0.2.0/lib/reda/utils/pseudo_positions.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:15:57.410293 reda-0.2.0/lib/reda.egg-info/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3179 2024-04-29 07:15:57.000000 reda-0.2.0/lib/reda.egg-info/PKG-INFO
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2753 2024-04-29 07:15:57.000000 reda-0.2.0/lib/reda.egg-info/SOURCES.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        1 2024-04-29 07:15:57.000000 reda-0.2.0/lib/reda.egg-info/dependency_links.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       65 2024-04-29 07:15:57.000000 reda-0.2.0/lib/reda.egg-info/requires.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        5 2024-04-29 07:15:57.000000 reda-0.2.0/lib/reda.egg-info/top_level.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       38 2024-04-29 07:15:57.434293 reda-0.2.0/setup.cfg
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1366 2024-04-29 07:10:59.000000 reda-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `reda-0.1.7/COPYING` & `reda-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/PKG-INFO` & `reda-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: reda
-Version: 0.1.7
+Version: 0.2.0
 Summary: Reproducible Electrical Data Analysis
 Home-page: https://github.com/geophysics-ubonn/reda
-Author: Maximilian Weigand and Florian M. Wagner
-Author-email: mweigand@geo.uni-bonn.de, wagner@geo.uni-bonn.de
+Author: Maximilian Weigand, Florian M. Wagner, and others
+Author-email: mweigand@geo.uni-bonn.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: crtomo
 License-File: COPYING
```

### Comparing `reda-0.1.7/README.md` & `reda-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/__init__.py` & `reda-0.2.0/lib/reda/__init__.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/configs/configManager.py` & `reda-0.2.0/lib/reda/configs/configManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # *-* coding: utf-8 *-*
 """Manage measurement configurations measurements.
 """
 import itertools
+import io
 
 import numpy as np
 import pandas as pd
 
 import reda.utils.mpl
 from reda.utils import opt_import
 
@@ -149,28 +150,37 @@
         return(injections)
 
     def load_crmod_config(self, filename):
         """Load a CRMod configuration file
 
         Parameters
         ----------
-        filename: string
-            absolute or relative path to a crmod config.dat file
+        filename: string|io.BytesIO
+            absolute or relative path to a crmod config.dat file. Can also be a
+            BytesIO object
 
         """
-        with open(filename, 'r') as fid:
-            nr_of_configs = int(fid.readline().strip())
-            configs = np.loadtxt(fid)
-            print('loaded configs:', configs.shape)
-            if nr_of_configs != configs.shape[0]:
-                raise Exception(
-                    'indicated number of measurements does not equal ' +
-                    'to actual number of measurements')
-            ABMN = self._crmod_to_abmn(configs[:, 0:2])
-            self.configs = ABMN
+        if isinstance(filename, io.BytesIO):
+            fid = filename
+        else:
+            fid = open(filename, 'r')
+
+        nr_of_configs = int(fid.readline().strip())
+        configs = np.loadtxt(fid)
+
+        if not isinstance(filename, io.BytesIO):
+            fid.close()
+
+        print('loaded configs:', configs.shape)
+        if nr_of_configs != configs.shape[0]:
+            raise Exception(
+                'indicated number of measurements does not equal ' +
+                'to actual number of measurements')
+        ABMN = self._crmod_to_abmn(configs[:, 0:2])
+        self.configs = ABMN
 
     def load_crmod_or_4c_configs(self, filename):
         """Load configurations either from a CRMod measurement file, or from a
         four-column file. Assume 1-indexed data (start with electrode 1).
 
         Parameters
         ----------
@@ -235,17 +245,19 @@
         )).T.astype(int)
         return ABMN
 
     def write_crmod_volt(self, filename, mid):
         """Write the measurements to the output file in the volt.dat file
         format that can be read by CRTomo.
 
+        Data is written in utf-8 encoding.
+
         Parameters
         ----------
-        filename: string
+        filename: string|io.BytesIO
             output filename
         mid: int or [int, int]
             measurement ids of magnitude and phase measurements. If only one ID
             is given, then the phase column is filled with zeros
 
         """
         ABMN = self._get_crmod_abmn()
@@ -253,30 +265,59 @@
         if isinstance(mid, (list, tuple)):
             mag_data = self.measurements[mid[0]]
             pha_data = self.measurements[mid[1]]
         else:
             mag_data = self.measurements[mid]
             pha_data = np.zeros(mag_data.shape)
 
-        all_data = np.hstack((ABMN, mag_data[:, np.newaxis],
-                              pha_data[:, np.newaxis]))
+        all_data = np.hstack(
+            (ABMN, mag_data[:, np.newaxis], pha_data[:, np.newaxis])
+        )
 
-        with open(filename, 'wb') as fid:
-            fid.write(bytes(
+        if isinstance(filename, io.BytesIO):
+            fid = filename
+        else:
+            fid = open(filename, 'wb')
+
+        fid.write(
+            bytes(
                 '{0}\n'.format(ABMN.shape[0]),
                 'utf-8',
-            ))
-            np.savetxt(fid, all_data, fmt='%i %i %f %f')
+            )
+        )
+        np.savetxt(fid, all_data, fmt='%i %i %f %f')
+        if not isinstance(filename, io.BytesIO):
+            fid.close()
+
 
     def write_crmod_volt_with_individual_errors(
             self, filename, data_mids, error_mids, norm_mag=1, norm_pha=1,
             ):
-        """
+        """Write the measurements and individual errors to the output file in
+        the volt.dat file format that can be read by CRTomo.
+
+        Data is written in utf-8 encoding.
+
+        Parameters
+        ----------
+        filename: string|io.BytesIO
+            output filename
+        data_mids: [int, int]
+            measurement ids of magnitude and phase measurements
+        error_mids: [int, int]
+            ids of magnitude and phase error estimates
+        norm_mag: float
+            Normalization factor for magnitude errors
+        norm_pha: float
+            Normalization factor for magnitude errors
 
         """
+        assert len(data_mids) == 2, "data_mids must be length 2"
+        assert len(error_mids) == 2, "error_mids must be length 2"
+
         ABMN = self._get_crmod_abmn()
 
         if isinstance(data_mids, (list, tuple)):
             mag_data = self.measurements[data_mids[0]]
             pha_data = self.measurements[data_mids[1]]
             mag_error = self.measurements[error_mids[0]]
             pha_error = self.measurements[error_mids[1]]
@@ -292,26 +333,33 @@
                 mag_data[:, np.newaxis],
                 pha_data[:, np.newaxis],
                 mag_error[:, np.newaxis],
                 pha_error[:, np.newaxis],
             )
         )
 
-        with open(filename, 'wb') as fid:
-            fid.write(bytes(
+        if isinstance(filename, io.BytesIO):
+            fid = filename
+        else:
+            fid = open(filename, 'wb')
+        fid.write(
+            bytes(
                 '{0} T\n'.format(ABMN.shape[0]),
                 'utf-8',
-            ))
-            np.savetxt(fid, all_data, fmt='%i %i %f %f %f %f')
-            fid.write(
-                bytes(
-                    '{} {}\n'.format(norm_mag, norm_pha),
-                    'utf-8',
-                )
             )
+        )
+        np.savetxt(fid, all_data, fmt='%i %i %f %f %f %f')
+        fid.write(
+            bytes(
+                '{} {}\n'.format(norm_mag, norm_pha),
+                'utf-8',
+            )
+        )
+        if not isinstance(filename, io.BytesIO):
+            fid.close()
 
     def write_crmod_config(self, filename):
         """Write the configurations to a configuration file in the CRMod format
         All configurations are merged into one previor to writing to file
 
         Parameters
         ----------
```

### Comparing `reda-0.1.7/lib/reda/containers/BaseContainer.py` & `reda-0.2.0/lib/reda/containers/BaseContainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import reda.plotters.pseudoplots as PS
 import reda.utils.fix_sign_with_K as redafixK
 import reda.utils.geometric_factors as redaK
 from reda.utils import has_multiple_timesteps
 from reda.utils.norrec import assign_norrec_diffs
 from reda.utils.norrec import assign_norrec_to_df
 from reda.utils.geometric_factors import apply_K
+from reda.utils.datetimes import ensure_dateteim64_is_in_ns
+
 
 from reda.utils.decorators_and_managers import LogDataChanges
 
 logger = logging.getLogger(__name__)
 
 
 class ImportersBase(object):
@@ -102,14 +104,16 @@
         ----------
         data : pandas.DataFrame
             Measurement data in the form of a DataFrame, must adhere to the
             container constraints (i.e., must have all required columns)
         no_norrec : bool (False)
             If True, then do not compute norrec ids and diffs
         """
+
+        ensure_dateteim64_is_in_ns(data)
         if self.data is None:
             self.data = data
         else:
             # we have existing data
             if 'timestep' in self.data.columns and 'timestep' in data.columns:
                 # we must check that the types of the new data and the old data
                 # timesteps match (we allow arbitrary types of timestep keys)
@@ -189,15 +193,14 @@
         self._add_to_data(data)
 
     def merge_container(self, container):
         """Merge the data and electrode positions from another container into
         this one.
         """
         logger.debug('Merging containers')
-        print(type(self))
 
         self._add_to_container(
             container.data,
             container.electrode_positions, container.topography)
 
     def get_norrec_pairs(self, test_column='rdiff'):
         """Return a dataframe that contains only valid normal-reciprocal pairs
@@ -497,14 +500,18 @@
     def histogram(self, column='r', filename=None, log10=False, **kwargs):
         """Plot a histogram of one data column"""
         return_dict = HS.plot_histograms(self.data, column)
         if filename is not None:
             return_dict['all'].savefig(filename, dpi=300)
         return return_dict
 
+    def plot_histogram(self, column='r', filename=None, log10=False, **kwargs):
+        """Wrapper for self.histogram"""
+        return self.histogram(column, filename, log10, **kwargs)
+
     def has_multiple_timesteps(self):
         """Return True if container has multiple timesteps."""
         return has_multiple_timesteps(self.data)
 
     def delete_measurements(self, row_or_rows):
         """Delete one or more measurements by index of the DataFrame.
```

### Comparing `reda-0.1.7/lib/reda/containers/CR.py` & `reda-0.2.0/lib/reda/containers/CR.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/containers/ERT.py` & `reda-0.2.0/lib/reda/containers/ERT.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/containers/SIP.py` & `reda-0.2.0/lib/reda/containers/SIP.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/containers/TDIP.py` & `reda-0.2.0/lib/reda/containers/TDIP.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/containers/sEIT.py` & `reda-0.2.0/lib/reda/containers/sEIT.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/eis/convert.py` & `reda-0.2.0/lib/reda/eis/convert.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/eis/plots.py` & `reda-0.2.0/lib/reda/eis/plots.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/eis/test_convert.py` & `reda-0.2.0/lib/reda/eis/test_convert.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/eis/units.py` & `reda-0.2.0/lib/reda/eis/units.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/exporters/bert.py` & `reda-0.2.0/lib/reda/exporters/bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     electrodes.columns = electrodes.columns.str.lower()
     data.columns = data.columns.str.lower()
 
     # Remove unnecessary columns and rename according to bert conventions
     # https://gitlab.com/resistivity-net/bert#the-unified-data-format
     cols_to_export = ["a", "b", "m", "n", "u", "i", "r", "rho_a", "error"]
-    data.drop(data.columns.difference(cols_to_export), 1, inplace=True)
+    data.drop(data.columns.difference(cols_to_export), axis=1, inplace=True)
     data.rename(columns={"rho_a": "rhoa", "error": "err"}, inplace=True)
 
     for key in electrodes.keys():
         f.write("%s " % key)
     f.write("\n")
     for row in electrodes.itertuples(index=False):
         for val in row:
```

### Comparing `reda-0.1.7/lib/reda/exporters/crtomo.py` & `reda-0.2.0/lib/reda/exporters/crtomo.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/exporters/syscal.py` & `reda-0.2.0/lib/reda/exporters/syscal.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/exporters/tsert_export.py` & `reda-0.2.0/lib/reda/exporters/tsert_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import logging
 import warnings
 import datetime
 
 import pandas as pd
+from pandas.api.types import is_datetime64_any_dtype
 import h5py
 
 
 class tsert_base(object):
     """Functionality related to the tsert file format used for both import and
     export
     """
@@ -107,23 +108,33 @@
     """
     def __init__(self, filename):
         super().__init__(filename)
         if not os.path.isfile(filename):
             self.add_file_information()
 
     def write_index(self, data_index):
+        print('write_index')
+        # import IPython
+        # IPython.embed()
         key = '/INDEX/index'
         self._open_file('a')
         if key in self.fid:
             del self.fid[key]
 
         self._close_file()
-        data_index.to_hdf(
+
+        data_index_final = data_index.copy()
+        if is_datetime64_any_dtype(data_index['value']):
+            data_index_final['value'] = data_index_final.astype(
+                'datetime64[ns]'
+            )
+
+        data_index_final.to_hdf(
             self.filename,
-            key,
+            key=key,
             append=True,
         )
 
     def get_empty_index(self):
         """Initialize an empty index"""
         index = pd.DataFrame(columns=['value', ])
         # index.index.name = 'index'
@@ -219,22 +230,20 @@
                 if len(data_index.index) == 0:
                     ts_key = 0
                 else:
                     ts_key = data_index.index.max() + 1
             elif len(row) > 1:
                 raise Exception('We only allow unique values in the index')
 
-            print('ts_key:', ts_key)
 
             key = '/'.join((
                 'ERT_DATA',
                 '{}'.format(ts_key),
                 version,
             ))
-            print('key', key)
             self._open_file('a')
             if key in self.fid:
                 # delete data before adding it
                 del self.fid[key]
             self._close_file()
 
             with warnings.catch_warnings():
@@ -250,14 +259,17 @@
             # update index
             data_index.loc[ts_key] = timestep
             if data_index.shape[
                     0] == 1 and data_index['value'].dtype == object:
                 data_index['value'] = data_index['value'].astype(
                     type(timestep))
 
+            print(data_index['value'])
+            print('---------------------------------')
+
             # write to file
             self.write_index(data_index)
 
     def set_electrode_positions(self, electrode_positions):
         """Write electrode positions into the file. Existing positions will be
         deleted.
 
@@ -281,15 +293,17 @@
         if key in f:
             del f[key]
         f.close()
         # make sure the file is closed
         self._close_file()
         # write to file
         electrode_positions.to_hdf(
-            self.filename, key, append=True,
+            self.filename,
+            key=key,
+            append=True,
             # complevel=9,
             # complib='lzo',
         )
 
     def set_topography(self, topography):
         """Write topography into the file. Existing positions will be
         deleted.
@@ -314,11 +328,13 @@
         if key in f:
             del f[key]
         f.close()
         # make sure the file is closed
         self._close_file()
         # write to file
         topography.to_hdf(
-            self.filename, key, append=True,
+            self.filename,
+            key=key,
+            append=True,
             # complevel=9,
             # complib='lzo',
         )
```

### Comparing `reda-0.1.7/lib/reda/importers/bert.py` & `reda-0.2.0/lib/reda/importers/bert.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/crtomo.py` & `reda-0.2.0/lib/reda/importers/crtomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         df = cexp.load_mod_file('volt_01_0.1Hz.crt')
         ert = reda.ERT(data=df)
 
     """
     df_raw = pd.read_csv(
         filename,
         skiprows=1,
-        delim_whitespace=True,
+        # delim_whitespace=True,
+        sep=r'\s+',
         names=['ab', 'mn', 'r', 'rpha']
     )
     df_raw['Zt'] = df_raw['r'] * np.exp(1j * df_raw['rpha'] / 1000.0)
     # ok, this is tricky: the preceding line, computing Zt, always makes sure
     # that the resulting complex number is located in the upper right quadrant
     # of the complex plane, thereby implicitly correcting for any negative
     # K-factor. We do not want this to ensure data integrity (i.e., electrode
```

### Comparing `reda-0.1.7/lib/reda/importers/eit_fzj.py` & `reda-0.2.0/lib/reda/importers/eit_fzj.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/eit_version_2010.py` & `reda-0.2.0/lib/reda/importers/eit_version_2010.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/eit_version_2013.py` & `reda-0.2.0/lib/reda/importers/eit_version_2013.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/eit_version_2017.py` & `reda-0.2.0/lib/reda/importers/eit_version_2017.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/eit_version_2018a.py` & `reda-0.2.0/lib/reda/importers/eit_version_2018a.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/eit_version_20200609.py` & `reda-0.2.0/lib/reda/importers/eit_version_20200609.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         )
         df = pd.DataFrame()
         # I THINK we can just sort a, b - the actual data should already
         # conform to the notation that the lower electrode number is assigned
         # to a
         df[['a', 'b']] = pd.DataFrame(
             np.sort(np.atleast_2d(fdata['cni']), axis=1))
-        df['datetime'] = timestamp
+        df['datetime'] = timestamp.astype(np.datetime64)
         df['frequency'] = fdata['fm']
         df['U0'] = fdata['U0']
         df['Zg1_ela'] = _to_3d(fdata['Zg3'])[:, 0, 0]
         df['Zg2_ela'] = _to_3d(fdata['Zg3'])[:, 0, 1]
         df['Zg3_ela'] = _to_3d(fdata['Zg3'])[:, 0, 2]
         df['Zg1_elb'] = _to_3d(fdata['Zg3'])[:, 1, 0]
         df['Zg2_elb'] = _to_3d(fdata['Zg3'])[:, 1, 1]
```

### Comparing `reda-0.1.7/lib/reda/importers/fzj_readbin.py` & `reda-0.2.0/lib/reda/importers/fzj_readbin.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/geotom.py` & `reda-0.2.0/lib/reda/importers/geotom.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/iris_syscal_pro.py` & `reda-0.2.0/lib/reda/importers/iris_syscal_pro.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # *-* coding: utf-8 *-*
 """Read binary data from the IRIS Instruments Syscal Pro system
 
 """
 import struct
 from io import StringIO
+import io
 import logging
 
 import pandas as pd
 import numpy as np
 
 import reda
 from reda.importers.utils.decorators import enable_result_transforms
@@ -25,15 +26,15 @@
     Parameters
     ----------
     filename: str
         Input filename
     assume_regular_electrodes_x : None|tuple(nr_electrodes, spacing)
         If not None, then assume measurements were taken using a profile of
         regular electrodes in x directions. Fill in any electrodes not used in
-        the data to align the logical electrode numbers wit the physical
+        the data to align the logical electrode numbers with the physical
         electrode numbers. Use the electrode spacing set in the system (usually
         a default of 1 m is used), and then change this to the real spacing
         using the 'elecs_transform_reg_spacing_x' parameter.
     elecs_transform_reg_spacing_x : tuple(old, new)|None, optional
         If not None, then assume a regular electrode spacing in x direction
         with spacing 'old'. This is often 1 m, a default of the systems.
         However, in reality often other spacings are used, and this parameter
@@ -75,15 +76,16 @@
 
     buffer = StringIO(text)
 
     # read data file
     data_raw = pd.read_csv(
         buffer,
         # sep='\t',
-        delim_whitespace=True,
+        sep=r'\s+',
+        # delim_whitespace=True,
     )
 
     # clean up column names
     data_raw.columns = [x.strip() for x in data_raw.columns.tolist()]
 
     # convert coordinates to logical electrode numbers
     elec_mgr = reda.electrode_manager()
@@ -156,16 +158,16 @@
     information from a given .bin file.
 
     Note that the .bin files contain electrodes positions for the electrodes.
     Electrode numbers are then inferred from those.
 
     Parameters
     ----------
-    filename : string
-        path to input filename
+    filename : string|io.BytesIO
+        path to input filename or io.BytesIO object containing the binary data
     assume_regular_electrodes_x : None|tuple(nr_electrodes, spacing)
         If not None, then assume measurements were taken using a profile of
         regular electrodes in x directions. Fill in any electrodes not used in
         the data to align the logical electrode numbers wit the physical
         electrode numbers. Use the electrode spacing set in the system (usually
         a default of 1 m is used), and then change this to the real spacing
         using the 'elecs_transform_reg_spacing_x' parameter.
@@ -324,26 +326,29 @@
 
 
 def _import_bin(filename):
     """Read a .bin file generated by the IRIS Instruments Syscal Pro System
 
     Parameters
     ----------
-    filename : string
+    filename : string|io.BytesIO
         Path to input filename
 
     Returns
     -------
     metadata : dict
         General information on the measurement
     df : :py:class:`pandas.DataFrame`
         dataframe containing all measurement data
 
     """
-    fid = open(filename, 'rb')
+    if isinstance(filename, io.BytesIO):
+        fid = filename
+    else:
+        fid = open(filename, 'rb')
 
     def fget(fid, fmt, tsize):
         buffer = fid.read(tsize)
         result_raw = struct.unpack(fmt, buffer)
         if len(result_raw) == 1:
             return result_raw[0]
         else:
@@ -377,15 +382,15 @@
         'syscal_type': syscal_type,
         'comment': comment,
     }
 
     measurements = []
     # for each measurement
     counter = 0
-    while(fid.tell() < total_size):
+    while (fid.tell() < total_size):
         dataentry = {}
 
         # print('COUNTER', counter)
         buffer = fid.read(2)
         array_type = struct.unpack('h', buffer)
         array_type
         # print(array_type)
@@ -529,12 +534,20 @@
                 # print('b', b)
                 b
 
         measurements.append(dataentry)
 
         counter += 1
 
+    # only close the fid if we read from a file - leave BytesIO open for
+    # further use
+    if not isinstance(filename, io.BytesIO):
+        fid.seek(0)
+    else:
+        # rewind
+        fid.close()
+
     # create a dataframe with all primary data
     df = pd.DataFrame(
         measurements
     ).reset_index()
     return metadata, df
```

### Comparing `reda-0.1.7/lib/reda/importers/legacy/eit160.py` & `reda-0.2.0/lib/reda/importers/legacy/eit160.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/legacy/eit40.py` & `reda-0.2.0/lib/reda/importers/legacy/eit40.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/mpt_das1.py` & `reda-0.2.0/lib/reda/importers/mpt_das1.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         # comment='!',
         # index_col=0,
         skiprows=tm_start - 1,
         nrows=tm_end - tm_start - 1
     )
 
     ngates = len(header)
-    ipw = np.array(header.iloc[:, 0]).astype(np.float)
+    ipw = np.array(header.iloc[:, 0]).astype(np.float64)
 
     data_new = pd.DataFrame()
 
     # def split_A(strA):
     #     return int(strA.split(',')[1])
 
     # data.iloc[:, 0].apply(split_A)
@@ -218,29 +218,29 @@
 
     # use helper DataFrames for Mx, Tm, dMx
     data_m = pd.DataFrame(
         columns=['M' + str(num) for num in range(1, ngates + 1)],
         index=data_new.index
     )
     data_m.loc[:, 'M1':'M' + str(ngates)] = np.array(
-        data.iloc[:, 8:8 + 2 * ngates:2]).astype(np.float)  # Mi
+        data.iloc[:, 8:8 + 2 * ngates:2]).astype(np.float64)  # Mi
 
     data_tm = pd.DataFrame(
         columns=['Tm' + str(num) for num in range(1, ngates + 1)],
         index=data_new.index
     )
     data_tm.loc[:, 'Tm1':'Tm' + str(ngates)] = ipw
 
     data_devm = pd.DataFrame(
         columns=['devm' + str(num) for num in range(1, ngates + 1)],
         index=data_new.index
     )
     data_devm.loc[:, 'devm1':'devm' + str(ngates)] = np.array(
         data.iloc[:, 9:9 + 2 * ngates:2]
-    ).astype(np.float)  # devMi
+    ).astype(np.float64)  # devMi
 
     # compute the global chargeability
     nominator = np.sum(
         np.array(data_m.loc[:, 'M1': 'M' + str(ngates)]) *
         np.array(data_tm.loc[:, 'Tm1': 'Tm' + str(ngates)]),
         axis=1
     )
@@ -249,21 +249,21 @@
         axis=1
     )
     data_new['chargeability'] = nominator / denominator
 
     datetime_series = pd.to_datetime(
         data.iloc[:, 10 + 2 * ngates],
         format='%Y%m%d_%H%M%S',
-        errors='ignore'
+        # errors='ignore'
     )
 
-    data_new['datetime'] = [
-        time for index, time in datetime_series.iteritems()]
+    data_new['datetime'] = datetime_series.sort_index().values
 
     data_new['decayCurve'] = 0
+    data_new['decayCurve'] = data_new['decayCurve'].astype(object)
     # construct a sub DataFrame for decay curve properties
     for index, meas in data_m.iterrows():
         decaycurve = pd.DataFrame(
             index=range(len(ipw)), columns=['Mx', 'T[ms]', 'dMx']
         )
         decaycurve['Mx'] = meas.values
         # use the gate ending as plotting point
```

### Comparing `reda-0.1.7/lib/reda/importers/radic_sip256c.py` & `reda-0.2.0/lib/reda/importers/radic_sip256c.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/res2dinv.py` & `reda-0.2.0/lib/reda/importers/res2dinv.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/sip04.py` & `reda-0.2.0/lib/reda/importers/sip04.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/tsert_import.py` & `reda-0.2.0/lib/reda/importers/tsert_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,47 +121,43 @@
             return
 
         # import IPython
         # IPython.embed()
         index_is_datetime = False
         if pd.api.types.is_datetime64_any_dtype(data_index["value"].dtype):
             index_is_datetime = True
-        print('DTYPES', data_index.dtypes)
 
         # all keys
         ts_keys = data_index.index.values
         reversed_data_index = data_index.reset_index().set_index(
             'value').sort_index()
 
         if timesteps == 'all':
             if not_before is not None or not_after is not None:
-                print('TRUNCATING')
                 if not index_is_datetime:
                     raise Exception('before/after requires datetime indices')
                 ts_keys = reversed_data_index.truncate(
                     before=not_before,
                     after=not_after,
                 )['index']
-                print('TS_KEYS filtered', ts_keys)
+                print('TS_KEYS after filtering:', ts_keys)
         else:
             assert timesteps in data_index['value'].values
             ts_keys = [
                 data_index.reset_index().set_index('value').loc[timesteps],
             ]
 
         print('loading version:', version)
 
         data_list = {}
         for ts_key in ts_keys:
             key = 'ERT_DATA/{}/{}'.format(ts_key, version)
-            print(key)
             # TODO check if key exists
             data = pd.read_hdf(self.filename, key)
             timestep = data_index.loc[ts_key, 'value']
-            print('timestep', timestep)
             data_list[timestep] = data
         return data_list
 
     def load_topography(self):
         self._open_file()
         key = '/TOPOGRAPHY/topography'
         if key in self.fid:
```

### Comparing `reda-0.1.7/lib/reda/importers/utils/decorators.py` & `reda-0.2.0/lib/reda/importers/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/importers/utils/transforms.py` & `reda-0.2.0/lib/reda/importers/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/main/logger.py` & `reda-0.2.0/lib/reda/main/logger.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/main/units.py` & `reda-0.2.0/lib/reda/main/units.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/plotters/histograms.py` & `reda-0.2.0/lib/reda/plotters/histograms.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/plotters/plots2d.py` & `reda-0.2.0/lib/reda/plotters/plots2d.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/plotters/pseudoplots.py` & `reda-0.2.0/lib/reda/plotters/pseudoplots.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/plotters/pseudoplots_type_3_crtomo.py` & `reda-0.2.0/lib/reda/plotters/pseudoplots_type_3_crtomo.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/plotters/time_series.py` & `reda-0.2.0/lib/reda/plotters/time_series.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/__init__.py` & `reda-0.2.0/lib/reda/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/containers.py` & `reda-0.2.0/lib/reda/testing/containers.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/data/seit_test_data.zip` & `reda-0.2.0/lib/reda/testing/data/seit_test_data.zip`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/ert_container/test_K_computation.py` & `reda-0.2.0/lib/reda/testing/ert_container/test_K_computation.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/fzj_readbin.py` & `reda-0.2.0/lib/reda/testing/fzj_readbin.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/test_container_ert.py` & `reda-0.2.0/lib/reda/testing/test_container_ert.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/test_container_seit.py` & `reda-0.2.0/lib/reda/testing/test_container_seit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import tempfile
 import zipfile
-from importlib_resources import files
+# from importlib_resources import files
+from importlib.resources import files
 
 import reda
 
 import matplotlib.pylab as plt
 
 
 def prepare_4d_data():
```

### Comparing `reda-0.1.7/lib/reda/testing/test_crtomo_import.py` & `reda-0.2.0/lib/reda/testing/test_crtomo_import.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/testing/test_electrode_manager.py` & `reda-0.2.0/lib/reda/testing/test_electrode_manager.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/data.py` & `reda-0.2.0/lib/reda/utils/data.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/decorators_and_managers.py` & `reda-0.2.0/lib/reda/utils/decorators_and_managers.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/eit_fzj_utils.py` & `reda-0.2.0/lib/reda/utils/eit_fzj_utils.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/electrode_manager.py` & `reda-0.2.0/lib/reda/utils/electrode_manager.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/enter_directory.py` & `reda-0.2.0/lib/reda/utils/enter_directory.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/filter_config_types.py` & `reda-0.2.0/lib/reda/utils/filter_config_types.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/fix_sign_with_K.py` & `reda-0.2.0/lib/reda/utils/fix_sign_with_K.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/geom_fac_crtomo.py` & `reda-0.2.0/lib/reda/utils/geom_fac_crtomo.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/geometric_factors.py` & `reda-0.2.0/lib/reda/utils/geometric_factors.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/helper_functions.py` & `reda-0.2.0/lib/reda/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/mpl.py` & `reda-0.2.0/lib/reda/utils/mpl.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/norrec.py` & `reda-0.2.0/lib/reda/utils/norrec.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda/utils/pseudo_positions.py` & `reda-0.2.0/lib/reda/utils/pseudo_positions.py`

 * *Files identical despite different names*

### Comparing `reda-0.1.7/lib/reda.egg-info/PKG-INFO` & `reda-0.2.0/lib/reda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: reda
-Version: 0.1.7
+Version: 0.2.0
 Summary: Reproducible Electrical Data Analysis
 Home-page: https://github.com/geophysics-ubonn/reda
-Author: Maximilian Weigand and Florian M. Wagner
-Author-email: mweigand@geo.uni-bonn.de, wagner@geo.uni-bonn.de
+Author: Maximilian Weigand, Florian M. Wagner, and others
+Author-email: mweigand@geo.uni-bonn.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: crtomo
 License-File: COPYING
```

### Comparing `reda-0.1.7/lib/reda.egg-info/SOURCES.txt` & `reda-0.2.0/lib/reda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 lib/reda/testing/test_crtomo_import.py
 lib/reda/testing/test_electrode_manager.py
 lib/reda/testing/data/seit_test_data.zip
 lib/reda/testing/ert_container/__init__.py
 lib/reda/testing/ert_container/test_K_computation.py
 lib/reda/utils/__init__.py
 lib/reda/utils/data.py
+lib/reda/utils/datetimes.py
 lib/reda/utils/decorators_and_managers.py
 lib/reda/utils/eit_fzj_utils.py
 lib/reda/utils/electrode_manager.py
 lib/reda/utils/enter_directory.py
 lib/reda/utils/filter_config_types.py
 lib/reda/utils/fix_sign_with_K.py
 lib/reda/utils/geom_fac_crtomo.py
```

### Comparing `reda-0.1.7/setup.py` & `reda-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 from setuptools import setup, find_packages
 
 # under windows, run
 # python.exe setup.py bdist --format msi
 # to create a windows installer
 
-version_long = '0.1.7'
+version_long = '0.2.0'
 
 # package data
 os.chdir('lib/reda/testing')
 package_data = glob.glob('data/*')
 os.chdir('../../../')
 
 
 if __name__ == '__main__':
     setup(
         name='reda',
         version=version_long,
         description='Reproducible Electrical Data Analysis',
         long_description=open('README.md', 'r').read(),
         long_description_content_type="text/markdown",
-        author='Maximilian Weigand and Florian M. Wagner',
-        author_email='mweigand@geo.uni-bonn.de, wagner@geo.uni-bonn.de',
+        author='Maximilian Weigand, Florian M. Wagner, and others',
+        author_email='mweigand@geo.uni-bonn.de',
         license='MIT',
         url='https://github.com/geophysics-ubonn/reda',
         packages=find_packages("lib"),
         package_dir={'': 'lib'},
         package_data={'reda.testing': package_data},
         install_requires=[
             'numpy',
```

