# Comparing `tmp/pyegeria-0.3.4.tar.gz` & `tmp/pyegeria-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegeria-0.3.4.tar", last modified: Thu Apr 11 21:14:10 2024, max compression
+gzip compressed data, was "pyegeria-0.3.5.tar", last modified: Mon Apr 29 05:50:14 2024, max compression
```

## Comparing `pyegeria-0.3.4.tar` & `pyegeria-0.3.5.tar`

### file list

```diff
@@ -1,87 +1,110 @@
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.618025 pyegeria-0.3.4/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.4/LICENSE
--rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-11 15:17:10.000000 pyegeria-0.3.4/MANIFEST.in
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-11 21:14:10.617867 pyegeria-0.3.4/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.4/README.md
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.610000 pyegeria-0.3.4/examples/
--rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-11 16:00:57.000000 pyegeria-0.3.4/examples/.DS_Store
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.611527 pyegeria-0.3.4/examples/Coco_config/
--rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-11 14:15:42.000000 pyegeria-0.3.4/examples/Coco_config/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS1.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS2.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS3.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS4.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS5.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS6.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDSx.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoView1.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_exchangeDL01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_governDL01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_monitorDev01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_monitorGov01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-11 14:25:11.000000 pyegeria-0.3.4/examples/Coco_config/globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-11 15:17:10.000000 pyegeria-0.3.4/examples/__init__.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.611632 pyegeria-0.3.4/examples/__pycache__/
--rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.4/examples/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.613196 pyegeria-0.3.4/examples/widgets/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1289 2024-04-11 02:07:05.000000 pyegeria-0.3.4/examples/widgets/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-11 14:02:30.000000 pyegeria-0.3.4/examples/widgets/__init__.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.613514 pyegeria-0.3.4/examples/widgets/__pycache__/
--rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.4/examples/widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.4/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3231 2024-04-11 16:57:09.000000 pyegeria-0.3.4/examples/widgets/coco_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5206 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/engine_action_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5185 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/find_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/glossary_view.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/gov_engine_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/integration_daemon_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3578 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/list_asset_types.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3740 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/multi-server_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-11 17:41:52.000000 pyegeria-0.3.4/examples/widgets/my_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/open_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/server_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-11 16:52:45.000000 pyegeria-0.3.4/examples/widgets/server_status_widget.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4599 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/view_my_profile.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-04-11 15:33:29.000000 pyegeria-0.3.4/pyproject.toml
--rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-11 21:14:10.618059 pyegeria-0.3.4/setup.cfg
--rw-r--r--   0 dwolfson   (501) staff       (20)     2102 2024-04-11 17:56:25.000000 pyegeria-0.3.4/setup.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.609280 pyegeria-0.3.4/src/
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.615674 pyegeria-0.3.4/src/pyegeria/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1612 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/_exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.4/src/pyegeria/_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/_validators.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   100106 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    93138 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-10 19:14:09.000000 pyegeria-0.3.4/src/pyegeria/exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/governance_author.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42441 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8775 2024-04-11 18:20:16.000000 pyegeria-0.3.4/src/pyegeria/registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/utils.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.617615 pyegeria-0.3.4/src/pyegeria.egg-info/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     2493 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/SOURCES.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/dependency_links.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/requires.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/top_level.txt
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.617474 pyegeria-0.3.4/tests/
--rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-10 19:14:09.000000 pyegeria-0.3.4/tests/test_automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-10 19:14:09.000000 pyegeria-0.3.4/tests/test_automated_curation_omvs_cray.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.4/tests/test_full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     9625 2024-04-11 17:35:38.000000 pyegeria-0.3.4/tests/test_my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    40081 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4727 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_util_exp.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_validators.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.566147 pyegeria-0.3.5/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.5/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-12 00:32:44.000000 pyegeria-0.3.5/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-29 05:50:14.565961 pyegeria-0.3.5/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.5/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.547383 pyegeria-0.3.5/examples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:37:23.000000 pyegeria-0.3.5/examples/.DS_Store
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.550418 pyegeria-0.3.5/examples/Coco_config/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-12 00:25:29.000000 pyegeria-0.3.5/examples/Coco_config/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS2.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS3.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS4.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS5.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS6.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDSx.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoView1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_exchangeDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_governDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_monitorDev01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_monitorGov01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-12 00:25:29.000000 pyegeria-0.3.5/examples/Coco_config/globals.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.550915 pyegeria-0.3.5/examples/Doc_Samples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11865 2024-04-18 16:25:08.000000 pyegeria-0.3.5/examples/Doc_Samples/Create_Collection_Sample.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5049 2024-04-28 23:10:47.000000 pyegeria-0.3.5/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.551178 pyegeria-0.3.5/examples/Jupyter Notebooks/
+-rw-r--r--   0 dwolfson   (501) staff       (20)   118151 2024-04-29 01:16:20.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/P-egeria-server-config.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)      170 2024-04-29 01:25:02.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.552255 pyegeria-0.3.5/examples/Jupyter Notebooks/common/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2914 2024-04-19 21:30:39.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/P-environment-check.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)      408 2024-03-20 02:16:23.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   276801 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/common-functions.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1449 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/environment-check.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     7842 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/globals.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5900 2024-04-19 21:30:39.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5849 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/orig_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.552353 pyegeria-0.3.5/examples/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.5/examples/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.556100 pyegeria-0.3.5/examples/widgets/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:47:25.000000 pyegeria-0.3.5/examples/widgets/.DS_Store
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1696 2024-04-29 00:22:17.000000 pyegeria-0.3.5/examples/widgets/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-12 00:25:29.000000 pyegeria-0.3.5/examples/widgets/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.556466 pyegeria-0.3.5/examples/widgets/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.5/examples/widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.5/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3157 2024-04-29 00:14:47.000000 pyegeria-0.3.5/examples/widgets/coco_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3642 2024-04-18 19:49:26.000000 pyegeria-0.3.5/examples/widgets/collection_viewer.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5206 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/engine_action_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5185 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/find_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4947 2024-04-25 14:18:41.000000 pyegeria-0.3.5/examples/widgets/get_relationship_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5299 2024-04-24 01:14:00.000000 pyegeria-0.3.5/examples/widgets/get_valid_metadata_values.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/glossary_view.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/gov_engine_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/integration_daemon_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3578 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/list_asset_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3704 2024-04-18 13:42:39.000000 pyegeria-0.3.5/examples/widgets/multi-server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/my_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/open_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5448 2024-04-24 21:32:52.000000 pyegeria-0.3.5/examples/widgets/project_list_viewer.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/server_status_widget.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4619 2024-04-26 14:50:59.000000 pyegeria-0.3.5/examples/widgets/view_my_profile.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-04-29 05:49:49.000000 pyegeria-0.3.5/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-29 05:50:14.566185 pyegeria-0.3.5/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2102 2024-04-12 00:32:44.000000 pyegeria-0.3.5/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.546086 pyegeria-0.3.5/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.561116 pyegeria-0.3.5/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1769 2024-04-23 16:53:51.000000 pyegeria-0.3.5/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.5/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   100106 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   114200 2024-04-29 01:32:02.000000 pyegeria-0.3.5/src/pyegeria/collection_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    93140 2024-04-23 14:39:07.000000 pyegeria-0.3.5/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42441 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    77305 2024-04-26 16:10:23.000000 pyegeria-0.3.5/src/pyegeria/project_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8775 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/utils.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    29710 2024-04-25 15:33:15.000000 pyegeria-0.3.5/src/pyegeria/valid_metadata_omvs.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.565648 pyegeria-0.3.5/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3407 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.565452 pyegeria-0.3.5/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18673 2024-04-29 01:39:21.000000 pyegeria-0.3.5/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    51872 2024-04-29 00:11:27.000000 pyegeria-0.3.5/tests/test_collection_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59270 2024-04-15 22:01:18.000000 pyegeria-0.3.5/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.5/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9625 2024-04-12 00:32:44.000000 pyegeria-0.3.5/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40084 2024-04-23 14:27:57.000000 pyegeria-0.3.5/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    28529 2024-04-26 16:12:52.000000 pyegeria-0.3.5/tests/test_project_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4727 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12782 2024-04-25 15:34:36.000000 pyegeria-0.3.5/tests/test_valid_metadata_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_validators.py
```

### Comparing `pyegeria-0.3.4/LICENSE` & `pyegeria-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/PKG-INFO` & `pyegeria-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.4/README.md` & `pyegeria-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/.DS_Store` & `pyegeria-0.3.5/examples/.DS_Store`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0086 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0001  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
 00000050: 0000 0001 0000 1000 0065 0074 0073 6473  .........e.t.sds
 00000060: 636c 626f 0000 0000 0000 0000 0000 0000  clbo............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 0001 0000 0007  ................
+00000080: 0000 0000 0000 0000 0000 0002 0000 0007  ................
 00000090: 0077 0069 0064 0067 0065 0074 0073 6473  .w.i.d.g.e.t.sds
-000000a0: 636c 626f 6f6c 0000 0000 0000 0000 0000  clbool..........
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000a0: 636c 626f 6f6c 0100 0000 0700 7700 6900  clbool......w.i.
+000000b0: 6400 6700 6500 7400 7366 6473 6362 6f6f  d.g.e.t.sfdscboo
+000000c0: 6c01 0000 0000 0000 0000 0000 0000 0000  l...............
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `pyegeria-0.3.4/examples/Coco_config/README.md` & `pyegeria-0.3.5/examples/Coco_config/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDS1.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS1.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDS2.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS2.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDS3.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS3.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDS4.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS4.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDS5.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS5.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDS6.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS6.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoMDSx.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoMDSx.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_cocoView1.py` & `pyegeria-0.3.5/examples/Coco_config/config_cocoView1.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_exchangeDL01.py` & `pyegeria-0.3.5/examples/Coco_config/config_exchangeDL01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_governDL01.py` & `pyegeria-0.3.5/examples/Coco_config/config_governDL01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_monitorDev01.py` & `pyegeria-0.3.5/examples/Coco_config/config_monitorDev01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/config_monitorGov01.py` & `pyegeria-0.3.5/examples/Coco_config/config_monitorGov01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/Coco_config/globals.py` & `pyegeria-0.3.5/examples/Coco_config/globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/README.md` & `pyegeria-0.3.5/examples/widgets/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 * find_todos: find and display outstanding todos
 * gov_engine_status: provide a live status view of a governance engine
 * integration_daemon_status: provide a live status view of an integration daemon
 * my_todos: provide a live view of my todos
 * view_my_profile: view an Egeria profile
 * list_asset_types: list the types of assets that have been configured in Egeria
 * multi-server_status: show the status from two platforms concurrently
