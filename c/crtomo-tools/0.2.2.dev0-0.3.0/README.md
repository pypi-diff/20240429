# Comparing `tmp/crtomo_tools-0.2.2.dev0.tar.gz` & `tmp/crtomo_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crtomo_tools-0.2.2.dev0.tar", last modified: Wed Jun 29 07:10:56 2022, max compression
+gzip compressed data, was "crtomo_tools-0.3.0.tar", last modified: Mon Apr 29 07:22:37 2024, max compression
```

## Comparing `crtomo_tools-0.2.2.dev0.tar` & `crtomo_tools-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,101 @@
-drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2022-06-29 07:10:56.933461 crtomo_tools-0.2.2.dev0/
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      270 2022-06-29 07:10:56.933461 crtomo_tools-0.2.2.dev0/PKG-INFO
-drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2022-06-29 07:10:56.917461 crtomo_tools-0.2.2.dev0/lib/
-drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2022-06-29 07:10:56.921461 crtomo_tools-0.2.2.dev0/lib/crtomo/
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      486 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/__init__.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3270 2020-01-03 18:17:55.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/analytical_solution.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2888 2021-01-22 08:59:59.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/binaries.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    10172 2021-07-29 07:22:58.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/cfg.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    13098 2021-07-29 07:22:58.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/configManager.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1432 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/debug.py
-drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2022-06-29 07:10:56.921461 crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      103 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/elec_20elecs.dat
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      220 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/elec_40elecs.dat
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)   103654 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/elem_20elecs.dat
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)   391409 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/elem_40elecs.dat
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    33013 2021-12-11 13:56:32.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/eitManager.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    44092 2021-12-11 13:56:28.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/grid.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    10274 2021-06-18 06:09:43.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/interface.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3979 2021-12-11 13:56:28.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/mpl.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3488 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/mpl_setup.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2894 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/nodeManager.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    23280 2022-04-27 07:01:54.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/parManager.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18707 2022-04-19 16:58:00.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/plotManager.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4766 2019-11-07 13:44:53.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/status.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    86065 2022-04-19 16:58:00.000000 crtomo_tools-0.2.2.dev0/lib/crtomo/tdManager.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)       38 2022-06-29 07:10:56.933461 crtomo_tools-0.2.2.dev0/setup.cfg
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1817 2020-11-19 10:52:17.000000 crtomo_tools-0.2.2.dev0/setup.py
-drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2022-06-29 07:10:56.933461 crtomo_tools-0.2.2.dev0/src/
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3743 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/cr_get_analytical_solutions.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5502 2021-06-18 06:09:43.000000 crtomo_tools-0.2.2.dev0/src/cr_get_modelling_errors.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    19258 2021-12-11 13:56:28.000000 crtomo_tools-0.2.2.dev0/src/cr_trig_create.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    15808 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/cr_trig_parse_gmsh.py
-drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2022-06-29 07:10:56.933461 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      270 2022-06-29 07:10:56.000000 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/PKG-INFO
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1404 2022-06-29 07:10:56.000000 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/SOURCES.txt
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)        1 2022-06-29 07:10:56.000000 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/dependency_links.txt
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1084 2022-06-29 07:10:56.000000 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/entry_points.txt
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)       70 2022-06-29 07:10:56.000000 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/requires.txt
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      452 2022-06-29 07:10:56.000000 crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/top_level.txt
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    14306 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_extralines_gen_decouplings.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1158 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_gen_decouplings.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5224 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_gen_depth_decoupling.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2012 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_gen_surface_files.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8771 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_homogenize.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)      670 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_plot_elem_angles.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5532 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_plot_wireframe.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2176 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_rotate.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2123 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_translate.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3726 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/grid_translate_model.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    14957 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/sd_plot.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    13522 2022-04-14 08:18:08.000000 crtomo_tools-0.2.2.dev0/src/sens_center_plot.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1791 2021-06-19 08:38:19.000000 crtomo_tools-0.2.2.dev0/src/td_clean.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8232 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/td_correct_temperature.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1910 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/td_init.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)    39078 2022-05-11 11:14:41.000000 crtomo_tools-0.2.2.dev0/src/td_plot.py
--rwxr-xr-x   0 mweigand  (1001) mweigand  (1001)     4773 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/td_residuals.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     7827 2020-11-19 10:52:17.000000 crtomo_tools-0.2.2.dev0/src/td_run_all_local.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2855 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/td_test.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3531 2019-11-07 13:44:55.000000 crtomo_tools-0.2.2.dev0/src/volt_correct_temperature.py
--rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4421 2021-12-03 07:04:26.000000 crtomo_tools-0.2.2.dev0/src/volt_histogram.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.885306 crtomo_tools-0.3.0/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       48 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/AUTHORS
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1063 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/LICENSE
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      270 2024-04-29 07:22:37.885306 crtomo_tools-0.3.0/PKG-INFO
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.833306 crtomo_tools-0.3.0/lib/
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.841306 crtomo_tools-0.3.0/lib/crtomo/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      533 2023-07-14 11:25:06.000000 crtomo_tools-0.3.0/lib/crtomo/__init__.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3270 2020-01-03 18:17:55.000000 crtomo_tools-0.3.0/lib/crtomo/analytical_solution.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2888 2021-01-22 08:59:59.000000 crtomo_tools-0.3.0/lib/crtomo/binaries.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    10964 2024-04-18 11:25:59.000000 crtomo_tools-0.3.0/lib/crtomo/cfg.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    13100 2024-04-18 11:26:02.000000 crtomo_tools-0.3.0/lib/crtomo/configManager.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1432 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/debug.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.845306 crtomo_tools-0.3.0/lib/crtomo/debug_data/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      103 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/debug_data/elec_20elecs.dat
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      220 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/debug_data/elec_40elecs.dat
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)   103654 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/debug_data/elem_20elecs.dat
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)   391409 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/debug_data/elem_40elecs.dat
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    33013 2021-12-11 13:56:32.000000 crtomo_tools-0.3.0/lib/crtomo/eitManager.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    50219 2024-04-29 07:17:32.000000 crtomo_tools-0.3.0/lib/crtomo/grid.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    10375 2024-02-23 14:02:53.000000 crtomo_tools-0.3.0/lib/crtomo/interface.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4214 2024-02-23 08:55:05.000000 crtomo_tools-0.3.0/lib/crtomo/mpl.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3488 2024-04-09 11:25:17.000000 crtomo_tools-0.3.0/lib/crtomo/mpl_setup.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2894 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/nodeManager.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.845306 crtomo_tools-0.3.0/lib/crtomo/notebook/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        0 2024-04-09 11:25:46.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/__init__.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.837306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.849306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18895 2024-04-23 06:19:05.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/about.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18953 2024-04-23 06:19:08.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/data_import.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    20555 2024-04-23 06:19:07.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/fe_meshes.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18904 2024-04-23 06:19:05.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/filtering.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18950 2024-04-23 06:19:07.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/index.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18945 2024-04-23 06:19:06.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/inv_analysis.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    18912 2024-04-23 06:19:06.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/inversion_settings.html
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2423 2024-04-23 06:19:08.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/search.json
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.837306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.857306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/bootstrap/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    98163 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)   176200 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)   462932 2024-04-23 06:19:07.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    80668 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.857306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/clipboard/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     9160 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.861306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5888 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    20084 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3135 2024-03-12 11:45:42.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    28427 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1409 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    24033 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.861306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-nav/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4570 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-nav/headroom.min.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8617 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.865306 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-search/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    92971 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    23539 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    37117 2024-02-15 14:37:13.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/site_libs/quarto-search/quarto-search.js
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       17 2024-04-18 08:29:43.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/manual/html/styles.css
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    42408 2024-04-25 09:53:58.000000 crtomo_tools-0.3.0/lib/crtomo/notebook/nb.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    26131 2024-02-20 15:03:07.000000 crtomo_tools-0.3.0/lib/crtomo/parManager.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    21982 2024-03-29 12:13:51.000000 crtomo_tools-0.3.0/lib/crtomo/plotManager.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4766 2019-11-07 13:44:53.000000 crtomo_tools-0.3.0/lib/crtomo/status.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    99991 2024-04-29 07:17:32.000000 crtomo_tools-0.3.0/lib/crtomo/tdManager.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       38 2024-04-29 07:22:37.885306 crtomo_tools-0.3.0/setup.cfg
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1992 2024-04-29 07:17:25.000000 crtomo_tools-0.3.0/setup.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.881306 crtomo_tools-0.3.0/src/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3743 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/cr_get_analytical_solutions.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5502 2021-06-18 06:09:43.000000 crtomo_tools-0.3.0/src/cr_get_modelling_errors.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    20053 2023-07-19 06:32:22.000000 crtomo_tools-0.3.0/src/cr_trig_create.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    17389 2024-04-29 07:17:32.000000 crtomo_tools-0.3.0/src/cr_trig_parse_gmsh.py
+drwxr-xr-x   0 mweigand  (1001) mweigand  (1001)        0 2024-04-29 07:22:37.885306 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      270 2024-04-29 07:22:37.000000 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/PKG-INFO
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3128 2024-04-29 07:22:37.000000 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)        1 2024-04-29 07:22:37.000000 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1266 2024-04-29 07:22:37.000000 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/entry_points.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)       70 2024-04-29 07:22:37.000000 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/requires.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      533 2024-04-29 07:22:37.000000 crtomo_tools-0.3.0/src/crtomo_tools.egg-info/top_level.txt
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1884 2024-02-20 15:03:07.000000 crtomo_tools-0.3.0/src/grid_convert_boundary_to_svg.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    17290 2023-08-08 09:33:21.000000 crtomo_tools-0.3.0/src/grid_extralines_gen_decouplings.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1158 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_gen_decouplings.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5224 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_gen_depth_decoupling.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2012 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_gen_surface_files.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8771 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_homogenize.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8321 2024-02-20 15:03:07.000000 crtomo_tools-0.3.0/src/grid_parse_svg_to_files.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)      670 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_plot_elem_angles.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     5533 2024-04-29 07:17:32.000000 crtomo_tools-0.3.0/src/grid_plot_wireframe.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2176 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_rotate.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2196 2023-10-16 17:49:52.000000 crtomo_tools-0.3.0/src/grid_translate.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3726 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/grid_translate_model.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    14957 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/sd_plot.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    13522 2022-04-14 08:18:08.000000 crtomo_tools-0.3.0/src/sens_center_plot.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1791 2021-06-19 08:38:19.000000 crtomo_tools-0.3.0/src/td_clean.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     8232 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/td_correct_temperature.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     1910 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/td_init.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)    39648 2023-08-17 11:42:40.000000 crtomo_tools-0.3.0/src/td_plot.py
+-rwxr-xr-x   0 mweigand  (1001) mweigand  (1001)     5241 2023-08-08 09:02:11.000000 crtomo_tools-0.3.0/src/td_residuals.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     7827 2020-11-19 10:52:17.000000 crtomo_tools-0.3.0/src/td_run_all_local.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     2855 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/td_test.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     3531 2019-11-07 13:44:55.000000 crtomo_tools-0.3.0/src/volt_correct_temperature.py
+-rwxr-xr-x   0 mweigand  (1001) mweigand  (1001)     3292 2023-08-08 09:52:29.000000 crtomo_tools-0.3.0/src/volt_filter_using_residuals.py
+-rw-r--r--   0 mweigand  (1001) mweigand  (1001)     4421 2021-12-03 07:04:26.000000 crtomo_tools-0.3.0/src/volt_histogram.py
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/analytical_solution.py` & `crtomo_tools-0.3.0/lib/crtomo/analytical_solution.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/binaries.py` & `crtomo_tools-0.3.0/lib/crtomo/binaries.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/cfg.py` & `crtomo_tools-0.3.0/lib/crtomo/cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 TODO
 ----
 
 * we could also add help texts here for each parameter
 
 """
+import io
 
 
 class crmod_config(dict):
     """
     Write CRMod configuration files (crmod.cfg).
 
     This class is essentially a dict of CRMod configurations with a few extra
@@ -127,23 +128,34 @@
         self['boundary_file'] = 'boundary.dat'
 
     def write_to_file(self, filename):
         """
         Write the configuration to a file. Use the correct order of values.
         """
         self._check_and_convert_bools()
-        fid = open(filename, 'w')
+
+        if isinstance(filename, io.BytesIO):
+            fid = filename
+        else:
+            fid = open(filename, 'wb')
 
         for key in self.key_order:
-            if(key == -1):
-                fid.write('\n')
+            if (key == -1):
+                fid.write(bytes('\n', 'utf-8'))
             else:
-                fid.write('{0}\n'.format(self[key]))
-
-        fid.close()
+                fid.write(
+                    bytes(
+                        '{0}\n'.format(self[key]),
+                        'utf-8',
+                    )
+                )
+
+        # do not close BytesIO stream
+        if not isinstance(filename, io.BytesIO):
+            fid.close()
 
     def __repr__(self):
         self._check_and_convert_bools()
         representation = ''
         for key in self.key_order:
             if key == -1:
                 representation += '\n'
@@ -256,23 +268,32 @@
             ) + self.mswitch_values[key]
         else:
             self['mswitch'] = (self['mswitch'] % self.mswitch_values[key])
 
     def write_to_file(self, filename):
         """ Write the configuration to a file. Use the correct order of values.
         """
-        fid = open(filename, 'w')
+        if isinstance(filename, io.BytesIO):
+            fid = filename
+        else:
+            fid = open(filename, 'wb')
 
         for key in self.key_order:
-            if(key == -1):
-                fid.write('\n')
+            if (key == -1):
+                fid.write(bytes('\n', 'utf-8'))
             else:
-                fid.write('{0}\n'.format(self[key]))
+                fid.write(
+                    bytes(
+                        '{0}\n'.format(self[key]),
+                        'utf-8',
+                    )
+                )
 
-        fid.close()
+        if not isinstance(filename, io.BytesIO):
+            fid.close()
 
     def copy(self):
         return self.__copy__()
 
     def __copy__(self):
         new_copy = crtomo_config()
         # translate the keys
@@ -309,15 +330,20 @@
         """Import a CRTomo configuration from an existing crtomo.cfg file
 
         Parameters
         ----------
         filename : str
             Path to crtomo.cfg file
         """
-        lines_raw = [x.strip() for x in open(filename, 'r').readlines()]
+        if isinstance(filename, io.BytesIO):
+            line_data = filename.readlines()
+        else:
+            with open(filename, 'r') as fid:
+                line_data = fid.readlines()
+        lines_raw = [x.strip() for x in line_data]
         key_index = 0
         for line in lines_raw:
             # ignore comments
             if line.startswith('#'):
                 continue
             else:
                 # check if we have inline comments
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/configManager.py` & `crtomo_tools-0.3.0/lib/crtomo/configManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,18 +207,18 @@
                         try_fix_signs=False):
         """Load CRMod measurement data, either from file or directly from a
         numpy array.
 
         Parameters
         ----------
         data_source : string|numpy.ndarray
-            if this is a string, treat it as an input filename. If it is a Nx5
+            if this is a string, treat it as an input filename. If it is a Nx6
             or Nx3 numpy array, use this data directly
         is_forward_response : bool, optional
-            If True this indicated volt.dat file created by CRTomo during an
+            If True this indicates a volt.dat file created by CRTomo during an
             inversion run to store forward responses of a given model
             iteration. In this case the third data column indicates the wdfak
             parameter, i.e., it indicates if a given data point was excluded
             from this iteration.
         try_fix_signs : bool, optional
             If True, try to fix sign reversals with respect to an already
             registered configuration set by swappend m and n entries.
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/debug.py` & `crtomo_tools-0.3.0/lib/crtomo/debug.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/elem_20elecs.dat` & `crtomo_tools-0.3.0/lib/crtomo/debug_data/elem_20elecs.dat`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/debug_data/elem_40elecs.dat` & `crtomo_tools-0.3.0/lib/crtomo/debug_data/elem_40elecs.dat`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/eitManager.py` & `crtomo_tools-0.3.0/lib/crtomo/eitManager.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/grid.py` & `crtomo_tools-0.3.0/lib/crtomo/grid.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     grid.nodes['presort'][grid.elements[0], :]
     # columns: node number - x position - z position
 """
 import tempfile
 import subprocess
 import os
 import time
+import io
 
 import numpy as np
 import scipy.sparse
 from scipy.spatial.distance import pdist
 import scipy.spatial
 import pandas as pd
 
@@ -105,14 +106,22 @@
             'electrode_color': 'k',
         }
         self.grid = None
         self.nr_of_elements = None
         self.nr_of_nodes = None
         self.nr_of_electrodes = None
 
