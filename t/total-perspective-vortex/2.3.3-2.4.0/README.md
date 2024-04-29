# Comparing `tmp/total-perspective-vortex-2.3.3.tar.gz` & `tmp/total_perspective_vortex-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total-perspective-vortex-2.3.3.tar", last modified: Tue Feb 13 12:20:05 2024, max compression
+gzip compressed data, was "total_perspective_vortex-2.4.0.tar", last modified: Mon Apr 29 06:34:36 2024, max compression
```

## Comparing `total-perspective-vortex-2.3.3.tar` & `total_perspective_vortex-2.4.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.539447 total-perspective-vortex-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-13 12:20:05.539447 total-perspective-vortex-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-13 12:20:05.539447 total-perspective-vortex-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.531447 total-perspective-vortex-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_merge_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_params_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_resubmit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_mapper_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tests/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.535447 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-13 12:20:05.000000 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-13 12:20:05.000000 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 12:20:05.000000 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-13 12:20:05.000000 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-13 12:20:05.000000 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-13 12:20:05.000000 total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.531447 total-perspective-vortex-2.3.3/tpv/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.531447 total-perspective-vortex-2.3.3/tpv/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/dryrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.535447 total-perspective-vortex-2.3.3/tpv/commands/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/commands/test/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.535447 total-perspective-vortex-2.3.3/tpv/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39592 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/core/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:20:05.535447 total-perspective-vortex-2.3.3/tpv/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-13 12:19:48.000000 total-perspective-vortex-2.3.3/tpv/rules/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.205335 total_perspective_vortex-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-29 06:34:36.205335 total_perspective_vortex-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-29 06:34:36.209335 total_perspective_vortex-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.197336 total_perspective_vortex-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_merge_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_params_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_mapper_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tests/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.201336 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-29 06:34:36.000000 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 06:34:36.000000 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 06:34:36.000000 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 06:34:36.000000 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 06:34:36.000000 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 06:34:36.000000 total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.201336 total_perspective_vortex-2.4.0/tpv/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.201336 total_perspective_vortex-2.4.0/tpv/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/dryrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.201336 total_perspective_vortex-2.4.0/tpv/commands/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/commands/test/mock_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.201336 total_perspective_vortex-2.4.0/tpv/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39592 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/core/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:36.201336 total_perspective_vortex-2.4.0/tpv/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-29 06:34:22.000000 total_perspective_vortex-2.4.0/tpv/rules/gateway.py
```

### Comparing `total-perspective-vortex-2.3.3/LICENSE` & `total_perspective_vortex-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/PKG-INFO` & `total_perspective_vortex-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.3.3
+Version: 2.4.0
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.3.3/README.md` & `total_perspective_vortex-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/setup.py` & `total_perspective_vortex-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_entity.py` & `total_perspective_vortex-2.4.0/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_helpers.py` & `total_perspective_vortex-2.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_basic.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_basic.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_context.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_context.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_destinations.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_destinations.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_inheritance.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_inheritance.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_merge_multiple.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_merge_multiple.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_params_specific.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_params_specific.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_rank.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_rank.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_resubmit.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_resubmit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import os
+
+import pytest
+
 from galaxy_test.driver.integration_util import IntegrationTestCase
 from galaxy.webapps.base import webapp
 
 
 class TestMapperResubmission(IntegrationTestCase):
     default_tool_conf = os.path.join(os.path.dirname(__file__), 'fixtures/resubmit/tool_conf_resubmit.xml')
 
@@ -27,13 +30,14 @@
         try:
             self._run_tool_test(tool_id, resource_parameters=resource_parameters)
         except Exception:
             exception_thrown = True
 
         assert exception_thrown
 
-    # FIXME: Temporarily disable tests till https://github.com/galaxyproject/galaxy/issues/14021 is resolved.
-    # def test_mapping_with_resubmission(self):
-    #     self._assert_job_passes(tool_id="exit_code_oom_with_resubmit")
-    #
-    # def test_mapping_without_resubmission(self):
-    #     self._assert_job_fails(tool_id="exit_code_oom_no_resubmit")
+    @pytest.mark.slow
+    def test_mapping_with_resubmission(self):
+        self._assert_job_passes(tool_id="exit_code_oom_with_resubmit")
+
+    @pytest.mark.slow
+    def test_mapping_without_resubmission(self):
+        self._assert_job_fails(tool_id="exit_code_oom_no_resubmit")
```

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_role.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_role.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_rules.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_rules.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_sample.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_sample.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_mapper_user.py` & `total_perspective_vortex-2.4.0/tests/test_mapper_user.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_scenarios.py` & `total_perspective_vortex-2.4.0/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tests/test_shell.py` & `total_perspective_vortex-2.4.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/PKG-INFO` & `total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.3.3
+Version: 2.4.0
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.3.3/total_perspective_vortex.egg-info/SOURCES.txt` & `total_perspective_vortex-2.4.0/total_perspective_vortex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 tests/__init__.py
+tests/conftest.py
 tests/test_entity.py
 tests/test_helpers.py
 tests/test_mapper_basic.py
 tests/test_mapper_context.py
 tests/test_mapper_destinations.py
 tests/test_mapper_inheritance.py
 tests/test_mapper_merge_multiple.py
```

### Comparing `total-perspective-vortex-2.3.3/tpv/commands/dryrunner.py` & `total_perspective_vortex-2.4.0/tpv/commands/dryrunner.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/commands/formatter.py` & `total_perspective_vortex-2.4.0/tpv/commands/formatter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/commands/linter.py` & `total_perspective_vortex-2.4.0/tpv/commands/linter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/commands/shell.py` & `total_perspective_vortex-2.4.0/tpv/commands/shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/commands/test/mock_galaxy.py` & `total_perspective_vortex-2.4.0/tpv/commands/test/mock_galaxy.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/core/entities.py` & `total_perspective_vortex-2.4.0/tpv/core/entities.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/core/helpers.py` & `total_perspective_vortex-2.4.0/tpv/core/helpers.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/core/loader.py` & `total_perspective_vortex-2.4.0/tpv/core/loader.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/core/mapper.py` & `total_perspective_vortex-2.4.0/tpv/core/mapper.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.3.3/tpv/rules/gateway.py` & `total_perspective_vortex-2.4.0/tpv/rules/gateway.py`

 * *Files identical despite different names*

