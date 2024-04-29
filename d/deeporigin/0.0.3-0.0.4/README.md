# Comparing `tmp/deeporigin-0.0.3.tar.gz` & `tmp/deeporigin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeporigin-0.0.3.tar", last modified: Thu Apr 18 20:08:40 2024, max compression
+gzip compressed data, was "deeporigin-0.0.4.tar", last modified: Mon Apr 29 13:57:08 2024, max compression
```

## Comparing `deeporigin-0.0.3.tar` & `deeporigin-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.476557 deeporigin-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 20:08:32.000000 deeporigin-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 20:08:32.000000 deeporigin-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 20:08:40.476557 deeporigin-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-18 20:08:32.000000 deeporigin-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.476557 deeporigin-0.0.3/deeporigin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 20:08:40.000000 deeporigin-0.0.3/deeporigin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 20:08:40.000000 deeporigin-0.0.3/deeporigin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:08:40.000000 deeporigin-0.0.3/deeporigin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 20:08:40.000000 deeporigin-0.0.3/deeporigin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-18 20:08:40.000000 deeporigin-0.0.3/deeporigin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 20:08:40.000000 deeporigin-0.0.3/deeporigin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 20:08:32.000000 deeporigin-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:08:40.476557 deeporigin-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.468557 deeporigin-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 20:08:37.000000 deeporigin-0.0.3/src/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.468557 deeporigin-0.0.3/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.468557 deeporigin-0.0.3/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/do_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/feature_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.468557 deeporigin-0.0.3/src/managed_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/managed_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/managed_data/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/managed_data/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/managed_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/managed_data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.472557 deeporigin-0.0.3/src/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.472557 deeporigin-0.0.3/src/variables/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/anthropic_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/git_http_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/gurobi_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/mosek_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/open_ai_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/private_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/private_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/secret_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/secret_env_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/secret_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/secret_file_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/variables/types/xpress_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 20:08:32.000000 deeporigin-0.0.3/src/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:08:40.472557 deeporigin-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-18 20:08:32.000000 deeporigin-0.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-18 20:08:32.000000 deeporigin-0.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-18 20:08:32.000000 deeporigin-0.0.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-18 20:08:32.000000 deeporigin-0.0.3/tests/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9920 2024-04-18 20:08:32.000000 deeporigin-0.0.3/tests/test_managed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-04-18 20:08:32.000000 deeporigin-0.0.3/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.388641 deeporigin-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 13:57:03.000000 deeporigin-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:57:03.000000 deeporigin-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 13:57:08.388641 deeporigin-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-29 13:57:03.000000 deeporigin-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.388641 deeporigin-0.0.4/deeporigin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 13:57:08.000000 deeporigin-0.0.4/deeporigin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-29 13:57:03.000000 deeporigin-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:57:08.388641 deeporigin-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 13:57:05.000000 deeporigin-0.0.4/src/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11909 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/do_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/feature_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/managed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/managed_data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.380641 deeporigin-0.0.4/src/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.384641 deeporigin-0.0.4/src/variables/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/anthropic_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/git_http_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/gurobi_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/mosek_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/open_ai_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/private_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/private_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_env_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/secret_file_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/variables/types/xpress_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 13:57:03.000000 deeporigin-0.0.4/src/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:08.388641 deeporigin-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_cli_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_managed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-04-29 13:57:03.000000 deeporigin-0.0.4/tests/test_variables.py
```

### Comparing `deeporigin-0.0.3/LICENSE.txt` & `deeporigin-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/PKG-INFO` & `deeporigin-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
@@ -23,7 +23,15 @@
 Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: parameterized; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Provides-Extra: jupyter
 Requires-Dist: ipykernel; extra == "jupyter"
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material-extensions; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocstrings; extra == "docs"
+Requires-Dist: mkdocstrings-python; extra == "docs"
+Requires-Dist: mkdocs-git-revision-date-localized-plugin; extra == "docs"
+Requires-Dist: black; extra == "docs"
```

### Comparing `deeporigin-0.0.3/README.md` & `deeporigin-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/deeporigin.egg-info/PKG-INFO` & `deeporigin-0.0.4/deeporigin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
@@ -23,7 +23,15 @@
 Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: parameterized; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Provides-Extra: jupyter
 Requires-Dist: ipykernel; extra == "jupyter"
+Provides-Extra: docs
+Requires-Dist: mkdocs; extra == "docs"
+Requires-Dist: mkdocs-material-extensions; extra == "docs"
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocstrings; extra == "docs"
+Requires-Dist: mkdocstrings-python; extra == "docs"
+Requires-Dist: mkdocs-git-revision-date-localized-plugin; extra == "docs"
+Requires-Dist: black; extra == "docs"
```

### Comparing `deeporigin-0.0.3/deeporigin.egg-info/SOURCES.txt` & `deeporigin-0.0.4/deeporigin.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -43,12 +43,13 @@
 src/variables/types/private_ssh_key.py
 src/variables/types/secret_env_var.py
 src/variables/types/secret_env_var_value.py
 src/variables/types/secret_file.py
 src/variables/types/secret_file_value.py
 src/variables/types/xpress_license_file.py
 tests/test_cli.py
+tests/test_cli_data.py
 tests/test_config.py
 tests/test_context.py
 tests/test_feature_flags.py
 tests/test_managed_data.py
 tests/test_variables.py
```

### Comparing `deeporigin-0.0.3/pyproject.toml` & `deeporigin-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 test = [
     "pytest",
     "parameterized",
     "coverage",
 ]
 jupyter = ["ipykernel"]
 
+docs=["mkdocs", "mkdocs-material-extensions", "mkdocs-material", "mkdocstrings" ,"mkdocstrings-python","mkdocs-git-revision-date-localized-plugin","black"]
+
+
 [tool.setuptools]
 package-dir = {"deeporigin" = "src"}
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = {file = ["src/VERSION"]}
 