+        # can hold an KDTree of the element centroids
+        self.centroid_tree = None
+        # can hold an KDTree of the node coordinates
+        self.node_tree = None
+
+        # can hold the distance matrix of the mesh, as a csr_array
+        self.distance_matrix = None
+
         # will be used for caching by .get_element_centroids
         self.centroids = None
 
         if elem_file is None and not empty:
             # check if elem.dat is present
             if os.path.isfile('elem.dat'):
                 elem_file = 'elem.dat'
@@ -226,41 +235,40 @@
             * "cutmck_index" : Array containing the indices in "presort" to
               obtain the "sorted" values:
               nodes['sorted'] = nodes['presort'] [nodes['cutmck_index'], :]
             * "rev_cutmck_index" : argsort(cutmck_index)
         """
         nodes = {}
 
-        #   # prepare nodes
-        #   nodes_sorted = np.zeros((number_of_nodes, 3), dtype=float)
-        #   nodes = np.zeros((number_of_nodes, 3), dtype=float)
-
         # read in nodes
         nodes_raw = np.empty((self.header['nr_nodes'], 3), dtype=float)
         for nr in range(0, self.header['nr_nodes']):
             node_line = fid.readline().lstrip()
             nodes_raw[nr, :] = np.fromstring(
                 node_line, dtype=float, sep='    ')
 
         # round node coordinates to 5th decimal point. Sometimes this is
         # important when we deal with mal-formatted node data
         nodes_raw[:, 1:3] = np.round(nodes_raw[:, 1:3], 5)
 
         # check for CutMcK
         # The check is based on the first node, but if one node was renumbered,
         # so were all the others.
-        if(nodes_raw[:, 0] != list(range(1, nodes_raw.shape[0]))):
+        if (
+                ~np.all(
+                    nodes_raw[:, 0] == list(
+                        range(1, nodes_raw.shape[0] + 1)))):
             self.header['cutmck'] = True
             print(
                 'This grid was sorted using CutMcK. The nodes were resorted!')
         else:
             self.header['cutmck'] = False
 
         # Rearrange nodes when CutMcK was used.
-        if(self.header['cutmck']):
+        if (self.header['cutmck']):
             nodes_cutmck = np.empty_like(nodes_raw)
             nodes_cutmck_index = np.zeros(nodes_raw.shape[0], dtype=int)
             for node in range(0, self.header['nr_nodes']):
                 new_index = np.where(nodes_raw[:, 0].astype(int) == (node + 1))
                 nodes_cutmck[new_index[0], 1:3] = nodes_raw[node, 1:3]
                 nodes_cutmck[new_index[0], 0] = new_index[0]
                 nodes_cutmck_index[node] = new_index[0]
@@ -314,15 +322,15 @@
         """
         depending on the type of grid (rectangular or triangle), prepare grids
         or triangle lists
 
         TODO: We want some nice way of not needing to know in the future if we
               loaded triangles or quadratic elements.
         """
-        if(self.header['element_infos'][0, 2] == 3):
+        if (self.header['element_infos'][0, 2] == 3):
             print('Triangular grid found')
             self.grid_is_rectangular = False
 
             triangles = self.element_data[3]
             triangles = [x.nodes for x in triangles]
             # python starts arrays with 0, but elem.dat with 1
             triangles = np.array(triangles) - 1
@@ -397,78 +405,108 @@
                         int(fid.readline().strip())
                     )
         except Exception as e:
             e
             raise Exception('Not enough neighbors in file')
 
     def load_elem_file(self, elem_file):
-        """
+        """Load a CRTomo/CRMod elem.dat mesh file from either a file, or from
+        stringIO
 
         """
-        with open(elem_file, 'r') as fid:
-            self._read_elem_header(fid)
-            self._read_elem_nodes(fid)
-            self._read_elem_elements(fid)
-            self._read_elem_neighbors(fid)
+        if isinstance(elem_file, (io.StringIO, io.BytesIO,)):
+            # the StringIO object can directly be used
+            fid = elem_file
+        else:
+            fid = open(elem_file, 'r')
+        self._read_elem_header(fid)
+        self._read_elem_nodes(fid)
+        self._read_elem_elements(fid)
+        self._read_elem_neighbors(fid)
+        fid.close()
+
         self._prepare_grids()
 
     def save_elem_file(self, output):
         """Save elem.dat to file.
         The grid is saved as read in, i.e., with or without applied cutmck.
         If you want to change node coordinates, use self.nodes['raw']
 
         Parameters
         ----------
         filename: string
             output filename
         """
-        with open(output, 'wb') as fid:
-            self._write_elem_header(fid)
-            self._write_nodes(fid)
-            self._write_elements(fid)
-            self._write_neighbors(fid)
+        if isinstance(output, (io.StringIO, io.BytesIO,)):
+            fid = output
+        else:
+            fid = open(output, 'wb')
+        self._write_elem_header(fid)
+        self._write_nodes(fid)
+        self._write_elements(fid)
+        self._write_neighbors(fid)
+        if not isinstance(fid, io.BytesIO):
+            fid.close()
 
     def save_elec_file(self, filename):
-        with open(filename, 'wb') as fid:
-            fid.write(
-                bytes(
-                    '{0}\n'.format(int(self.electrodes.shape[0])),
-                    'utf-8',
-                )
+        if isinstance(filename, (io.StringIO, io.BytesIO,)):
+            fid = filename
+        else:
+            fid = open(filename, 'wb')
+        fid.write(
+            bytes(
+                '{0}\n'.format(int(self.electrodes.shape[0])),
+                'utf-8',
             )
-            # the + 1 fixes the zero-indexing
-            np.savetxt(fid, self.electrodes[:, 0].astype(int) + 1, fmt='%i')
+        )
+        # the + 1 fixes the zero-indexing
+        np.savetxt(
+            fid, self.electrodes[:, 0].astype(int) + 1, fmt='%i',
+            encoding='utf-8',
+        )
+        if not isinstance(fid, io.BytesIO):
+            fid.close()
 
     def _write_neighbors(self, fid):
         for key in (11, 12):
             if key in self.neighbors:
-                np.savetxt(fid, self.neighbors[key], fmt='%i')
+                np.savetxt(
+                    fid, self.neighbors[key], fmt='%i', encoding='utf-8'
+                )
 
     def _write_elements(self, fid):
         for dtype in self.header['element_infos'][:, 0]:
             for elm in self.element_data[dtype]:
-                np.savetxt(fid, np.atleast_2d(elm.nodes), fmt='%i')
+                np.savetxt(
+                    fid, np.atleast_2d(elm.nodes), fmt='%i', encoding='utf-8')
 
     def _write_nodes(self, fid):
-        np.savetxt(fid, self.nodes['raw'], fmt='%i %f %f')
+        np.savetxt(fid, self.nodes['raw'], fmt='%i %f %f', encoding='utf-8')
 
     def _write_elem_header(self, fid):
         fid.write(
             bytes(
                 '{0} {1} {2}\n'.format(
                     self.header['nr_nodes'],
                     self.header['nr_element_types'],
                     self.header['bandwidth']),
                 'utf-8',
             )
         )
-        np.savetxt(fid, self.header['element_infos'], fmt='%i')
+        np.savetxt(
+            fid, self.header['element_infos'], fmt='%i', encoding='utf-8')
 
     def load_elec_file(self, elec_file):
-        electrode_nodes_raw = np.loadtxt(elec_file, skiprows=1, dtype=int) - 1
+        if isinstance(elec_file, (io.StringIO, io.BytesIO,)):
+            # the StringIO object can directly be used
+            fid = elec_file
+        else:
+            fid = open(elec_file, 'r')
+        electrode_nodes_raw = np.loadtxt(fid, skiprows=1, dtype=int) - 1
+        fid.close()
         self.electrodes = self.nodes['presort'][electrode_nodes_raw]
         self.nr_of_electrodes = self.electrodes.shape[0]
 
     def load_grid(self, elem_file, elec_file):
         """Load elem.dat and elec.dat
         """
         self.load_elem_file(elem_file)
@@ -476,15 +514,15 @@
 
     def get_electrode_node(self, electrode):
         """
         For a given electrode (e.g. from a config.dat file), return the true
         node number as in self.nodes['sorted']
         """
         elec_node_raw = int(self.electrodes[electrode - 1][0])
-        if(self.header['cutmck']):
+        if (self.header['cutmck']):
             elec_node = self.nodes['rev_cutmck_index'][elec_node_raw]
         else:
             elec_node = elec_node_raw - 1
         return int(elec_node)
 
     def plot_grid_to_ax(self, ax, **kwargs):
         """
@@ -509,14 +547,16 @@
                 self.electrodes[:, 1],
                 self.electrodes[:, 2],
                 color=self.props['electrode_color'],
                 clip_on=False,
             )
         ax.set_xlim(self.grid['x'].min(), self.grid['x'].max())
         ax.set_ylim(self.grid['z'].min(), self.grid['z'].max())
+        ax.set_xlabel('x [m]')
+        ax.set_ylabel('z [m]')
         # ax.autoscale_view()
         ax.set_aspect('equal')
 
         if kwargs.get('plot_electrode_numbers', False):
             for nr, xy in enumerate(self.electrodes[:, 1:3]):
                 ax.text(
                     xy[0], xy[1],
@@ -719,14 +759,65 @@
             ax.set_ylabel('count')
             fig.tight_layout()
             # fig.savefig('plot_element_angles.jpg', dpi=300)
             return fig, ax
 
     @property
     def element_neighbors(self):
+        if self.element_neighbors_data is not None:
+            return self.element_neighbors_data
+
+        if self.centroid_tree is None:
+            centroids = self.get_element_centroids()
+            self.centroid_tree = scipy.spatial.cKDTree(centroids)
+
+        max_nr_edges = self.header['element_infos'][0, 2]
+
+        A = self.get_element_areas().max()
+        # A = pi * r^2
+        radius = np.sqrt(A / np.pi)
+
+        # initialize the neighbor array
+        self.element_neighbors_data = []
+        self.element_neighbors_edges = []
+
+        print('Looking for neighbors (V2 with cKDTree)')
+        time_start = time.perf_counter()
+        for nr, element_nodes in enumerate(self.elements):
+            neighbors_edges = []
+            neighbors_indices = []
+            # r = set(self.centroid_tree.query(centroids[nr], max_nr_edges)[1])
+            r = set(
+                self.centroid_tree.query_ball_point(
+                    centroids[nr],
+                    2 * radius
+                )
+            )
+            for index in list(r):
+                el_test = self.elements[index]
+                intersect_nodes = np.intersect1d(element_nodes, el_test)
+                if len(intersect_nodes) == 2:
+                    neighbors_indices += [index]
+                    neighbors_edges += [intersect_nodes]
+                # if len(intersect_nodes) in (0, 1, 3):
+                #     r.remove(index)
+                # neighbors_edges.append(intersect_nodes)
+                if len(neighbors_indices) == max_nr_edges:
+                    break
+            self.element_neighbors_edges.append(neighbors_edges)
+            self.element_neighbors_data.append(neighbors_indices)
+
+        # import IPython
+        # IPython.embed()
+        time_end = time.perf_counter()
+        print('elapsed time: {} s'.format(time_end - time_start))
+        return self.element_neighbors_data
+
+    @property
+    def element_neighbors_old(self):
         """Return a list with element numbers (zero indexed) of neighboring
         elements. Note that the elements are not sorted. No spacial orientation
         can be inferred from the order of neighbors.
 
         WARNING: This function is slow due to a nested loop. This would be a
         good starting point for further optimizations.
 
@@ -949,15 +1040,15 @@
         ...     lines=[0.4, 0.8], debug=False, workdir=None)
         >>> import pylab as plt
         >>> fig, ax = plt.subplots()
         >>> grid.plot_grid_to_ax(ax)
 
         """
         # check if all required information are present
-        if(electrodes_x is None and
+        if (electrodes_x is None and
            (nr_electrodes is None or spacing is None)):
             raise Exception(
                 'You must provide either the parameter "electrodes_" or ' +
                 'the parameters "nr_electrodes" AND "spacing"'
             )
 
         if electrodes_x is None:
@@ -990,19 +1081,19 @@
 
         # min/max coordinates of final grid
         minimum_x = minx - left
         maximum_x = maxx + left
         minimum_z = np.min(electrodes[:, 1]) - depth
         # maximum_z = 0
 
-        boundary_noflow = 11
-        boundary_mixed = 12
+        boundary_noflow = 12
+        boundary_mixed = 11
 
         if force_neumann_only:
-            boundary_mixed = 11
+            boundary_mixed = 12
 
         # prepare extra lines
         extra_lines = []
         add_boundary_nodes_left = []
         add_boundary_nodes_right = []
 
         if electrodes_x is not None and lines is not None:
@@ -1081,27 +1172,33 @@
         else:
             if not os.path.isdir(workdir):
                 os.makedirs(workdir)
             tempdir = workdir
 
         np.savetxt(
             tempdir + os.sep + 'electrodes.dat', electrodes,
-            fmt='%.3f %.3f'
+            fmt='%.3f %.3f',
+            encoding='utf-8',
+        )
+        np.savetxt(
+            tempdir + os.sep + 'boundaries.dat', boundaries,
+            fmt='%.3f %.3f %i',
+            encoding='utf-8',
         )
-        np.savetxt(tempdir + os.sep + 'boundaries.dat', boundaries,
-                   fmt='%.3f %.3f %i')
         np.savetxt(
             tempdir + os.sep + 'char_length.dat',
-            np.atleast_1d(char_lengths)
+            np.atleast_1d(char_lengths),
+            encoding='utf-8',
         )
         if extra_lines:
             np.savetxt(
                 tempdir + os.sep + 'extra_lines.dat',
                 np.atleast_2d(extra_lines),
-                fmt='%.3f %.3f %.3f %.3f'
+                fmt='%.3f %.3f %.3f %.3f',
+                encoding='utf-8',
             )
         pwd = os.getcwd()
         os.chdir(tempdir)
         try:
             if debug:
                 subprocess.call(
                     'cr_trig_create grid',
@@ -1136,16 +1233,18 @@
         points = np.array(
             [(x, y) for x, y in zip(
                 np.linspace(p0[0], p1[0], N), np.linspace(p0[1], p1[1], N)
             )]
         )
         centroids = self.get_element_centroids()
 
-        tree = scipy.spatial.cKDTree(centroids)
-        element_indices = tree.query(points)[1]
+        if self.centroid_tree is None:
+            self.centroid_tree = scipy.spatial.cKDTree(centroids)
+
+        element_indices = self.centroid_tree.query(points)[1]
         return element_indices
 
     def get_element_indices_within_rectangle(self, xmin, xmax, zmin, zmax):
         """Return the indices of all elements whose center is located within
         the rectangle defined by the parameters.
 
         The indices can then be used, e.g., to select values from inversion
@@ -1240,7 +1339,88 @@
             ][i].xcoords[::-1]
 
             self.element_data[
                 element_type
             ][i].zcoords = self.element_data[
                 element_type
             ][i].zcoords[::-1]
+
+    def get_distance_matrix(self):
+        if self.distance_matrix is not None:
+            return self.distance_matrix
+
+        N = self.nr_of_nodes
+        self.distance_matrix = scipy.sparse.lil_array((N, N))
+        for element in self.elements:
+            # works only for triangles!
+            for a, b in zip((0, 1, 2), (1, 2, 0)):
+                index_a = element[a]
+                index_b = element[b]
+
+                coords_a = self.nodes['presort'][element[a]][1:3]
+                coords_b = self.nodes['presort'][element[b]][1:3]
+
+                # compute distance between nodes
+                distance = np.linalg.norm(
+                    coords_a - coords_b
+                )
+
+                self.distance_matrix[index_a, index_b] = distance
+                self.distance_matrix[index_b, index_a] = distance
+        return self.distance_matrix
+
+    def get_node_tree(self):
+        if self.node_tree is not None:
+            return self.node_tree
+        self.node_tree = scipy.spatial.KDTree(
+            self.nodes['presort'][:, 1:3]
+        )
+        return self.node_tree
+
+    def find_nearest_node(self, coords, return_node_coords=True):
+        node_tree = self.get_node_tree()
+        result = node_tree.query(coords, 1)[1]
+        if return_node_coords:
+            return result, self.nodes['presort'][result][1:3]
+        return result
+
+    def determine_path_along_nodes(self, start_coordinate, end_coordinate):
+        """
+
+        """
+        start, (sx, sy) = self.find_nearest_node(start_coordinate, True)
+        end, (ex, ey) = self.find_nearest_node(end_coordinate, True)
+
+        path_dist, path_pred = scipy.sparse.csgraph.shortest_path(
+            self.get_distance_matrix(),
+            directed=False,
+            return_predecessors=True,
+            unweighted=False,
+        )
+        path_nodes = []
+        path_pred[start]
+
+        # determine the nodes of the path
+        N = self.nr_of_elements
+        index = end
+        path_nodes += [end]
+        for i in range(N):
+            next_index = path_pred[start][index]
+            if next_index > 0:
+                path_nodes += [path_pred[start][index]]
+                index = next_index
+            else:
+                break
+
+        # determine elements adjacent to the path
+        el_pairs = []
+        for i in range(len(path_nodes) - 1):
+            a1 = path_nodes[i]
+            a2 = path_nodes[i+1]
+            relevant_elements = np.intersect1d(
+                np.where(np.any(self.elements == a1, axis=1))[0],
+                np.where(np.any(self.elements == a2, axis=1))[0]
+            )
+
+            if len(relevant_elements) == 2:
+                el_pairs += [np.hstack(([a1, a2], relevant_elements))]
+        return np.array(el_pairs)
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/interface.py` & `crtomo_tools-0.3.0/lib/crtomo/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,25 @@
         if m.shape[1] == 2:
             pid_pha = tdm.parman.add_data(m[:, 1])
         else:
             pid_pha = tdm.parman.add_data(np.zeros(m.shape[0]))
         tdm.register_phase_model(pid_pha)
         return tdm
 