-* 
+* coco_statys.py: example showing the status of the Coco Pharmacutical platforms from the Jupyter Labs.
+* get_relationship_types.py: display the different types of relationships for a given Entity type.
+* get_valid_metadata_values.py: retrieve the currently defined valid metadata values for a given attribute and entity
+* open_todos.py: list the open todo items
+* project_list_viewer.py: List defined projects
```

### Comparing `pyegeria-0.3.4/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc` & `pyegeria-0.3.5/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/coco_status.py` & `pyegeria-0.3.5/examples/widgets/coco_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,37 +5,35 @@
 
 Unit tests for the Utils helper functions using the Pytest framework.
 
 
 A simple server status display
 """
 
-import time
 import argparse
+import time
 
-from rich.box import Box
+from rich import box
+from rich import print
+from rich.layout import Layout
+from rich.live import Live
+from rich.panel import Panel
+from rich.table import Table
 
 from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
 )
-from rich.table import Table
-from rich.live import Live
-from rich import print
-from rich.console import Group
-from rich.panel import Panel
-from rich import box, align
-from rich.layout import Layout
-import rich
 from pyegeria.server_operations import ServerOps
 
 disable_ssl_warnings = True
 
+
 def test_display_status(server: str, url: str, username: str):
     layout = Layout()
     print(layout)
 
     print(layout)
     p_client1 = ServerOps("Core Catalog", "https://localhost:9443", username)
     p_client2 = ServerOps('Datalake Catalog', "https://localhost:9444", username)
```

### Comparing `pyegeria-0.3.4/examples/widgets/engine_action_status.py` & `pyegeria-0.3.5/examples/widgets/engine_action_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/find_todos.py` & `pyegeria-0.3.5/examples/widgets/find_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/glossary_view.py` & `pyegeria-0.3.5/examples/widgets/glossary_view.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/gov_engine_status.py` & `pyegeria-0.3.5/examples/widgets/gov_engine_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/integration_daemon_status.py` & `pyegeria-0.3.5/examples/widgets/integration_daemon_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/list_asset_types.py` & `pyegeria-0.3.5/examples/widgets/list_asset_types.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/multi-server_status.py` & `pyegeria-0.3.5/examples/widgets/multi-server_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/env python3
 """
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
-Unit tests for the Utils helper functions using the Pytest framework.
-
-
-A simple server status display
+An example of displaying the status of two platforms concurrently.
 """
 
 import time
 import argparse
 
 from rich.box import Box
```

### Comparing `pyegeria-0.3.4/examples/widgets/my_todos.py` & `pyegeria-0.3.5/examples/widgets/my_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/open_todos.py` & `pyegeria-0.3.5/examples/widgets/open_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/server_status.py` & `pyegeria-0.3.5/examples/widgets/server_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/server_status_widget.py` & `pyegeria-0.3.5/examples/widgets/server_status_widget.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/examples/widgets/view_my_profile.py` & `pyegeria-0.3.5/examples/widgets/view_my_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         """Make a new table."""
         table = Table(
             title=f"My Profile Information {good_platform1_url} @ {time.asctime()}",
             # style = "black on grey66",
             header_style="white on dark_blue",
             show_lines=True,
             box=box.ROUNDED,
-            caption=f"My Profile from Server '{server}' @ Platform - {url}",
+            caption=f"My Profile from Server '{server}' @ Platform - {url}\n Press 'q' to Quit",
             expand=True
         )
 
         table.add_column("Name")
         table.add_column("Job Title")
         table.add_column("userId")
         table.add_column("myGUID")
```

### Comparing `pyegeria-0.3.4/pyproject.toml` & `pyegeria-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #requires = ["hatchling"]
 requires = ["setuptools", "wheel"]
 #build-backend = "hatchling.build"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.3.4"
+version = "0.3.5"
 #license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
 dependencies = [
     "requests~=2.31.0",
     "validators~=0.22.0",
```

### Comparing `pyegeria-0.3.4/setup.py` & `pyegeria-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/__init__.py` & `pyegeria-0.3.5/src/pyegeria/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,9 +36,11 @@
 from ._validators import (validate_user_id, validate_name, validate_guid, validate_server_name, validate_search_string,
                           validate_url, is_json, validate_public)
 # from .asset_catalog_omvs import AssetCatalog
 from .gov_engine import GovEng
 from .my_profile_omvs import MyProfile
 from .full_omag_server_config import FullServerConfig
 from .server_operations import ServerOps
-
+from .collection_manager_omvs import CollectionManager
+from .project_manager_omvs import ProjectManager
+from .valid_metadata_omvs import ValidMetadataManager
 __version__ = "0.3"
```

### Comparing `pyegeria-0.3.4/src/pyegeria/_client.py` & `pyegeria-0.3.5/src/pyegeria/_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/_exceptions.py` & `pyegeria-0.3.5/src/pyegeria/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/_globals.py` & `pyegeria-0.3.5/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/_validators.py` & `pyegeria-0.3.5/src/pyegeria/_validators.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/automated_curation_omvs.py` & `pyegeria-0.3.5/src/pyegeria/automated_curation_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.5/src/pyegeria/core_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1714,15 +1714,15 @@
         if server_name is None:
             server_name = self.server_name
         url = f"{self.admin_command_root}/servers/{server_name}/view-services"
         response = self.make_request("GET", url)
 
         return response.json().get("services", "No view services found")
 
-    def config_all_view_services(self, mdr_server_name: str,
+    def __config_all_view_services(self, mdr_server_name: str,
                                  mdr_server_platform_root_url: str, server_name: str = None) -> None:
         """ Enable all view services that are registered with this OMAG server platform.
 
         Parameters
         ----------
 
         mdr_server_name : str