@@ -65,8 +68,13 @@
 
 
 
 [tool.ruff.lint.isort]
 case-sensitive = true
 
 [tool.distutils.bdist_wheel]
-universal = true
+universal = true
+
+[tool.coverage.run]
+omit = [
+    "src/managed_data/client.py"
+]
```

### Comparing `deeporigin-0.0.3/src/cli/__init__.py` & `deeporigin-0.0.4/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/cli/context.py` & `deeporigin-0.0.4/src/cli/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/cli/data.py` & `deeporigin-0.0.4/src/cli/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 """this implements controllers and hooks to connect to
 managed_data.py"""
 
 import json
+import os
 from typing import Union
 
 import cement
 from beartype import beartype
 from deeporigin.exceptions import DeepOriginException
-from deeporigin.managed_data import _api
-from deeporigin.managed_data.api import (
-    download,
-    get_dataframe,
-    get_row_data,
-    get_tree,
-    upload,
-)
+from deeporigin.managed_data import _api, api
 from deeporigin.managed_data.client import DeepOriginClient
 from deeporigin.utils import PREFIX
 from tabulate import tabulate
 
-client = DeepOriginClient()
-client.authenticate(refresh_tokens=False)
-
 
 @beartype
 def _print_tree(tree: dict, offset: int = 0) -> None:
     """helper function to pretty print a tree"""
     print(" " * offset + tree["hid"])
 
     if "children" not in tree.keys():
@@ -66,14 +57,81 @@
         stacked_type = "nested"
         help = "explore and fetch data from Deep Origin managed data"
         description = """
 List data in managed data on Deep Origin, and save
 databases to CSV files. 
             """
 
+    def _get_client(self):
+        """helper method that returns an authenticated
+        client if the app has no client configured"""
+        try:
+            return self.app.client
+        except Exception:
+            client = DeepOriginClient()  # pragma: no cover
+            client.authenticate(refresh_tokens=False)  # pragma: no cover
+
+            return client  # pragma: no cover
+
+    @cement.ex(
+        help="Merge to databases into a single one, integrating cross-references",
+        arguments=[
+            (
+                ["--databases"],
+                {
+                    "help": "List of databases to merge",
+                    "action": "store",
+                    "nargs": "*",
+                    "required": True,
+                },
+            ),
+            (
+                ["--destination"],
+                {
+                    "type": str,
+                    "required": True,
+                    "metavar": "<destination>",
+                    "help": "Folder on local disk to save to",
+                },
+            ),
+            (
+                ["--include-files"],
+                {
+                    "action": "store_true",
+                    "help": "Whether to download files in database [default: False]",
+                },
+            ),
+        ],
+    )
+    def merge_db(self):
+        """Merge databases and save as CSV"""
+
+        databases = self.app.pargs.databases
+        destination = self.app.pargs.destination
+        dfs = []
+        save_name = "-".join(databases)
+        for db in databases:
+            df = api.get_dataframe(
+                db,
+                client=self._get_client(),
+            )
+            dfs.append(df)
+        df = api.merge_databases(dfs)
+
+        # save to CSV
+        df.to_csv(os.path.join(destination, f"merged-{save_name}.csv"))
+
+        if not self.app.pargs.include_files:
+            return
+
+        for df in dfs:
+            files = df.attrs["file_ids"]
+            for file in files:
+                _api.download_file(file, destination=destination)
+
     @cement.ex(
         help="Describe and get metadata of file uploaded to database in your Deep Origin data management system",
         arguments=[
             (
                 ["file_id"],
                 {"help": "File ID", "action": "store"},
             ),
@@ -83,17 +141,20 @@
                     "action": "store_true",
                     "help": "Whether to return JSON formatted data [default: False]",
                 },
             ),
         ],
     )
     def describe_file(self):
-        """describe row"""
+        """describe file"""
 
-        data = _api.describe_file(self.app.pargs.file_id, client=client)
+        data = _api.describe_file(
+            self.app.pargs.file_id,
+            client=self._get_client(),
+        )
 
         _print_dict(data, json=self.app.pargs.json)
 
     @cement.ex(
         help="Describe row",
         arguments=[
             (
@@ -108,19 +169,83 @@
                 },
             ),
         ],
     )
     def describe_row(self):
         """describe row"""
 
-        data = _api.describe_row(self.app.pargs.row_id, client=client)
+        data = _api.describe_row(
+            self.app.pargs.row_id,
+            client=self._get_client(),
+        )
 
         _print_dict(data, json=self.app.pargs.json)
 
     @cement.ex(
+        help="List files in a database or row",
+        arguments=[
+            (
+                ["--assigned_row_ids"],
+                {
+                    "help": "Row IDs that files are assigned to",
+                    "action": "store",
+                    "nargs": "*",
+                },
+            ),
+            (
+                ["--unassigned"],
+                {
+                    "action": "store_true",
+                    "help": "Whether to only find unassigned files: False]",
+                },
+            ),
+            (
+                ["--json"],
+                {
+                    "action": "store_true",
+                    "help": "Whether to return JSON formatted data [default: False]",
+                },
+            ),
+            (
+                ["--show-uri"],
+                {
+                    "action": "store_true",
+                    "help": "Whether to show the URI [default: False]",
+                },
+            ),
+        ],
+    )
+    def list_files(self):
+        """list rows"""
+
+        files = _api.list_files(
+            assigned_row_ids=self.app.pargs.assigned_row_ids,
+            is_unassigned=self.app.pargs.unassigned,
+            client=self._get_client(),
+        )
+
+        if len(files) == 0:
+            print("No files found")
+            return
+
+        if self.app.pargs.json:
+            _show_json(files)
+            return
+
+        # convert a list of dicts to a dict of lists
+        data = {}
+        keys = files[0]["file"].keys()
+        for key in keys:
+            if not self.app.pargs.show_uri and key == "uri":
+                continue
+            data[key] = [file["file"][key] for file in files]
+
+        _print_dict(data, json=False, transpose=False)
+
+    @cement.ex(
         help="List rows in a database or row",
         arguments=[
             (
                 ["row_id"],
                 {"help": "Row or Database ID", "action": "store"},
             ),
             (
@@ -133,15 +258,15 @@
         ],
     )
     def list_rows(self):
         """list rows"""
 
         rows = _api.list_rows(
             parent_id=self.app.pargs.row_id,
-            client=client,
+            client=self._get_client(),
         )
 
         if self.app.pargs.json:
             _show_json(rows)
             return
 
         # convert a list of dicts to a dict of lists
@@ -170,15 +295,19 @@
                 },
             ),
         ],
     )
     def show_db(self):
         """list database row"""
 
