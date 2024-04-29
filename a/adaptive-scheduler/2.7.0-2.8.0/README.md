# Comparing `tmp/adaptive_scheduler-2.7.0.tar.gz` & `tmp/adaptive_scheduler-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_scheduler-2.7.0.tar", last modified: Tue Apr 23 19:15:58 2024, max compression
+gzip compressed data, was "adaptive_scheduler-2.8.0.tar", last modified: Mon Apr 29 17:33:30 2024, max compression
```

## Comparing `adaptive_scheduler-2.7.0.tar` & `adaptive_scheduler-2.8.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:58.151565 adaptive_scheduler-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-23 19:15:58.151565 adaptive_scheduler-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:58.155565 adaptive_scheduler-2.7.0/adaptive_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7996 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_mock_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:58.147565 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:58.147565 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/base_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/run_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 19:15:58.155565 adaptive_scheduler-2.7.0/adaptive_scheduler/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/client_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/server_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    42831 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32917 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/adaptive_scheduler/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:58.151565 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-23 19:15:58.000000 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 19:15:58.000000 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:15:58.000000 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 19:15:58.000000 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-23 19:15:58.000000 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 19:15:58.000000 adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:15:58.151565 adaptive_scheduler-2.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:15:58.151565 adaptive_scheduler-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_client_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    17884 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_log_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_log_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_run_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_server_support_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_slurm_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_utils_file_creation_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-04-23 19:15:43.000000 adaptive_scheduler-2.7.0/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:30.507909 adaptive_scheduler-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 17:33:30.507909 adaptive_scheduler-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:30.511909 adaptive_scheduler-2.8.0/adaptive_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7996 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_mock_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:30.503909 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19631 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:30.503909 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-29 17:33:30.511909 adaptive_scheduler-2.8.0/adaptive_scheduler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/client_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/server_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42831 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32917 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/adaptive_scheduler/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:30.507909 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 17:33:30.000000 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-29 17:33:30.000000 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:33:30.000000 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 17:33:30.000000 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-29 17:33:30.000000 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 17:33:30.000000 adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:33:30.507909 adaptive_scheduler-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:30.507909 adaptive_scheduler-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_client_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17884 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_log_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_log_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_server_support_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_slurm_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_utils_file_creation_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-04-29 17:33:19.000000 adaptive_scheduler-2.8.0/tests/test_widgets.py
```

### Comparing `adaptive_scheduler-2.7.0/LICENSE` & `adaptive_scheduler-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/PKG-INFO` & `adaptive_scheduler-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 2.7.0
+Version: 2.8.0
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.7.0/README.md` & `adaptive_scheduler-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_mock_scheduler.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_mock_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/base_scheduler.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/common.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/local.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/local.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/pbs.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_scheduler/slurm.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_scheduler/slurm.py`

 * *Files 12% similar despite different names*

```diff
@@ -368,15 +368,16 @@
         output_opt = f"--output {output_str}"
         name_opt = f"--job-name {name}"
         submit_cmd = (
             f"{self.submit_cmd} {name_opt} {output_opt} {self.batch_fname(name_prefix)}"
         )
         run_submit(submit_cmd, name)
 