```

### Comparing `pyegeria-0.3.4/src/pyegeria/full_omag_server_config.py` & `pyegeria-0.3.5/src/pyegeria/full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.5/src/pyegeria/glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/gov_engine.py` & `pyegeria-0.3.5/src/pyegeria/gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/governance_author.py` & `pyegeria-0.3.5/src/pyegeria/governance_author.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/my_profile_omvs.py` & `pyegeria-0.3.5/src/pyegeria/my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/platform_services.py` & `pyegeria-0.3.5/src/pyegeria/platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/registered_info.py` & `pyegeria-0.3.5/src/pyegeria/registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/server_operations.py` & `pyegeria-0.3.5/src/pyegeria/server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria/utils.py` & `pyegeria-0.3.5/src/pyegeria/utils.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/src/pyegeria.egg-info/PKG-INFO` & `pyegeria-0.3.5/src/pyegeria.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.4/src/pyegeria.egg-info/SOURCES.txt` & `pyegeria-0.3.5/src/pyegeria.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,60 +16,80 @@
 examples/Coco_config/config_cocoMDSx.py
 examples/Coco_config/config_cocoView1.py
 examples/Coco_config/config_exchangeDL01.py
 examples/Coco_config/config_governDL01.py
 examples/Coco_config/config_monitorDev01.py
 examples/Coco_config/config_monitorGov01.py
 examples/Coco_config/globals.py