-        data = get_dataframe(self.app.pargs.db_id, return_type="dict")
+        data = api.get_dataframe(
+            self.app.pargs.db_id,
+            return_type="dict",
+            client=self._get_client(),
+        )
 
         _print_dict(data, json=self.app.pargs.json, transpose=False)
 
     @cement.ex(
         help="List child workspaces and databases in given workspace",
         arguments=[
             (
@@ -191,15 +320,17 @@
                 },
             )
         ],
     )
     def ls(self):
         """list rows in db"""
 
-        tree = get_tree(client=client)
+        tree = api.get_tree(
+            client=self._get_client(),
+        )
         _print_tree(tree)
 
     @cement.ex(
         help="Show column names and values for a given row",
         arguments=[
             (
                 ["row_id"],
@@ -212,15 +343,18 @@
                     "help": "Whether to return JSON formatted data [default: False]",
                 },
             ),
         ],
     )
     def row(self):
         """list the columns of the row and their values, where applicable"""
-        row_data = get_row_data(self.app.pargs.row_id, client=client)
+        row_data = api.get_row_data(
+            self.app.pargs.row_id,
+            client=self._get_client(),
+        )
 
         _print_dict(row_data, json=self.app.pargs.json)
 
 
 class CopyController(cement.Controller):
     class Meta:
         label = "cp"
@@ -258,21 +392,22 @@
         ]
 
     @cement.ex(hide=True)
     def _default(self):
         args = self.app.pargs
 
         if PREFIX in args.source and PREFIX not in args.destination:
-            download(
+            api.download(
                 args.source,
                 args.destination,
                 include_files=args.include_files,
             )
         elif PREFIX in args.destination and PREFIX not in args.source:
-            upload(args.source, args.destination)
+            raise NotImplementedError("Uploading has not been implemented yet")
+            # upload(args.source, args.destination)
         else:
             raise DeepOriginException(
                 f"Exactly one of <source> and <destination> should be prefixed with `{PREFIX}`"
             )
 
 
 @beartype
```

### Comparing `deeporigin-0.0.3/src/cli/variables.py` & `deeporigin-0.0.4/src/cli/variables.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/config/__init__.py` & `deeporigin-0.0.4/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/config/default.yml` & `deeporigin-0.0.4/src/config/default.yml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/context.py` & `deeporigin-0.0.4/src/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/do_api.py` & `deeporigin-0.0.4/src/do_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/feature_flags.py` & `deeporigin-0.0.4/src/feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/managed_data/api.py` & `deeporigin-0.0.4/src/managed_data/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-"""this module contains high-level functions used to
-interact with the data product"""
+"""The `deeporigin.managed_data.api` module contains high-level functions for
+interacting with Deep Origin managed data."""
 
 import os
-from typing import Literal, Optional, Union
+from typing import Any, Optional, Union
 
 from beartype import beartype
 from deeporigin.exceptions import DeepOriginException
 from deeporigin.managed_data._api import (
     convert_id_format,
     describe_file,
     describe_row,
     download_file,
     list_database_rows,
     list_rows,
 )
-from deeporigin.managed_data.client import DeepOriginClient
+from deeporigin.managed_data.client import Client
+from deeporigin.managed_data.schema import DatabaseReturnType, IDFormat
 from deeporigin.utils import PREFIX
 
-id_format = Literal["human-id", "system-id"]
-
-DatabaseReturnType = Literal["dataframe", "dict"]
-
 
 @beartype
 def get_tree(
     *,
     include_rows: bool = True,
-    client: Optional[DeepOriginClient] = None,
+    client: Optional[Client] = None,
 ) -> dict:
-    """construct a tree of workspaces, databases, and optionally,
-    all rows"""
+    """Construct a tree of all workspaces, databases and rows.
+
+    Returns a tree that contains all workspaces, databases and
+    (optionally) rows. The tree is returned as a dictionary,
+    and children of each object are contained in a field
+    called `children`.
+
+
+    Args:
+        include_rows: If `True`, rows are included in the tree.
+
+    Returns:
+        A dictionary describing the tree structure of all workspaces
+        and databases.
+
+    """
 
     if include_rows:
         # we need to fetch everything, so use a single call
         objects = list_rows(client=client)
         rows = [obj for obj in objects if obj["type"] == "row"]
         workspaces = [obj for obj in objects if obj["type"] == "workspace"]
         databases = [obj for obj in objects if obj["type"] == "database"]
@@ -64,153 +75,179 @@
             _add_children(database, rows)
 
     return tree
 
 
 @beartype
 def _add_children(node: dict, objects: list[dict]) -> None:
-    """helper function to add children to a node from a list
-    of objects"""
+    """Internal function to add children to a node
+
+
+    Warning: Internal function
+        Do not use this function.
+
+    """
     node["children"] = [obj for obj in objects if obj["parentId"] == node["id"]]
 
 
 @beartype
-def get_cell_data(*, row_id: str, column_name: str):
-    """extract data from a cell in a database, referenced
-    by row_id and column_name"""
+def get_cell_data(
+    *,
+    row_id: str,
+    column_name: str,
+    client: Optional[Client] = None,
+) -> Any:
+    """Extract data from a cell in a database, referenced
+    by `row_id` and `column_name`.
+
+    Returns the value in a single cell in a database.
+
+    Warning: Caution
+        This function internally calls
+        [get_row_data][src.managed_data.api.get_row_data],
+        so it is not efficient to write a loop to get all values
+        of cells from a row. It will be faster to call
+        [get_row_data][src.managed_data.api.get_row_data] directly.
+
+
+    Args:
+        row_id: ID (or human ID) of a row.
+        column_name: Name of column.
 
-    data = get_row_data(row_id)
+    Returns:
+        Value of that cell.
+
+    """
+
+    data = get_row_data(row_id, client=client)
     return data[column_name]
 
 
 @beartype
 def download(
     source: str,
     destination: str,
     *,
     include_files: bool = False,
-):
-    """download resources from source and save to destination"""
+    client: Optional[Client] = None,
+) -> None:
+    """Download resources from Deep Origin and save them to
+    a local destination.
+
+    Download databases, objects and other entities from
+    Deep Origin managed data and save them to local disk.
+
+    Info: Work in progress
+        All features in this function have not been implemented yet.
+
+
+    Args:
+        source: ID (or human ID) of a resource on Deep Origin.
+        destination: Path to local directory to save resources.
+        include_files: if `True`, download files in database.
+
+    """
 
     if not os.path.isdir(destination):
         raise DeepOriginException(f"{destination} should be a path to a folder.")
 
     source = source.replace(PREFIX, "")
 
     # first, need to determine what this is.
