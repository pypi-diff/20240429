# Comparing `tmp/launch-cli-0.4.1.tar.gz` & `tmp/launch_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launch-cli-0.4.1.tar", last modified: Tue Apr  9 19:05:11 2024, max compression
+gzip compressed data, was "launch_cli-0.5.0.tar", last modified: Mon Apr 29 17:07:21 2024, max compression
```

## Comparing `launch-cli-0.4.1.tar` & `launch_cli-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 19:04:59.000000 launch-cli-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-09 19:05:11.935057 launch-cli-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-09 19:04:59.000000 launch-cli-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/launch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 19:04:59.000000 launch-cli-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:05:11.935057 launch-cli-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.923057 launch-cli-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/common/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/helm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/helm/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/aws/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/provider/az/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/az/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/az/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/terragrunt/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/access/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/access/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/hooks/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/repo/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/repo/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/version/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/version/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/helm/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/helm/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/service/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/service/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/terragrunt/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/src/launch/local_repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/src/launch/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.414942 launch_cli-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 17:07:08.000000 launch_cli-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-04-29 17:07:21.414942 launch_cli-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-29 17:07:08.000000 launch_cli-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/launch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 17:07:08.000000 launch_cli-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:07:21.414942 launch_cli-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.398942 launch_cli-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/common/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/helm/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/aws/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/provider/az/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/az/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/az/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/terragrunt/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/access/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/access/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/hooks/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/repo/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/version/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/cli/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/helm/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/service/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/cli/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/terragrunt/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/local_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/update.py
```

### Comparing `launch-cli-0.4.1/LICENSE` & `launch_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/PKG-INFO` & `launch_cli-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.4.1
+Version: 0.5.0
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 Requires-Dist: ruamel.yaml>=0.17.32
 Provides-Extra: dev
 Requires-Dist: pytest~=7.0; extra == "dev"
 Requires-Dist: pytest-mock~=3.0; extra == "dev"
 Requires-Dist: responses~=0.24.0; extra == "dev"
 Requires-Dist: black>=23.11.0; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
+Requires-Dist: faker>=24.14; extra == "dev"
 
 # Launch CLI
 
 Simple CLI utility for common Launch tasks. This is intended to be built upon as new tasks are discovered.
 
 ## Prerequisites
```

### Comparing `launch-cli-0.4.1/README.md` & `launch_cli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/launch_cli.egg-info/PKG-INFO` & `launch_cli-0.5.0/launch_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.4.1
+Version: 0.5.0
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 Requires-Dist: ruamel.yaml>=0.17.32
 Provides-Extra: dev
 Requires-Dist: pytest~=7.0; extra == "dev"
 Requires-Dist: pytest-mock~=3.0; extra == "dev"
 Requires-Dist: responses~=0.24.0; extra == "dev"
 Requires-Dist: black>=23.11.0; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
+Requires-Dist: faker>=24.14; extra == "dev"
 
 # Launch CLI
 
 Simple CLI utility for common Launch tasks. This is intended to be built upon as new tasks are discovered.
 
 ## Prerequisites
```

### Comparing `launch-cli-0.4.1/launch_cli.egg-info/SOURCES.txt` & `launch_cli-0.5.0/launch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/pyproject.toml` & `launch_cli-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launch-cli"
-version = "0.4.1"
+version = "0.5.0"
 description = "CLI tooling for common Launch functions"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -16,15 +16,15 @@
 Homepage = "https://github.com/launchbynttdata/launch-cli"
 Issues = "https://github.com/launchbynttdata/launch-cli/issues"
 
 [tool.setuptools]
 package-dir = {launch="src/launch"}
 
 [project.optional-dependencies]
-dev = ["pytest~=7.0", "pytest-mock~=3.0", "responses~=0.24.0", "black>=23.11.0", "isort>=5.12.0"]
+dev = ["pytest~=7.0", "pytest-mock~=3.0", "responses~=0.24.0", "black>=23.11.0", "isort>=5.12.0", "faker>=24.14"]
 
 [project.scripts]
 launch = "launch.cli.entrypoint:cli"
 
 [tool.isort]
 profile = "black"
```

### Comparing `launch-cli-0.4.1/src/launch/__init__.py` & `launch_cli-0.5.0/src/launch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from semver import Version
 
-VERSION = "0.4.1"
+VERSION = "0.5.0"
 
 SEMANTIC_VERSION = Version.parse(VERSION)
 GITHUB_ORG_NAME = "launchbynttdata"
 GITHUB_REPO_NAME = "launch-cli"