+examples/Doc_Samples/Create_Collection_Sample.py
+examples/Doc_Samples/Create_Sustainability_Collection_Sample.py
+examples/Jupyter Notebooks/P-egeria-server-config.ipynb
+examples/Jupyter Notebooks/README.md
+examples/Jupyter Notebooks/common/P-environment-check.ipynb
+examples/Jupyter Notebooks/common/__init__.py
+examples/Jupyter Notebooks/common/common-functions.ipynb
+examples/Jupyter Notebooks/common/environment-check.ipynb
+examples/Jupyter Notebooks/common/globals.ipynb
+examples/Jupyter Notebooks/common/globals.py
+examples/Jupyter Notebooks/common/orig_globals.py
 examples/__pycache__/__init__.cpython-312.pyc
+examples/widgets/.DS_Store
 examples/widgets/README.md
 examples/widgets/__init__.py
 examples/widgets/coco_status.py
+examples/widgets/collection_viewer.py
 examples/widgets/engine_action_status.py
 examples/widgets/find_todos.py
+examples/widgets/get_relationship_types.py
+examples/widgets/get_valid_metadata_values.py
 examples/widgets/glossary_view.py
 examples/widgets/gov_engine_status.py
 examples/widgets/integration_daemon_status.py
 examples/widgets/list_asset_types.py
 examples/widgets/multi-server_status.py
 examples/widgets/my_todos.py
 examples/widgets/open_todos.py