-    def forward_complex(self, log_sigma):
+    def forward_complex(self, log_sigma, silent=True):
         r"""Compute a model response, i.e. complex impedances
 
         Parameters
         ----------
         log_sigma : 1xN or 2xN numpy.ndarray
             Model parameters. First column: :math:`log_e(\sigma)`, second
             column: :math:`\phi_{cond} [mrad]`.  If first dimension is of
             length one, assume phase values to be zero.
+        silent : bool (True)
+            If True, suppress output of CRMod
 
         Returns
         -------
         measurements : Nx2 numpy.ndarray
             Return log_e Y values of computed forward response
         """
         log_sigma = np.atleast_2d(log_sigma)
@@ -93,15 +95,15 @@
         if log_sigma.shape[0] == 1:
             rpha = np.zeros_like(rmag)
         else:
             # convert to resistivities
             rpha = -log_sigma[1, :]
         m = np.vstack((rmag, rpha)).T
         tdm = self._get_tdm(m)
-        measurements = tdm.measurements()
+        measurements = tdm.measurements(silent=silent)
         # convert R to log Y
         measurements[:, 0] = np.log(1.0 / measurements[:, 0])
         # convert rpha to cpha
         measurements[:, 1] *= -1
         return measurements
 
     def J(self, log_sigma):
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/mpl.py` & `crtomo_tools-0.3.0/lib/crtomo/mpl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """Thils file set ups matplotlib plot functions for the whole package.
 
 Import all necessary Matplotlib modules and set default options
-To use this module, import * from it:
+To use this module, call the setup() function.
 
 Examples
 --------
 
     >>> import crtomo.mpl
     >>> crtomo.mpl.setup()
 
@@ -23,15 +23,21 @@
     import matplotlib as mpl
 
     if not already_loaded:
         mpl.use('Agg')
 
     import matplotlib.pyplot as plt
 
-    plt.style.use('seaborn')
+    mpl_version = [int(x) for x in mpl.__version__.split('.')]
+
+    if mpl_version[0] >= 3 and mpl_version[1] > 6:
+        plt.style.use("seaborn-v0_8")
+    else:
+        # old style for older matplotlib versions (<= 3.6)
+        plt.style.use("seaborn")
 
     general_settings()
 
     import mpl_toolkits.axes_grid1 as axes_grid1
     axes_grid1
     return plt, mpl
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/mpl_setup.py` & `crtomo_tools-0.3.0/lib/crtomo/mpl_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Thils file set ups matplotlib plot functions for the whole package.
+"""This file set ups matplotlib plot functions for the whole package.
 
 Import all necessary Matplotlib modules and set default options
 To use this module, import * from it:
 
 Examples
 --------
 
@@ -21,16 +21,15 @@
 
 # general settings
 mpl.rcParams["lines.linewidth"] = 2.0
 mpl.rcParams["lines.markeredgewidth"] = 3.0
 mpl.rcParams["lines.markersize"] = 3.0
 mpl.rcParams["font.size"] = 8
 # mpl.rcParams['font.sans-serif'] = 'Droid Sans'
-
-mpl.rcParams['font.family'] = 'Open Sans'
+# mpl.rcParams['font.family'] = 'Open Sans'
 # mpl.rcParams['font.weight'] = 400
 mpl.rcParams['mathtext.default'] = 'regular'
 
 # mpl.rcParams['font.family'] = 'Droid Sans'
 
 mpl.rcParams['text.usetex'] = False
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/nodeManager.py` & `crtomo_tools-0.3.0/lib/crtomo/nodeManager.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/parManager.py` & `crtomo_tools-0.3.0/lib/crtomo/parManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         return self.index
 
     def reset(self):
         """Resets the ParMan instance. This process deletes all data and
         metadata, and resets the index variable
         """
         self.index = -1
-        del(self.parsets)
+        del (self.parsets)
         self.parsets = {}
-        del(self.metadata)
+        del (self.metadata)
         self.metadata = {}
 
     def add_data(self, data, metadata=None):
         """Add data to the parameter set
 
         Parameters
         ----------
@@ -98,15 +98,15 @@
                     'elements in the grid'
                 )
 
         # now make sure that metadata can be zipped with the subdata
         K = subdata.shape[0]
         if metadata is not None:
             if K > 1:
-                if(not isinstance(
+                if (not isinstance(
                    metadata, (list, tuple)) or len(metadata) != K):
                     raise Exception('metadata does not fit the provided data')
             else:
                 # K == 1
                 metadata = [metadata, ]
 
         if metadata is None:
@@ -353,18 +353,54 @@
         """
         area_polygon = shapgeo.Polygon(
             ((xmin, zmax), (xmax, zmax), (xmax, zmin), (xmin, zmin))
         )
         self.modify_polygon(pid, area_polygon, value)
 
     def modify_polygon(self, pid, polygon, value):
+        """Modify parts of a parameter set by modifying all elements within a
+        provided :class:`shapely.geometry.Polygon` instance. Hereby, an element
+        is modified if its center lies within the polygon.
+
+        Parameters
+        ----------
+        pid: int
+            id of parameter set to vary
+        polygon: :class:`shapely.geometry.Polygon` instance
+            polygon that determines the area to modify
+        value: float
+            value that is assigned to all elements in the polygon
+
+        Examples
+        --------
+        >>> import shapely.geometry
+            polygon = shapely.geometry.Polygon((
+                (2, 0), (4, -1), (2, -1)
+            ))
+            tdman.parman.modify_polygon_centroids(pid, polygon, 3)
+
+        """
+        centroids = self.grid.get_element_centroids()
+        # now determine elements in area
+        elements_in_area = []
+        for nr, centroid in enumerate(centroids):
+            if polygon.contains(shapgeo.Point(centroid)):
+                elements_in_area.append(nr)
+        # change the values
+        pid_clean = self._clean_pid(pid)
+        self.parsets[pid_clean][elements_in_area] = value
+
+    def modify_polygon_old(self, pid, polygon, value):
         """Modify parts of a parameter set by setting all parameters located
         in, or touching, the provided :class:`shapely.geometry.Polygon`
         instance.
 
+        WARNING: This implementation often leads to ragged borders in the
+        selected polygons. Use the new modify_polygon function!
+
         Parameters
         ----------
         pid: int
             id of parameter set to vary
         polygon: :class:`shapely.geometry.Polygon` instance
             polygon that determines the area to modify
         value: float
@@ -713,7 +749,53 @@
                     (coords[:, 0] <= pos_x + anomaly_width) &
                     (coords[:, 1] <= pos_z) &
                     (coords[:, 1] >= (pos_z - anomaly_height))
                 )
                 paradd[indices] = peak_value
 
         self.parsets[pid] += paradd
+
+    def _com_data_trafo_mode(self, subdata, mode):
+        if mode == "none":
+            # just take the absolute values
+            s = np.abs(subdata)
+        elif mode == "log10":
+            # log10 values of absolutes
+            s = np.abs(np.log10(np.abs(subdata)))
+        elif mode == "sqrt":
+            # square roots of absolutes
+            s = np.sqrt(np.abs(subdata))
+        return s
+
+    def center_of_mass_value(self, pid, mode='log10'):
+        """Compute the center of mass value of a given parameter set.
+        """
+        centroids = self.grid.get_element_centroids()
+
+        # compute the integrative value
+        subdata = self.parsets[pid]
+        s = self._com_data_trafo_mode(subdata, mode)
+
+        com_x = np.sum(centroids[:, 0] * s) / np.sum(s)
+        com_y = np.sum(centroids[:, 1] * s) / np.sum(s)
+        # to check: do we need to norm here?
+
+        return [com_x, com_y]
+
+    def center_of_mass_value_multiple(self, pid_list, mode='none'):
+        print('center_of_mass_value_multiple')
+        centroids = self.grid.get_element_centroids()
+        values = np.vstack(
+            [self.parsets[index] for index in pid_list]
+        )
+        s = self._com_data_trafo_mode(values, mode)
+        xy = np.dot(s, centroids)
+
+        s_sum = np.sum(s, axis=1)
+
+        s_sum_stacked = np.tile(s_sum, (2, 1))
+        s_sum_T = s_sum_stacked.T
+
+        com = xy / s_sum_T
+        return com
+        # import IPython
+        # IPython.embed()
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/plotManager.py` & `crtomo_tools-0.3.0/lib/crtomo/plotManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 color=self.grid.props['electrode_color'],
                 # clip_on=False,
             )
 
             return fig, ax, pc, cb
         return fig, ax, pc
 
-    def plot_nodes_contour_to_ax(self, nid, **kwargs):
+    def plot_nodes_contour_to_ax(self, ax, nid, **kwargs):
         """Plot node data to an axes object
 
         Parameters
         ----------
         ax : axes object, optional
             axes to plot to. If not provided, generate a new figure and axes
         nid : int
@@ -168,132 +168,197 @@
             Minimum colorbar value
         cbmax : float, optional
             Maximum colorbar value
         plot_colorbar : bool, optional
             if true, plot a colorbar next to the plot
         use_aspect: bool, optional
             plot grid in correct aspect ratio. Default: True
+        fill_contours: bool, optional (true)
+            If True, the fill the contours (contourf)
 
         """
-        if 'ax' not in kwargs:
-            fig, ax = plt.subplots(1, 1)
-        else:
-            ax = kwargs.get('ax')
+        # if 'ax' not in kwargs:
+        #     fig, ax = plt.subplots(1, 1)
+        # else:
+        #     ax = kwargs.get('ax')
 
+        fig = ax.get_figure()
         x = self.grid.nodes['presort'][:, 1]
         z = self.grid.nodes['presort'][:, 2]
         xz = np.vstack((x, z)).T
 
         # generate grid
         X, Z = np.meshgrid(
             np.linspace(x.min(), x.max(), 1000),
             np.linspace(z.min(), z.max(), 1000),
         )
 
         values = np.array(self.nodeman.nodevals[nid])
+        if kwargs.get('converter', None) is not None:
+            values = kwargs['converter'](values)
         # linear
         # cubic
         cint = scipy.interpolate.griddata(
             xz,
             values,
             (X, Z),
-            method='linear',
+            method='cubic',
             # method='linear',
             # method='nearest',
             fill_value=np.nan,
         )
         cint_ma = np.ma.masked_invalid(cint)
 
-        pc = ax.contourf(
-            X, Z, cint_ma,
-            cmap=kwargs.get('cmap', 'jet'),
-            vmin=kwargs.get('cbmin', None),
-            vmax=kwargs.get('cbmax', None),
-        )
+        cmap = mpl.colormaps['turbo'].resampled(1)
+        if kwargs.get('fill_contours', True):
+            pc = ax.contourf(
+                X, Z, cint_ma,
+                cmap=kwargs.get('cmap', 'jet'),
+                vmin=kwargs.get('cbmin', None),
+                vmax=kwargs.get('cbmax', None),
+                levels=kwargs.get('cblevels', None)
+            )
+        else:
+            pc = ax.contour(
+                X, Z, cint_ma,
+                cmap=cmap,
+                vmin=kwargs.get('cbmin', None),
+                vmax=kwargs.get('cbmax', None),
+                levels=kwargs.get('cblevels', None),
+                alpha=kwargs.get('alpha', 1.0),
+            )
 
         # plot electrodes
         ax.scatter(
             self.grid.electrodes[:, 1],
             self.grid.electrodes[:, 2],
         )
 
         # pc = ax.pcolormesh(
         #     X, Z, cint_ma,
         #     vmin=-40,
         #     vmax=40,
         # )
         if kwargs.get('use_aspect', True):
             ax.set_aspect('equal')
+        ax.set_xlabel(kwargs.get('xlabel', 'x [m]'))
+        ax.set_ylabel(kwargs.get('zlabel', 'z [m]'))
+        # if kwargs.get('plot_colorbar', False):
+        #     fig = ax.get_figure()
+        #     cb = fig.colorbar(pc, ax=ax)
+        if kwargs.get('plot_colorbar', False):
+            divider = make_axes_locatable(ax)
+            cbposition = kwargs.get('cbposition', 'vertical')
+            if cbposition == 'horizontal':
+                ax_cb = divider.new_vertical(
+                    size=0.1, pad=0.4, pack_start=True
+                )
+            elif cbposition == 'vertical':
+                ax_cb = divider.new_horizontal(
+                    size=0.1, pad=0.4,
+                )
+            else:
+                raise Exception('cbposition not recognized')
+
+            fig.add_axes(ax_cb)
+
+            cb = fig.colorbar(
+                pc,
+                cax=ax_cb,
+                orientation=cbposition,
+                label=kwargs.get('cblabel', ''),
+                ticks=mpl.ticker.MaxNLocator(kwargs.get('cbnrticks', 3)),
+                format=kwargs.get('cbformat', None),
+                extend='both',
+            )
+
         if kwargs.get('plot_colorbar', False):
-            fig = ax.get_figure()
-            cb = fig.colorbar(pc, ax=ax)
             return fig, ax, pc, cb
         return fig, ax, pc
 
-    def plot_nodes_streamlines_to_ax(self, ax, cid, **kwargs):
+    def plot_nodes_current_streamlines_to_ax(self, ax, cid, model_pid, **kwargs):
         """
 
         """
         # node locations
         x = self.grid.nodes['presort'][:, 1]
         z = self.grid.nodes['presort'][:, 2]
         xz = np.vstack((x, z)).T
 
-        # generate grid
+        # generate a fine grid
         X, Z = np.meshgrid(
-            np.linspace(x.min(), x.max(), 100),
-            np.linspace(z.min(), z.max(), 100),
+            np.linspace(x.min(), x.max(), 1000),
+            np.linspace(z.min(), z.max(), 1000),
         )
 
         values = np.array(self.nodeman.nodevals[cid])
 
         # linear
         # cubic
         cint = scipy.interpolate.griddata(
             xz,
             values,
             (X, Z),
-            method='linear',
+            method='cubic',
             # method='linear',
             # method='nearest',
             fill_value=np.nan,
         )
         cint_ma = np.ma.masked_invalid(cint)
 
-        print(cint_ma.shape)
+        # now compute the gradients in both directions, using the fine
+        # interpolation
         U, V = np.gradient(cint_ma)
 
-        current = np.sqrt(U ** 2 + V ** 2)
-        start_points = np.array((
-            (1.0, 0.0),
-            (11.0, 0.0),
-        ))
-        print(start_points.shape)
+        resistivity = self.parman.parsets[model_pid]
+        res = scipy.interpolate.griddata(
+            self.grid.get_element_centroids(),
+            resistivity,
+            (X, Z),
+            method='cubic',
+            # method='linear',
+            # method='nearest',
+            fill_value=np.nan,
+        )
+
+        jx = -U / res
+        jz = -V / res
+        # jx = U
+        # jz = V
+
+        # current = np.sqrt(U ** 2 + V ** 2)
+        # start_points = np.array((
+        #     (1.0, 0.0),
+        #     (11.0, 0.0),
+        # ))
+        # print(start_points.shape)
         ax.streamplot(
             X,
             Z,
-            V,
-            U,
-            density=2.0,
-            minlength=0.5,
+            jz,
+            jx,
+            density=kwargs.get('density', 2.0),
+            linewidth=kwargs.get('linewidth', 1.0),
+            minlength=kwargs.get('minlength', 0.5),
+            broken_streamlines=kwargs.get('broken_streamlines', False),
             # start_points=start_points,
         )
 
-        ax.contour(
-            X,
-            Z,
-            current,
-        )
+        # ax.contour(
+        #     X,
+        #     Z,
+        #     current,
+        # )
 
-        pc = ax.contourf(
-            X,
-            Z,
-            cint,
-            N=10,
-        )
+        # pc = ax.contourf(
+        #     X,
+        #     Z,
+        #     cint,
+        #     N=10,
+        # )
         # pc = ax.pcolormesh(
         #     X, Z, current,
         #     # vmin=-40,
         #     # vmax=40,
         # )
         # pc
         # Q = ax.quiver(X, Z, U, V, units='width')
@@ -306,18 +371,18 @@
         #             vmin=-40,
         #             vmax=40,
         #         )
         #         # cb = fig.colorbar(pc)
         #         return pc
         if kwargs.get('use_aspect', True):
             ax.set_aspect('equal')
-        if kwargs.get('plot_colorbar', False):
-            fig = ax.get_figure()
-            cb = fig.colorbar(pc)
-            return cb
+        # if kwargs.get('plot_colorbar', False):
+        #     fig = ax.get_figure()
+        #     cb = fig.colorbar(pc)
+        #     return cb
 
     def plot_elements_to_ax(self, cid, ax=None, **kwargs):
         """Plot element data (parameter sets).
 
         If the parameter *ax* is not set, then a new figure will be created
         with a corresponding axes.
 
