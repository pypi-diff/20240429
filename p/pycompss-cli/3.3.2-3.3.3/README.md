# Comparing `tmp/pycompss-cli-3.3.2.tar.gz` & `tmp/pycompss-cli-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompss-cli-3.3.2.tar", last modified: Tue Jan  9 13:48:18 2024, max compression
+gzip compressed data, was "pycompss-cli-3.3.3.tar", last modified: Mon Apr 29 12:19:09 2024, max compression
```

## Comparing `pycompss-cli-3.3.2.tar` & `pycompss-cli-3.3.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.594781 pycompss-cli-3.3.2/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11406 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/LICENSE.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      266 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/MANIFEST.in
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4067 2024-01-09 13:48:18.594781 pycompss-cli-3.3.2/PKG-INFO
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     3144 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/README.rst
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)        6 2024-01-09 11:38:47.000000 pycompss-cli-3.3.2/VERSION.txt
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.564781 pycompss-cli-3.3.2/pycompss_cli/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/__init__.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.574781 pycompss-cli-3.3.2/pycompss_cli/assets/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/assets/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    25356 2023-05-08 14:01:10.000000 pycompss-cli-3.3.2/pycompss_cli/assets/enqueue_compss_args.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    15861 2023-05-08 14:01:10.000000 pycompss-cli-3.3.2/pycompss_cli/assets/runcompss_args.txt
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.574781 pycompss-cli-3.3.2/pycompss_cli/cli/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/cli/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      775 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/cli/compss.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      892 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/cli/dislib.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1364 2023-05-09 09:24:49.000000 pycompss-cli-3.3.2/pycompss_cli/cli/pycompss.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.574781 pycompss-cli-3.3.2/pycompss_cli/core/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5239 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/actions.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4494 2024-01-09 11:37:42.000000 pycompss-cli-3.3.2/pycompss_cli/core/actions_dispatcher.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    15553 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/arguments.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1723 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/cmd_helpers.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.574781 pycompss-cli-3.3.2/pycompss_cli/core/docker/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/docker/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     8616 2023-11-10 09:20:20.000000 pycompss-cli-3.3.2/pycompss_cli/core/docker/actions.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2811 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/docker/arguments.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    23127 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/docker/cmd.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.574781 pycompss-cli-3.3.2/pycompss_cli/core/local/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/local/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11979 2023-11-08 09:07:17.000000 pycompss-cli-3.3.2/pycompss_cli/core/local/actions.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1936 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/local/arguments.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4666 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/local/cmd.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.584781 pycompss-cli-3.3.2/pycompss_cli/core/remote/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    16046 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/actions.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     9112 2023-11-08 20:27:01.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/arguments.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     7026 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/cmd.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.584781 pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    13095 2023-05-08 14:01:10.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/core.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5510 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/defaults.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.584781 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2242 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/cancel.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    10277 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/commons.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2385 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/find.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     3398 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/info.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1798 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/status.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.584781 pycompss-cli-3.3.2/pycompss_cli/core/unicore/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      152 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/unicore/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11077 2024-01-09 11:39:54.000000 pycompss-cli-3.3.2/pycompss_cli/core/unicore/actions.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2822 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/unicore/arguments.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5541 2023-10-10 08:14:47.000000 pycompss-cli-3.3.2/pycompss_cli/core/utils.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.594781 pycompss-cli-3.3.2/pycompss_cli/models/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/pycompss_cli/models/__init__.py
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      767 2023-05-29 06:55:20.000000 pycompss-cli-3.3.2/pycompss_cli/models/app.py
-drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-01-09 13:48:18.564781 pycompss-cli-3.3.2/pycompss_cli.egg-info/
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4067 2024-01-09 13:48:17.000000 pycompss-cli-3.3.2/pycompss_cli.egg-info/PKG-INFO
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1763 2024-01-09 13:48:18.000000 pycompss-cli-3.3.2/pycompss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)        1 2024-01-09 13:48:17.000000 pycompss-cli-3.3.2/pycompss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)      136 2024-01-09 13:48:17.000000 pycompss-cli-3.3.2/pycompss_cli.egg-info/entry_points.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)       11 2024-01-09 13:48:17.000000 pycompss-cli-3.3.2/pycompss_cli.egg-info/requires.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)       13 2024-01-09 13:48:17.000000 pycompss-cli-3.3.2/pycompss_cli.egg-info/top_level.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)        7 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/requirements.txt
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)       38 2024-01-09 13:48:18.594781 pycompss-cli-3.3.2/setup.cfg
--rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1536 2023-01-18 08:52:05.000000 pycompss-cli-3.3.2/setup.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11406 2023-01-18 08:52:05.000000 pycompss-cli-3.3.3/LICENSE.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      266 2023-01-18 08:52:05.000000 pycompss-cli-3.3.3/MANIFEST.in
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4067 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/PKG-INFO
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     3144 2023-10-10 08:14:47.000000 pycompss-cli-3.3.3/README.rst
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)        6 2024-04-29 10:04:58.000000 pycompss-cli-3.3.3/VERSION.txt
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.807859 pycompss-cli-3.3.3/pycompss_cli/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/__init__.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.807859 pycompss-cli-3.3.3/pycompss_cli/assets/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/assets/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    25356 2023-05-08 14:01:10.000000 pycompss-cli-3.3.3/pycompss_cli/assets/enqueue_compss_args.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    15861 2023-05-08 14:01:10.000000 pycompss-cli-3.3.3/pycompss_cli/assets/runcompss_args.txt
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.807859 pycompss-cli-3.3.3/pycompss_cli/cli/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/cli/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      775 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/cli/compss.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      892 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/cli/dislib.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1364 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/cli/pycompss.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.817859 pycompss-cli-3.3.3/pycompss_cli/core/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5239 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4704 2024-04-29 08:25:59.000000 pycompss-cli-3.3.3/pycompss_cli/core/actions_dispatcher.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    15697 2024-04-29 10:19:13.000000 pycompss-cli-3.3.3/pycompss_cli/core/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1723 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/cmd_helpers.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.817859 pycompss-cli-3.3.3/pycompss_cli/core/docker/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/docker/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     8510 2024-04-29 09:20:28.000000 pycompss-cli-3.3.3/pycompss_cli/core/docker/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2811 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/docker/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    23142 2024-01-28 21:21:16.000000 pycompss-cli-3.3.3/pycompss_cli/core/docker/cmd.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.817859 pycompss-cli-3.3.3/pycompss_cli/core/local/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/local/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11922 2024-01-19 09:50:28.000000 pycompss-cli-3.3.3/pycompss_cli/core/local/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1936 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/local/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4693 2024-01-19 09:50:28.000000 pycompss-cli-3.3.3/pycompss_cli/core/local/cmd.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.817859 pycompss-cli-3.3.3/pycompss_cli/core/remote/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    16043 2024-04-29 10:27:54.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     9152 2024-04-29 10:01:43.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     7054 2024-04-29 10:20:39.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/cmd.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    13095 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/core.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5510 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/defaults.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2242 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/cancel.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    10277 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/commons.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2385 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/find.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     3398 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/info.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1798 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/status.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/pycompss_cli/core/unicore/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      798 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/unicore/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11723 2024-01-19 09:50:28.000000 pycompss-cli-3.3.3/pycompss_cli/core/unicore/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2823 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/unicore/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5541 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/core/utils.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/pycompss_cli/models/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/models/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      767 2024-01-19 09:50:27.000000 pycompss-cli-3.3.3/pycompss_cli/models/app.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2024-04-29 12:19:09.807859 pycompss-cli-3.3.3/pycompss_cli.egg-info/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4067 2024-04-29 12:19:08.000000 pycompss-cli-3.3.3/pycompss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1763 2024-04-29 12:19:09.000000 pycompss-cli-3.3.3/pycompss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)        1 2024-04-29 12:19:08.000000 pycompss-cli-3.3.3/pycompss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      136 2024-04-29 12:19:08.000000 pycompss-cli-3.3.3/pycompss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)       11 2024-04-29 12:19:08.000000 pycompss-cli-3.3.3/pycompss_cli.egg-info/requires.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)       13 2024-04-29 12:19:09.000000 pycompss-cli-3.3.3/pycompss_cli.egg-info/top_level.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)        7 2023-01-18 08:52:05.000000 pycompss-cli-3.3.3/requirements.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)       38 2024-04-29 12:19:09.827859 pycompss-cli-3.3.3/setup.cfg
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1536 2023-01-18 08:52:05.000000 pycompss-cli-3.3.3/setup.py
```

### Comparing `pycompss-cli-3.3.2/LICENSE.txt` & `pycompss-cli-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.3.2/PKG-INFO` & `pycompss-cli-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompss-cli
-Version: 3.3.2
+Version: 3.3.3
 Summary: PyCOMPSs cli
 Home-page: https://compss.bsc.es
 Author: Workflows and Distributed Computing Group (WDC) - Barcelona Supercomputing Center (BSC)
 Author-email: support-compss@bsc.es
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pycompss-cli-3.3.2/README.rst` & `pycompss-cli-3.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.3.2/pycompss_cli/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/assets/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/assets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/assets/enqueue_compss_args.txt` & `pycompss-cli-3.3.3/pycompss_cli/assets/enqueue_compss_args.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.3.2/pycompss_cli/assets/runcompss_args.txt` & `pycompss-cli-3.3.3/pycompss_cli/assets/runcompss_args.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.3.2/pycompss_cli/cli/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/cli/compss.py` & `pycompss-cli-3.3.3/pycompss_cli/cli/compss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/cli/dislib.py` & `pycompss-cli-3.3.3/pycompss_cli/cli/dislib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/cli/pycompss.py` & `pycompss-cli-3.3.3/pycompss_cli/cli/pycompss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/actions.py` & `pycompss-cli-3.3.3/pycompss_cli/core/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/actions_dispatcher.py` & `pycompss-cli-3.3.3/pycompss_cli/core/actions_dispatcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,14 +36,19 @@
             if not os.path.isdir(envs_path) or len(list(os.walk(envs_path))) == 1:
                 print("There are no environments created. Try using `pycompss init`")
                 exit(1)
 
             if arguments.action == 'environment':
                 if arguments.environment and arguments.environment.startswith('r'):
                     self.__delete_envs(arguments.env_id, arguments)