-    obj = describe_row(source)
+    obj = describe_row(source, client=client)
     if obj["type"] == "database":
         download_database(
             obj,
             destination,
             include_files=include_files,
+            client=client,
         )
     else:
         raise NotImplementedError(
             "Downloading this type of data object has not been implemented yet"
         )
 
 
 @beartype
 def download_database(
     source: Union[str, dict],
-    destination: str,
+    destination: str = os.getcwd(),
     *,
     include_files: bool = False,
+    client: Optional[Client] = None,
 ) -> None:
-    """download a database and save it to a CSV
+    """Download a database and save it to a CSV file on the local disk.
+
+    Download a database from Deep Origin managed data
+    and save to local disk as a CSV file.
+
+    Args:
+        source: ID (or human ID) of a resource on Deep Origin.
+        destination: Path to local directory to save resources.
+        include_files: if `True`, download files in database.
 
-    if include_files is True, files are also downloaded
-        and saved to the same folder as the CSV is in
     """
 
     if not os.path.isdir(destination):
         raise DeepOriginException(f"{destination} should be a path to a folder.")
 
     if isinstance(source, str):
-        source = describe_row(source)
+        source = describe_row(source, client=client)
+    elif not {"hid", "id"}.issubset(set(list(source.keys()))):
+        raise DeepOriginException(
+            f"If `source` is a dictionary, expected it contain the `hid` and `id` keys. These keys were not found. Instead, the keys are: {source.keys()}"
+        )
 
     database_id = source["id"]
     database_hid = source["hid"]
-    df = get_dataframe(database_id, use_file_names=True)
+    df = get_dataframe(
+        database_id,
+        use_file_names=True,
+        client=client,
+    )
 
     # now download all files in the database
     if include_files:
         file_ids = df.attrs["file_ids"]
 
         for file_id in file_ids:
-            download_file(file_id, destination)
+            download_file(file_id, destination, client=client)
 
     df.to_csv(os.path.join(destination, database_hid + ".csv"))
 
 
 @beartype
-def upload(source: str, destination: str) -> None:
-    """upload resources from source to destination"""
-
-    pass
-
-
-@beartype
-def get_children(
-    objects: Optional[Union[list[dict], str]] = None,
-) -> list[dict]:
-    """recursively find all workspaces, databases, rows"""
-
-    if objects is None:
-        objects = list_rows(parent_is_root=True)
-    elif isinstance(objects, str):
-        # need to convert a string to a object
-        obj = describe_row(objects)
-        obj = {key: obj[key] for key in ["id", "name", "type", "hid"]}
-        objects = [obj]
-
-    # TODO parallelize this using async/await
-    for obj in objects:
-        if obj["type"] == "row":
-            # this object is a row, and we assume that
-            # rows cannot have children, so we're going to
-            # skip this and assume this is a leaf node
-            continue
-
-        children = list_rows(parent_id=obj["id"])
-        if len(children) == 0:
-            continue
-        obj["children"] = get_children(children)
-
-    return objects
-
-
-@beartype
 def get_dataframe(
     database_id: str,
     *,
     use_file_names: bool = True,
-    reference_format: id_format = "human-id",
-    client: Optional[DeepOriginClient] = None,
+    reference_format: IDFormat = "human-id",
     return_type: DatabaseReturnType = "dataframe",
+    client: Optional[Client] = None,
 ):
-    """return a dataframe of all rows in a database
+    """Generate a `pandas.DataFrame` or dictionary for a database.
 
-    Arguments:
-    -database_id: ID of database
-    -use_file_name: if True, cells containing files will
-        contain the name of the original uploaded file.
-        if False, fileIDs are used
+    Download a database from Deep Origin managed data
+    and return it as a data frame or dictionary.
 
+    Args:
+        database_id: ID (or human ID) of a database on Deep Origin.
+        use_file_names: If `True`, refer to files by name rather than ID.
+        reference_format: Refer to rows on Deep Origin using human IDs or system IDs.
+        return_type: Whether to return a `pandas.Dataframe` or a dictionary.
     """
 
     # figure out the rows
     rows = list_database_rows(database_id, client=client)
 
     # figure out the column names and ID of the database
     response = describe_row(database_id, client=client)
     assert (
         response["type"] == "database"
-    ), "Expected database_id to resolve to a database"
+    ), f"Expected database_id: {database_id} to resolve to a database, but instead, it resolved to a {response['type']}"
 
     columns = response["cols"]
     database_id = response["id"]
     row_id = response["hidPrefix"] + "-id"
 
     # make a dictionary with all data in the database
     data = dict()