@@ -326,15 +391,15 @@
         ----------
         cid : int or :py:class:`numpy.ndarray`
             if *cid* is an int, then treat it as the id of the parameter set
             stored in self.parman. Otherwise, expect it to be the data to plot.
             At the moment no checks are made that the data fits the grid.
         ax : matplotlib.Axes, optional
             plot to this axes object, if provided
-        alpha_cid : int, optional
+        cid_alpha : int, optional
             if given, use the corresponding dataset in self.parman as the alpha
             channel. No checks are made if all values of this data set lie
             between 0 and 1 (0 being fully transparent, and 1 being opaque).
         xmin : float, optional
             minimal x limit to plot
         xmax : float, optional
             maximal x limit to plot
@@ -441,15 +506,15 @@
         cmap.set_over(over)
         cmap.set_under(under)
         cmap.set_bad(bad)
 
         # normalize data
         data_min = kwargs.get('cbmin', np.nanmin(subdata))
         data_max = kwargs.get('cbmax', np.nanmax(subdata))
-        if(data_min is not None and data_max is not None
+        if (data_min is not None and data_max is not None
                 and data_min == data_max):
             data_min -= 1
             data_max += 1
         cnorm = mpl.colors.Normalize(vmin=data_min, vmax=data_max)
         scalarMap = mpl.cm.ScalarMappable(norm=cnorm, cmap=cmap)
         fcolors = scalarMap.to_rgba(subdata)
         scalarMap.set_array(subdata)
@@ -485,15 +550,15 @@
         ax.add_collection(collection)
         no_elecs = kwargs.get('no_elecs', False)
         if self.grid.electrodes is not None and no_elecs is not True:
             ax.scatter(
                 self.grid.electrodes[:, 1],
                 self.grid.electrodes[:, 2],
                 color=self.grid.props['electrode_color'],
-                # clip_on=False,
+                clip_on=False,
             )
 
         ax.set_xlim(xmin, xmax)
         ax.set_ylim(zmin, zmax)
         ax.set_xlabel(kwargs.get('xlabel', 'x [m]'))
         ax.set_ylabel(kwargs.get('zlabel', 'z [m]'))
         ax.set_aspect(kwargs.get('aspect', 'equal'))
@@ -603,7 +668,36 @@
 
     data_transformed = np.arcsinh(
         10 ** dyn * data / norm
     ) / np.arcsinh(
         10 ** dyn
     )
     return data_transformed
+
+
+def converter_sensitivity(data):
+    """
+
+    """
+    norm_value = np.abs(data).max()
+    sens_normed = data / norm_value
+
+    indices_gt_zero = data > 1e-5
+    indices_lt_zero = data < -1e-5
+
+    # map all values greater than zero to the range [0.5, 1]
+    x = np.log10(sens_normed[indices_gt_zero])
+    # log_norm_factor = np.abs(x).max()
+    log_norm_factor = -5
+    y1 = 1 - x / (2 * log_norm_factor)
+
+    # map all values smaller than zero to the range [0, 0.5]
+    x = np.log10(np.abs(sens_normed[indices_lt_zero]))
+    y = x / (2 * log_norm_factor)
+
+    y2 = np.abs(y)
+
+    # reassign values
+    data_transformed = np.ones_like(data) * 0.5
+    data_transformed[indices_gt_zero] = y1
+    data_transformed[indices_lt_zero] = y2
+    return data_transformed
```

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/status.py` & `crtomo_tools-0.3.0/lib/crtomo/status.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/lib/crtomo/tdManager.py` & `crtomo_tools-0.3.0/lib/crtomo/tdManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,22 +45,26 @@
 * plot potential distributions
 
     * also plot current lines via streamlines?
     * can we generate current densities? not sure how to mix element data
       (sigma) and potential data (nodes) in j = sigma E
 
 """
+import time
+import datetime
 from glob import glob
 import re
 import os
 import tempfile
 import subprocess
+import io
 from io import StringIO
 import itertools
 import functools
+import tarfile
 
 import matplotlib.colors
 import matplotlib.cm
 import numpy as np
 import pandas as pd
 
 import crtomo.mpl
@@ -227,14 +231,17 @@
         # if we did measure electrode capacitances, store the average electrode
         # capacitance here
         # See Zimmermann et al. 2018 for more information
         # For now this is only one value [S/m] = omega * C and will be
         # multiplied for each electrode
         self.electrode_admittance = None
 
+        # when calling CRTomo, store output here
+        self.crtomo_error_msg = None
+        self.crtomo_output = None
         self._initialize_components(kwargs)
 
     def __repr__(self):
         """Return meaningful information on current state of the object"""
         str_list = []
         str_list.append(80 * '-')
         str_list.append('tdMan instance')
@@ -342,32 +349,92 @@
 
         self.plot = PlotManager.plotManager(
             grid=self.grid,
             nm=self.nodeman,
             pm=self.parman,
         )
 
+        # store decoupling data for the inversion here
+        # will become a Yx3 array
+        self.decouplings = None
+
         # if we load from a tomodir, also load configs and inversion results
         if tomodir is not None:
             print('importing tomodir results')
             # if present, read crtomo.cfg file
             crtomo_cfg_file = tomodir + os.sep + 'exe' + os.sep + 'crtomo.cfg'
             if os.path.isfile(crtomo_cfg_file):
                 self.crtomo_cfg.import_from_file(crtomo_cfg_file)
+
             # forward configurations
             config_file = tomodir + os.sep + 'config' + os.sep + 'config.dat'
             if os.path.isfile(config_file):
                 self.configs.load_crmod_config(config_file)
 
+            # forward model
+            rho_file = tomodir + os.sep + 'rho' + os.sep + 'rho.dat'
+            if os.path.isfile(rho_file):
+                pid_mag, pid_pha = self.parman.load_from_rho_file(rho_file)
+                self.register_forward_model(pid_mag, pid_pha)
+
             # load data/modeling results
             self._read_modeling_results(tomodir + os.sep + 'mod')
 
             # load inversion results
             self.read_inversion_results(tomodir)
 
+            self.read_decouplings_file(
+                tomodir + os.sep + 'exe' + os.sep + 'decouplings.dat'
+            )
+
+        # if tomodir_tarxz is not None:
+        #     # read from a tarxz file/BytesIO file
+        #     raise Exception('Reading from tar.xz files is not supported yet')
+
+    def read_decouplings_file(self, filename):
+        """Import decoupling data for the inversion. This is usally a file
+        called decouplings.dat in the exe/ directory of a tomodir, but we can
+        also read from an BytesIO object.
+
+        Do nothing if the file does not exist
+
+        Overwrite any existing decouplings
+        """
+        if not isinstance(filename, io.BytesIO):
+            if not os.path.isfile(filename):
+                return
+        decouplings = np.loadtxt(filename, skiprows=1)
+        assert decouplings.shape[1] == 3
+        if self.decouplings is not None:
+            print('WARNING: overwriting existing decouplings')
+            self.decouplings = decouplings
+
+    def save_decouplins_file(self, filename):
+        if self.decouplings is None:
+            return
+        if isinstance(filename, io.BytesIO):
+            fid = filename
+        else:
+            fid = open(filename, 'w')
+
+        fid.write('{}\n'.format(self.decouplings.shape[0]))
+        np.savetxt(fid, self.decouplings, fmt='%i %i %f')
+
+        if not isinstance(filename, io.BytesIO):
+            fid.close()
+
+    def add_to_decouplings(self, new_decouplings):
+        assert new_decouplings.shape[1] == 3
+        if self.decouplings is None:
+            self.decouplings = new_decouplings
+        self.decouplings = np.vstack((
+            self.decouplings,
+            new_decouplings
+        ))
+
     def inv_get_last_pid(self, parameter):
         """Return the pid of the parameter set corresponding to the final
         inversion results of a given parameter. Return None if the parameter
         type does not exist, or no inversion result was registered.
 
         Parameters
         ----------
@@ -375,15 +442,15 @@
             The requested parameter type: cre, cim, rmag, rpha
 
         Returns
         -------
         pid : int|None
             The parameter id, or None
         """
-        if('inversion' in self.a and parameter in self.a['inversion'] and
+        if ('inversion' in self.a and parameter in self.a['inversion'] and
                 len(self.a['inversion'][parameter]) > 0):
             pid = self.a['inversion'][parameter][-1]
             return pid
         return None
 
     def inv_last_rmag_parset(self):
         """Return the resistivity magnitude of the last iteration. None if no
@@ -484,20 +551,20 @@
                 os.makedirs(directory)
 
         os.chdir(pwd)
 
     def _check_state(self):
         """Check if this instance can model and/or can invert
         """
-        if(self.grid is not None and
+        if (self.grid is not None and
            self.configs.configs is not None and
            self.assignments['forward_model'] is not None):
             self.can_model = True
 
-        if(self.grid is not None and
+        if (self.grid is not None and
            self.assignments['measurements'] is not None):
             self.can_invert = True
 
     def load_parset_from_file(self, filename, columns=0):
         """
         Parameters
         ----------
@@ -533,14 +600,144 @@
 
         """
         pids = self.parman.load_from_rho_file(filename)
         self.register_magnitude_model(pids[0])
         self.register_phase_model(pids[1])
         return pids
 
+    def save_to_tarfile(self):
+        """Save the current modeling/inversion data into a tarfile. Return the
+        file as an io.BytesIO object. The tar file is generated completely in
+        memory - no files are written to the disc
+
+        Returns
+        -------
+        tomodir_tar : io.BytesIO
+            Tomodir stored in tar file
+        """
+        tomodir = io.BytesIO()
+        tar = tarfile.open(fileobj=tomodir, mode='w:xz')
+
+        # prepare buffers and write them to the tar file
+        elem_data = io.BytesIO()
+        self.grid.save_elem_file(elem_data)
+        info = tarfile.TarInfo()
+        info.name = 'grid/elem.dat'
+        info.mtime = time.time()
+        info.size = elem_data.tell()
+        info.type = tarfile.REGTYPE
+        elem_data.seek(0)
+        tar.addfile(info, elem_data)
+
+        elec_data = io.BytesIO()
+        self.grid.save_elec_file(elec_data)
+        info = tarfile.TarInfo()
+        info.name = 'grid/elec.dat'
+        info.mtime = time.time()
+        info.size = elec_data.tell()
+        info.type = tarfile.REGTYPE
+        elec_data.seek(0)
+        tar.addfile(info, elec_data)
+
+        crtomo_cfg = io.BytesIO()
+        self.crtomo_cfg.write_to_file(crtomo_cfg)
+        info = tarfile.TarInfo()
+        info.name = 'exe/crtomo.cfg'
+        info.mtime = time.time()
+        info.size = crtomo_cfg.tell()
+        info.type = tarfile.REGTYPE
+        crtomo_cfg.seek(0)
+        tar.addfile(info, crtomo_cfg)
+
+        decouplings = io.BytesIO()
+        self.save_decouplins_file(decouplings)
+        info = tarfile.TarInfo()
+        info.name = 'exe/decouplings.dat'
+        info.mtime = time.time()
+        info.size = crtomo_cfg.tell()
+        info.type = tarfile.REGTYPE
+        decouplings.seek(0)
+        tar.addfile(info, decouplings)
+
+        volt_data = io.BytesIO()
+        self.save_measurements(volt_data)
+        info = tarfile.TarInfo()
+        info.name = 'mod/volt.dat'
+        info.mtime = time.time()
+        info.size = volt_data.tell()
+        info.type = tarfile.REGTYPE
+        volt_data.seek(0)
+        tar.addfile(info, volt_data)
+
+        tar.close()
+        tomodir.seek(0)
+        return tomodir
+
+        # modelling
+        """
+        config/config.dat
+        rho/rho.dat
+
+        exe/crmod.cfg
+        exe/crtomo.cfg
+        exe/crt.noisemod
+        exe/electrode_capactitances.dat
+        exe/decouplings.dat
+        exe/prior.model
+        [TODO]exe/crt.lamnull
+
+        mod/sens/*
+        [TODO] mod/volt.dat
+        [TODO] mod/pot/*
+
+        inv/cjg.ctr
+        inv/coverage.mag
+        coverage.mag.fpi
+        [TODO] inv/ata.diag
+        [TODO] inv/ata_reg.diag
+        [TODO] inv/cov1_m.diag
+        [TODO] inv/cov2_m.diag
+        [TODO] inv/res_m.diag
+        [TODO] inv/eps.ctr
+        [TODO] inv/inv.ctr
+        [TODO] inv/*.model
+        [TODO] inv/*.mag
+        [TODO] inv/*.pha
+        [TODO] inv/run.ctr
+        [TODO] inv/voltXX.dat
+        """
+        # file1 = io.BytesIO()
+        # content_file1 = 'Hi there\nNew line\n'.encode('utf-8')
+        # file1.write(content_file1)
+        # file1.seek(0)
+
+        # tar = tarfile.open(fileobj=target_file, mode='w:xz')
+
+        # info1 = tarfile.TarInfo()
+        # info1.name = 'subdir/File1.txt'
+        # info1.mtime = time.time()
+        # info1.size = len(content_file1)
+        # info1.type = tarfile.REGTYPE
+
+        # tar.addfile(info1, file1)
+        # tar.close()
+
+        # target_file.seek(0)
+        # print('Reading tar file from memory:')
+        # print(
+        #     target_file.read()
+        #     )
+        #     with open('test.tar.xz', 'wb') as fid:
+        #         target_file.seek(0)
+        #             fid.write(target_file.read())
+        #             # extract with tar xvJf test.tar.xz
+
+        #             ## Reading
+        #             tar = tarfile.open(fileobj=target_file, mode='r')
+
     def save_to_tomodir(self, directory, only_for_inversion=False):
         """Save the tomodir instance to a directory structure.
 
         At this point forward modeling results (voltages, potentials and
         sensitivities) will be saved.
 
         Inversion results will, at this stage, not be saved (TODO!!!).
@@ -563,66 +760,72 @@
             * inversion only
             * modeling and inversion
 
         """
         self.create_tomodir(directory)
 
         self.grid.save_elem_file(
-            directory + os.sep + 'grid/elem.dat'
+            directory + os.sep + 'grid' + os.sep + 'elem.dat'
         )
 
         self.grid.save_elec_file(
-            directory + os.sep + 'grid/elec.dat'
+            directory + os.sep + 'grid' + os.sep + 'elec.dat'
         )
 
         # modeling
         if not only_for_inversion:
-            if(self.configs.configs is not None and
+            if (self.configs.configs is not None and
                     self.assignments['forward_model'] is not None):
                 self.configs.write_crmod_config(
-                    directory + os.sep + 'config/config.dat'
+                    directory + os.sep + 'config' + os.sep + 'config.dat'
                 )
 
             if self.assignments['forward_model'] is not None:
                 self.parman.save_to_rho_file(
-                    directory + os.sep + 'rho/rho.dat',
+                    directory + os.sep + 'rho' + os.sep + 'rho.dat',
                     self.assignments['forward_model'][0],
                     self.assignments['forward_model'][1],
                 )
 
             self.crmod_cfg.write_to_file(
-                directory + os.sep + 'exe/crmod.cfg'
+                directory + os.sep + 'exe' + os.sep + 'crmod.cfg'
             )
 
             if self.assignments['sensitivities'] is not None:
                 self._save_sensitivities(
-                    directory + os.sep + 'mod/sens',
+                    directory + os.sep + 'mod' + os.sep + 'sens',
                 )
 
             if self.assignments['potentials'] is not None:
                 self._save_potentials(
-                    directory + os.sep + 'mod/pot',
+                    directory + os.sep + 'mod' + os.sep + 'pot',
                 )
 
         # we always want to save the measurements
-        self.save_measurements(directory + os.sep + 'mod/volt.dat')
+        self.save_measurements(
+            directory + os.sep + 'mod' + os.sep + 'volt.dat'
+        )
 
         # inversion
         self.crtomo_cfg.write_to_file(
-            directory + os.sep + 'exe/crtomo.cfg'
+            directory + os.sep + 'exe' + os.sep + 'crtomo.cfg'
         )
 
         if self.electrode_admittance is not None:
             self._write_el_admittance(directory)
 
         if self.noise_model is not None:
             self.noise_model.write_crt_noisemod(
-                directory + os.sep + 'exe/crt.noisemod'
+                directory + os.sep + 'exe' + os.sep + 'crt.noisemod'
             )
 
+        self.save_decouplins_file(
+            directory + os.sep + 'exe' + os.sep + 'crt.noisemod'
+        )
+
         if not os.path.isdir(directory + os.sep + 'inv'):
             os.makedirs(directory + os.sep + 'inv')
 
         if self.a['prior_model'] is not None:
             self.parman.save_to_rho_file(
                 directory + os.sep + 'inv/prior.model',
                 *self.a['prior_model']
@@ -776,26 +979,26 @@
             self.read_voltages(voltage_file)
 
         sens_files = sorted(glob(
             mod_directory + os.sep + 'sens' + os.sep + 'sens*.dat')
         )
         # check if there are sensitivity files, and that the nr corresponds to
         # the nr of configs
-        if(len(sens_files) > 0 and
+        if (len(sens_files) > 0 and
            len(sens_files) == self.configs.nr_of_configs):
             print('reading sensitivities')
             self._read_sensitivities(mod_directory + os.sep + 'sens')
 
         # same for potentials
         pot_files = sorted(glob(
             mod_directory + os.sep + 'pot' + os.sep + 'pot*.dat')
         )
         # check if there are sensitivity files, and that the nr corresponds to
         # the nr of configs
-        if(len(pot_files) > 0 and
+        if (len(pot_files) > 0 and
            len(pot_files) == self.configs.nr_of_configs):
             print('reading potentials')
             self._read_potentials(mod_directory + os.sep + 'pot')
 
     def _read_sensitivities(self, sens_dir):
         """import sensitivities from a directory
 
@@ -876,15 +1079,15 @@
     def get_sensitivity(self, config_nr):
         """return a sensitivity, as well as corresponding metadata, for a given
         measurement configuration. Indices start at zero.
         """
         if self.assignments['sensitivities'] is None:
             self._check_state()
             if self.can_model:
-                self.model(sensitivities=True)
+                self.model(sensitivities=True, silent=True)
         cids = self.assignments['sensitivities'][config_nr]
         sens_data = [self.parman.parsets[cid] for cid in cids]
         meta_data = [self.parman.metadata[cid] for cid in cids]
 
         return sens_data, meta_data
 
     def plot_sensitivity(self, config_nr=None, sens_data=None,
@@ -928,15 +1131,18 @@
             fig.tight_layout()
             fig.savefig('sens_plot.pdf', bbox_inches='tight')
 
         """
 
         def _rescale_sensitivity(sens_data):
             norm_value = np.abs(sens_data).max()
-            sens_normed = sens_data / norm_value
+            if norm_value == 0:
+                sens_normed = sens_data * 0
+            else:
+                sens_normed = sens_data / norm_value
 
             indices_gt_zero = sens_data > 1e-5
             indices_lt_zero = sens_data < -1e-5
 
             # map all values greater than zero to the range [0.5, 1]
             x = np.log10(sens_normed[indices_gt_zero])
             # log_norm_factor = np.abs(x).max()
@@ -1069,44 +1275,61 @@
         """Import voltages from a volt.dat file
 
         Parameters
         ----------
         voltage_file : str
             Path to volt.dat file
         """
-        with open(voltage_file, 'r') as fid:
-            items_first_line = fid.readline().strip().split(' ')
+        if isinstance(voltage_file, (StringIO, )):
+            fid = voltage_file
+            fid.seek(0)
+        else:
+            fid = open(voltage_file, 'r')
+
+        items_first_line = fid.readline().strip().split(' ')
+
+        # rewind for reading of complete file later on
+        fid.seek(0)
+
+        if int(items_first_line[0]) == 0:
+            # empty file
+            return
 
         individual_errors = False
         if len(items_first_line) == 1:
             # regular volt.dat file
             measurements_raw = np.loadtxt(
-                voltage_file,
+                fid,
                 skiprows=1,
             )
         elif len(items_first_line) == 2 and items_first_line[1] == 'T':
             individual_errors = True
             # Individual data errors
-            with open(voltage_file, 'r') as fid:
-                measurements_raw = np.genfromtxt(
-                    fid,
-                    skip_header=1,
-                    max_rows=int(items_first_line[0]),
-                )
-                (norm_mag, norm_pha) = np.genfromtxt(fid, max_rows=1)
+            measurements_raw = np.genfromtxt(
+                fid,
+                skip_header=1,
+                max_rows=int(items_first_line[0]),
+            )
+            fid.seek(0)
+            (norm_mag, norm_pha) = np.genfromtxt(fid, max_rows=1)
+
+        fid.close()
 
         measurements = np.atleast_2d(measurements_raw)
 
         # extract measurement configurations
         A = (measurements[:, 0] / 1e4).astype(int)
         B = (measurements[:, 0] % 1e4).astype(int)
         M = (measurements[:, 1] / 1e4).astype(int)
         N = (measurements[:, 1] % 1e4).astype(int)
         ABMN = np.vstack((A, B, M, N)).T
 
+        # it may happen that we need to switch signs of measurements
+        switch_signs = []
+
         if self.configs.configs is None:
             self.configs.configs = ABMN
         else:
             # configurations don't match
             if not np.all(ABMN == self.configs.configs):
                 for nr, (old_config, new_config) in enumerate(zip(
                         self.configs.configs, ABMN)):
@@ -1117,37 +1340,47 @@
                     current_electrodes_are_equal = np.all(
                         old_config[0:2] == new_config[0:2]
                     )
                     voltage_electrodes_are_switched = np.all(
                         old_config[2:4] == new_config[4:1:-1]
                     )
 
-                    if(current_electrodes_are_equal and
+                    if (current_electrodes_are_equal and
                        voltage_electrodes_are_switched):
 
                         if len(self.configs.measurements.keys()) > 0:
-                            raise Exception(
-                                'need to switch electrode polarity, but ' +
-                                'there are already measurements stored for ' +
-                                'the old configuration!')
+                            # print('asdasd')
+                            # import IPython
+                            # IPython.embed()
+                            # raise Exception(
+                            #     'need to switch electrode polarity, but ' +
+                            #     'there are already measurements stored for '
+                            #     + 'the old configuration!')
+                            # exit()
+                            switch_signs += [nr]
                         else:
                             # switch M/N in configurations
                             self.configs.configs[nr, :] = new_config
                     else:
                         raise Exception(
                             'There was an error matching configurations of ' +
                             'voltages with configurations already imported'
                         )
 
+        # change sign of R measurements that require it
+        measurements[switch_signs, 2] *= -1
+
         # add measurements to the config instance
         mid_mag = self.configs.add_measurements(measurements[:, 2])
         if measurements.shape[1] >= 4:
             mid_pha = self.configs.add_measurements(measurements[:, 3])
         else:
             mid_pha = None
+        # register those measurements as 'the measurements', used, e.g., for a
+        # subsequent inversion
         self.assignments['measurements'] = [mid_mag, mid_pha]
 
         if individual_errors:
             mid_mag_error = self.configs.add_measurements(measurements[:, 4])
             mid_pha_error = self.configs.add_measurements(measurements[:, 5])
             self.register_data_errors(
                 mid_mag_error, mid_pha_error, norm_mag, norm_pha
@@ -1200,14 +1433,19 @@
               sensitivities=False,
               potentials=False,
               output_directory=None,
               silent=False,
               ):
         """Forward model the tomodir and read in the results
 
+        Note that this function will always do the full modeling. No caching
+        involved.
+
+        Please use .measurements to accessed cached measurements.
+
         Parameters
         ----------
         voltages : bool, optional
             if True, compute voltages for registered quadrupoles. Default: True
         sensitivities : bool, optional
             if True, compute sensitivities for registered quadrupoles. Default:
             False
@@ -1263,49 +1501,75 @@
         ----------
         tempdir : str
             directory which to use as a tomodir
         catch_output : bool, optional
             if True, catch all outputs of the CRTomo call (default: True)
         cores : int, optional
             how many cores to use. (default 2)
+
+        Returns
+        -------
+        success: bool
+            False if an error was detected
+        error_msg: str
+            Error message. None if not error was encountered.
+        output: str
+            Output of the actual CRTomo call
         """
         nr_cores = kwargs.get('cores', 2)
         print('Attempting inversion in directory: {0}'.format(tempdir))
         pwd = os.getcwd()
         os.chdir(tempdir)
 
         self.save_to_tomodir('.')
         os.chdir('exe')
         binary = CRBin.get('CRTomo')
         print('Using binary: {0}'.format(binary))
         print('Calling CRTomo')
         # store env variable
         env_omp = os.environ.get('OMP_NUM_THREADS', '')
         os.environ['OMP_NUM_THREADS'] = '{0}'.format(nr_cores)
+        output = None
         if catch_output:
-            subprocess.check_output(
+            output = subprocess.check_output(
                 binary,
                 shell=True,
                 stderr=subprocess.STDOUT,
             )
         else:
             subprocess.call(
                 binary,
                 shell=True,
             )
+
         # reset environment variable
         os.environ['OMP_NUM_THREADS'] = env_omp
 
-        print('Inversion finished')
-        print('Attempting to import the results')
+        print('Inversion attempt finished')
+        if os.path.isfile('error.dat'):
+            error_message = open('error.dat', 'r').read()
+            success = False
+        else:
+            success = True
+            error_message = None
 
         os.chdir(pwd)
-        self.read_inversion_results(tempdir)
-        print('Statistics of last iteration:')
-        print(self.inv_stats.iloc[-1])
+        if success:
+            print('Attempting to import the results')
+            self.read_inversion_results(tempdir)
+            print('Statistics of last iteration:')
+            print(self.inv_stats.iloc[-1])
+        else:
+            print('There was an error while trying to invert')
+            print('Please see .crtomo_error_msg and .crtomo_output')
+
+        self.crtomo_output = output
+        self.crtomo_error_msg = error_message
+
+        return success
 
     def invert(self, output_directory=None, catch_output=True, **kwargs):
         """Invert this instance, and import the result files
 
         No directories/files will be overwritten. Raise an IOError if the
         output directory exists.
 
@@ -1329,58 +1593,139 @@
         """
         self._check_state()
         if self.can_invert:
             if output_directory is not None:
                 if not os.path.isdir(output_directory):
                     os.makedirs(output_directory)
                     tempdir = output_directory
-                    self._invert(tempdir, catch_output, **kwargs)
+                    success = self._invert(
+                        tempdir, catch_output, **kwargs
+                    )
                 else:
                     raise IOError(
                         'Output directory already exists: {0}'.format(
                             output_directory
                         )
                     )
             else:
                 with tempfile.TemporaryDirectory(dir=self.tempdir) as tempdir:
-                    self._invert(tempdir, catch_output, **kwargs)
+                    success = self._invert(
+                        tempdir, catch_output, **kwargs
+                    )
 
-            return 0
+            if success:
+                return 0
+            else:
+                return 1
         else:
             print(
                 'Sorry, no measurements present, cannot model yet'
             )
             return 1
 
+    def invert_with_crhydra(self):
+        import cr_hydra.settings
+        import crh_add
+        import crh_retrieve
+        import hashlib
+        import platform
+
+        cr_hydra_config, error_code = cr_hydra.settings.get_config(True)
+        if error_code != 0:
+            assert ('No cr_hydra config file found. Cannot proceed')
+        print('cr_hydra config found. Proceeding')
+
+        print('Creating in-memory .tar.xz file of tomodir')
+        tarxz = self.save_to_tarfile()
+
+        # upload the simulation
+        crh_settings = {
+            'datetime_init': '{}'.format(
+                datetime.datetime.now(tz=datetime.timezone.utc)
+            ),
+        }
+        crh_settings['source_computer'] = platform.node()
+        crh_settings['sim_type'] = 'inv'
+        crh_settings['crh_file'] = 'jupyter-lab'
+        crh_settings['username'] = 'crtomo-tools'
+
+        engine = crh_add._get_db_engine(cr_hydra_config)
+        connection = engine.connect()
+
+        archive_file = 'dasdasd'
+        file_id = crh_add._upload_binary_data(
+            tarxz, archive_file, connection
+        )
+        crh_settings['tomodir_unfinished_file'] = file_id
+
+        sim_id = crh_add._upload_simulation(crh_settings, connection)
+        crh_settings['sim_id'] = sim_id
+        crh_add._activate_simulation(sim_id, connection)
+
+        print('cr_hydra simulation id:', sim_id)
+
+        # wait until the inversion finished
+        is_finished = None
+        while is_finished is None:
+            print('Waiting for inversion to finish')
+            time.sleep(5)
+            is_finished = crh_retrieve._is_finished(sim_id, connection)
+        print('Inversion finished')
+
+        print('Downloading')
+        # retrieve the inversion
+        # NOTE: This should be called from crh_retrieve
+        result = connection.execute(
+            crh_retrieve.text(
+                'select hash, data from binary_data where index=:data_id;'
+            ),
+            parameters={
+                'data_id': is_finished,
+            },
+        )
+        assert result.rowcount == 1
+        file_hash, binary_data = result.fetchone()
+
+        # check hash
+        m = hashlib.sha256()
+        m.update(binary_data)
+        assert file_hash == m.hexdigest(), "sha256 does not match"
+
+        result_data = io.BytesIO(bytes(binary_data))
+        with open('output.tar.xz', 'wb') as fid:
+            fid.write(result_data.read())
+
     def read_inversion_results(self, tomodir):
         """Import inversion results from a tomodir into this instance
 
         .. warning::
             This function is not finished yet and does not import ALL crtomo
             information yet.
 
         Parameters
         ----------
         tomodir : str
             Path to tomodir
 
         """
+        print('Reading inversion results')
         self._read_inversion_results(tomodir)
         self._read_inversion_fwd_responses(tomodir)
         self.inv_stats = self._read_inv_ctr(tomodir)
         self._read_resm_m(tomodir)
         self._read_l1_coverage(tomodir)
         self._read_l2_coverage(tomodir)
         self.eps_data = self._read_eps_ctr(tomodir)
         # for simplicity, add configurations to psi data
         has_eps_data = False
         if isinstance(self.eps_data, list):
             if len(self.eps_data) > 1:
                 has_eps_data = True
-        if len(self.configs.configs) > 0 and has_eps_data:
+        if self.configs.configs is not None and len(
+                self.configs.configs) > 0 and has_eps_data:
             for iteration in range(1, len(self.eps_data)):
                 for index, key in enumerate('abmn'):
                     self.eps_data[
                         iteration
                     ][key] = self.configs.configs[:, index]
 
     def _read_inversion_fwd_responses(self, tomodir):
@@ -1437,20 +1782,29 @@
             ) for filename in inv_sig
         ]
 
         if len(pids_sig) > 0:
             pids_cre = [x[0] for x in pids_sig]
             pids_cim = [x[1] for x in pids_sig]
         else:
-            pids_cre = None
-            pids_cim = None
+            if len(pids_pha) > 0:
+                pids_cre = []
+                pids_cim = []
+                for pid_rmag, pid_rpha in zip(pids_mag, pids_pha):
+                    # compute the admittances by hand
+                    impedance = self.parman.parsets[pid_rmag] * np.exp(
+                        1j * self.parman.parsets[pid_rpha] / 1000
+                    )
+                    admittance = 1 / impedance
+                    pids_cre += [self.parman.add_data(np.real(admittance))]
+                    pids_cim += [self.parman.add_data(np.imag(admittance))]
+            else:
+                pids_cre = None
+                pids_cim = None
 
-        # print(pids_sig)
-        # import IPython
-        # IPython.embed()
         self.assignments['inversion'] = {
             'rmag': pids_mag,
             'rpha': pids_pha,
             'cre_cim': pids_sig,
             'cre': pids_cre,
             'cim': pids_cim,
         }
@@ -1696,20 +2050,21 @@
         dfs = []
         # group
         for x in group:
             # print(x)
             if not x[0]:
                 data = [y for y in x[1]]
                 if data[0].startswith('IT') or data[0].startswith('PIT'):
-                    del(data[0])
+                    del (data[0])
                 data[0] = data[0].replace('-Phase (rad)', '-Phase(rad)')
                 tfile = StringIO(''.join(data))
                 df = pd.read_csv(
                     tfile,
-                    delim_whitespace=True,
+                    sep=r'\s+',
+                    # delim_whitespace=True,
                     na_values=['Infinity'],
                 )
                 dfs.append(df)
         return dfs
 
     def _read_inv_ctr(self, tomodir):
         """Read in selected results of the inv.ctr file
@@ -2554,7 +2909,83 @@
             raise Exception('not implemented yet')
 
         # data
         if len(self.a['measurements']) > 1:
             raise Exception('not implemented yet')
 
         return tdm_copy
+
+    def sensitivity_center_of_masses(self, mode='none'):
+        """
+
+        """
+        assert 'sensitivities' in self.a, \
+            "This function requires sensitivities"
+        mag_sens_indices = [
+            self.a['sensitivities'][key][0] for key in sorted(
+                self.a['sensitivities'].keys()
+            )
+        ]
+        coms = self.parman.center_of_mass_value_multiple(
+            mag_sens_indices,
+            mode=mode,
+        )
+        return coms
+
+    def plot_inversion_result_rmag(self, ):
+        """Plot the final inversion results, magnitude-results only
+
+        """
+        assert self.assignments['inversion'] is not None, \
+            'need inversion results to plot anything'
+        pid_mag = self.assignments['inversion']['rmag'][-1]
+
+        fig, ax = plt.subplots(1, 1, figsize=(16 / 2.54, 8 / 2.54))
+
+        self.plot.plot_elements_to_ax(
+            pid_mag,
+            ax=ax,
+            plot_colorbar=True,
+            cblabel=r'$|\rho| [\Omega m]$',
+        )
+
+        fig.tight_layout()
+        return fig, ax
+
+    def plot_decouplings_to_ax(self, ax, plot_transistions=True):
+        """Visualize decouplings. Usually you may want to plot the mesh to this
+        axis first
+
+        Parameters
+        ----------
+        ax: matplotlib.Axes
+            Axis to plot to
+        plot_transistions: bool (True)
+            If True, then also visualize the decoupled transitions
+
+        """
+        if self.decouplings is None:
+            return
+
+        if plot_transistions:
+            centroids = self.grid.get_element_centroids()
+            for A, B, strength in self.decouplings:
+                A = int(A)
+                B = int(B)
+                ax.plot(
+                    [centroids[A][0], centroids[B][0]],
+                    [centroids[A][1], centroids[B][1]],
+                    color='green',
+                    linewidth=1.0 * strength + 0.1,
+                )
+
+        for element1, element2, strength in self.decouplings:
+            element1 = int(element1)
+            element2 = int(element2)
+
+            nodes = np.intersect1d(
+                self.grid.elements[element1],
+                self.grid.elements[element2]
+            )
+            (a_x, a_y) = self.grid.nodes['presort'][nodes[0]][1:3]
+            (b_x, b_y) = self.grid.nodes['presort'][nodes[1]][1:3]
+            ax.plot([a_x, b_x], [a_y, b_y], color='r')
```

### Comparing `crtomo_tools-0.2.2.dev0/setup.py` & `crtomo_tools-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 #!/usr/bin/env python
 from setuptools import setup
 import os
 import glob
 
 scripts = glob.glob('src/*.py')
 
-version_long = '0.2.2-dev'
+version_long = '0.3.0'
 
 # generate entry points
 entry_points = {'console_scripts': []}
 scripts = [os.path.basename(script)[0:-3] for script in glob.glob('src/*.py')]
 for script in scripts:
     print(script)
     entry_points['console_scripts'].append(
         '{0} = {0}:main'.format(script)
     )
 
 # package data
 os.chdir('lib/crtomo')
 package_data = glob.glob('debug_data/*')
+package_data += glob.glob('notebook/manual/html/**', recursive=True)
 os.chdir('../../')
 
 
 if __name__ == '__main__':
     setup(
         name='crtomo_tools',
         version=version_long,
         description='CRTomo Python Toolbox',
         author='Maximilian Weigand',
         license='MIT',
         author_email='mweigand@geo.uni-bonn.de',
         url='https://github.com/geophysics-ubonn/crtomo_tools',
         entry_points=entry_points,
+        # python_requires='>=3.11',
         # entry_points={
         #     'console_scripts': [
         #         'td_test = td_test:main',
         #     ],
         # },
         # package_dir={'': 'src/', 'crtomo': 'lib/crtomo'},
         package_dir={
             '': 'src',
-            'crtomo': 'lib/crtomo'
+            'crtomo': 'lib/crtomo',
+            'crtomo.notebook': 'lib/crtomo/notebook',
         },
         # packages=[''],
         # package_dir={'': 'lib', 'grid_tools': 'src/GRID_TOOLS'},
         # packages=find_packages(),
-        packages=['crtomo', ],
+        packages=['crtomo', 'crtomo.notebook', ],
         package_data={'crtomo': package_data},
         py_modules=scripts,
         # py_modules=[
         #     splitext(basename(i))[0] for i in glob.glob("src/*.py")
         # ]
         # packages=[
         #     'crtomo',
```

### Comparing `crtomo_tools-0.2.2.dev0/src/cr_get_analytical_solutions.py` & `crtomo_tools-0.3.0/src/cr_get_analytical_solutions.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/cr_get_modelling_errors.py` & `crtomo_tools-0.3.0/src/cr_get_modelling_errors.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/cr_trig_create.py` & `crtomo_tools-0.3.0/src/cr_trig_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,22 +113,22 @@
         """
         Return the id of the given point (x,y) tuple.
         """
         print('Checking point', p)
         # TODO: This search loop NEEDS to be replaced with something sane
         index = -1
         for nr, i in enumerate(self.Points):
-            if(np.all(i == p)):
+            if (np.all(i == p)):
                 print('Point already in list at index {0}'.format(nr))
                 if self.Charlengths[nr] > char_length:
                     print('Updating characteristic length')
                     self.Charlengths[nr] = char_length
                 return nr
 
-        if(index == -1):
+        if (index == -1):
             print('adding point:', p)
             self.Points.append(p)
             self.Charlengths.append(char_length)
             return len(self.Points) - 1
 
     def add_boundary(self, p1, p2, btype):
         """
@@ -153,15 +153,15 @@
 
     def is_in(self, search_list, pair):
         """
         If pair is in search_list, return the index. Otherwise return -1
         """
         index = -1
         for nr, i in enumerate(search_list):
-            if(np.all(i == pair)):
+            if (np.all(i == pair)):
                 return nr
         return index
 
     def read_electrodes(self, electrodes):
         """
         Read in electrodes, check if points already exist
         """
@@ -358,15 +358,15 @@
 
             fid.write('\n')
             fid.write(additional_commands)
 
         fid.close()
 
 
-def check_boundaries(boundaries):
+def _check_for_duplicate_boundary_nodes(boundaries):
     # generate a complex number for each (x,y) pair
     xy = boundaries[:, 0] + 1j * boundaries[:, 1]
     """
     # for numpy > 1.9 , use:
     unique_values, indices, indices_rev, counts = np.unique(
         xy,
         return_index=True,
@@ -394,14 +394,36 @@
             print('x y type:')
             print(boundaries[doublet, :])
             print('lines: ')
             print(np.where(indices_rev == doublet)[0])
         raise Exception('Duplicate boundary coordinates found!')
 
 
+def _check_boundary_type_ordering(boundaries):
+    """Check that type 12 boundaries come before type 11 boundaries, and that
+    type 11 and type 12 boundaries are continuous
+    """
+    type_11_indices = np.where(boundaries[:, 2] == 11)[0]
+    type_12_indices = np.where(boundaries[:, 2] == 12)[0]
+
+    if len(type_12_indices):
+        # type 12 should be at the beginning
+        assert 0 in type_12_indices, \
+            "boundaries must begin with type 12 boundaries"
+
+        if len(type_11_indices):
+            assert type_11_indices.min() > type_12_indices.max(), \
+                "type 11 boundaries must come after type 12"
+
+
+def check_boundaries(boundaries):
+    _check_for_duplicate_boundary_nodes(boundaries)
+    _check_boundary_type_ordering(boundaries)
+
+
 def add_stabilizer_nodes(boundaries_raw, electrodes, nr_nodes_between):
     """
     Segmentation of nodes:
         we have the existing nodes
         N.F is the ratio of required nodes and existing nodes
         first, add N nodes to each segment
         then, add one more node to the F first segments
@@ -478,15 +500,15 @@
     os.makedirs(directory)
 
     shutil.copy('electrodes.dat', directory + os.sep + 'electrodes.dat')
     shutil.copy('boundaries.dat', directory + os.sep + 'boundaries.dat')
 
     if os.path.isfile('extra_nodes.dat'):
         shutil.copy('extra_nodes.dat', directory + os.sep + 'extra_nodes.dat')
-    if(os.path.isfile('char_length.dat')):
+    if (os.path.isfile('char_length.dat')):
         shutil.copy('char_length.dat', directory + os.sep + 'char_length.dat')
     if os.path.isfile('extra_lines.dat'):
         shutil.copy('extra_lines.dat',
                     directory + os.sep + 'extra_lines.dat')
     if os.path.isfile('gmsh_commands.dat'):
         shutil.copy('gmsh_commands.dat',
                     directory + os.sep + 'gmsh_commands.dat')
```

### Comparing `crtomo_tools-0.2.2.dev0/src/cr_trig_parse_gmsh.py` & `crtomo_tools-0.3.0/src/cr_trig_parse_gmsh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,84 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 Parse a GMSH mesh and produce a FEM grid for CRMod/CRTomo. This script should
 not be called directly, as it requires the input and output files from
 "cr_trig_create.py".
-
-TODO
-----
-
-* the program at some point looks for nodes on the boundary line. Perhaps some
-  funtions in "grid_extralines_gen_decouplings.py" can be used here (code
-  deduplication and speed improvements)
-
-
 """
-from crtomo.mpl_setup import *
-mpl.rcParams['font.size'] = 6.0
+import time
+import crtomo.mpl
 import numpy as np
 
+plt, mpl = crtomo.mpl.setup()
+mpl.rcParams['font.size'] = 6.0
+
 
 def parse_gmsh(filename, boundary_file):
     """
     Parse a GMSH .msh file and return a dictionary containing the data
     neccessary to create CRTomo grids
     """
     mesh = {}
 
     fid = open(filename, 'r')
     line = fid.readline()
-    while(line):
-        if(line.startswith('$MeshFormat')):
+    while (line):
+        if (line.startswith('$MeshFormat')):
             pass
-        elif(line.startswith('$Nodes')):
+        elif (line.startswith('$Nodes')):
             nodes = []
             line = fid.readline()
             nr_nodes = np.fromstring(line, dtype=int, count=1, sep=r'\n')
             nr_nodes
-            while(line):
+            while (line):
                 line = fid.readline()
-                if(line.startswith('$EndNodes')):
+                if (line.startswith('$EndNodes')):
                     break
                 node = np.fromstring(line, dtype=float, sep=' ')
                 nodes.append(node)
             mesh['nodes'] = nodes
-        elif(line.startswith('$Elements')):
+        elif (line.startswith('$Elements')):
             """
             Create a dictionary with the element types as keys. E.g.:
             elements['15'] provides all elements of type 15 (Points)
             """
             elements = {}
             line = fid.readline()
             nr_elements = np.fromstring(line, dtype=int, count=1, sep=r'\n')
             nr_elements
-            while(line):
+            while (line):
                 line = fid.readline()
-                if(line.startswith('$EndElements')):
+                if (line.startswith('$EndElements')):
                     break
                 element = np.fromstring(line, dtype=int, sep=' ')
                 # el_nr = element[0]
                 el_type = element[1]
                 el_nr_tags = element[2]
                 # el_tags = element[3:3 + el_nr_tags]
                 el_nodes = element[3 + el_nr_tags:]
 
                 # now decide where to put it
                 key = str(el_type)
-                if(key in elements.keys()):
+                if (key in elements.keys()):
                     elements[key].append(el_nodes)
                 else:
                     elements[key] = []
                     elements[key].append(el_nodes)
 
             mesh['elements'] = elements
         line = fid.readline()
 
     fid.close()
 
     # if boundary_file is != None, then sort the lines (element type 1)
     # according to the element types
     boundaries = {}
 
-    if(boundary_file is not None):
+    if (boundary_file is not None):
         # load the original boundary lines
         # it is possible that GMSH added additional nodes on these lines, and
         # that is why we need to find all mesh lines that lie on these original
         # lines.
         bids = np.loadtxt(boundary_file)
 
         for btype in ('12', '11'):
@@ -102,21 +96,21 @@
                 # x1 == x2 ?
                 # split into coordinates
                 ox1 = orig_line[0]
                 ox2 = orig_line[2]
                 oy1 = orig_line[1]
                 oy2 = orig_line[3]
 
-                if(orig_line[0] == orig_line[2]):
+                if (orig_line[0] == orig_line[2]):
                     # special case: we only need to find all lines with x1 ==
                     # x2 == x1_orig and y_min >= y_orig_min and y_max <=
                     # <_orig_max
                     for line in elements['1']:
-                        if(btype == '11'):
-                            if(line[0] == 48 and line[1] == 150):
+                        if (btype == '11'):
+                            if (line[0] == 48 and line[1] == 150):
                                 pass
                                 # print('Find all lines lying on the line: ')
                                 # print('This is the line')
 
                         # it doesn't matter any more to be able to assign x ->
                         # y values. Thus we can sort the y values and just
                         # check
@@ -132,15 +126,15 @@
                             [
                                 mesh['nodes'][line[0] - 1][2],
                                 mesh['nodes'][line[1] - 1][2]
                             ]
                         )
 
                         if np.isclose(x1, x2) and np.isclose(x2, ox1):
-                            if(y1 >= oy1 and y2 <= oy2):
+                            if (y1 >= oy1 and y2 <= oy2):
                                 found_one_line = True
                                 boundaries[btype].append(line)
 
                 else:
                     # print('checking with full line equation')
                     # no vertical line
                     # we need the full check using the line equation
@@ -154,39 +148,39 @@
                         x2 = mesh['nodes'][line[1] - 1][1]
                         y2 = mesh['nodes'][line[1] - 1][2]
 
                         # print(x1, x2, y1, y1)
                         check = False
                         # check if x coordinates of the test line fit in the
                         # original line
-                        if(ox1 < ox2):
-                            if(x1 < x2):
-                                if((np.isclose(x1, ox1) or x1 > ox1) and
+                        if (ox1 < ox2):
+                            if (x1 < x2):
+                                if ((np.isclose(x1, ox1) or x1 > ox1) and
                                    (np.isclose(x2, ox2) or x2 < ox2)):
                                     check = True
                             else:
-                                if((np.isclose(x2, ox1) or x2 >= ox1) and
+                                if ((np.isclose(x2, ox1) or x2 >= ox1) and
                                    (np.isclose(x1, ox2) or x1 <= ox2)):
                                     check = True
                         else:
-                            if(x1 < x2):
-                                if((np.isclose(x1, ox2) or x1 >= ox2) and
+                            if (x1 < x2):
+                                if ((np.isclose(x1, ox2) or x1 >= ox2) and
                                    (np.isclose(x2, ox1) or x2 <= ox1)):
                                     check = True
                             else:
-                                if((np.isclose(x2, ox2) or x2 >= ox2) and
+                                if ((np.isclose(x2, ox2) or x2 >= ox2) and
                                    (np.isclose(x1, ox1) or x1 <= ox1)):
                                     check = True
 
                         # print('boundary check:', check)
-                        if(check):
+                        if (check):
                             # the line lies within the x-range of the orig line
                             ytest1 = slope * x1 + intersect
                             ytest2 = slope * x2 + intersect
-                            if(np.around(ytest1 - y1, 5) == 0 and
+                            if (np.around(ytest1 - y1, 5) == 0 and
                                np.around(ytest2 - y2, 5) == 0):
                                 boundaries[btype].append(line)
                                 # found = True
                                 found_one_line = True
                                 # print('found it new', line)
                 # add a weak check: we need to find at least one line in the
                 # mesh corresponding to this boundary line:
@@ -240,15 +234,15 @@
     tx = nodes[:, 1]
     ty = nodes[:, 2]
 
     # adapt height of plot to size of grid
     tx_size = np.abs(np.max(tx) - np.min(tx))
     ty_size = np.abs(np.max(ty) - np.min(ty))
 
-    if(plot_large):
+    if (plot_large):
         width = 10
     else:
         width = 7
     size_x = width
     size_y = width * (ty_size / tx_size) * 1.5
 
     # plot triangles
@@ -290,15 +284,15 @@
     # plot electrodes
     electrodes = np.loadtxt('../electrode_positions.dat')
     ax.scatter(electrodes[:, 0], electrodes[:, 1], s=30,
                color='blue',
                label='electrodes')
 
     fig.tight_layout()
-    if(plot_large):
+    if (plot_large):
         dpi = 600
     else:
         dpi = 300
     fig.savefig('../../triangle_grid.jpg', dpi=dpi)
 
 
 def get_header(mesh):
@@ -311,36 +305,36 @@
     # compute bandwidth
     bandwidth = -1
     for triangle in mesh['elements']['2']:
         diff1 = abs(triangle[0] - triangle[1])
         diff2 = abs(triangle[0] - triangle[2])
         diff3 = abs(triangle[1] - triangle[2])
         diffm = max(diff1, diff2, diff3)
-        if(diffm > bandwidth):
+        if (diffm > bandwidth):
             bandwidth = diffm
 
     el_infos = []
     # triangles
     for element in ('2',):
         el = mesh['elements'][element]
-        if(element == '2'):
+        if (element == '2'):
             el_type = 3
-        elif(element == '1'):
+        elif (element == '1'):
             el_type = 12  # Neumann
         nr = len(el)
         nr_nodes = len(el[0])
         el_infos.append((el_type, nr, nr_nodes))
 
     # boundary elements
     for btype in ('12', '11'):
-        if(btype in mesh['boundaries']):
+        if (btype in mesh['boundaries']):
             el_type = int(btype)
             nr = len(mesh['boundaries'][btype])
             nr_nodes = 2
-            if(nr > 0):
+            if (nr > 0):
                 nr_types += 1
                 el_infos.append((el_type, nr, nr_nodes))
 
     # now convert to string
     str_header = ''
     for a, b, c in [(nr_all_nodes, nr_types, bandwidth), ] + el_infos:
         str_header = str_header + '{0}  {1} {2}\n'.format(a, b, c)
@@ -361,51 +355,92 @@
     # print('Get elements')
     str_elements = ''
     # triangles
     for element in ('2'):
         el = mesh['elements'][element]
         for item in el:
             # the reverse should ensure counter-clockwise element nodes
-            if(element == '1'):
+            if (element == '1'):
                 # boundary elements
                 lst = item
             else:
                 lst = reversed(item)
 
             for i in lst:
                 str_elements += '{0}  '.format(i)
             str_elements += '\n'
     # boundary elements
     for btype in ('12', '11'):
         for line in mesh['boundaries'][btype]:
             str_elements += '{0} {1}\n'.format(line[0], line[1])
 
-    return(str_elements)
+    return (str_elements)
 
 
-def get_ajd_bound(mesh):
+def get_adj_bound_v1(mesh):
     """
-    Determine triangular elements adjacend to the boundary elements
+    Determine triangular elements adjacent to the boundary elements
     """
-    print('Get elements adjacent to boundaries')
+    print('Get elements adjacent to boundaries V1')
+    start = time.perf_counter()
     boundary_elements = []
     str_adj_boundaries = ''
     # for boundary in mesh['elements']['1']:
     boundaries = mesh['boundaries']['12'] + mesh['boundaries']['11']
     for boundary in boundaries:
         # now find the triangle ('2') with two nodes equal to this boundary
         indices = [nr if (boundary[0] in x and boundary[1] in x) else np.nan
                    for (nr, x) in enumerate(mesh['elements']['2'])]
         indices = np.array(indices)[~np.isnan(indices)]
-        if(len(indices) != 1):
+        # import IPython
+        # IPython.embed()
+        # exit()
+        if (len(indices) != 1):
+            print('More than one neighbour found!')
+        elif (len(indices) == 0):
+            print('No neighbour found!')
+        boundary_elements.append(indices[0])
+        str_adj_boundaries += '{0}\n'.format(int(indices[0]) + 1)
+    end = time.perf_counter()
+    print('Elapsed time: {:.2}s'.format(end - start))
+    return str_adj_boundaries, boundary_elements
+
+
+def get_adj_bound_v2(mesh):
+    """
+    Determine triangular elements adjacent to the boundary elements
+    """
+    print('Get elements adjacent to boundaries V2')
+    start = time.perf_counter()
+    boundary_elements = []
+    str_adj_boundaries = ''
+    # for boundary in mesh['elements']['1']:
+    boundaries = mesh['boundaries']['12'] + mesh['boundaries']['11']
+    elements = np.array(mesh['elements']['2'])
+    for boundary in boundaries:
+        # # now find the triangle ('2') with two nodes equal to this boundary
+        # indices = [nr if (boundary[0] in x and boundary[1] in x) else np.nan
+        #            for (nr, x) in enumerate(mesh['elements']['2'])]
+        # indices = np.array(indices)[~np.isnan(indices)]
+        indices = np.intersect1d(
+            np.where(np.any(elements == boundary[0], axis=1))[0],
+            np.where(np.any(elements == boundary[1], axis=1))[0]
+        )
+
+        # import IPython
+        # IPython.embed()
+        # exit()
+        if (len(indices) != 1):
             print('More than one neighbour found!')
-        elif(len(indices) == 0):
+        elif (len(indices) == 0):
             print('No neighbour found!')
         boundary_elements.append(indices[0])
         str_adj_boundaries += '{0}\n'.format(int(indices[0]) + 1)
+    end = time.perf_counter()
+    print('Elapsed time: {:.2}s'.format(end - start))
     return str_adj_boundaries, boundary_elements
 
 
 def write_elec_file(filename, mesh):
     """
     Read in the electrode positions and return the indices of the electrodes
 
@@ -437,17 +472,23 @@
     3. Elements: Triangles, Boundary elements
     4. Element ids for adjoining boundary elements
     """
 
     str_header = get_header(mesh)
     str_nodes = get_nodes(mesh)
     str_elements = get_elements(mesh)
-    str_adj_boundaries, boundary_elements = get_ajd_bound(mesh)
 
-    crt_mesh = str_header + str_nodes + str_elements + str_adj_boundaries
+    # v1 is slow....
+    # str_adj_boundaries1, boundary_elements1 = get_adj_bound_v1(mesh)
+    str_adj_boundaries2, boundary_elements2 = get_adj_bound_v2(mesh)
+    # import IPython
+    # IPython.embed()
+    # exit()
+
+    crt_mesh = str_header + str_nodes + str_elements + str_adj_boundaries2
 
     fid = open('../elem.dat', 'w')
     fid.write(crt_mesh)
     fid.close()
 
     write_elec_file('../electrode_positions.dat', mesh)
-    debug_plot_mesh(mesh, boundary_elements)
+    debug_plot_mesh(mesh, boundary_elements2)
```

### Comparing `crtomo_tools-0.2.2.dev0/src/crtomo_tools.egg-info/entry_points.txt` & `crtomo_tools-0.3.0/src/crtomo_tools.egg-info/entry_points.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [console_scripts]
 cr_get_analytical_solutions = cr_get_analytical_solutions:main
 cr_get_modelling_errors = cr_get_modelling_errors:main
 cr_trig_create = cr_trig_create:main
 cr_trig_parse_gmsh = cr_trig_parse_gmsh:main
+grid_convert_boundary_to_svg = grid_convert_boundary_to_svg:main
 grid_extralines_gen_decouplings = grid_extralines_gen_decouplings:main
 grid_gen_decouplings = grid_gen_decouplings:main
 grid_gen_depth_decoupling = grid_gen_depth_decoupling:main
 grid_gen_surface_files = grid_gen_surface_files:main
 grid_homogenize = grid_homogenize:main
+grid_parse_svg_to_files = grid_parse_svg_to_files:main
 grid_plot_elem_angles = grid_plot_elem_angles:main
 grid_plot_wireframe = grid_plot_wireframe:main
 grid_rotate = grid_rotate:main
 grid_translate = grid_translate:main
 grid_translate_model = grid_translate_model:main
 sd_plot = sd_plot:main
 sens_center_plot = sens_center_plot:main
@@ -19,9 +21,9 @@
 td_correct_temperature = td_correct_temperature:main
 td_init = td_init:main
 td_plot = td_plot:main
 td_residuals = td_residuals:main
 td_run_all_local = td_run_all_local:main
 td_test = td_test:main
 volt_correct_temperature = volt_correct_temperature:main
+volt_filter_using_residuals = volt_filter_using_residuals:main
 volt_histogram = volt_histogram:main
-
```

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_extralines_gen_decouplings.py` & `crtomo_tools-0.3.0/src/grid_extralines_gen_decouplings.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,101 +20,192 @@
 broadcasting rules.
 
 Examples
 --------
 
     # enter the output directory of cr_trig_create.py
     grid_extralines_gen_decouplings.py
-    # this create the file decouplings.dat
 
+    # this creates the file decouplings.dat
     grid_extralines_gen_decouplings.py --plot_node_nrs --plot_elm_nrs
 
 """
+import sys
 import os
-from optparse import OptionParser
+# from optparse import OptionParser
+from argparse import ArgumentParser
 import numpy as np
-from crtomo.mpl_setup import *
+import crtomo.mpl
 import crtomo.grid as CRGrid
 
+import matplotlib.pylab as plt
+import matplotlib as mpl
 
-def handle_cmd_options():
-    parser = OptionParser()
-    parser.add_option(
+import IPython
+IPython
+
+crtomo.mpl.setup()
+
+
+def handle_cmd_options_v2():
+    parser = ArgumentParser()
+    parser.add_argument(
         '-e',
         "--elem",
         dest="elem_file",
-        type="string",
+        type=str,
         help="elem.dat file (default: elem.dat)",
         default="elem.dat",
     )
-    parser.add_option(
+    parser.add_argument(
         "--eps",
         dest="eps",
-        type="float",
+        type=float,
         help="User override for distance eps",
         default=None,
     )
-    parser.add_option(
+    parser.add_argument(
+        '-w',
         "--eta",
-        action="store",
+        action="append",
         dest="eta",
-        type="float",
-        help="User override for coupling coefficient",
-        default=0.001,
+        type=float,
+        help="User override for coupling coefficient (default: 0)",
+        # default=0.0,
     )
-    parser.add_option(
+    parser.add_argument(
         '-l',
         "--linefile",
-        dest="linefile",
-        help="Line file (default: extra_lines.dat)",
-        default='extra_lines.dat',
+        # dest="linefile",
+        action='append',
+        # type=str,
+        # help="Line file (default: extra_lines.dat)",
+        # default='extra_lines.dat',
     )
-    parser.add_option(
+    parser.add_argument(
         "-o",
         "--output",
         dest="output",
         help="Output file (default: decouplings.dat)",
         metavar="FILE", default="decouplings.dat",
     )
 
-    parser.add_option(
+    parser.add_argument(
+        '-linenr',
         "--ln",
         action="store",
         dest="line_nr",
-        type="int",
+        type=int,
         help="Process only one line with index N (zero indexed)",
         default=None,
     )
 
-    parser.add_option(
+    parser.add_argument(
         '--debug_plot',
         action='store_true',
         dest='debug_plot',
         default=True,
         help='plot a debug plot',
     )
 
-    parser.add_option(
+    parser.add_argument(
         '--plot_node_nrs',
         action='store_true',
         dest='plot_node_nrs',
         default=False,
         help='plot node numbers in the debug plot. default: False',
     )
 
-    parser.add_option(
+    parser.add_argument(
         '--plot_elm_nrs',
         action='store_true',
         dest='plot_elm_nrs',
         default=False,
         help='plot elements numbers in the debug plot. default: False',
     )
 
-    (options, args) = parser.parse_args()
-    return options
+    args = parser.parse_args()
+    return args
+
+
+# def handle_cmd_options():
+#     parser = OptionParser()
+#     parser.add_option(
+#         '-e',
+#         "--elem",
+#         dest="elem_file",
+#         type="string",
+#         help="elem.dat file (default: elem.dat)",
+#         default="elem.dat",
+#     )
+#     parser.add_option(
+#         "--eps",
+#         dest="eps",
+#         type="float",
+#         help="User override for distance eps",
+#         default=None,
+#     )
+#     parser.add_option(
+#         "--eta",
+#         action="store",
+#         dest="eta",
+#         type="float",
+#         help="User override for coupling coefficient (default: 0)",
+#         default=0,
+#     )
+#     parser.add_option(
+#         '-l',
+#         "--linefile",
+#         dest="linefile",
+#         help="Line file (default: extra_lines.dat)",
+#         default='extra_lines.dat',
+#     )
+#     parser.add_option(
+#         "-o",
+#         "--output",
+#         dest="output",
+#         help="Output file (default: decouplings.dat)",
+#         metavar="FILE", default="decouplings.dat",
+#     )
+
+#     parser.add_option(
+#         "--ln",
+#         action="store",
+#         dest="line_nr",
+#         type="int",
+#         help="Process only one line with index N (zero indexed)",
+#         default=None,
+#     )
+
+#     parser.add_option(
+#         '--debug_plot',
+#         action='store_true',
+#         dest='debug_plot',
+#         default=True,
+#         help='plot a debug plot',
+#     )
+
+#     parser.add_option(
+#         '--plot_node_nrs',
+#         action='store_true',
+#         dest='plot_node_nrs',
+#         default=False,
+#         help='plot node numbers in the debug plot. default: False',
+#     )
+
+#     parser.add_option(
+#         '--plot_elm_nrs',
+#         action='store_true',
+#         dest='plot_elm_nrs',
+#         default=False,
+#         help='plot elements numbers in the debug plot. default: False',
+#     )
+
+#     (options, args) = parser.parse_args()
+#     return options
 
 
 def line_line_intersect(x, y):
     """Compute the intersection point of two lines
 
     Parameters
     ----------
@@ -198,15 +289,15 @@
             index += 1
         ax.plot(x, y)
         ax.set_aspect('equal')
     return dist
 
 
 def get_decouplings_for_line(grid, line, settings, fids=None):
-    """Compute the element pairs for regulazisation decoupling, given a grid
+    """Compute the element pairs for regularisation decoupling, given a grid
     object and a line, denoted by start and end coordinates, in the grid.
 
     Parameters
     ----------
     grid: a crtomo.grid.crt_grid object
     line: np.array/list with 4 entries: x1, y1, x2, x2, denoting start and end
           point
@@ -322,15 +413,23 @@
             pass
             print('No neighbors found. Strange...')
 
     return np.array(neighbors)
 
 
 def check_options(options):
-    for filename in (options.elem_file, options.linefile):
+    if options.linefile is None:
+        options.linefile = ['extra_lines.dat', ]
+    if options.eta is None:
+        options.eta = [0.0, ]
+
+    assert len(options.linefile) == len(options.eta), \
+        "require same number of --linefile and --eta parameters"
+
+    for filename in [options.elem_file, ] + options.linefile:
         if not os.path.isfile(filename):
             raise IOError('File not found: {0}'.format(filename))
 
 
 def debug_plot(grid, extra_lines, decoupling_elements, options,):
     print('Creating debug plot...')
     fig, ax = plt.subplots(1, 1, figsize=(10, 10))
@@ -380,15 +479,15 @@
         z = grid.nodes['presort'][ints, 2]
 
         ax.plot(
             x,
             z,
             '.-',
             color='r',
-            linestyle='dashed',
+            # linestyle='dashed',
             label=label,
         )
         label = ''
 
     # plot search nodes
     nodes = np.loadtxt('debug_search_nodes.dat')
     ax.scatter(
@@ -453,62 +552,77 @@
     )
     fig.subplots_adjust(bottom=0.1)
 
     fig.savefig('debug_plot_decoupling.png', dpi=300, bbox_inches='tight')
 
 
 def main():
-    options = handle_cmd_options()
+    # options = handle_cmd_options()
+    options = handle_cmd_options_v2()
+
     check_options(options)
+    # import IPython
+    # IPython.embed()
+    # exit()
     grid = CRGrid.crt_grid()
     grid.load_elem_file(options.elem_file)
 
-    extra_lines = np.atleast_2d(np.loadtxt(options.linefile))
-
     fids = []
     fids.append(
         open('debug_search_nodes.dat', 'wb')
     )
     fids.append(
         open('debug_dist.dat', 'wb')
     )
     neighbors = None
-    if options.line_nr is None:
-        lines = extra_lines
-    else:
-        print('processing only line: {0}'.format(options.line_nr))
-        lines = (extra_lines[options.line_nr], )
-    for line in lines:
-        data = get_decouplings_for_line(
-            grid,
-            line,
-            {
-                'eps': options.eps,
-                'eta': options.eta,
-            },
-            fids
-        )
-        if neighbors is None:
-            neighbors = data
+
+    for linefile, eta in zip(options.linefile, options.eta):
+        extra_lines = np.atleast_2d(np.loadtxt(linefile))
+
+        if options.line_nr is None:
+            lines = extra_lines
         else:
-            try:
-                neighbors = np.vstack(
-                    (neighbors, data)
-                )
-            except:
-                import IPython
-                IPython.embed()
+            print('processing only line: {0}'.format(options.line_nr))
+            lines = (extra_lines[options.line_nr], )
+        for line in lines:
+            data = get_decouplings_for_line(
+                grid,
+                line,
+                {
+                    'eps': options.eps,
+                    'eta': eta,
+                },
+                fids
+            )
+            if neighbors is None:
+                neighbors = data
+            else:
+                #     neighbors = np.vstack(
+                #         (neighbors, data)
+                #     )
+
+                try:
+                    if data.size > 0:
+                        neighbors = np.vstack(
+                            (neighbors, data)
+                        )
+                except Exception as e:
+                    print('Exception')
+                    print(e)
+                    print(data)
+                    import IPython
+                    IPython.embed()
 
     for fid in fids:
         fid.close()
 
     with open(options.output, 'w') as fid:
         fid.write('{0}\n'.format(neighbors.shape[0]))
     with open(options.output, 'ab') as fid:
-        np.savetxt(fid, np.array(neighbors), fmt='%i %i %.2f')
+        np.savetxt(fid, np.array(neighbors), fmt='%i %i %.3f')
 
     if options.debug_plot:
         debug_plot(
             grid=grid,
             extra_lines=extra_lines,
             decoupling_elements=np.array(neighbors),
             options=options,
```

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_gen_decouplings.py` & `crtomo_tools-0.3.0/src/grid_gen_decouplings.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_gen_depth_decoupling.py` & `crtomo_tools-0.3.0/src/grid_gen_depth_decoupling.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_gen_surface_files.py` & `crtomo_tools-0.3.0/src/grid_gen_surface_files.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_homogenize.py` & `crtomo_tools-0.3.0/src/grid_homogenize.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_plot_elem_angles.py` & `crtomo_tools-0.3.0/src/grid_plot_elem_angles.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_plot_wireframe.py` & `crtomo_tools-0.3.0/src/grid_plot_wireframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from optparse import OptionParser
 import numpy as np
 from crtomo.mpl_setup import *
 import crtomo.grid as CRGrid
 
 # # environment variables
 #
-node_mark_size = float(os.environ.get('MARK_SIZE', 1.0))
+node_mark_size = float(os.environ.get('MARK_SIZE', 30.0))
 # line width
 cell_mark_size = float(os.environ.get('MARK_WIDTH', 1.0))
 cell_line_width = float(os.environ.get('CELL_WIDTH', 1.0))
 # electrode size
 elec_size = float(os.environ.get('ELEC_SIZE', 30.0))
 dpi = int(os.environ.get('DPI', 300))
```

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_rotate.py` & `crtomo_tools-0.3.0/src/grid_rotate.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_translate.py` & `crtomo_tools-0.3.0/src/grid_translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,19 @@
 
 def main():
     options = handle_cmd_options()
     # put in dummy center coordinates
     options.center_x = 0.0
     options.center_y = 0.0
 
-    grid = CRGrid.crt_grid()
-    grid.load_elem_file(options.elem_file)
+    grid = CRGrid.crt_grid(
+        elem_file=options.elem_file,
+        elec_file='elec.dat'
+    )
+    # grid.load_elem_file(options.elem_file)
     rotated_nodes = translate_nodes(
         grid.nodes['raw'][:, 1:3],
         options.dx,
         options.dz
     )
     grid.nodes['raw'][:, 1:3] = rotated_nodes
     grid.save_elem_file(options.output)
```

### Comparing `crtomo_tools-0.2.2.dev0/src/grid_translate_model.py` & `crtomo_tools-0.3.0/src/grid_translate_model.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/sd_plot.py` & `crtomo_tools-0.3.0/src/sd_plot.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/sens_center_plot.py` & `crtomo_tools-0.3.0/src/sens_center_plot.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/td_clean.py` & `crtomo_tools-0.3.0/src/td_clean.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/td_correct_temperature.py` & `crtomo_tools-0.3.0/src/td_correct_temperature.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/td_init.py` & `crtomo_tools-0.3.0/src/td_init.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/td_plot.py` & `crtomo_tools-0.3.0/src/td_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,19 @@
                       default=2,
                       )
     parser.add_option("--cmaglin",
                       action="store_true",
                       dest="cmaglin",
                       help="linear colorbar for magnitude",
                       )
+    parser.add_option("--crholin",
+                      action="store_true",
+                      dest="crholin",
+                      help="linear colorbar for fwd model magnitude",
+                      )
     # geometric options
     parser.add_option('-x',
                       '--xmin',
                       dest='xmin',
                       help='Minium X range',
                       type='float',
                       )
@@ -234,20 +239,20 @@
 def read_iter(use_fpi):
     '''Return the path to the final .mag file either for the complex or the fpi
     inversion.
     '''
     filename_rhosuffix = 'exe/inv.lastmod_rho'
     filename = 'exe/inv.lastmod'
     # filename HAS to exist. Otherwise the inversion was not finished
-    if(not os.path.isfile(filename)):
+    if (not os.path.isfile(filename)):
         print('Inversion was not finished! No last iteration found.')
         return 0
 
-    if(use_fpi is True):
-        if(os.path.isfile(filename_rhosuffix)):
+    if (use_fpi is True):
+        if (os.path.isfile(filename_rhosuffix)):
             filename = filename_rhosuffix
 
     linestring = open(filename, 'r').readline().strip()
     linestring = linestring.replace('\n', '')
     linestring = linestring.replace('../', '')
     return linestring
 
@@ -293,17 +298,17 @@
 
     return files, dtype
 
 
 def read_datafiles(files, dtype, column):
     '''Load the datafiles and return cov, mag, phase and fpi phase values.
     '''
-    mag = []
-    pha = []
-    pha_fpi = []
+    mag = None
+    pha = None
+    pha_fpi = None
     for filename, filetype in zip(files, dtype):
         if filetype == 'cov':
             cov = load_cov(filename)
         elif filetype == 'mag':
             mag = load_rho(filename, column)
         elif filetype == 'pha':
             pha = load_rho(filename, 2)
@@ -593,15 +598,15 @@
     cov_file = 'inv/coverage.mag'
     if not os.path.isfile(cov_file):
         return None, plotman
 
     abscov = np.abs(load_cov(cov_file))
 
     if alpha_cov:
-        normcov = np.divide(abscov, 2.5)
+        normcov = np.divide(abscov, 3)
         normcov[np.where(normcov > 1)] = 1
         mask = np.subtract(1, normcov)
         alpha = plotman.parman.add_data(mask)
     else:
         alpha = plotman.parman.add_data(np.ones(len(abscov)))
     return alpha, plotman
 
@@ -747,23 +752,23 @@
     '''
     if len(mag) == 0:
         mag = np.ones(plotman.grid.nr_of_elements) * np.nan
     if cov is None:
         cov = np.ones_like(mag) * np.nan
 
     magunit = 'log_rho'
-    if not pha == []:
+    if pha is not None:
         [real, imag] = calc_complex(mag, pha)
         if options.c_in_log:
             real = np.log10(real)
             with np.errstate(divide='ignore'):
                 imag = np.log10(imag)
             imag[np.isinf(imag)] = np.nan
 
-        if not pha_fpi == []:
+        if pha_fpi is not None:
             [real_fpi, imag_fpi] = calc_complex(mag, pha_fpi)
             if options.cmaglin:
                 mag = np.power(10, mag)
                 magunit = 'rho'
             if options.c_in_log:
                 real_fpi = np.log10(real_fpi)
                 with np.errstate(divide='ignore'):
@@ -801,15 +806,18 @@
                      'jet_r', 'jet_r', 'plasma_r',
                      'jet_r', 'jet_r', 'plasma_r']
             saves = ['rho', 'cov',
                      'phi', 'real', 'imag',
                      'fpi_phi', 'fpi_real', 'fpi_imag']
         else:
             if options.cmaglin:
+                print('Cmaglin')
+                print(mag, mag.min(), mag.max())
                 mag = np.power(10, mag)
+                print('after', mag.min(), mag.max())
                 magunit = 'rho'
             data = np.column_stack((mag, cov, pha, real, imag))
             titles = ['Magnitude', 'Coverage',
                       'Phase', 'Real Part', 'Imaginary Part']
             unites = [magunit, 'cov',
                       'phi', 'log_real', 'log_imag']
             vmins = [options.mag_vmin, options.cov_vmin,
@@ -826,47 +834,54 @@
         unites = [magunit, 'cov']
         vmins = [options.mag_vmin, options.cov_vmin]
         vmaxs = [options.mag_vmax, options.cov_vmax]
         cmaps = ['jet', 'GnBu']
         saves = ['rho', 'cov']
     try:
         mod_rho = np.genfromtxt('rho/rho.dat', skip_header=1, usecols=([0]))
+        if not options.crholin:
+            mod_rho = np.log10(mod_rho)
         mod_pha = np.genfromtxt('rho/rho.dat', skip_header=1, usecols=([1]))
         if data.size == 0:
             data = np.column_stack((mod_rho, mod_pha))
         else:
             data = np.column_stack((data, mod_rho, mod_pha))
         titles.append('Model')
         titles.append('Model')
-        unites.append('rho')
+        if not options.crholin:
+            unites.append('log_rho')
+        else:
+            unites.append('rho')
         unites.append('phi')
         vmins.append(options.mag_vmin)
         vmins.append(options.pha_vmin)
         vmaxs.append(options.mag_vmax)
         vmaxs.append(options.pha_vmax)
         cmaps.append('jet')
         cmaps.append('plasma')
         saves.append('rhomod')
         saves.append('phamod')
-    except Exception:
+    except Exception as e:
+        print(e)
+        print('BAD ERROR')
         pass
 
     for datum, title, unit, vmin, vmax, cm, save in zip(
             np.transpose(data), titles, unites, vmins, vmaxs, cmaps, saves):
         if len(datum) == 0:
             continue
         if np.all(np.isnan(datum)):
             continue
         # print(save)
         # if save == 'fpi_imag':
         #     import IPython
         #     IPython.embed()
-        if save == 'rho' and options.cmaglin:
-            datum = np.power(10, datum)
-            unit = 'rho'
+        # if save == 'rho' and options.cmaglin:
+        #     datum = np.power(10, datum)
+        #     unit = 'rho'
 
         sizex, sizez = getfigsize(plotman)
         f, ax = plt.subplots(1, figsize=(sizex, sizez))
         cid = plotman.parman.add_data(datum)
         # handle options
         cblabel = units.get_label(unit)
         if options.title is not None:
```

### Comparing `crtomo_tools-0.2.2.dev0/src/td_residuals.py` & `crtomo_tools-0.3.0/src/td_residuals.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import numpy as np
 import os
 import matplotlib.pyplot as plt
 import matplotlib as mpl
+import pandas as pd
 # from mpl_toolkits.axes_grid1 import AxesGrid
 
 
 def shiftedColorMap(cmap, start=0, midpoint=0.5, stop=1.0, name='shiftedcmap'):
     '''
     Function to offset the "center" of a colormap. Useful for
     data with a negative min and positive max and you want the
@@ -51,26 +52,27 @@
 
         cdict['red'].append((si, r, r))
         cdict['green'].append((si, g, g))
         cdict['blue'].append((si, b, b))
         cdict['alpha'].append((si, a, a))
 
     newcmap = mpl.colors.LinearSegmentedColormap(name, cdict)
-    plt.register_cmap(cmap=newcmap)
+
+    # plt.register_cmap(cmap=newcmap)
 
     return newcmap
 
 
 def read_lastmodfile(directory):
     """
     Return the number of the final inversion result.
     """
     filename = '{0}/exe/inv.lastmod'.format(directory)
     # filename HAS to exist. Otherwise the inversion was not finished
-    if(not os.path.isfile(filename)):
+    if not os.path.isfile(filename):
         return None
 
     linestring = open(filename, 'r').readline().strip()
     linestring = linestring.replace("\n", '')
     linestring = linestring.replace(".mag", '')
     linestring = linestring.replace("../inv/rho", '')
     return linestring
@@ -86,69 +88,82 @@
     content = np.loadtxt('inv/volt' + num + '.dat', skiprows=1)
     return content  # , array
 
 
 def main():
     data = open_data()
     inv = open_inv()
-    if(
-            (data[:, 0].all() - inv[:, 0].all() == 0) and
-            (data[:, 1].all() - inv[:, 1].all() == 0)):
+    # import IPython
+    # IPython.embed()
+    ab_are_equal = (data[:, 0] - inv[:, 0] == 0).all()
+    mn_are_equal = (data[:, 1] - inv[:, 1] == 0).all()
+    if ab_are_equal and mn_are_equal:
         print('Dipoles are equal')
-        source = []
-        receiver = []
-        for AB, MN, rho, pha in data:
-            s = ((AB % 1e4) - (round(AB / 1e4))) / 2 + round(AB / 1e4)
-            source.append(s)
-            r = ((round(MN / 1e4)) - (MN % 1e4)) / 2 + (MN % 1e4)
-            receiver.append(r)
-        mag_res = np.column_stack(
-            (source, receiver, data[:, 2] - inv[:, 2], )
-        )
+        rdata = pd.DataFrame((data[:, 0] / 1e4).astype(int), columns=['a', ])
+        rdata['b'] = (data[:, 0] % 1e4).astype(int)
+        rdata['m'] = (data[:, 1] / 1e4).astype(int)
+        rdata['n'] = (data[:, 1] % 1e4).astype(int)
+        rdata['ab_pos'] = (rdata['b'] - rdata['a']) / 2 + rdata['a']
+        rdata['mn_pos'] = (rdata['n'] - rdata['m']) / 2 + rdata['m']
+        rdata['diff_res'] = data[:, 2] - inv[:, 2]
+        rdata['diff_pha'] = data[:, 3] - inv[:, 3]
+        rdata['diff_res_abs'] = np.abs(rdata['diff_res'])
+        rdata['diff_pha_abs'] = np.abs(rdata['diff_pha'])
+
+        # import IPython
+        # IPython.embed()
 
-        vmin = min(mag_res[:, 2])
-        vmax = max(mag_res[:, 2])
+        vmin = min(rdata['diff_res'])
+        vmax = max(rdata['diff_res'])
         shrunk_cmap = shiftedColorMap(
-            mpl.cm.coolwarm, midpoint=1 - vmax / (vmax + abs(vmin))
+            mpl.cm.coolwarm,
+            midpoint=1 - vmax / (vmax + abs(vmin)),
+            name='map1',
         )
         fig, ax = plt.subplots()
-        sc = ax.scatter(mag_res[:, 0],
-                        mag_res[:, 1],
-                        c=mag_res[:, 2],
-                        # s=7,
-                        edgecolor='k',
-                        linewidth=.1,
-                        cmap=shrunk_cmap
-                        )
+        sc = ax.scatter(
+            rdata['ab_pos'],
+            rdata['mn_pos'],
+            c=rdata['diff_res'],
+            # s=7,
+            edgecolor='k',
+            linewidth=.1,
+            cmap=shrunk_cmap
+        )
         plt.colorbar(sc)
         ax.set_xlabel('source position [m]')
         ax.set_ylabel('receiver position [m]')
         fig.tight_layout()
         fig.savefig('residuals_mag.png', dpi=300)
-        pha_res = np.column_stack(
-            (source, receiver, data[:, 3] - inv[:, 3], )
-        )
 
-        vmin = min(pha_res[:, 2])
-        vmax = max(pha_res[:, 2])
+        vmin = min(rdata['diff_pha'])
+        vmax = max(rdata['diff_pha'])
         shrunk_cmap = shiftedColorMap(
-            mpl.cm.coolwarm, midpoint=1 - vmax / (vmax + abs(vmin))
+            mpl.cm.coolwarm, midpoint=1 - vmax / (vmax + abs(vmin)),
+            name='map2',
         )
         fig, ax = plt.subplots()
         sc = ax.scatter(
-            pha_res[:, 0],
-            pha_res[:, 1],
-            c=pha_res[:, 2],
+            rdata['ab_pos'],
+            rdata['mn_pos'],
+            c=rdata['diff_pha'],
             # s=7,
             edgecolor='k',
             linewidth=.1,
             cmap=shrunk_cmap
         )
         plt.colorbar(sc)
         ax.set_xlabel('source position [m]')
         ax.set_ylabel('receiver position [m]')
         fig.tight_layout()
         fig.savefig('residuals_pha.png', dpi=300)
 
+        # save residuals to file
+        rdata.sort_values('diff_res_abs', ascending=False).to_csv(
+            'residuals.csv',
+            sep='\t',
+            float_format='%.3f',
+        )
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `crtomo_tools-0.2.2.dev0/src/td_run_all_local.py` & `crtomo_tools-0.3.0/src/td_run_all_local.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/td_test.py` & `crtomo_tools-0.3.0/src/td_test.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/volt_correct_temperature.py` & `crtomo_tools-0.3.0/src/volt_correct_temperature.py`

 * *Files identical despite different names*

### Comparing `crtomo_tools-0.2.2.dev0/src/volt_histogram.py` & `crtomo_tools-0.3.0/src/volt_histogram.py`

 * *Files identical despite different names*