+                    exit(0)
+
+            if arguments.env_id and arguments.env_id not in list(os.walk(envs_path))[0][1]:
+                print("ERROR: There's no environment named " + arguments.env_id)
+                exit(1)
 
             env_id = arguments.env_id if arguments.env_id else None
                 
             env_conf = utils.get_current_env_conf(env_id=env_id)
             env_type = env_conf['env']
 
         self.__actions_cmd = self.__getactions_cmd(env_type, arguments, env_conf)
@@ -62,15 +67,14 @@
                 print('ERROR: `default` environment is required and cannot be deleted')
                 continue
             env_conf = utils.get_env_conf_by_name(env_id)
             env_arguments = deepcopy(arguments)
             env_arguments.env_id = env_id
             action_cmd = self.__getactions_cmd(env_type, env_arguments, env_conf=env_conf)
             action_cmd.env_remove()
-        exit(0)
 
     def __get_env_type_from_name(self, env_name):
         envs_path = self.home_path + '/.COMPSs/envs'
         env_dir_tree = list(os.walk(envs_path))
         envs_names = env_dir_tree[0][1]
         env_dir_tree = env_dir_tree[1:]
         for i in range(len(env_dir_tree)):
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/arguments.py` & `pycompss-cli-3.3.3/pycompss_cli/core/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -152,14 +152,18 @@
     # JUPYTER
     parser_jupyter = subparsers.add_parser("jupyter",
                                            aliases=["jpy"],
                                            help="Starts Jupyter within the COMPSs\' environment.",  # noqa: E501
                                            parents=[parent_parser],
                                            formatter_class=FORMATTER_CLASS)
     parser_jupyter.set_defaults(action='jupyter')