@@ -276,17 +313,21 @@
 def _parse_column_value(
     *,
     column: dict,
     fields: list[dict],
     file_ids: list,
     reference_ids: list,
     use_file_names: bool,
-    reference_format: id_format,
+    reference_format: IDFormat,
 ):
-    """utility function to parse value of a column"""
+    """Internal function parse column values
+
+    Warning: Internal function
+        Do not use this function.
+    """
 
     value = [field["value"] for field in fields if field["columnId"] == column["id"]]
 
     # special treatment for some column types
     if column["type"] == "select" and len(value) == 1:
         value = value[0]["selectedOptions"]
     elif column["type"] == "file" and len(value) == 1:
@@ -312,16 +353,19 @@
 
 
 @beartype
 def _type_and_cleanup_dataframe(
     df,  # pd.Dataframe, not typed to avoid pandas import
     columns: list[dict],
 ):
-    """utility function to clean up the dataframe and
-    make it more usable"""
+    """Internal function to type and clean a pandas dataframe
+
+    Warning: Internal function
+        Do not use this function.
+    """
 
     # this import is here because we don't want to
     # import pandas unless we actually use this function
     import pandas as pd
 
     column_mapper = dict()
     for column in columns:
@@ -352,20 +396,25 @@
     return df
 
 
 @beartype
 def get_columns(
     row_id: str,
     *,
-    client: Optional[DeepOriginClient] = None,
+    client: Optional[Client] = None,
 ) -> list[dict]:
-    """return column information.
+    """Get information about the columns of a row or database.
 
-    if row_id is a database, then column metadata and names are returned.
-    if row_id is a row, then a dictionary of hids and values are returned"""
+    If `row_id` is a database, then column metadata and names
+    are returned. If `row_id` is a row, then a dictionary of
+    human IDs and values are returned.
+
+    Args:
+        row_id: ID (or human ID) of a row or database on Deep Origin.
+    """
 
     response = describe_row(row_id, fields=True, client=client)
 
     assert response["type"] in [
         "row",
         "database",
     ], "Expected row_id to resolve to a row or a database"
@@ -378,34 +427,42 @@
 
 
 @beartype
 def get_row_data(
     row_id: str,
     *,
     use_column_keys: bool = False,
-    client: Optional[DeepOriginClient] = None,
+    client: Optional[Client] = None,
 ) -> dict:
-    """name needs improving? this returns fields in this
-    row as a dictionary, where keys are HIDs
+    """Get the data in a row.
 