-SERVICE_SKELETON = "https://github.com/launchbynttdata/launch-terragrunt-skeleton.git"
+SERVICE_SKELETON = "https://github.com/launchbynttdata/lcaf-skeleton-terragrunt.git"
 SKELETON_BRANCH = "main"
 MAIN_BRANCH = "main"
 INIT_BRANCH = "feature/init"
 BUILD_DEPENDENCIES_DIR = ".launch"
 CODE_GENERATION_DIR_SUFFIX = "-singleRun"
 DISCOVERY_FORBIDDEN_DIRECTORIES = [
     ".git",
```

### Comparing `launch-cli-0.4.1/src/launch/automation/common/functions.py` & `launch_cli-0.5.0/src/launch/automation/common/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/automation/helm/functions.py` & `launch_cli-0.5.0/src/launch/automation/helm/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/automation/provider/aws/functions.py` & `launch_cli-0.5.0/src/launch/automation/provider/aws/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/automation/provider/az/functions.py` & `launch_cli-0.5.0/src/launch/automation/provider/az/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/automation/terragrunt/functions.py` & `launch_cli-0.5.0/src/launch/automation/terragrunt/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/entrypoint.py` & `launch_cli-0.5.0/src/launch/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/github/access/commands.py` & `launch_cli-0.5.0/src/launch/cli/github/access/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/github/hooks/commands.py` & `launch_cli-0.5.0/src/launch/cli/github/hooks/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/github/repo/commands.py` & `launch_cli-0.5.0/src/launch/cli/github/repo/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/github/version/commands.py` & `launch_cli-0.5.0/src/launch/cli/github/version/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/helm/commands.py` & `launch_cli-0.5.0/src/launch/cli/helm/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/cli/service/commands.py` & `launch_cli-0.5.0/src/launch/cli/service/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -173,14 +173,92 @@
         path=Path(f"{service_path}/.launch_config"),
     )
     if not skip_commit:
         push_branch(repository=repository, branch=remote_branch, commit_msg=git_message)
 
 
 @click.command()