+
+    parser_jupyter.add_argument("-lab",
+                             action="store_true",
+                             help="Run Jupyter Lab")
     
     
     parser_jupyter.add_argument("-app", "--app_name",
                              default="",
                              type=str,
                              help="Name of the app where the notebook will be deployed. Only required for `remote` type environment")
     parser_jupyter.add_argument('rest_args',
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/cmd_helpers.py` & `pycompss-cli-3.3.3/pycompss_cli/core/cmd_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/docker/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/core/docker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/docker/actions.py` & `pycompss-cli-3.3.3/pycompss_cli/core/docker/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -151,21 +151,18 @@
         :param arguments: Command line arguments
         :param debug: Debug mode
         :returns: None
         """
 
         self.docker_cmd.docker_exec_in_daemon('pkill jupyter')
         
-        cmd = 'notebook'
-        if len(self.arguments.rest_args) > 0:
-            if self.arguments.rest_args[0] == 'lab' or self.arguments.rest_args[0] == 'notebook':
-                cmd = ''
+        lab_or_notebook = 'lab' if self.arguments.lab else 'notebook'
 
         arguments = " ".join(self.arguments.rest_args)
-        jupyter_cmd = f"jupyter {cmd} " + \
+        jupyter_cmd = f"jupyter {lab_or_notebook} " + \
                 arguments + " " + \
                 f"--ip={self.env_conf['master_ip']} " + \
                 "--allow-root " + \
                 "--NotebookApp.token="
 
         try:
             for out_line in self.docker_cmd.docker_exec_in_daemon(jupyter_cmd, return_stream=True):
@@ -188,16 +185,16 @@
         dot_path = self.arguments.dot_file
         
         command = "compss_gengraph " + dot_path
         self.docker_cmd.docker_exec_in_daemon(command)
 
 
     def gentrace(self):
-        command = f"compss_gentrace {self.arguments.trace_dir} "
-        command += ' '.join(self.arguments.rest_args)
+        command = f"compss_gentrace " + ' '.join(self.arguments.rest_args)
+        command += f' {self.arguments.trace_dir}'
         self.docker_cmd.docker_exec_in_daemon(command)
         if self.arguments.download_dir:
             self.docker_cmd.docker_exec_in_daemon(f'cp {self.arguments.trace_dir}/* {self.arguments.download_dir}/')
 
 
     def app(self):
         print("ERROR: Wrong Environment! Try using a `remote` or `local` environment")
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/docker/arguments.py` & `pycompss-cli-3.3.3/pycompss_cli/core/docker/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/docker/cmd.py` & `pycompss-cli-3.3.3/pycompss_cli/core/docker/cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -132,15 +132,15 @@
 
         if not self.is_running(self.master_name):
             print("Starting %s container in dir %s" % (self.master_name, working_dir))
             print("If this is your first time running PyCOMPSs it may take a " +
                 "while because it needs to download the docker image. " +
                 "Please be patient.")
             if update_image:
-                subprocess.run(f'docker pull {docker_image}', shell=True)
+                subprocess.run(['docker', 'pull', docker_image], stdout=subprocess.PIPE)
             mounts = self._get_mounts(user_working_dir=working_dir, log_dir=log_dir)
             ports = {"8888/tcp": 8888,  # required for jupyter notebooks
                     "8080/tcp": 8080}  # required for monitor
             container: Container = self.client.containers.run(image=docker_image, name=self.master_name,
                                     mounts=mounts, detach=True, ports=ports, privileged=privileged)
             self._generate_resources_cfg(ips=["localhost"])
             self._generate_project_cfg(ips=["localhost"])
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/local/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/core/local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/local/actions.py` & `pycompss-cli-3.3.3/pycompss_cli/core/local/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -103,20 +103,17 @@
             print('ERROR: Jupyter not found!')
             exit(1)
 
         working_dir = '.'
         if 'working_dir' in self.env_conf:
             working_dir = self.env_conf['working_dir']
 
-        jupyter_args = self.arguments.rest_args
-        if jupyter_args[0] == 'lab':
-            cmd = 'lab'
-        else:
-            cmd = 'notebook'
-        local_jupyter(working_dir, cmd, ' '.join(jupyter_args))
+        lab_or_notebook = 'lab' if self.arguments.lab else 'notebook'
+
+        local_jupyter(working_dir, lab_or_notebook, ' '.join(self.arguments.rest_args))
 
     def exec(self):
         command = ' '.join(self.arguments.exec_cmd)
         local_exec_app(command)
 
     def app(self):
         if not self.arguments.app:
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/local/arguments.py` & `pycompss-cli-3.3.3/pycompss_cli/core/local/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/local/cmd.py` & `pycompss-cli-3.3.3/pycompss_cli/core/local/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -56,16 +56,16 @@
     if utils.check_exit_code('which enqueue_compss') == 1:
         cmd = ['module load COMPSs'] + cmd
     cmd = ';'.join(cmd)
 
     subprocess.run(cmd, shell=True)
 
 
-def local_jupyter(work_dir, jupyter_args):
-    cmd = 'jupyter notebook --notebook-dir=' + work_dir
+def local_jupyter(work_dir, lab_or_notebook, jupyter_args):
+    cmd = f'jupyter {lab_or_notebook} --notebook-dir=' + work_dir
     process = subprocess.Popen(cmd + ' ' + jupyter_args, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     try:
         while True:
             line = process.stdout.readline()
             if line == '' and process.poll() is not None:
                 break
             if line:
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/actions.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -311,15 +311,15 @@
         remote_exec_app(self.env_conf['login'], command)
 
     def gentrace(self):
         modules = self.__get_modules()
 
         trace_ls = f"ls {self.arguments.trace_dir}"
         trace_ls = remote_exec_app(self.env_conf['login'], trace_ls, self.debug)
-        if not '.prv.gz' in trace_ls:
+        if not '.prv' in trace_ls:
             gentrace_cmd = f"compss_gentrace {self.arguments.trace_dir} "
             gentrace_cmd += ' '.join(self.arguments.rest_args)
 
             commands = [
                 *modules,
                 gentrace_cmd
             ]
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/arguments.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -43,15 +43,16 @@
 
     parser_init.add_argument("-l", "--login",
                              type=str,
                              required=True,
                              help="Login info username@remote_hostname")
 
     parser_init.add_argument("-m", "--modules",
-                             help="Module list or file to load in remote environment")
+                             help="Module list or file to load in remote environment",
+                             nargs='+')
 
     return parser_init
 
 def remote_parser_app():
     parser = argparse.ArgumentParser(formatter_class=FORMATTER_CLASS)
 
     # Parent parser - includes all arguments which are common to all actions
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/cmd.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -40,15 +40,15 @@
     :param image: Given docker image
     :param restart: Force stop the existing and start a new one.
     :returns: None
     """
 
     subprocess.run(f"ssh {login_info} 'mkdir -p ~/.COMPSs'", shell=True)
 
-    if isinstance(modules, str):
+    if isinstance(modules, str) and os.path.isfile(modules):
         modules_file = modules
     else:
         tmp_modules = tempfile.NamedTemporaryFile(delete=False)
         env_vars = '\n'.join([f'export {var}' for var in envars])
         mod_script = '\n'.join([f'module load {m}' for m in modules])
         tmp_modules.write((env_vars + '\n').encode())
         tmp_modules.write((mod_script + '\n').encode())
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/core.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/interactive_sc/defaults.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/interactive_sc/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/cancel.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/cancel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/commons.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/commons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/find.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/find.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/info.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/remote/job_scripts/status.py` & `pycompss-cli-3.3.3/pycompss_cli/core/remote/job_scripts/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/unicore/actions.py` & `pycompss-cli-3.3.3/pycompss_cli/core/unicore/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+#!/usr/bin/python
+#
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+#
 
 from shutil import copyfile
 import traceback
 from pycompss_cli.core.actions import Actions
 from pycompss_cli.core.unicore import UNICORE_URL_ENVAR
 from pycompss_cli.core.unicore import UNICORE_USER_ENVAR
 from pycompss_cli.core.unicore import UNICORE_PASSWORD_ENVAR
@@ -294,8 +310,8 @@
 
     def monitor(self):
         print('ERROR: Not Implemented Yet')
         exit(1)
 
     def run(self):
         print('ERROR: Not Implemented Yet')
-        exit(1)
+        exit(1)
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/unicore/arguments.py` & `pycompss-cli-3.3.3/pycompss_cli/core/unicore/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -62,8 +62,8 @@
                              type=str,
                              help=f"Unicore JWT token signed by the server. Also can be used envar {UNICORE_TOKEN_ENVAR}")
 
     parser_init.add_argument("-m", "--modules",
                              nargs='*',
                              help="Modules file to load in remote environment")
 
-    return parser_init
+    return parser_init
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/core/utils.py` & `pycompss-cli-3.3.3/pycompss_cli/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/models/__init__.py` & `pycompss-cli-3.3.3/pycompss_cli/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli/models/app.py` & `pycompss-cli-3.3.3/pycompss_cli/models/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-#  Copyright 2002-2022 Barcelona Supercomputing Center (www.bsc.es)
+#  Copyright 2002-2023 Barcelona Supercomputing Center (www.bsc.es)
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli.egg-info/PKG-INFO` & `pycompss-cli-3.3.3/pycompss_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompss-cli
-Version: 3.3.2
+Version: 3.3.3
 Summary: PyCOMPSs cli
 Home-page: https://compss.bsc.es
 Author: Workflows and Distributed Computing Group (WDC) - Barcelona Supercomputing Center (BSC)
 Author-email: support-compss@bsc.es
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pycompss-cli-3.3.2/pycompss_cli.egg-info/SOURCES.txt` & `pycompss-cli-3.3.3/pycompss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.3.2/setup.py` & `pycompss-cli-3.3.3/setup.py`

 * *Files identical despite different names*