+examples/widgets/project_list_viewer.py
 examples/widgets/server_status.py
 examples/widgets/server_status_widget.py
 examples/widgets/view_my_profile.py
 examples/widgets/__pycache__/__init__.cpython-312.pyc
 examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
 src/pyegeria/__init__.py
 src/pyegeria/_client.py
 src/pyegeria/_exceptions.py
 src/pyegeria/_globals.py
 src/pyegeria/_validators.py
 src/pyegeria/automated_curation_omvs.py
+src/pyegeria/collection_manager_omvs.py
 src/pyegeria/core_omag_server_config.py
-src/pyegeria/exceptions.py
 src/pyegeria/full_omag_server_config.py
 src/pyegeria/glossary_omvs.py
 src/pyegeria/gov_engine.py
 src/pyegeria/governance_author.py
 src/pyegeria/my_profile_omvs.py
 src/pyegeria/platform_services.py
+src/pyegeria/project_manager_omvs.py
 src/pyegeria/registered_info.py
 src/pyegeria/server_operations.py
 src/pyegeria/utils.py
+src/pyegeria/valid_metadata_omvs.py
 src/pyegeria.egg-info/PKG-INFO
 src/pyegeria.egg-info/SOURCES.txt
 src/pyegeria.egg-info/dependency_links.txt
 src/pyegeria.egg-info/requires.txt
 src/pyegeria.egg-info/top_level.txt
 tests/test_automated_curation_omvs.py
-tests/test_automated_curation_omvs_cray.py
 tests/test_client.py
