# Comparing `tmp/tinybird-cli-3.9.1.dev3.tar.gz` & `tmp/tinybird-cli-3.9.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.9.1.dev3.tar", last modified: Thu Apr 25 14:38:01 2024, max compression
+gzip compressed data, was "tinybird-cli-3.9.1.dev4.tar", last modified: Mon Apr 29 10:41:53 2024, max compression
```

## Comparing `tinybird-cli-3.9.1.dev3.tar` & `tinybird-cli-3.9.1.dev4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:38:01.632516 tinybird-cli-3.9.1.dev3/
--rw-r--r--   0 root         (0) root         (0)    68507 2024-04-25 14:38:01.632516 tinybird-cli-3.9.1.dev3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:38:01.632516 tinybird-cli-3.9.1.dev3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:38:01.629516 tinybird-cli-3.9.1.dev3/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-25 14:38:00.000000 tinybird-cli-3.9.1.dev3/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:38:01.629516 tinybird-cli-3.9.1.dev3/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59114 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41589 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:38:01.631517 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    30927 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:38:01.631517 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-25 14:37:56.000000 tinybird-cli-3.9.1.dev3/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:38:01.632516 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    68507 2024-04-25 14:38:01.000000 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-25 14:38:01.000000 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:38:01.000000 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-25 14:38:01.000000 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-25 14:38:01.000000 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-25 14:38:01.000000 tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/
+-rw-r--r--   0 root         (0) root         (0)    68632 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.524615 tinybird-cli-3.9.1.dev4/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-29 10:41:52.000000 tinybird-cli-3.9.1.dev4/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.524615 tinybird-cli-3.9.1.dev4/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59638 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41589 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.526615 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    31660 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.526615 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-29 10:41:47.000000 tinybird-cli-3.9.1.dev4/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 10:41:53.527615 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    68632 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-29 10:41:53.000000 tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.9.1.dev3/PKG-INFO` & `tinybird-cli-3.9.1.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev3
+Version: 3.9.1.dev4
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -12,15 +12,21 @@
 
 Tinybird CLI
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
----------
+----------
+
+
+3.9.1.dev4
+************
+
+- `Fixed` s3 iamrole connection creation will not fail when `pbcopy` dependency is not available
 
 3.9.1.dev3
 ************
 
 - `Fixed` Fixed a bug on data branching
 
 3.9.1.dev2
```

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/ch_utils/constants.py` & `tinybird-cli-3.9.1.dev4/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/ch_utils/engine.py` & `tinybird-cli-3.9.1.dev4/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/check_pypi.py` & `tinybird-cli-3.9.1.dev4/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/client.py` & `tinybird-cli-3.9.1.dev4/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/config.py` & `tinybird-cli-3.9.1.dev4/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/connectors.py` & `tinybird-cli-3.9.1.dev4/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/context.py` & `tinybird-cli-3.9.1.dev4/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/datafile.py` & `tinybird-cli-3.9.1.dev4/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/datatypes.py` & `tinybird-cli-3.9.1.dev4/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/feedback_manager.py` & `tinybird-cli-3.9.1.dev4/tinybird/feedback_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,18 +401,23 @@
 Ready? """
     )
 
     prompt_s3_iamrole_connection_login_aws = prompt_message("""[1] Log into your AWS Console\n\n""")
     prompt_s3_iamrole_connection_policy = prompt_message(
         """\n[2] Go to IAM > Policies. Create a new policy with the following permissions. Please, replace <bucket> with your bucket name:\n\n{access_policy}\n\n(The policy has been copied to your clipboard)\n\n"""
     )
+    prompt_s3_iamrole_connection_policy_not_copied = prompt_message(
+        """\n[2] Go to IAM > Policies. Create a new policy with the following permissions. Please, copy this policy and replace <bucket> with your bucket name:\n\n{access_policy}\n\n"""
+    )
     prompt_s3_iamrole_connection_role = prompt_message(
         """\n[3] Go to IAM > Roles. Create a new IAM Role using the following custom trust policy and attach the access policy you just created in the previous step:\n\n{trust_policy}\n\n(The policy has been copied to your clipboard)\n\n"""
     )
-
+    prompt_s3_iamrole_connection_role_not_copied = prompt_message(
+        """\n[3] Go to IAM > Roles. Create a new IAM Role using the following custom trust policy and attach the access policy you just created in the previous step:\n\n{trust_policy}\n\n"""
+    )
     prompt_init_git_release_pull = prompt_message(
         "❓ Download the Data Project to continue, otherwise you can't initialize Workspace with Git. Execute '{pull_command}'?"
     )
     prompt_init_cicd = prompt_message("\n Do you want to generate CI/CD config files?")
     prompt_init_git_release_force = prompt_message(
         "You are going to manually update workspace release commit reference manually, this is just for special ocasions. Do you want to update current commit release reference '{current_commit}' to '{new_commit}'?"
     )
```

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/git_settings.py` & `tinybird-cli-3.9.1.dev4/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/sql.py` & `tinybird-cli-3.9.1.dev4/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/sql_template.py` & `tinybird-cli-3.9.1.dev4/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/sql_template_fmt.py` & `tinybird-cli-3.9.1.dev4/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/sql_toolset.py` & `tinybird-cli-3.9.1.dev4/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/syncasync.py` & `tinybird-cli-3.9.1.dev4/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,25 +768,43 @@
                 if not click.confirm(
                     FeedbackManager.prompt_s3_iamrole_connection_login_aws(),
                     show_default=False,
                     prompt_suffix="Press y to continue:",
                 ):
                     sys.exit(1)
 
-                pyperclip.copy(access_policy)
+                access_policy_copied = True
+                try:
+                    pyperclip.copy(access_policy)
+                except Exception:
+                    access_policy_copied = False
+
                 if not click.confirm(
-                    FeedbackManager.prompt_s3_iamrole_connection_policy(access_policy=access_policy),
+                    (
+                        FeedbackManager.prompt_s3_iamrole_connection_policy(access_policy=access_policy)
+                        if access_policy_copied
+                        else FeedbackManager.prompt_s3_iamrole_connection_policy_not_copied(access_policy=access_policy)
+                    ),
                     show_default=False,
                     prompt_suffix="Press y to continue:",
                 ):
                     sys.exit(1)
 
-                pyperclip.copy(trust_policy)
+                trust_policy_copied = True
+                try:
+                    pyperclip.copy(trust_policy)
+                except Exception:
+                    trust_policy_copied = False
+
                 if not click.confirm(
-                    FeedbackManager.prompt_s3_iamrole_connection_role(trust_policy=trust_policy),
+                    (
+                        FeedbackManager.prompt_s3_iamrole_connection_role(trust_policy=trust_policy)
+                        if trust_policy_copied
+                        else FeedbackManager.prompt_s3_iamrole_connection_role_not_copied(trust_policy=trust_policy)
+                    ),
                     show_default=False,
                     prompt_suffix="Press y to continue:",
                 ):
                     sys.exit(1)
 
         if not role_arn:
             role_arn = click.prompt("Enter the ARN of the role you just created")
```

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.9.1.dev4/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird/tornado_template.py` & `tinybird-cli-3.9.1.dev4/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev3
+Version: 3.9.1.dev4
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -12,15 +12,21 @@
 
 Tinybird CLI
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
----------
+----------
+
+
+3.9.1.dev4
+************
+
+- `Fixed` s3 iamrole connection creation will not fail when `pbcopy` dependency is not available
 
 3.9.1.dev3
 ************
 
 - `Fixed` Fixed a bug on data branching
 
 3.9.1.dev2
```

### Comparing `tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev3/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.9.1.dev4/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