-    if row_id is not a row, an error is raised.
+    Read data from a row, and return it as a dictionary, where
+    the keys are column names (or keys), and the values are the values of those
+    cells.
+
+    Args:
+        row_id: ID (or human ID) of a row or database on Deep Origin.
+        use_column_keys: if `True`, keys of dictionary are column keys.
+
+    Raises:
+        DeepOriginException: If row_id is not a row
     """
 
     response = describe_row(row_id, fields=True, client=client)
 
     if response["type"] != "row":
-        raise ValueError(
+        raise DeepOriginException(
             f"Expected `row_id` to resolve to a row, instead, it resolves to a `{response['type']}`"
         )
 
     # ask parent for column names
     parent_response = describe_row(response["parentId"], client=client)
 
     if parent_response["type"] != "database":
-        raise ValueError(
+        raise DeepOriginException(
             f"Expected parent of `{row_id}` to resolve to a database, instead, it resolves to a `{parent_response['type']}`"
         )
 
     # make a dictionary from column IDs to column names
     column_name_mapper = dict()
     column_cardinality_mapper = dict()
     for col in parent_response["cols"]:
@@ -415,14 +472,18 @@
             column_name_mapper[col["id"]] = col["name"]
         column_cardinality_mapper[col["id"]] = col["cardinality"]
 
     # now use this to construct the required dictionary
     row_data = dict()
     for field in response["fields"]:
         column_id = field["columnId"]
+
+        if "value" not in field:
+            continue
+
         value = field["value"]
         if isinstance(value, dict):
             if "selectedOptions" in value.keys():
                 value = value["selectedOptions"]
             elif "fileIds" in value.keys():
                 value = value["fileIds"]
 
@@ -432,16 +493,29 @@
         row_data[column_name_mapper[column_id]] = value
 
     return row_data
 
 
 @beartype
 def merge_databases(dfs: list):
-    """merge a list of databases into a single database,
-    uniting keys across databases"""
+    """Merge dataframes for multiple databases into a single dataframes.
+
+    Given a list of dataframes derived from Deep Origin databases,
+    merge them into a single dataframe, resolving cross-references
+    across the databases.
+
+    Info: Work in progress
+        All features in this function have not been implemented yet.
+
+
+    Args:
+        dfs: List of `pandas.DataFrames`.
+
+
+    """
 
     import pandas as pd
 
     for df in dfs:
         assert isinstance(df, pd.DataFrame), "Expected a list of dataframes to merge"
 
     assert len(dfs) == 2, "For now we only support merging 2 databases"
@@ -463,11 +537,11 @@
             attrs = df[column].attrs
 
             if "referenceDatabaseRowId" in attrs.keys():
                 column_mapper[column] = cross_reference_mapper[
                     attrs["referenceDatabaseRowId"]
                 ]
 
-        df = df.rename(columns=column_mapper)
+        df.rename(columns=column_mapper, inplace=True)
 
     # for now we only support merging 2 DBs
     return dfs[0].merge(dfs[1], how="outer")
```

### Comparing `deeporigin-0.0.3/src/utils.py` & `deeporigin-0.0.4/src/utils.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/base_type.py` & `deeporigin-0.0.4/src/variables/base_type.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/core.py` & `deeporigin-0.0.4/src/variables/core.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/__init__.py` & `deeporigin-0.0.4/src/variables/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/aws_profile.py` & `deeporigin-0.0.4/src/variables/types/aws_profile.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/env_var.py` & `deeporigin-0.0.4/src/variables/types/env_var.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/file.py` & `deeporigin-0.0.4/src/variables/types/file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/git_http_credentials.py` & `deeporigin-0.0.4/src/variables/types/git_http_credentials.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/private_gpg_key.py` & `deeporigin-0.0.4/src/variables/types/private_gpg_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/private_ssh_key.py` & `deeporigin-0.0.4/src/variables/types/private_ssh_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/secret_env_var_value.py` & `deeporigin-0.0.4/src/variables/types/secret_env_var_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/secret_file_value.py` & `deeporigin-0.0.4/src/variables/types/secret_file_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/src/variables/types/xpress_license_file.py` & `deeporigin-0.0.4/src/variables/types/xpress_license_file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/tests/test_cli.py` & `deeporigin-0.0.4/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,28 @@
             with cli.App(argv=["--version"]) as app:
                 app.run()
 
         stdout = stdout_capture.getvalue().strip()
 
         self.assertEqual(__version__, stdout)
 
+    def test_data(self):
+        stdout_capture = io.StringIO()
+        stderr_capture = io.StringIO()
+
+        with redirect_stdout(stdout_capture), redirect_stderr(stderr_capture):
+            with cli.App(argv=["data"]) as app:
+                app.run()
+
+        stdout = stdout_capture.getvalue().strip()
+
+        self.assertRegex(stdout, "List data in managed data on Deep Origin")
+
     @pytest.mark.skipif(
-        sys.version_info < (3, 11), reason="requires python3.10 or higher"
+        sys.version_info < (3, 11), reason="requires python 3.10 or higher"
     )
     def test_except_hook(self):
         mock_code = MockCode("mock_filename.py", "mock_function")
         mock_frame = MockFrame(mock_code, {})
         mock_tb = MockTraceback([mock_frame], [1])
 
         cli.except_hook(sys.excepthook, DeepOriginException, "error", mock_tb)
```

### Comparing `deeporigin-0.0.3/tests/test_config.py` & `deeporigin-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/tests/test_context.py` & `deeporigin-0.0.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/tests/test_feature_flags.py` & `deeporigin-0.0.4/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.3/tests/test_managed_data.py` & `deeporigin-0.0.4/tests/test_managed_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,95 @@
 """this tests low level functions in the data API"""
 
-from dataclasses import asdict
-from typing import Optional
+import os
 
+import pandas as pd
 import pytest
 from deeporigin.exceptions import DeepOriginException
-from deeporigin.managed_data import _api, api, schema
-from deeporigin.managed_data._api import DeepOriginClient
-
-# constants
-dataframe_attr_keys = {
-    "file_ids",
-    "id",
-    "primary_key",
-    "reference_ids",
-}
-
-
-describe_file_keys = {
-    "id",
-    "uri",
-    "name",
-    "status",
-    "contentLength",
-    "contentType",
-}
-
-list_row_keys = {"id", "hid", "type", "name", "parentId"}
-
-list_database_rows_keys = {
-    "createdByUserDrn",
-    "dateCreated",
-    "dateUpdated",
-    "editedByUserDrn",
-    "fields",
-    "hid",
-    "hidNum",
-    "id",
-    "parentId",
-    "submissionStatus",
-    "type",
-    "validationStatus",
-}
-
-
-def _row_object(
-    *,
-    parentId: Optional[str] = "_row:placeholder",
-    id: str = "row:placeholder",
-    type: str = "row",
-    name: Optional[str] = None,
-    hid: str = "placeholder-1",
-) -> dict:
-    """helper function to create dummy responses"""
-    return dict(
-        id=id,
-        parentId=parentId,
-        type=type,
-        name=name,
-        hid=hid,
-    )
-
-
-class MockClient(DeepOriginClient):
-    """mock client to respond with static data"""
-
-    def invoke(self, endpoint, data):
-        """overload this function so that we can return
-        static data"""
-
-        if endpoint == "ListRows":
-            if data == dict(filters=[dict(parent=dict(id="db-sample"))]):
-                return [
-                    _row_object(hid="sample-1"),
-                    _row_object(hid="sample-2"),
-                ]
-            elif data == dict(filters=[dict(parent=dict(isRoot=True))]) or data == dict(
-                filters=[dict(rowType="workspace")]
-            ):
-                return [
-                    _row_object(
-                        type="workspace",
-                        parentId=None,
-                    )
-                ]
-
-        elif endpoint == "DescribeRow":
-            if data["rowId"].startswith("db-"):
-                # we are likely asking for a database
-                row = asdict(schema.DatabaseRowDescription())
-
-            else:
-                # we are asking for a row in a database
-                row = asdict(schema.RowDescription())
-
-                if not data["fields"]:
-                    row.pop("fields", None)
-
-            return row
-
-        elif endpoint == "ConvertIdFormat":
-            return [{"id": "_row:W6DjtaCrZ201EGLpmZtGO", "hid": "sample-1"}]
-
-        elif endpoint == "ListDatabaseRows":
-            row = asdict(schema.RowDescription())
-            row.pop("cols", None)
-            row.pop("parent", None)
-            row.pop("rowJsonSchema", None)
-
-            return [row for _ in range(5)]
-
-        elif endpoint == "DescribeFile":
-            return {
-                "id": "_file:V08GBdErNGqynC3O7bill",
-                "uri": "s3://deeporigin-nucleus-local-uploads/files/_file:V08GBdErNGqynC3O7bill",
-                "name": "pbr322_egfr (1).gb",
-                "status": "ready",
-                "contentLength": 9757,
-                "contentType": "",
-            }
-
-        elif endpoint == "DescribeDatabaseStats":
-            return {"rowCount": 5}
-        elif endpoint == "ListFiles":
-            if data == dict(filters=[dict(isUnassigned=True)]):
-                return [
-                    {
-                        "file": {
-                            "id": "_file:2n5jHmnbLC4tJShNrk6Df",
-                            "uri": "s3://deeporigin-nucleus-local-uploads/files/_file:2n5jHmnbLC4tJShNrk6Df",
-                            "name": "QC report (1).pdf",
-                            "status": "archived",
-                            "contentLength": 237478,
-                            "contentType": "application/pdf",
-                        }
-                    },
-                ]
-            elif dict(filters=[dict(isUnassigned=False)]):
-                return [
-                    {
-                        "file": {
-                            "id": "_file:Fi7dHZJHgA3nqT1y1Ro5u",
-                            "uri": "s3://deeporigin-nucleus-local-uploads/files/_file:Fi7dHZJHgA3nqT1y1Ro5u",
-                            "name": "sequence_preprocessing.pdf",
-                            "status": "ready",
-                            "contentLength": 698255,
-                            "contentType": "application/pdf",
-                        },
-                        "assignments": [
-                            {"rowId": "_row:ZEaEUIgsbHmGLVlgnxfvU"},
-                            {"rowId": "_row:aCWxUxumDFDnu8ZhmhQ0X"},
-                            {"rowId": "_row:WZVb1jsebafhfLgrHtz2l"},
-                            {"rowId": "_row:3A3okCbvuaZvEkOZLqLwY"},
-                        ],
-                    },
-                ]
+from deeporigin.managed_data import _api, api
+from deeporigin.managed_data.client import (
+    DeepOriginClient,
+    MockClient,
+    file_description,
+)
+from deeporigin.managed_data.schema import (
+    DATAFRAME_ATTRIBUTE_KEYS,
+    DescribeFileResponse,
+    DescribeRowResponseDatabase,
+    DescribeRowResponseRow,
+    ListRowsResponse,
+)
+from deeporigin.utils import PREFIX
 
 
 @pytest.fixture(scope="session", autouse=True)
 def config(pytestconfig):
     """this fixture performs some setup tasks
     before all tests are run, and runs only once"""
 
     data = dict()
 
     # set up client
     if pytestconfig.getoption("client") == "mock":
         data["client"] = MockClient()
-
-        data["databases"] = ["db-sample"]
-        data["rows"] = ["sample-1"]
+        data["mock"] = True
+        data["workspaces"] = data["client"].workspaces
+        data["databases"] = data["client"].databases
+        data["rows"] = data["client"].rows
+        data["file"] = file_description()
     else:
+        data["mock"] = False
         client = DeepOriginClient()
         client.authenticate()
         data["client"] = client
 
         # if we're going to be making requests to a live
         # instance, we need to make sensible requests
         databases = _api.list_rows(row_type="database")
         data["databases"] = [db["hid"] for db in databases]
         rows = _api.list_rows(row_type="row")
-        data["rows"] = [row["hid"] for row in rows]
+        data["rows"] = [row["hid"] for row in rows if row["type"] == "row"]
+
+        # get a list of all files
+        files = _api.list_files()
+        if len(files) > 0:
+            data["file"] = files[0]["file"]
 
     # tests run on yield
     yield data
 
     # teardown tasks, if any
 
 
 def test_list_rows(config):
     rows = _api.list_rows(
         parent_id=config["databases"][0],
         client=config["client"],
     )
 
     for row in rows:
-        assert set(row.keys()) == list_row_keys
         assert row["type"] == "row"
 
+        # check type
+        ListRowsResponse(**row)
+
 
 def test_list_rows_root_parent(config):
     root = _api.list_rows(
         parent_is_root=True,
         client=config["client"],
     )
 
     assert len(root) == 1, "Expected there to be exactly one root"
+    root = root[0]
+
+    assert root["parentId"] is None, "Expected root to have no parent"
 
-    assert root[0]["parentId"] is None, "Expected root to have no parent"
+    # check type
+    ListRowsResponse(**root)
 
 
 def test_list_rows_by_type(config):
     rows = _api.list_rows(
         row_type="workspace",
         client=config["client"],
     )
@@ -219,14 +97,17 @@
     assert len(rows) > 0, "Expected at least one workspace"
 
     for row in rows:
         assert (
             row["type"] == "workspace"
         ), f"Expected to get a list of workspaces, but {row} is not a workspace"
 
+        # check type
+        ListRowsResponse(**row)
+
 
 def test_list_files_unassigned(config):
     files = _api.list_files(
         is_unassigned=True,
         client=config["client"],
     )
 
@@ -280,59 +161,226 @@
 
     row = _api.describe_row(
         config["rows"][0],
         client=config["client"],
         fields=True,
     )
 
-    keys_with_fields = set(asdict(schema.RowDescription()).keys())
+    assert "fields" in row.keys(), "Expected to find fields in response"
 
-    assert set(row.keys()) == keys_with_fields
+    # check if we can coerce into response type
+    DescribeRowResponseRow(**row)
 
     row = _api.describe_row(
         config["rows"][0],
         client=config["client"],
         fields=False,
     )
 
-    assert set(row.keys()) == keys_with_fields.difference({"fields"})
+    assert "fields" not in row.keys(), "Expected to NOT find fields in response"
+
+    # check if we can coerce into response type
+    DescribeRowResponseRow(**row)
+
+    # database
+    row = _api.describe_row(
+        config["databases"][0],
+        client=config["client"],
+    )
+
+    # check if we can coerce into response type
+    DescribeRowResponseDatabase(**row)
 
 
 def test_convert_id_format(config):
     conversions = _api.convert_id_format(
-        hids=[config["rows"][0]],
+        hids=config["rows"],
+        client=config["client"],
+    )
+
+    system_ids = []
+    for conversion in conversions:
+        system_ids.append(conversion["id"])
+        assert {"id", "hid"} == set(conversion.keys())
+
+    conversions = _api.convert_id_format(
+        ids=system_ids,
         client=config["client"],
     )
+
     for conversion in conversions:
         assert {"id", "hid"} == set(conversion.keys())
 
     with pytest.raises(DeepOriginException, match="non-None and a list of strings"):
         _api.convert_id_format()
 
 
 def test_list_database_rows(config):
     rows = _api.list_database_rows(
         config["databases"][0],
         client=config["client"],
     )
 
+    # coerce into type
     for row in rows:
-        assert set(row.keys()).difference({"name"}) == list_database_rows_keys
+        DescribeRowResponseRow(**row)
 
 
 def test_get_dataframe(config):
     df = api.get_dataframe(
         config["databases"][0],
         client=config["client"],
     )
 
+    assert isinstance(df, pd.DataFrame), "Expected return type to be a pandas Dataframe"
+
     assert (
-        set(df.attrs.keys()) == dataframe_attr_keys
-    ), f"Expected to find a dictionary in `df.attrs` with these keys: {dataframe_attr_keys}, instead found a dictionary with these keys: {df.attrs.keys()}"
+        set(df.attrs.keys()) == DATAFRAME_ATTRIBUTE_KEYS
+    ), f"Expected to find a dictionary in `df.attrs` with these keys: {DATAFRAME_ATTRIBUTE_KEYS}, instead found a dictionary with these keys: {df.attrs.keys()}"
 
     assert (
         "Validation Status" in df.columns
     ), f"Expected to find a column called `Validation Status` in the dataframe. Instead, the columns in this dataframe are: {df.columns}"
 
     assert (
         df.attrs["primary_key"] in df.columns
     ), "Expected to find the primary key as a column"
+
+    data = api.get_dataframe(
+        config["databases"][0],
+        client=config["client"],
+        return_type="dict",
+    )
+
+    assert isinstance(data, dict), "Expected return type to be a dict"
+
+
+def test_list_mentions(config):
+    data = _api.list_mentions(
+        config["rows"][0],
+        client=config["client"],
+    )
+
+    assert (
+        "mentions" in data.keys()
+    ), "Expected to find a dictionary with the key `mentions`"
+
+    assert isinstance(data["mentions"], list), "Expected `mentions` to be a list"
+
+
+def test_get_tree(config):
+    tree = api.get_tree(client=config["client"])
+
+    assert tree["parentId"] is None, "Expected the root of the tree to have no parent"
+
+    tree.pop("children")
+    ListRowsResponse(**tree)
+
+    tree = api.get_tree(client=config["client"], include_rows=False)
+    assert tree["parentId"] is None, "Expected the root of the tree to have no parent"
+
+    tree.pop("children")
+    ListRowsResponse(**tree)
+
+
+def test_create_file_download_url(config):
+    file_id = config["file"]["id"]
+    data = _api.create_file_download_url(
+        file_id,
+        client=config["client"],
+    )
+
+    assert (
+        "downloadUrl" in data.keys()
+    ), "Expected to find `downloadUrl` in data response"
+
+
+def test_download_file(config):
+    if "file" not in config.keys():
+        return
+
+    file_id = config["file"]["id"]
+
+    if config["mock"]:
+        _api.download_file(file_id, client=config["client"])
+        os.remove("placeholder")
+
+        with pytest.raises(DeepOriginException, match="should be a path to a folder"):
+            _api.download_file(
+                file_id,
+                client=config["client"],
+                destination="non-existent-path",
+            )
+
+    else:
+        _api.download_file(file_id, client=config["client"])
+
+
+def test_describe_file(config):
+    file_id = config["file"]["id"]
+
+    data = _api.describe_file(file_id, client=config["client"])
+
+    assert isinstance(data, dict), "Expected response to be a dict"
+
+    DescribeFileResponse(**data)
+
+
+def test_get_row_data(config):
+    row_id = config["rows"][0]
+
+    data = api.get_row_data(row_id, client=config["client"])
+    assert isinstance(data, dict), "Expected response to be a dict"
+
+    data = api.get_row_data(
+        row_id,
+        client=config["client"],
+        use_column_keys=True,
+    )
+    assert isinstance(data, dict), "Expected response to be a dict"
+
+
+def test_get_cell_data(config):
+    row_id = config["rows"][0]
+    data = api.get_row_data(row_id, client=config["client"])
+    column_name = list(data.keys())[0]
+    data = api.get_cell_data(
+        row_id=row_id,
+        column_name=column_name,
+        client=config["client"],
+    )
+
+
+def test_download_database(config):
+    db_id = config["databases"][0]
+    api.download_database(
+        db_id,
+        include_files=False,
+        client=config["client"],
+    )
+
+    file_name = db_id + ".csv"
+    assert os.path.exists(file_name), f"Expected to find a CSV file called {file_name}"
+    os.remove(file_name)
+
+
+def test_download(config):
+    db_id = config["databases"][0]
+    api.download(
+        db_id,
+        destination=os.getcwd(),
+        client=config["client"],
+    )
+
+    file_name = db_id + ".csv"
+    assert os.path.exists(file_name), f"Expected to find a CSV file called {file_name}"
+    os.remove(file_name)
+
+    api.download(
+        f"{PREFIX}{db_id}",
+        destination=os.getcwd(),
+        client=config["client"],
+    )
+
+    file_name = db_id + ".csv"
+    assert os.path.exists(file_name), f"Expected to find a CSV file called {file_name}"
+    os.remove(file_name)
```

### Comparing `deeporigin-0.0.3/tests/test_variables.py` & `deeporigin-0.0.4/tests/test_variables.py`

 * *Files identical despite different names*