+tests/test_collection_manager_omvs.py
 tests/test_core_omag_server_config.py
 tests/test_full_omag_server_config.py
 tests/test_glossary_omvs.py
 tests/test_gov_engine.py
 tests/test_my_profile_omvs.py
 tests/test_platform_services.py
+tests/test_project_manager_omvs.py
 tests/test_registered_info.py
 tests/test_server_operations.py
 tests/test_util_exp.py
+tests/test_valid_metadata_omvs.py
 tests/test_validators.py
```

### Comparing `pyegeria-0.3.4/tests/test_automated_curation_omvs.py` & `pyegeria-0.3.5/tests/test_automated_curation_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,17 @@
     def test_create_postgres_element_from_template(self):
         try:
             a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
                                          user_id=self.good_user_2, user_pwd="secret")
             token = a_client.create_egeria_bearer_token()
 
             start_time = time.perf_counter()
-            response = a_client.create_postgres_server_element_from_template("observations_base",
-                                                                             "egeria.pdr-associates.com",
-                                                                             "5432", db_user="surveyor",
+            response = a_client.create_postgres_server_element_from_template("observations",
+                                                                             "home.com",
+                                                                             "5432", db_user="garygeeke",
                                                                              db_pwd="secret")
             duration = time.perf_counter() - start_time
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is list :
                 out = ("\n\n" + json.dumps(response, indent=4))
                 count = len(response)
                 pprint(f"Found {count} elements")
```

### Comparing `pyegeria-0.3.4/tests/test_automated_curation_omvs_cray.py` & `pyegeria-0.3.5/tests/test_valid_metadata_omvs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 """
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
 
 
-This module is for testing the Automated Curation View Service module.
+This module is for testing the core OMAG config class and methods
 The routines assume that pytest is being used as the test tool and framework.
 
 A running Egeria environment is needed to run these tests.
 
 """
+import json
 import time
 
-import pytest
-import asyncio
-import json
 from rich import print, print_json
-from rich.pretty import pprint
-
-from rich.console import Console
-from contextlib import nullcontext as does_not_raise
 
-from pyegeria._exceptions import (
+from pyegeria import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
+    ValidMetadataManager
 )
-
-from pyegeria import AutomatedCuration, GlossaryBrowser
-from pyegeria.utils import print_json_list_as_table
+from pyegeria.glossary_omvs import GlossaryBrowser
 
 # from pyegeria.admin_services import FullServerConfig
 
 disable_ssl_warnings = True
-console = Console()
 
-class TestAutomatedCuration:
-    good_platform1_url = "https://cray.local:9443"
 
+class TestValidMetadataOMVs:
+    good_platform1_url = "https://127.0.0.1:9443"
+    good_platform2_url = "https://oak.local:9443"
+    bad_platform1_url = "https://localhost:9443"
+
+    # good_platform1_url = "https://127.0.0.1:30080"
+    # good_platform2_url = "https://127.0.0.1:30081"
+    # bad_platform1_url = "https://localhost:9443"
 
     good_user_1 = "garygeeke"
     good_user_2 = "erinoverview"
     good_user_3 = "peterprofile"
     bad_user_1 = "eviledna"
     bad_user_2 = ""
     good_integ_1 = "fluffy_integration"
@@ -54,267 +52,295 @@
     good_server_6 = "cocoVIew1"
     good_engine_host_1 = "governDL01"
     good_view_server_1 = "view-server"
     good_view_server_2 = "fluffy_view"
     bad_server_1 = "coco"
     bad_server_2 = ""
 
-    def test_create_kafka_element_from_template(self):
+    def test_get_all_entity_types(self):
         try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
 
-            response = a_client.create_kafka_server_element_from_template(kafka_server="pdr-kafka-server",
-                                                                          host_name='egeria.pdr-associates.com',
-                                                                          port='9092')
+            response = m_client.get_all_entity_types()
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
-            if type(response) is dict:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+            if type(response) is list:
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\nGUID is: " + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
-    def test_create_postgres_element_from_template(self):
+    def test_get_all_entity_defs(self):
         try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
 
-            response = a_client.create_postgres_server_element_from_template(postgres_server="egeriadashboard",
-                                                                             host_name='egeria.pdr-associates.com',
-                                                                             port="5432",
-                                                                             db_user="surveyor",
-                                                                             db_pwd='secret')
+            response = m_client.get_all_entity_defs()
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
-            if type(response) is dict:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+            if type(response) is list:
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\nGUID is: " + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
-    #
-    # Engine Functions
-    #
-    def test_get_engine_actions(self):
+    def test_get_all_relationship_defs(self):
         try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
 
-            response = a_client.get_engine_actions()
+            response = m_client.get_all_relationship_defs()
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is list:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\nGUID is: " + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
             InvalidParameterException,
             PropertyServerException,
             UserNotAuthorizedException
         ) as e:
-                print_exception_response(e)
-                assert False, "Invalid request"
+            print_exception_response(e)
+            assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
+    def test_get_all_classification_defs(self):
+        try:
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
+            start_time = time.perf_counter()
 
+            response = m_client.get_all_classification_defs()
+            duration = time.perf_counter() - start_time
 
-    def test_initiate_gov_action_type(self):
-        try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
+            print(f"\n\tDuration was {duration} seconds")
+            if type(response) is list:
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is str:
+                print("\n\nGUID is: " + response)
+            assert True
 
+        except (
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
+        ) as e:
+            print_exception_response(e)
+            assert False, "Invalid request"
+
+        finally:
+            m_client.close_session()
+
+    def test_get_valid_metadata_values(self):
+        try:
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
-            gov_action_type_qn = "Egeria:GovernanceActionType:2adeb8f1-0f59-4970-b6f2-6cc25d4d2402survey-folder"
+            type_name = "Project"
+            property_name = "projectStatus"
+            # type_name = None
+            # property_name = "stewardTypeName"
 
-            response = a_client.initiate_gov_action_type("PostgreSQL Server")
+            response = m_client.get_valid_metadata_values(property_name, type_name)
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is dict:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\n" + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
-    def test_initiate_file_folder_survey(self):
+    def test_get_valid_metadata_value(self):
         try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
-            folder_guid = "9f547ca9-3b23-45cb-a6dd-1f7e317e4336"
+            type_name = "Project"
+            property_name = "projectHealth"
+            preferred_value = "At Risk"
 
-            response = a_client.initiate_file_folder_survey(folder_guid)
+            response = m_client.get_valid_metadata_value(property_name, type_name, preferred_value)
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is dict:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\n" + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
-    def test_initiate_postgres_server_survey(self):
+    def test_get_valid_relationship_types(self):
         try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
-            postgres_server_guid = "a095cb16-c108-40cf-b7bb-bfda003ea60b"
+            entity_type = "AssetOwner"
 
-            response = a_client.initiate_postgres_server_survey(postgres_server_guid)
+            response = m_client.get_valid_relationship_types(entity_type)
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
-            if type(response) is dict:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+            if type(response) is list:
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\n" + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
-    def test_initiate_kafka_server_survey(self):
+    def test_get_valid_classification_types(self):
         try:
-            a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
-                                         user_id=self.good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
-            kafka_server_guid = " d744474c-54ee-47b8-bc46-3cac9662f489"
+            entity_type = "AssetOwner"
 
-            response = a_client.initiate_kafka_server_survey(kafka_server_guid)
+            response = m_client.get_valid_classification_types(entity_type)
             duration = time.perf_counter() - start_time
+
             print(f"\n\tDuration was {duration} seconds")
-            if type(response) is dict:
-                out = ("\n\n" + json.dumps(response, indent=4))
-                count = len(response)
-                console.log(f"Found {count} elements")
-                print_json(out)
+            if type(response) is list:
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
             elif type(response) is str:
-                console.log("\n\n" + response)
+                print("\n\nGUID is: " + response)
             assert True
 
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
 
-    if __name__ == "__main__":
+    def test_get_typedef_by_name(self):
         try:
-            a_client = AutomatedCuration(good_view_server_1, good_platform1_url,
-                                         user_id=good_user_2, user_pwd="secret")
-            token = a_client.create_egeria_bearer_token()
-
+            m_client = ValidMetadataManager(self.good_view_server_1, self.good_platform1_url,
+                                     user_id=self.good_user_2)
+            token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             start_time = time.perf_counter()
-            response = a_client.create_postgres_server_element_from_template("cray-server",
-                                                                             "egeria.pdr-associates.com",
-                                                                             "5432", db_user="surveyor",
-                                                                             db_pwd="secret")
+            entity_type = "AssetOwner"
+
+            response = m_client.get_typedef_by_name(entity_type)
             duration = time.perf_counter() - start_time
 
             print(f"\n\tDuration was {duration} seconds")
