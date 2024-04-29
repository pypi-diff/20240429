# Comparing `tmp/prismacloud-cli-0.8.6.tar.gz` & `tmp/prismacloud_cli-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud-cli-0.8.6.tar", last modified: Fri Apr 12 12:58:31 2024, max compression
+gzip compressed data, was "prismacloud_cli-0.8.7.tar", last modified: Mon Apr 29 15:23:04 2024, max compression
```

## Comparing `prismacloud-cli-0.8.6.tar` & `prismacloud_cli-0.8.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.136698 prismacloud-cli-0.8.6/prismacloud/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.140698 prismacloud-cli-0.8.6/prismacloud/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.140698 prismacloud-cli-0.8.6/prismacloud/cli/cspm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_current.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_pov.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_rql.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_saas_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.144698 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_audits.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_defenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_incidents.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/prismacloud/cli/pccs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_reviews.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.514956 prismacloud_cli-0.8.7/prismacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.518956 prismacloud_cli-0.8.7/prismacloud/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.518956 prismacloud_cli-0.8.7/prismacloud/cli/cspm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_pov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_rql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_saas_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.522956 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_audits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.522956 prismacloud_cli-0.8.7/prismacloud/cli/pccs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/prismacloud/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 15:23:04.000000 prismacloud_cli-0.8.7/prismacloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:23:04.526956 prismacloud_cli-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-29 15:22:23.000000 prismacloud_cli-0.8.7/tests/test_cli.py
```

### Comparing `prismacloud-cli-0.8.6/LICENSE` & `prismacloud_cli-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/PKG-INFO` & `prismacloud_cli-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.8.6
+Version: 0.8.7
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prismacloud-cli-0.8.6/README.md` & `prismacloud_cli-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/__init__.py` & `prismacloud_cli-0.8.7/prismacloud/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/api.py` & `prismacloud_cli-0.8.7/prismacloud/cli/api.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_alert.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_alert.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import logging
 import click
+import datetime
 
 from prismacloud.cli import cli_output, pass_environment
 from prismacloud.cli.api import pc_api
 from urllib.parse import quote
 
 
+# Helper function to convert epoch (in milliseconds) to a datetime object
+def convert_epoch_to_datetime(epoch_ms):
+    return datetime.datetime.fromtimestamp(int(epoch_ms) / 1000)
+
+
+# Helper function to convert datetime to human-readable format
+def datetime_to_readable(dt):
+    return dt.strftime("%Y-%m-%d %H:%M:%S")
+
+
 @click.group(
     "alert", short_help="[CSPM] Returns a list of alerts that match the constraints specified in the query parameters."
 )
 @pass_environment
 def cli(ctx):
     pass
 
@@ -24,15 +35,18 @@
 @click.option(
     "--unit", default="day", type=click.Choice(["minute", "hour", "day", "week", "month", "year"], case_sensitive=False)
 )
 @click.option(
     "--status", default="open", type=click.Choice(["open", "resolved", "snoozed", "dismissed"], case_sensitive=False)
 )
 @click.option("--detailed/--no-detailed", default=False)
-def list_alerts(compliance_standard, cloud_account, account_group, amount, unit, status, detailed, policy_id, alert_rule):
+@click.option("--days-ahead", default=0, type=int, help="Filter alerts that are dismissing until the next X days.")
+def list_alerts(
+    compliance_standard, cloud_account, account_group, amount, unit, status, detailed, policy_id, alert_rule, days_ahead
+):
     """Returns a list of alerts from the Prisma Cloud platform"""
     data = {
         "alert.status": status,
         "alertRule.name": alert_rule,
         "detailed": detailed,
         "limit": "10000",
         "policy.complianceStandard": compliance_standard,
@@ -49,20 +63,36 @@
 
     if account_group:
         data["account.group"] = account_group
 
     # Fetch the alerts
     alerts = pc_api.get_endpoint("alert", query_params=data, api="cspm")
 
+    if days_ahead > 0 and status == "snoozed":
+        # Calculate future date for filter only if days_ahead > 0 and status is 'snoozed'
+        future_date = datetime.datetime.now() + datetime.timedelta(days=days_ahead)
+
+        # Filter alerts where dismissalUntilTs is before the future date
+        alerts = [
+            alert
+            for alert in alerts
+            if "dismissalUntilTs" in alert and convert_epoch_to_datetime(alert["dismissalUntilTs"]) < future_date
+        ]
+
     # Try to add a new column with a url to the alert investigate page
     base_url = f"https://{pc_api.api.replace('api', 'app')}/alerts/overview?viewId=default"
 
     for alert in alerts:
         try:
             alert_id = alert["id"]
+
+            for key in ["firstSeen", "lastSeen", "alertTime", "lastUpdated", "eventOccurred", "dismissalUntilTs"]:
+                if key in alert:
+                    alert[key] = datetime_to_readable(convert_epoch_to_datetime(alert[key]))
+
             # Correctly using double braces for literal curly braces in f-string
             filters = (
                 f'{{"timeRange":{{"type":"to_now","value":"epoch"}},'
                 f'"timeRange.type":"ALERT_OPENED","alert.status":["open"],'
                 f'"alert.id":["{alert_id}"]}}'
             )
             # Encoding the filters part
```

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_cloud.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_compliance.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_compliance.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_iam.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_iam.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_inventory.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_inventory.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_licenses.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_licenses.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_policy.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_policy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_pov.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_pov.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_resource.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_resource.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_rql.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_rql.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_saas_version.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cspm/cmd_saas_version.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_audits.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_containers.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_defenders.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_discovery.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_discovery.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_host_auto_deploy.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_host_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_hosts.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_images.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_incidents.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_incidents.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_logs.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_monitor.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_monitor.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_policies.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_registry.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_scans.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_stats.py` & `prismacloud_cli-0.8.7/prismacloud/cli/cwpp/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_repositories.py` & `prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_suppressions.py` & `prismacloud_cli-0.8.7/prismacloud/cli/pccs/cmd_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/prismacloud_cli.egg-info/PKG-INFO` & `prismacloud_cli-0.8.7/prismacloud_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.8.6
+Version: 0.8.7
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prismacloud-cli-0.8.6/prismacloud_cli.egg-info/SOURCES.txt` & `prismacloud_cli-0.8.7/prismacloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/setup.py` & `prismacloud_cli-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.6/tests/test_cli.py` & `prismacloud_cli-0.8.7/tests/test_cli.py`

 * *Files identical despite different names*