+@click.option("--name", required=True, help="Name of the service to  be created.")
+@click.option(
+    "--in-file",
+    required=True,
+    type=click.File("r"),
+    help="Inputs to be used with the skeleton during creation.",
+)
+@click.option(
+    "--no-uuid",
+    is_flag=True,
+    default=False,
+    help="If set, it will not generate a UUID to be used in skeleton files.",
+)
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    default=False,
+    help="Perform a dry run that reports on what it would do, but does not create webhooks.",
+)
+def create_no_git(
+    name: str,
+    in_file: IO[Any],
+    no_uuid: bool,
+    dry_run: bool,
+):
+    """Creates a new service without any Git interactions."""
+
+    if dry_run:
+        click.secho("Performing a dry run, nothing will be created", fg="yellow")
+        # TODO: add a dry run for the create command
+        return
+
+    service_path = f"{Path.cwd()}/{name}"
+    input_data = json.load(in_file)
+    input_data = input_data_validation(input_data)
+
+    needs_create = not Path(service_path).exists()
+    if needs_create:
+        Path(service_path).mkdir(exist_ok=False)
+    is_service_path_git_repo = (
+        Path(service_path).joinpath(".git").exists()
+        and Path(service_path).joinpath(".git").is_dir()
+    )
+
+    traverse_with_callback(
+        dictionary=input_data["platform"],
+        callback=callback_create_directories,
+        base_path=f"{service_path}/{BUILD_DEPENDENCIES_DIR}/",
+    )
+
+    input_data["platform"] = traverse_with_callback(
+        dictionary=input_data["platform"],
+        callback=callback_copy_properties_files,
+        base_path=f"{service_path}/{BUILD_DEPENDENCIES_DIR}/",
+        uuid=not no_uuid,
+    )
+    write_text(
+        data=input_data,
+        path=Path(f"{service_path}/.launch_config"),
+    )
+    click.echo(f"Service configuration files have been written to {service_path}")
+
+    if is_service_path_git_repo:
+        click.echo(
+            f"{service_path} appears to be a git repository! You will need to add, commit, and push these files manually."
+        )
+    else:
+        if needs_create:
+            click.echo(
+                f"{service_path} was created, but has not yet been initialized as a git repository. You will need to initialize it."
+            )
+        else:
+            click.echo(
+                f"{service_path} already existed, but has not yet been initialized as a git repository. You will need to initialize it."
+            )
+
+
+@click.command()
 @click.option(
     "--organization",
     default=GITHUB_ORG_NAME,
     help=f"GitHub organization containing your repository. Defaults to the {GITHUB_ORG_NAME} organization.",
 )
 @click.option("--name", required=True, help="Name of the service to  be created.")
 @click.option(
@@ -325,67 +403,61 @@
 @click.option(
     "--skip-git",
     is_flag=True,
     default=False,
     help="If set, it will ignore cloning and checking out the git repository and it's properties.",
 )
 @click.option(
-    "--work-dir",
-    default=Path.cwd(),
-    help="The work directory to generate launch platform files. Defaults to the current directory.",
-)
-@click.option(
     "--dry-run",
     is_flag=True,
     default=False,
     help="Perform a dry run that reports on what it would do, but does not create webhooks.",
 )
 # TODO: Optimize this function and logic
 # Ticket: 1633
 def generate(
     organization: str,
     name: str,
     service_branch: str,
     skip_git: bool,
-    work_dir: Path,
     dry_run: bool,
 ):
     """Dynamically generates terragrunt files based off a service."""
 
     if dry_run:
         click.secho("Performing a dry run, nothing will be created", fg="yellow")
 
-    singlerun_path = f"{work_dir}/{name}{CODE_GENERATION_DIR_SUFFIX}"
     service_path = f"{Path.cwd()}/{name}"
+    singlerun_path = f"{service_path}{CODE_GENERATION_DIR_SUFFIX}"
 
     if Path(singlerun_path).exists():
         click.secho(
             f"Generation repo {singlerun_path} already exist locally. Please remove this directory or run launch service cleanup.",
             fg="red",
         )
         return
 
-    g = get_github_instance()
-    repo = g.get_repo(f"{organization}/{name}")
-
     if not skip_git:
+        g = get_github_instance()
+        repo = g.get_repo(f"{organization}/{name}")
+
         clone_repository(
             repository_url=repo.clone_url,
-            target=f"{work_dir}/{name}",
+            target=name,
             branch=service_branch,
         )
     else:
         if not Path(service_path).exists():
             click.secho(
                 f"Service repo {service_path} does not exist locally. Please remove the --skip-git flag to clone and continue generation.",
                 fg="red",
             )
             return
 
-    with open(f"{work_dir}/{name}/.launch_config", "r") as f:
+    with open(f"{name}/.launch_config", "r") as f:
         input_data = json.load(f)
         input_data = input_data_validation(input_data)
 
     clone_repository(
         repository_url=input_data["skeleton"]["url"],
         target=singlerun_path,
         branch=input_data["skeleton"]["tag"],
@@ -426,36 +498,33 @@
     # Remove the .launch directory
     shutil.rmtree(f"{singlerun_path}/.launch")
 
 
 @click.command()
 @click.option("--name", required=True, help="Name of the service to  be created.")
 @click.option(
-    "--work-dir",
-    default=Path.cwd(),
-    help="The work directory to clean the launch generated files from. Defaults to the current directory.",
-)
-@click.option(
     "--dry-run",
     is_flag=True,
     default=False,
     help="Perform a dry run that reports on what it would do, but does not create webhooks.",
 )
 def cleanup(
     name: str,
-    work_dir: Path,
     dry_run: bool,
 ):
     """Cleans up launch-cli reources that are created from code generation."""
 
     if dry_run:
         click.secho("Performing a dry run, nothing will be cleaned", fg="yellow")
         return
 
+    code_generation_dir_name = f"{name}{CODE_GENERATION_DIR_SUFFIX}"
+    code_generation_path = Path.cwd().joinpath(code_generation_dir_name)
+
     try:
-        shutil.rmtree(f"{work_dir}/{name}{CODE_GENERATION_DIR_SUFFIX}")
-        logger.info(f"Deleted {work_dir}/{name}{CODE_GENERATION_DIR_SUFFIX} directory.")
+        shutil.rmtree(code_generation_path)
+        logger.info(f"Deleted the {code_generation_path} directory.")
     except FileNotFoundError:
         click.secho(
-            f"Repository not found: {work_dir}/{name}{CODE_GENERATION_DIR_SUFFIX}",
+            f"Directory not found: {code_generation_path}",
             fg="red",
         )
```

### Comparing `launch-cli-0.4.1/src/launch/cli/terragrunt/commands.py` & `launch_cli-0.5.0/src/launch/cli/terragrunt/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/env.py` & `launch_cli-0.5.0/src/launch/env.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/github/access.py` & `launch_cli-0.5.0/src/launch/github/access.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/github/auth.py` & `launch_cli-0.5.0/src/launch/github/auth.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/github/hooks.py` & `launch_cli-0.5.0/src/launch/github/hooks.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/github/repo.py` & `launch_cli-0.5.0/src/launch/github/repo.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/github/tags.py` & `launch_cli-0.5.0/src/launch/github/tags.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/local_repo/predict.py` & `launch_cli-0.5.0/src/launch/local_repo/predict.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/local_repo/repo.py` & `launch_cli-0.5.0/src/launch/local_repo/repo.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/local_repo/tags.py` & `launch_cli-0.5.0/src/launch/local_repo/tags.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/service/common.py` & `launch_cli-0.5.0/src/launch/service/common.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.1/src/launch/update.py` & `launch_cli-0.5.0/src/launch/update.py`

 * *Files identical despite different names*