+            if type(response) is dict:
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is tuple:
+                print(f"Type is {type(response)}")
+                print_json("\n\n" + json.dumps(response, indent=4))
+            elif type(response) is str:
+                print("\n\nGUID is: " + response)
+            assert True
 
-            pprint("Database Server GUID is " + response)
-
-            a_client.initiate_gov_action_type("PostgreSQL Server")
         except (
-                InvalidParameterException,
-                PropertyServerException,
-                UserNotAuthorizedException
+            InvalidParameterException,
+            PropertyServerException,
+            UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
         finally:
-            a_client.close_session()
+            m_client.close_session()
```

### Comparing `pyegeria-0.3.4/tests/test_client.py` & `pyegeria-0.3.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_core_omag_server_config.py` & `pyegeria-0.3.5/tests/test_core_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1222,15 +1222,15 @@
     def test_clear_view_svc(self, server:str = good_view_server_1):
 
         try:
             o_client: CoreServerConfig = CoreServerConfig(
                 server, self.good_platform1_url,
                 self.good_user_1)
 
-            o_client.clear_view_service("tex")
+            o_client.clear_view_service("server-author")
             assert True
 
             print(f"\n\n\t\tServer {server}: view service cleared")
 
         except (
                 InvalidParameterException,
                 PropertyServerException,
```

### Comparing `pyegeria-0.3.4/tests/test_full_omag_server_config.py` & `pyegeria-0.3.5/tests/test_full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_glossary_omvs.py` & `pyegeria-0.3.5/tests/test_glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_gov_engine.py` & `pyegeria-0.3.5/tests/test_gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_my_profile_omvs.py` & `pyegeria-0.3.5/tests/test_my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_platform_services.py` & `pyegeria-0.3.5/tests/test_platform_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
             print_exception_response(e)
             assert e.related_http_code is not "200", "Invalid parameters"
         finally:
             p_client.close_session()
 
-    def test_activate_server_stored_config(self, server: str = "cocoMDS1"):
+    def test_activate_server_stored_config(self, server: str = "view-server"):
         """
         Need to decide if its worth it to broaden out the test cases..for instance
         in this method if there is an exception - such as invalid server name
         then the test case fails because the response is used before set..
 
         """
         try:
@@ -598,15 +598,15 @@
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "404", "Invalid parameters"
 
         finally:
             p_client.close_session()
 
-    def test_get_active_server_instance_status(self, server: str = good_server_2):
+    def test_get_active_server_instance_status(self, server: str = good_server_1):
         try:
             p_client = Platform(server, self.good_platform1_url, self.good_user_1)
             response = p_client.get_active_server_instance_status()
             if type(response) is str:
                 print("Server instance status indicates: " + response)
             else:
                 print (f"\n\n\tActive server status: {json.dumps(response, indent=4)}")
@@ -731,15 +731,15 @@
             print(f"\n\n\tKnown servers on the platform are: {known_servers}")
             assert True, "Issues encountered "
 
         if p_client.exc_type:
             print_exception_response(p_client.exc_val)
             assert False
 
-    def test_activate_platform(self, server:str = good_server_1):
+    def test_activate_platform(self, server:str = good_server_3):
         try:
             p_client = Platform(server, self.good_platform1_url, self.good_user_1)
             p_client.activate_platform("laz", ["active-metadata-store","simple-metadata-store"])
             print(f"\n\n\tPlatform laz activated")
             assert True
 
         except (InvalidParameterException, PropertyServerException) as e:
```

### Comparing `pyegeria-0.3.4/tests/test_registered_info.py` & `pyegeria-0.3.5/tests/test_registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_server_operations.py` & `pyegeria-0.3.5/tests/test_server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_util_exp.py` & `pyegeria-0.3.5/tests/test_util_exp.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.4/tests/test_validators.py` & `pyegeria-0.3.5/tests/test_validators.py`

 * *Files identical despite different names*