-    def queue(self, *, me_only: bool = True) -> dict[str, dict[str, str]]:
+    @staticmethod
+    def queue(*, me_only: bool = True) -> dict[str, dict[str, str]]:
         """Get the queue of jobs."""
         python_format = {
             "JobID": 100,
             "Name": 100,
             "state": 100,
             "NumNodes": 100,
             "NumTasks": 100,
@@ -427,14 +428,67 @@
         return running
 
     @cached_property
     def partitions(self) -> dict[str, int]:
         """Get the partitions of the SLURM scheduler."""
         return slurm_partitions()  # type: ignore[return-value]
 
+    @staticmethod
+    def cancel_jobs(name: str, *, dry: bool = False) -> None:
+        """Cancel jobs with names matching the pattern '{name}-{i}' where i is an integer.
+
+        Parameters
+        ----------
+        name
+            The base name of the jobs to cancel. Jobs with names that start with '{name}-'
+            followed by an integer will be canceled.
+        dry
+            If True, perform a dry run and print the job IDs that would be canceled without
+            actually canceling them. Default is False.
+
+        Raises
+        ------
+        RuntimeError
+            If there is an error while canceling the jobs.
+
+        Examples
+        --------
+        >>> SLURM.cancel_jobs("my_job")
+        # Cancels all running jobs with names like "my_job-1", "my_job-2", etc.
+
+        >>> SLURM.cancel_jobs("my_job", dry=True)
+        # Prints the job IDs that would be canceled without actually canceling them.
+
+        """
+        running_jobs = SLURM.queue()
+        job_ids_to_cancel = []
+
+        for job_id, job_info in running_jobs.items():
+            job_name = job_info["job_name"]
+            if job_name.startswith(f"{name}-"):
+                suffix = job_name[len(name) + 1 :]
+                if suffix.isdigit():
+                    job_ids_to_cancel.append(job_id)
+
+        if job_ids_to_cancel:
+            job_ids_str = ",".join(job_ids_to_cancel)
+            cmd = f"{SLURM._cancel_cmd} {job_ids_str}"
+            if dry:
+                print(f"Dry run: would cancel jobs with IDs: {job_ids_str}")
+            else:
+                try:
+                    subprocess.run(cmd.split(), check=True)
+                except subprocess.CalledProcessError as e:
+                    msg = f"Failed to cancel jobs with name {name}. Error: {e}"
+                    raise RuntimeError(
+                        msg,
+                    ) from e
+        else:
+            print(f"No running jobs found with name pattern '{name}-<integer>'")
+
 
 def _get_ncores(partition: str) -> int | None:
     numbers = re.findall(r"\d+", partition)
     if not numbers:
         return None
     return int(numbers[0])
```

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/base_manager.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/base_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/common.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/database_manager.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/database_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/job_manager.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/job_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/kill_manager.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/launcher.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/parse_logs.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/parse_logs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/run_manager.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/run_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/_server_support/slurm_run.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/_server_support/slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/client_support.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/scheduler.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/server_support.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/server_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/utils.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler/widgets.py` & `adaptive_scheduler-2.8.0/adaptive_scheduler/widgets.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/PKG-INFO` & `adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 2.7.0
+Version: 2.8.0
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.7.0/adaptive_scheduler.egg-info/SOURCES.txt` & `adaptive_scheduler-2.8.0/adaptive_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/pyproject.toml` & `adaptive_scheduler-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_base_scheduler.py` & `adaptive_scheduler-2.8.0/tests/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_client_support.py` & `adaptive_scheduler-2.8.0/tests/test_client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_database_manager.py` & `adaptive_scheduler-2.8.0/tests/test_database_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_job_manager.py` & `adaptive_scheduler-2.8.0/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_kill_manager.py` & `adaptive_scheduler-2.8.0/tests/test_kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_launcher.py` & `adaptive_scheduler-2.8.0/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_log_generation.py` & `adaptive_scheduler-2.8.0/tests/test_log_generation.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_log_parsing.py` & `adaptive_scheduler-2.8.0/tests/test_log_parsing.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_run_manager.py` & `adaptive_scheduler-2.8.0/tests/test_run_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_server_support_common.py` & `adaptive_scheduler-2.8.0/tests/test_server_support_common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_slurm_run.py` & `adaptive_scheduler-2.8.0/tests/test_slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_slurm_scheduler.py` & `adaptive_scheduler-2.8.0/tests/test_slurm_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_utils.py` & `adaptive_scheduler-2.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_utils_file_creation_progress.py` & `adaptive_scheduler-2.8.0/tests/test_utils_file_creation_progress.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.7.0/tests/test_widgets.py` & `adaptive_scheduler-2.8.0/tests/test_widgets.py`

 * *Files identical despite different names*

