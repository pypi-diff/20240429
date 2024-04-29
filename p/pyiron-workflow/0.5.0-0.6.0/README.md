# Comparing `tmp/pyiron_workflow-0.5.0.tar.gz` & `tmp/pyiron_workflow-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_workflow-0.5.0.tar", last modified: Wed Apr  3 17:46:20 2024, max compression
+gzip compressed data, was "pyiron_workflow-0.6.0.tar", last modified: Mon Apr 29 18:41:49 2024, max compression
```

## Comparing `pyiron_workflow-0.5.0.tar` & `pyiron_workflow-0.6.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/pyiron_workflow/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    27357 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/executors/cloudpickleprocesspool.py
--rw-r--r--   0 runner    (1001) docker     (127)    27380 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/has_interface_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/has_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    28289 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/node_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/pyiron_atomistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/semantics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/single_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/has_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/type_hinting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/working.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 17:46:19.000000 pyiron_workflow-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.287286 pyiron_workflow-0.6.0/pyiron_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/pyiron_workflow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21826 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/executors/cloudpickleprocesspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/has_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/has_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/io_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39289 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/node_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/pyiron_atomistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/single_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/has_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/type_hinting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/working.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-29 18:41:48.000000 pyiron_workflow-0.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/versioneer.py
```

### Comparing `pyiron_workflow-0.5.0/LICENSE` & `pyiron_workflow-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/PKG-INFO` & `pyiron_workflow-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.5.0
+Version: 0.6.0
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
@@ -15,22 +15,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: bidict>=0.23.1
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: graphviz>=0.20.3
 Requires-Dist: h5io>=0.2.2
-Requires-Dist: h5io_browser>=0.0.10
-Requires-Dist: matplotlib>=3.8.3
-Requires-Dist: pyiron_base>=0.8.0
+Requires-Dist: h5io_browser>=0.0.12
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: pyiron_base>=0.8.2
 Requires-Dist: pyiron_contrib>=0.1.16
 Requires-Dist: pympipool>=0.7.17
 Requires-Dist: toposort>=1.10
 Requires-Dist: typeguard>=4.2.1
 Provides-Extra: node-library
 Requires-Dist: ase>=3.22.1; extra == "node-library"
-Requires-Dist: atomistics>=0.1.24; extra == "node-library"
+Requires-Dist: atomistics>=0.1.27; extra == "node-library"
 Requires-Dist: numpy>=1.26.4; extra == "node-library"
 Requires-Dist: phonopy>=2.22.1; extra == "node-library"
-Requires-Dist: pyiron_atomistics>=0.5.0; extra == "node-library"
+Requires-Dist: pyiron_atomistics>=0.5.3; extra == "node-library"
 
 http://pyiron.org
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/__init__.py` & `pyiron_workflow-0.6.0/pyiron_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/channels.py` & `pyiron_workflow-0.6.0/pyiron_workflow/channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,29 +115,34 @@
     def connect(self, *others: Channel) -> None:
         """
         Form a connection between this and one or more other channels.
         Connections are reflexive, and should only occur between input and output
         channels, i.e. they are instances of each others
         :attr:`connection_partner_type`.
 
+        New connections get _prepended_ to the connection lists, so they appear first
+        when searching over connections.
+
         Args:
             *others (Channel): The other channel objects to attempt to connect with.
 
         Raises:
             (ChannelConnectionError): If the other channel is of the correct type, but
                 nonetheless not a valid connection.
             (TypeError): If the other channel is not an instance of this channel's
                 partner type.
         """
         for other in others:
             if other in self.connections:
                 continue
             elif self._valid_connection(other):
-                self.connections.append(other)
-                other.connections.append(self)
+                # Prepend new connections
+                # so that connection searches run newest to oldest
+                self.connections.insert(0, other)
+                other.connections.insert(0, self)
             else:
                 if isinstance(other, self.connection_partner_type):
                     raise ChannelConnectionError(
                         f"{other.label} ({other.__class__.__name__}) has the correct "
                         f"type ({self.connection_partner_type.__name__} to connect "
                         f"with {self.label} ({self.__class__.__name__}), but is not a "
                         f"valid connection. Please check type hints, etc."
@@ -501,18 +506,18 @@
 class InputData(DataChannel):
     @property
     def connection_partner_type(self):
         return OutputData
 
     def fetch(self) -> None:
         """
-        Sets :attr:`value` to the first value among connections that is something other
-        than `NOT_DATA`; if no such value exists (e.g. because there are no connections
-        or because all the connected output channels have `NOT_DATA` as their value),
-        :attr:`value` remains unchanged.
+        Sets :attr:`value` to the first value among connections (i.e. the most recent)
+        that is something other than `NOT_DATA`; if no such value exists (e.g. because
+        there are no connections or because all the connected output channels have
+        `NOT_DATA` as their value), :attr:`value` remains unchanged.
         I.e., the connection with the highest priority for updating input data is the
         0th connection; build graphs accordingly.
 
         Raises:
             RuntimeError: If the owner is :attr:`running`.
         """
         for out in self.connections:
@@ -584,41 +589,46 @@
         Args:
             label (str): A name for the channel.
             owner (pyiron_workflow.io.HasIO): The channel's owner.
             callback (callable): An argument-free callback to invoke when calling this
                 object. Must be a method on the owner.
         """
         super().__init__(label=label, owner=owner)
-        if self._is_method_on_owner(callback) and self._takes_zero_arguments(callback):
+        if self._is_method_on_owner(callback) and self._all_args_arg_optional(callback):
             self._callback: str = callback.__name__
         else:
             raise BadCallbackError(
                 f"The channel {self.label} on {self.owner.label} got an unexpected "
                 f"callback: {callback}. "
                 f"Lives on owner: {self._is_method_on_owner(callback)}; "
-                f"take no args: {self._takes_zero_arguments(callback)} "
+                f"all args are optional: {self._all_args_arg_optional(callback)} "
             )
 
     def _is_method_on_owner(self, callback):
         try:
             return callback == getattr(self.owner, callback.__name__)
         except AttributeError:
             return False
 
-    def _takes_zero_arguments(self, callback):
-        return callable(callback) and self._no_positional_args(callback)
+    def _all_args_arg_optional(self, callback):
+        return callable(callback) and not self._has_required_args(callback)
 
     @staticmethod
-    def _no_positional_args(func):
-        return all(
-            [
-                parameter.default != inspect.Parameter.empty
-                or parameter.kind == inspect.Parameter.VAR_KEYWORD
-                for parameter in inspect.signature(func).parameters.values()
-            ]
+    def _has_required_args(func):
+        return any(
+            (
+                param.kind
+                in (
+                    inspect.Parameter.POSITIONAL_ONLY,
+                    inspect.Parameter.POSITIONAL_OR_KEYWORD,
+                    inspect.Parameter.KEYWORD_ONLY,
+                )
+                and param.default == inspect.Parameter.empty
+            )
+            for param in inspect.signature(func).parameters.values()
         )
 
     @property
     def callback(self) -> callable:
         return getattr(self.owner, self._callback)
 
     def __call__(self, other: typing.Optional[OutputSignal] = None) -> None:
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/composite.py` & `pyiron_workflow-0.6.0/pyiron_workflow/workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,255 @@
 """
-A base class for nodal objects that have internal structure -- i.e. they hold a
-sub-graph
+Provides the main workhorse class for creating and running workflows.
+
+This class is intended as the single point of entry for users making an import.
 """
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from functools import wraps
 from typing import Literal, Optional, TYPE_CHECKING
 
 from bidict import bidict
 
-from pyiron_workflow.create import Creator, Wrappers
-from pyiron_workflow.io import Outputs, Inputs
-from pyiron_workflow.node import Node
-from pyiron_workflow.node_package import NodePackage
-from pyiron_workflow.semantics import SemanticParent
-from pyiron_workflow.topology import set_run_connections_according_to_dag
-from pyiron_workflow.snippets.colors import SeabornColors
-from pyiron_workflow.snippets.dotdict import DotDict
+from pyiron_workflow.composite import Composite
+from pyiron_workflow.io import Inputs, Outputs
+from pyiron_workflow.semantics import ParentMost
+
 
 if TYPE_CHECKING:
-    from pyiron_workflow.channels import Channel, InputData, OutputData
+    from pyiron_workflow.channels import InputData, OutputData
+    from pyiron_workflow.io import IO
+    from pyiron_workflow.node import Node
 
 
-class Composite(Node, SemanticParent, ABC):
+class Workflow(ParentMost, Composite):
     """
-    A base class for nodes that have internal graph structure -- i.e. they hold a
-    collection of child nodes and their computation is to execute that graph.
+    Workflows are a dynamic composite node -- i.e. they hold and run a collection of
+    nodes (a subgraph) which can be dynamically modified (adding and removing nodes,
+    and modifying their connections).
+
+    Nodes can be added to the workflow at instantiation or with dot-assignment later on.
+    They are then accessible either under the :attr:`nodes` dot-dictionary, or just directly
+    by dot-access on the workflow object itself.
+
+    Using the :attr:`input` and :attr:`output` attributes, the workflow gives by-reference access
+    to all the IO channels among its nodes which are currently unconnected.
+
+    The :class:`Workflow` class acts as a single-point-of-import for us;
+    Directly from the class we can use the :meth:`create` method to instantiate workflow
+    objects.
+    When called from a workflow _instance_, any created nodes get their parent set to
+    the workflow instance being used.
+
+    Workflows are "living" -- i.e. their IO is always by reference to their owned nodes
+    and you are meant to add and remove nodes as children -- and "parent-most" -- i.e.
+    they sit at the top of any data dependency tree and may never have a parent of
+    their own.
+    They are flexible and great for development, but once you have a setup you like,
+    you should consider reformulating it as a :class:`Macro`, which operates somewhat more
+    efficiently.
 
     Promises (in addition parent class promises):
 
-    - The class offers access...
-        - To the node-izing :mod:`pyiron_workflow` decorators
-        - To a creator for other :mod:`pyiron_workflow` objects (namely nodes)
-            - From the class level, this simply creates these objects
-            - From the instance level, created nodes get the instance as their parent
-    - Child nodes...
-        - Can be added by...
-            - Passing a node instance to the adding method
-            - Setting the composite instance as the node's parent at node instantiation
-            - Assigning a node instance as an attribute
-        - Can be accessed by...
-            - Attribute access using their node label
-            - Attribute or item access in the child nodes collection
-            - Iterating over the composite instance
-        - Can be removed by method
-        - Each have a unique label (within the scope of this composite)
-        - Have no other parent
-        - Can be replaced in-place with another node that has commensurate IO
-        - Have their working directory nested inside the composite's
-        - Are disallowed from having a label that conflicts with any of the parent's
-            other methods or attributes
-    - The length of a composite instance is its number of child nodes
-    - Running the composite...
-        - Runs the child nodes (either using manually specified execution signals, or
-            leveraging a helper tool that automates this process for data DAGs --
-            details are left to child classes)
-        - Returns a dot-dictionary of output IO
-    - Composite IO...
-        - Is some subset of the child nodes IO
-            - Default channel labels indicate both child and child's channel labels
-            - Default behaviour is to expose all unconnected child nodes' IO
-        - Bijective maps can be used to...
-            - Rename IO
-            - Force a child node's IO to appear
-            - Force a child node's IO to _not_ appear
+    - Workflows are living, their IO always reflects their current state of child nodes
+    - Workflows are parent-most objects, they cannot be a sub-graph of a larger graph
 
-    Attributes:
+    Attribute:
         inputs/outputs_map (bidict|None): Maps in the form
-         `{"node_label__channel_label": "some_better_name"}` that expose canonically
+        `{"node_label__channel_label": "some_better_name"}` that expose canonically
          named channels of child nodes under a new name. This can be used both for re-
          naming regular IO (i.e. unconnected child channels), as well as forcing the
          exposure of irregular IO (i.e. child channels that are already internally
          connected to some other child channel). Non-`None` values provided at input
          can be in regular dictionary form, but get re-cast as a clean bidict to ensure
          the bijective nature of the maps (i.e. there is a 1:1 connection between any
          IO exposed at the :class:`Composite` level and the underlying channels).
         children (bidict.bidict[pyiron_workflow.node.Node]): The owned nodes that
          form the composite subgraph.
-        strict_naming (bool): When true, repeated assignment of a new node to an
-         existing node label will raise an error, otherwise the label gets appended
-         with an index and the assignment proceeds. (Default is true: disallow assigning
-         to existing labels.)
-        create (Creator): A tool for adding new nodes to this subgraph.
-        starting_nodes (None | list[pyiron_workflow.node.Node]): A subset
-         of the owned nodes to be used on running. Only necessary if the execution graph
-         has been manually specified with `run` signals. (Default is an empty list.)
-        wrap_as (Wrappers): A tool for accessing node-creating decorators
-
-    Methods:
-        add_child(node: Node): Add the node instance to this subgraph.
-        remove_child(node: Node): Break all connections the node has, remove_child it from this
-         subgraph, and set its parent to `None`.
-        (de)activate_strict_hints(): Recursively (de)activate strict type hints.
-        replace_child(owned_node: Node | str, replacement: Node | type[Node]): Replaces an
-            owned node with a new node, as long as the new node's IO is commensurate
-            with the node being replaced.
-        register(): A short-cut to registering a new node package with the node creator.
-    """
 
-    wrap_as = Wrappers()
-    create = Creator()
+    Examples:
+        We allow adding nodes to workflows in five equivalent ways:
+
+        >>> from pyiron_workflow.workflow import Workflow
+        >>>
+        >>> @Workflow.wrap.as_function_node()
+        ... def fnc(x=0):
+        ...     return x + 1
+        >>>
+        >>> # (1) As *args at instantiation
+        >>> n1 = fnc(label="n1")
+        >>> wf = Workflow("my_workflow", n1)
+        >>>
+        >>> # (2) Being passed to the `add` method
+        >>> n2 = wf.add_child(fnc(label="n2"))
+        >>>
+        >>> # (3) By attribute assignment
+        >>> wf.n3 = fnc(label="anyhow_n3_gets_used")
+        >>>
+        >>> # (4) By creating from the workflow class but specifying the parent kwarg
+        >>> n4 = fnc(label="n4", parent=wf)
+
+        By default, the node naming scheme is strict, so if you try to add a node to a
+        label that already exists, you will get an error. This behaviour can be changed
+        at instantiation with the :attr:`strict_naming` kwarg, or afterwards by assigning a
+        bool to this property. When deactivated, repeated assignments to the same label
+        just get appended with an index:
+
+        >>> wf.strict_naming = False
+        >>> wf.my_node = fnc(x=0)
+        >>> wf.my_node = fnc(x=1)
+        >>> wf.my_node = fnc(x=2)
+        >>> print(wf.my_node.inputs.x, wf.my_node0.inputs.x, wf.my_node1.inputs.x)
+        0 1 2
+
+        The :class:`Workflow` class is designed as a single point of entry for workflows, so
+        you can also access decorators to define new node classes right from the
+        workflow (cf. the :class:`Node` docs for more detail on the node types).
+        Let's use these to explore a workflow's input and output, which are dynamically
+        generated from the unconnected IO of its nodes:
+
+        >>> @Workflow.wrap.as_function_node("y")
+        ... def plus_one(x: int = 0):
+        ...     return x + 1
+        >>>
+        >>> wf = Workflow("io_workflow")
+        >>> wf.first = plus_one()
+        >>> wf.second = plus_one()
+        >>> print(len(wf.inputs), len(wf.outputs))
+        2 2
+
+        If we connect the output of one node to the input of the other, there are fewer
+        dangling channels for the workflow IO to find:
+
+        >>> wf.second.inputs.x = wf.first.outputs.y
+        >>> print(len(wf.inputs), len(wf.outputs))
+        1 1
+
+        Then we just run the workflow
+
+        >>> out = wf.run()
+
+        The workflow joins node lavels and channel labels with a `_` character to
+        provide direct access to the output:
+
+        >>> print(wf.outputs.second__y.value)
+        2
+
+        These input keys can be used when calling the workflow to update the input. In
+        our example, the nodes update automatically when their input gets updated, so
+        all we need to do to see updated workflow output is update the input:
+
+        >>> out = wf(first__x=10)
+        >>> out
+        {'second__y': 12}
+
+        Note: this _looks_ like a dictionary, but has some extra convenience that we
+        can dot-access data:
+
+        >>> out.second__y
+        12
+
+        We can give more convenient names to IO, and even access IO that would normally
+        be hidden (because it's connected) by specifying an :attr:`inputs_map` and/or
+        :attr:`outputs_map`:
+
+        >>> wf.inputs_map = {"first__x": "x"}
+        >>> wf.outputs_map = {
+        ...     "first__y": "intermediate",
+        ...     "second__y": "y"
+        ... }
+        >>> wf(x=0)
+        {'intermediate': 1, 'y': 2}
+
+        Workflows can be visualized in the notebook using graphviz:
+
+        >>> graphviz_graph = wf.draw()
+
+        The resulting object can be saved as an image, e.g.
+
+        >>> wf.draw().render(filename="demo", format="png")
+        'demo.png'
+
+        Let's clean up after ourselves (for when the CI runs the docstrings)
+
+        >>> from os import remove
+        >>> remove("demo")
+        >>> remove("demo.png")
+
+        Workflows also give access to packages of pre-built nodes under different
+        namespaces. These need to be registered first, like the standard package is
+        automatically registered:
+
+        >>> Workflow.register("pyiron_workflow.node_library.standard", "standard")
+
+        When your workflow's data follows a directed-acyclic pattern, it will determine
+        the execution flow automatically.
+        If you want or need more control, you can set the `automate_execution` flag to
+        `False` and manually specify an execution flow.
+
+    TODO: Workflows can be serialized.
+
+    TODO: Once you're satisfied with how a workflow is structured, you can export it
+        as a macro node for use in other workflows. (Maybe we should allow for nested
+        workflows without exporting to a node? I was concerned then what happens to the
+        nesting abstraction if, instead of accessing IO through the workflow's IO flags,
+        a user manually connects IO from individual nodes from two different, nested or
+        sibling workflows when those connections were _previously internal to their own
+        workflow_. This seems very unsafe. Maybe there is something like a lock we can
+        apply that falls short of a full export, but still guarantees the internal
+        integrity of workflows when they're used somewhere else?
+    """
 
     def __init__(
         self,
         label: str,
-        *args,
-        parent: Optional[Composite] = None,
+        *nodes: Node,
         overwrite_save: bool = False,
         run_after_init: bool = False,
         storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
         save_after_run: bool = False,
         strict_naming: bool = True,
         inputs_map: Optional[dict | bidict] = None,
         outputs_map: Optional[dict | bidict] = None,
+        automate_execution: bool = True,
         **kwargs,
     ):
+        self._inputs_map = None
+        self._outputs_map = None
+        self.inputs_map = inputs_map
+        self.outputs_map = outputs_map
+        self._inputs = None
+        self._outputs = None
+        self.automate_execution = automate_execution
+
         super().__init__(
-            *args,
+            *nodes,
             label=label,
-            parent=parent,
+            parent=None,
+            overwrite_save=overwrite_save,
+            run_after_init=run_after_init,
             save_after_run=save_after_run,
             storage_backend=storage_backend,
             strict_naming=strict_naming,
             **kwargs,
         )
-        self._inputs_map = None
-        self._outputs_map = None
-        self.inputs_map = inputs_map
-        self.outputs_map = outputs_map
-        self.starting_nodes: list[Node] = []
+
+    def _after_node_setup(
+        self,
+        *args,
+        overwrite_save: bool = False,
+        run_after_init: bool = False,
+        **kwargs,
+    ):
+
+        for node in args:
+            self.add_child(node)
+        super()._after_node_setup(
+            overwrite_save=overwrite_save, run_after_init=run_after_init, **kwargs
+        )
 
     @property
     def inputs_map(self) -> bidict | None:
         self._deduplicate_nones(self._inputs_map)
         return self._inputs_map
 
     @inputs_map.setter
@@ -159,76 +274,27 @@
     @staticmethod
     def _deduplicate_nones(some_map: dict | bidict | None) -> dict | bidict | None:
         if some_map is not None:
             for k, v in some_map.items():
                 if v is None:
                     some_map[k] = (None, f"{k} disabled")
 
-    def activate_strict_hints(self):
-        super().activate_strict_hints()
-        for node in self:
-            node.activate_strict_hints()
-
-    def deactivate_strict_hints(self):
-        super().deactivate_strict_hints()
-        for node in self:
-            node.deactivate_strict_hints()
-
-    def to_dict(self):
-        return {
-            "label": self.label,
-            "nodes": {n.label: n.to_dict() for n in self.children.values()},
-        }
-
     @property
-    def on_run(self):
-        return self.run_graph
+    def inputs(self) -> Inputs:
+        return self._build_inputs()
 
-    @staticmethod
-    def run_graph(_composite: Composite):
-        for node in _composite.starting_nodes:
-            node.run()
-        return _composite
+    def _build_inputs(self):
+        return self._build_io("inputs", self.inputs_map)
 
     @property
-    def run_args(self) -> dict:
-        return {"_composite": self}
+    def outputs(self) -> Outputs:
+        return self._build_outputs()
 
-    def process_run_result(self, run_output):
-        if run_output is not self:
-            self._parse_remotely_executed_self(run_output)
-        return DotDict(self.outputs.to_value_dict())
-
-    def _parse_remotely_executed_self(self, other_self):
-        # Un-parent existing nodes before ditching them
-        for node in self:
-            node._parent = None
-        other_self.running = False  # It's done now
-        self.__setstate__(other_self.__getstate__())
-
-    def disconnect_run(self) -> list[tuple[Channel, Channel]]:
-        """
-        Disconnect all `signals.input.run` connections on all child nodes.
-
-        Returns:
-            list[tuple[Channel, Channel]]: Any disconnected pairs.
-        """
-        disconnected_pairs = []
-        for node in self.children.values():
-            disconnected_pairs.extend(node.signals.disconnect_run())
-        return disconnected_pairs
-
-    def set_run_signals_to_dag_execution(self):
-        """
-        Disconnects all `signals.input.run` connections among children and attempts to
-        reconnect these according to the DAG flow of the data. On success, sets the
-        starting nodes to just be the upstream-most node in this linear DAG flow.
-        """
-        _, upstream_most_nodes = set_run_connections_according_to_dag(self.children)
-        self.starting_nodes = upstream_most_nodes
+    def _build_outputs(self):
+        return self._build_io("outputs", self.outputs_map)
 
     def _build_io(
         self,
         i_or_o: Literal["inputs", "outputs"],
         key_map: dict[str, str | None] | None,
     ) -> Inputs | Outputs:
         """
@@ -255,161 +321,97 @@
             for channel in panel:
                 try:
                     io_panel_key = key_map[channel.scoped_label]
                     if not isinstance(io_panel_key, tuple):
                         # Tuples indicate that the channel has been deactivated
                         # This is a necessary misdirection to keep the bidict working,
                         # as we can't simply map _multiple_ keys to `None`
-                        io[io_panel_key] = self._get_linking_channel(
-                            channel, io_panel_key
-                        )
+                        io[io_panel_key] = channel
                 except KeyError:
                     if not channel.connected:
-                        io[channel.scoped_label] = self._get_linking_channel(
-                            channel, channel.scoped_label
-                        )
+                        io[channel.scoped_label] = channel
         return io
 
-    @abstractmethod
-    def _get_linking_channel(
+    def run(
         self,
-        child_reference_channel: InputData | OutputData,
-        composite_io_key: str,
-    ) -> InputData | OutputData:
-        """
-        Returns the channel that will be the link between the provided child channel,
-        and the composite's IO at the given key.
-
-        The returned channel should be fully compatible with the provided child channel,
-        i.e. same type, same type hint... (For instance, the child channel itself is a
-        valid return, which would create a composite IO panel that works by reference.)
+        check_readiness: bool = True,
+        force_local_execution: bool = False,
+        **kwargs,
+    ):
+        # Note: Workflows may have neither parents nor siblings, so we don't need to
+        # worry about running their data trees first, fetching their input, nor firing
+        # their `ran` signal, hence the change in signature from Node.run
+        if self.automate_execution:
+            self.set_run_signals_to_dag_execution()
+        return super().run(
+            run_data_tree=False,
+            run_parent_trees_too=False,
+            fetch_input=False,
+            check_readiness=check_readiness,
+            force_local_execution=force_local_execution,
+            emit_ran_signal=False,
+            **kwargs,
+        )
 
-        Args:
-            child_reference_channel (InputData | OutputData): The child channel
-            composite_io_key (str): The key under which this channel will be stored on
-                the composite's IO.
+    def pull(self, run_parent_trees_too=False, **kwargs):
+        """Workflows are a parent-most object, so this simply runs without pulling."""
+        return self.run(**kwargs)
 
-        Returns:
-            (Channel): A channel with the same type, type hint, etc. as the reference
-                channel passed in.
+    def to_node(self):
         """
-        pass
-
-    def _build_inputs(self) -> Inputs:
-        return self._build_io("inputs", self.inputs_map)
-
-    def _build_outputs(self) -> Outputs:
-        return self._build_io("outputs", self.outputs_map)
-
-    def add_child(
-        self,
-        child: Node,
-        label: Optional[str] = None,
-        strict_naming: Optional[bool] = None,
-    ) -> Node:
-        if not isinstance(child, Node):
-            raise TypeError(
-                f"Only new {Node.__name__} instances may be added, but got "
-                f"{type(child)}."
-            )
-        return super().add_child(child, label=label, strict_naming=strict_naming)
+        Export the workflow to a macro node, with the currently exposed IO mapped to
+        new IO channels, and the workflow mapped into the node_function.
+        """
+        raise NotImplementedError
 
-    def remove_child(self, child: Node | str) -> list[tuple[Channel, Channel]]:
+    @property
+    def _data_connections(self) -> list[tuple[tuple[str, str], tuple[str, str]]]:
         """
-        Remove a child from the :attr:`children` collection, disconnecting it and
-        setting its :attr:`parent` to None.
+        A string-tuple representation of all connections between the data channels of
+        child nodes.
 
-        Args:
-            child (Node|str): The child (or its label) to remove.
+        Intended for internal use during storage, so that connections can be
+        represented in plain strings, and stored on an attribute to guarantee that the
+        name does not conflict with a child node label.
 
         Returns:
-            (list[tuple[Channel, Channel]]): Any connections that node had.
+            (list): Nested-pair tuples of (node label, channel label) data for
+                (input, output) channels of data connections between children.
         """
-        child = super().remove_child(child)
-        disconnected = child.disconnect()
-        if child in self.starting_nodes:
-            self.starting_nodes.remove(child)
-        return disconnected
+        data_connections = []
+        for node in self:
+            for inp_label, inp in node.inputs.items():
+                for conn in inp.connections:
+                    data_connections.append(
+                        ((node.label, inp_label), (conn.owner.label, conn.label))
+                    )
+        return data_connections
 
-    def replace_child(
-        self, owned_node: Node | str, replacement: Node | type[Node]
-    ) -> Node:
+    @property
+    def _signal_connections(self) -> list[tuple[tuple[str, str], tuple[str, str]]]:
         """
-        Replaces a node currently owned with a new node instance.
-        The replacement must not belong to any other parent or have any connections.
-        The IO of the new node must be a perfect superset of the replaced node, i.e.
-        channel labels need to match precisely, but additional channels may be present.
-        After replacement, the new node will have the old node's connections, label,
-        and belong to this composite.
-        The labels are swapped, such that the replaced node gets the name of its
-        replacement (which might be silly, but is useful in case you want to revert the
-        change and swap the replaced node back in!)
+        A string-tuple representation of all connections between the signal channels of
+        child nodes.
 
-        If replacement fails for some reason, the replacement and replacing node are
-        both returned to their original state, and the composite is left unchanged.
-
-        Args:
-            owned_node (Node|str): The node to replace or its label.
-            replacement (Node | type[Node]): The node or class to replace it with. (If
-                a class is passed, it has all the same requirements on IO compatibility
-                and simply gets instantiated.)
+        Intended for internal use during storage, so that connections can be
+        represented in plain strings, and stored on an attribute to guarantee that the
+        name does not conflict
 
         Returns:
-            (Node): The node that got removed
+            (list): Nested-pair tuples of (node label, channel label) data for
+                (input, output) channels of signal connections between children.
         """
-        if isinstance(owned_node, str):
-            owned_node = self.children[owned_node]
-
-        if owned_node.parent is not self:
-            raise ValueError(
-                f"The node being replaced should be a child of this composite, but "
-                f"another parent was found: {owned_node.parent}"
-            )
-
-        if isinstance(replacement, Node):
-            if replacement.parent is not None:
-                raise ValueError(
-                    f"Replacement node must have no parent, but got "
-                    f"{replacement.parent}"
-                )
-            if replacement.connected:
-                raise ValueError("Replacement node must not have any connections")
-        elif issubclass(replacement, Node):
-            replacement = replacement(label=owned_node.label)
-        else:
-            raise TypeError(
-                f"Expected replacement node to be a node instance or node subclass, but "
-                f"got {replacement}"
-            )
-
-        replacement.copy_io(owned_node)  # If the replacement is incompatible, we'll
-        # fail here before we've changed the parent at all. Since the replacement was
-        # first guaranteed to be an unconnected orphan, there is not yet any permanent
-        # damage
-        is_starting_node = owned_node in self.starting_nodes
-        self.remove_child(owned_node)
-        replacement.label, owned_node.label = owned_node.label, replacement.label
-        self.add_child(replacement)
-        if is_starting_node:
-            self.starting_nodes.append(replacement)
-
-        # Finally, make sure the IO is constructible with this new node, which will
-        # catch things like incompatible IO maps
-        try:
-            # Make sure node-level IO is pointing to the new node and that macro-level
-            # IO gets safely reconstructed
-            self._rebuild_data_io()
-        except Exception as e:
-            # If IO can't be successfully rebuilt using this node, revert changes and
-            # raise the exception
-            self.replace_child(replacement, owned_node)  # Guaranteed to work since
-            # replacement in the other direction was already a success
-            raise e
-
-        return owned_node
+        signal_connections = []
+        for node in self:
+            for inp_label, inp in node.signals.input.items():
+                for conn in inp.connections:
+                    signal_connections.append(
+                        ((node.label, inp_label), (conn.owner.label, conn.label))
+                    )
+        return signal_connections
 
     def _rebuild_data_io(self):
         """
         Try to rebuild the IO.
 
         If an error is encountered, revert back to the existing IO then raise it.
         """
@@ -441,236 +443,145 @@
             self._outputs = old_outputs
             e.message = (
                 f"Unable to rebuild IO for {self.label}; reverting to old IO."
                 f"{e.message}"
             )
             raise e
 
-    @classmethod
-    @wraps(Creator.register)
-    def register(cls, package_identifier: str, domain: Optional[str] = None) -> None:
-        cls.create.register(package_identifier=package_identifier, domain=domain)
-
-    def executor_shutdown(self, wait=True, *, cancel_futures=False):
-        """
-        Invoke shutdown on the executor (if present), and recursively invoke shutdown
-        for children.
-        """
-        super().executor_shutdown(wait=wait, cancel_futures=cancel_futures)
-        for node in self:
-            node.executor_shutdown(wait=wait, cancel_futures=cancel_futures)
-
-    def __setattr__(self, key: str, node: Node):
-        if isinstance(node, Composite) and key in ["_parent", "parent"]:
-            # This is an edge case for assigning a node to an attribute
-            # We either defer to the setter with super, or directly assign the private
-            # variable (as requested in the setter)
-            super().__setattr__(key, node)
-        elif isinstance(node, Node):
-            self.add_child(node, label=key)
-        elif (
-            isinstance(node, type)
-            and issubclass(node, Node)
-            and key in self.children.keys()
-        ):
-            # When a class is assigned to an existing node, try a replacement
-            self.replace_child(key, node)
-        else:
-            super().__setattr__(key, node)
-
-    def __getitem__(self, item):
-        return self.__getattr__(item)
-
-    def __setitem__(self, key, value):
-        self.__setattr__(key, value)
-
-    @property
-    def color(self) -> str:
-        """For drawing the graph"""
-        return SeabornColors.brown
-
-    @property
-    def package_requirements(self) -> set[str]:
-        """
-        A list of node package identifiers for children.
-        """
-        return set(n.package_identifier for n in self)
-
     def to_storage(self, storage):
-        storage["nodes"] = list(self.children.keys())
-        for label, node in self.children.items():
-            node.to_storage(storage.create_group(label))
-
+        storage["package_requirements"] = list(self.package_requirements)
+        storage["automate_execution"] = self.automate_execution
         storage["inputs_map"] = self.inputs_map
         storage["outputs_map"] = self.outputs_map
-
         super().to_storage(storage)
 
+        storage["_data_connections"] = self._data_connections
+
+        if not self.automate_execution:
+            storage["_signal_connections"] = self._signal_connections
+            storage["starting_nodes"] = [n.label for n in self.starting_nodes]
+
     def from_storage(self, storage):
         from pyiron_contrib.tinybase.storage import GenericStorage
 
         self.inputs_map = (
             storage["inputs_map"].to_object()
             if isinstance(storage["inputs_map"], GenericStorage)
             else storage["inputs_map"]
         )
         self.outputs_map = (
             storage["outputs_map"].to_object()
             if isinstance(storage["outputs_map"], GenericStorage)
             else storage["outputs_map"]
         )
-        self._rebuild_data_io()  # To apply any map that was saved
 
+        self._reinstantiate_children(storage)
+        self.automate_execution = storage["automate_execution"]
         super().from_storage(storage)
+        self._rebuild_data_io()  # To apply any map that was saved
+        self._rebuild_connections(storage)
 
-    def tidy_working_directory(self):
-        for node in self:
-            node.tidy_working_directory()
-        super().tidy_working_directory()
+    def _reinstantiate_children(self, storage):
+        # Parents attempt to reload their data on instantiation,
+        # so there is no need to explicitly load any of these children
+        for package_identifier in storage["package_requirements"]:
+            self.register(package_identifier)
+
+        for child_label in storage["nodes"]:
+            child_data = storage[child_label]
+            pid = child_data["package_identifier"]
+            cls = child_data["class_name"]
+            self.create[pid][cls](
+                label=child_label, parent=self, storage_backend="tinybase"
+            )
 
-    def _get_connections_as_strings(
-        self, panel_getter: callable
-    ) -> list[tuple[tuple[str, str], tuple[str, str]]]:
-        """
-        Connections between children in string representation based on labels.
+    def _rebuild_connections(self, storage):
+        self._rebuild_data_connections(storage)
+        if not self.automate_execution:
+            self._rebuild_execution_graph(storage)
+
+    def _rebuild_data_connections(self, storage):
+        for data_connection in storage["_data_connections"]:
+            (inp_label, inp_channel), (out_label, out_channel) = data_connection
+            self.children[inp_label].inputs[inp_channel].connect(
+                self.children[out_label].outputs[out_channel]
+            )
 
-        The string representation helps storage, and having it as a property ensures
-        the name is protected.
-        """
-        return [
-            ((inp.owner.label, inp.label), (out.owner.label, out.label))
-            for child in self
-            for inp in panel_getter(child)
-            for out in inp.connections
+    def _rebuild_execution_graph(self, storage):
+        for signal_connection in storage["_signal_connections"]:
+            (inp_label, inp_channel), (out_label, out_channel) = signal_connection
+            self.children[inp_label].signals.input[inp_channel].connect(
+                self.children[out_label].signals.output[out_channel]
+            )
+        self.starting_nodes = [
+            self.children[label] for label in storage["starting_nodes"]
         ]
 
-    @staticmethod
-    def _get_data_inputs(node: Node):
-        return node.inputs
-
-    @staticmethod
-    def _get_signals_input(node: Node):
-        return node.signals.input
-
-    @property
-    def _child_data_connections(self) -> list[tuple[tuple[str, str], tuple[str, str]]]:
-        return self._get_connections_as_strings(self._get_data_inputs)
-
-    @property
-    def _child_signal_connections(
-        self,
-    ) -> list[tuple[tuple[str, str], tuple[str, str]]]:
-        return self._get_connections_as_strings(self._get_signals_input)
-
-    @property
-    def _starting_node_labels(self):
-        # As a property so it appears in `__dir__` and thus is guaranteed to not
-        # conflict with a child node name in the state
-        return tuple(n.label for n in self.starting_nodes)
-
     def __getstate__(self):
         state = super().__getstate__()
-        # Store connections as strings
-        state["_child_data_connections"] = self._child_data_connections
-        state["_child_signal_connections"] = self._child_signal_connections
 
         # Transform the IO maps into a datatype that plays well with h5io
         # (Bidict implements a custom reconstructor, which hurts us)
         state["_inputs_map"] = (
             None if self._inputs_map is None else dict(self._inputs_map)
         )
         state["_outputs_map"] = (
             None if self._outputs_map is None else dict(self._outputs_map)
         )
 
-        # Also remove the starting node instances
-        del state["starting_nodes"]
-        state["_starting_node_labels"] = self._starting_node_labels
-
         return state
 
     def __setstate__(self, state):
-        # Purge child connection info from the state
-        child_data_connections = state.pop("_child_data_connections")
-        child_signal_connections = state.pop("_child_signal_connections")
-
         # Transform the IO maps back into the right class (bidict)
         state["_inputs_map"] = (
             None if state["_inputs_map"] is None else bidict(state["_inputs_map"])
         )
         state["_outputs_map"] = (
             None if state["_outputs_map"] is None else bidict(state["_outputs_map"])
         )
 
-        # Restore starting nodes
-        state["starting_nodes"] = [
-            state[label] for label in state.pop("_starting_node_labels")
-        ]
-
         super().__setstate__(state)
 
-        # Nodes don't store connection information, so restore it to them
-        self._restore_data_connections_from_strings(child_data_connections)
-        self._restore_signal_connections_from_strings(child_signal_connections)
-
-    @staticmethod
-    def _restore_connections_from_strings(
-        nodes: dict[str, Node] | DotDict[str, Node],
-        connections: list[tuple[tuple[str, str], tuple[str, str]]],
-        input_panel_getter: callable,
-        output_panel_getter: callable,
-    ) -> None:
-        """
-        Set connections among a dictionary of nodes.
-
-        This is useful for recreating node connections after (de)serialization of the
-        individual nodes, which don't know about their connections (that information is
-        the responsibility of their parent `Composite`).
-
-        Args:
-            nodes (dict[Node]): The nodes to connect.
-            connections (list[tuple[tuple[str, str], tuple[str, str]]]): Connections
-                among these nodes in the format ((input node label, input channel label
-                ), (output node label, output channel label)).
-        """
-        for (inp_node, inp), (out_node, out) in connections:
-            input_panel_getter(nodes[inp_node])[inp].connect(
-                output_panel_getter(nodes[out_node])[out]
+    def save(self):
+        if self.storage_backend == "tinybase" and any(
+            node.package_identifier is None for node in self
+        ):
+            raise NotImplementedError(
+                f"{self.__class__.__name__} can currently only save itself to file if "
+                f"_all_ of its child nodes were created via the creator and have an "
+                f"associated `package_identifier` -- otherwise we won't know how to "
+                f"re-instantiate them at load time! Right now this is as easy as "
+                f"moving your custom nodes to their own .py file and registering it "
+                f"like any other node package. Remember that this new module needs to "
+                f"be in your python path and importable at load time too."
             )
+        super().save()
 
-    @staticmethod
-    def _get_data_outputs(node: Node):
-        return node.outputs
-
-    @staticmethod
-    def _get_signals_output(node: Node):
-        return node.signals.output
-
-    def _restore_data_connections_from_strings(
-        self, connections: list[tuple[tuple[str, str], tuple[str, str]]]
-    ) -> None:
-        self._restore_connections_from_strings(
-            self.children,
-            connections,
-            self._get_data_inputs,
-            self._get_data_outputs,
-        )
+    @property
+    def _owned_io_panels(self) -> list[IO]:
+        # Workflow data IO is just pointers to child IO, not actually owned directly
+        # by the workflow; this is used in re-parenting channels, and we don't want to
+        # override the real parent with this workflow!
+        return [
+            self.signals.input,
+            self.signals.output,
+        ]
 
-    def _restore_signal_connections_from_strings(
-        self, connections: list[tuple[tuple[str, str], tuple[str, str]]]
-    ) -> None:
-        self._restore_connections_from_strings(
-            self.children,
-            connections,
-            self._get_signals_input,
-            self._get_signals_output,
-        )
+    def replace_child(
+        self, owned_node: Node | str, replacement: Node | type[Node]
+    ) -> Node:
+        super().replace_child(owned_node=owned_node, replacement=replacement)
 
-    @property
-    def import_ready(self) -> bool:
-        return super().import_ready and all(node.import_ready for node in self)
+        # Finally, make sure the IO is constructible with this new node, which will
+        # catch things like incompatible IO maps
+        try:
+            # Make sure node-level IO is pointing to the new node and that macro-level
+            # IO gets safely reconstructed
+            self._rebuild_data_io()
+        except Exception as e:
+            # If IO can't be successfully rebuilt using this node, revert changes and
+            # raise the exception
+            self.replace_child(replacement, owned_node)  # Guaranteed to work since
+            # replacement in the other direction was already a success
+            raise e
 
-    def report_import_readiness(self, tabs=0, report_so_far=""):
-        report = super().report_import_readiness(tabs=tabs, report_so_far=report_so_far)
-        for node in self:
-            report = node.report_import_readiness(tabs=tabs + 1, report_so_far=report)
-        return report
+        return owned_node
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/create.py` & `pyiron_workflow-0.6.0/pyiron_workflow/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Container classes for giving access to various workflow objects and tools
 """
 
 from __future__ import annotations
 
+from abc import ABC
+from functools import wraps
 from importlib import import_module
 import pkgutil
 from sys import version_info
 from types import ModuleType
 from typing import Optional, TYPE_CHECKING
 
 from bidict import bidict
@@ -26,15 +28,15 @@
     PyFluxExecutor = None
 
 from pyiron_workflow.executors import CloudpickleProcessPoolExecutor
 
 # Then choose one executor to be "standard"
 Executor = PyMpiPoolExecutor
 
-from pyiron_workflow.function import Function, function_node
+from pyiron_workflow.function import function_node, as_function_node
 from pyiron_workflow.snippets.dotdict import DotDict
 
 if TYPE_CHECKING:
     from pyiron_workflow.node_package import NodePackage
 
 
 class Creator(metaclass=Singleton):
@@ -56,18 +58,18 @@
         self._package_registry = bidict()
 
         self.Executor = Executor
         self.CloudpickleProcessPoolExecutor = CloudpickleProcessPoolExecutor
         self.PyMPIExecutor = PyMPIExecutor
         self.PyMpiPoolExecutor = PyMpiPoolExecutor
 
-        self.Function = Function
+        self.function_node = function_node
 
         # Avoid circular imports by delaying import for children of Composite
-        self._macro = None
+        self._macro_node = None
         self._workflow = None
         self._meta = None
 
         if version_info[0] == 3 and version_info[1] >= 10:
             # These modules use syntactic sugar for type hinting that is only supported
             # in python >=3.10
             # If the CI skips testing on 3.9 gets dropped, we can think about removing
@@ -83,38 +85,38 @@
     @property
     def PySlurmExecutor(self):
         if PySlurmExecutor is None:
             raise ImportError(f"{PySlurmExecutor.__name__} is not available")
         return PySlurmExecutor
 
     @property
-    def Macro(self):
-        if self._macro is None:
-            from pyiron_workflow.macro import Macro
+    def macro_node(self):
+        if self._macro_node is None:
+            from pyiron_workflow.macro import macro_node
 
-            self._macro = Macro
-        return self._macro
+            self._macro_node = macro_node
+        return self._macro_node
 
     @property
     def Workflow(self):
         if self._workflow is None:
             from pyiron_workflow.workflow import Workflow
 
             self._workflow = Workflow
         return self._workflow
 
     @property
     def meta(self):
         if self._meta is None:
             from pyiron_workflow.meta import (
-                for_loop,
                 input_to_list,
                 list_to_output,
-                while_loop,
             )
+            from pyiron_workflow.loops import while_loop
+            from pyiron_workflow.loops import for_loop
             from pyiron_workflow.snippets.dotdict import DotDict
 
             self._meta = DotDict(
                 {
                     for_loop.__name__: for_loop,
                     input_to_list.__name__: input_to_list,
                     list_to_output.__name__: list_to_output,
@@ -312,19 +314,34 @@
 
 class Wrappers(metaclass=Singleton):
     """
     A container class giving access to the decorators that transform functions to nodes.
     """
 
     def __init__(self):
-        self.function_node = function_node
+        self.as_function_node = as_function_node
 
         # Avoid circular imports by delaying import when wrapping children of Composite
-        self._macro_node = None
+        self._as_macro_node = None
 
     @property
-    def macro_node(self):
-        if self._macro_node is None:
-            from pyiron_workflow.macro import macro_node
+    def as_macro_node(self):
+        if self._as_macro_node is None:
+            from pyiron_workflow.macro import as_macro_node
 
-            self._macro_node = macro_node
-        return self._macro_node
+            self._as_macro_node = as_macro_node
+        return self._as_macro_node
+
+
+class HasCreator(ABC):
+    """
+    A mixin class for creator (including both class-like and decorator) and
+    registration methods.
+    """
+
+    create = Creator()
+    wrap = Wrappers()
+
+    @classmethod
+    @wraps(Creator.register)
+    def register(cls, package_identifier: str, domain: Optional[str] = None) -> None:
+        cls.create.register(package_identifier=package_identifier, domain=domain)
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/draw.py` & `pyiron_workflow-0.6.0/pyiron_workflow/draw.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/executors/cloudpickleprocesspool.py` & `pyiron_workflow-0.6.0/pyiron_workflow/executors/cloudpickleprocesspool.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,19 @@
 
         >>> print(fs.result().__class__.__name__)
         DynamicFoo
 
         >>> print(fs.done())
         True
 
+        >>> import time
+        >>> time.sleep(1)  # Debugging doctest on github CI for python3.10
         >>> print(instance.result.result)
         This was an arg
+
     """
 
     def submit(self, fn, /, *args, **kwargs):
         return self._submit(
             _CloudPickledCallable(fn),
             _CloudPickledCallable.dumps(args),
             _CloudPickledCallable.dumps(kwargs),
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/function.py` & `pyiron_workflow-0.6.0/pyiron_workflow/function.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from __future__ import annotations
 
-import inspect
-import warnings
-from functools import partialmethod
-from typing import Any, get_args, get_type_hints, Literal, Optional, TYPE_CHECKING
-
-from pyiron_workflow.channels import InputData, OutputData, NOT_DATA
-from pyiron_workflow.has_interface_mixins import HasChannel
-from pyiron_workflow.injection import OutputDataWithInjection
-from pyiron_workflow.io import Inputs, Outputs
-from pyiron_workflow.node import Node
-from pyiron_workflow.output_parser import ParseOutput
+from abc import ABC, abstractmethod
+from typing import Any, Literal, Optional, TYPE_CHECKING
+
+from pyiron_workflow.io_preview import DecoratedNode, decorated_node_decorator_factory
 from pyiron_workflow.snippets.colors import SeabornColors
 
 if TYPE_CHECKING:
     from pyiron_workflow.composite import Composite
 
 
-class Function(Node):
+class Function(DecoratedNode, ABC):
     """
     Function nodes wrap an arbitrary python function.
 
     Actual function node instances can either be instances of the base node class, in
     which case the callable node function *must* be provided OR they can be instances
     of children of this class which provide the node function as a class-level method.
     Those children may define some or all of the node behaviour at the class level, and
@@ -45,42 +38,24 @@
         - A single tuple output channel can be forced by manually providing exactly one
             output label
     - Running the node executes the wrapped function and returns its result
     - Input updates can be made with `*args` as well as the usual `**kwargs`, following
         the same input order as the wrapped function.
     - A default label can be scraped from the name of the wrapped function
 
-    Args:
-        node_function (callable): The function determining the behaviour of the node.
-        label (str): The node's label. (Defaults to the node function's name.)
-        output_labels (Optional[str | list[str] | tuple[str]]): A name for each return
-            value of the node function OR a single label. (Default is None, which
-            scrapes output labels automatically from the source code of the wrapped
-            function.) This can be useful when returned values are not well named, e.g.
-            to make the output channel dot-accessible if it would otherwise have a label
-            that requires item-string-based access. Additionally, specifying a _single_
-            label for a wrapped function that returns a tuple of values ensures that a
-            _single_ output channel (holding the tuple) is created, instead of one
-            channel for each return value. The default approach of extracting labels
-            from the function source code also requires that the function body contain
-            _at most_ one `return` expression, so providing explicit labels can be used
-            to circumvent this (at your own risk).
-        **kwargs: Any additional keyword arguments whose keyword matches the label of an
-            input channel will have their value assigned to that channel.
-
     Examples:
         At the most basic level, to use nodes all we need to do is provide the
         `Function` class with a function and labels for its output, like so:
 
-        >>> from pyiron_workflow.function import Function
+        >>> from pyiron_workflow.function import function_node
         >>>
         >>> def mwe(x, y):
         ...     return x+1, y-1
         >>>
-        >>> plus_minus_1 = Function(mwe)
+        >>> plus_minus_1 = function_node(mwe)
         >>>
         >>> print(plus_minus_1.outputs["x+1"])
         NOT_DATA
 
         There is no output because we haven't given our function any input, it has
         no defaults, and we never ran it! So outputs have the channel default value of
         `NOT_DATA` -- a special non-data singleton (since `None` is sometimes a
@@ -125,57 +100,57 @@
 
         >>> plus_minus_1.failed = False
         >>> plus_minus_1.inputs.y = 3
         >>> out = plus_minus_1.run()
         >>> plus_minus_1.outputs.to_value_dict()
         {'x+1': 3, 'y-1': 2}
 
-        We can also, optionally, provide initial values for some or all of the input and
-        labels for the output:
+        We can also, optionally, provide initial values for some or all of the input
+        and labels for the output:
 
-        >>> plus_minus_1 = Function(mwe, output_labels=("p1", "m1"),  x=1)
+        >>> plus_minus_1 = function_node(mwe, output_labels=("p1", "m1"),  x=1)
         >>> plus_minus_1.inputs.y = 2
         >>> out = plus_minus_1.run()
         >>> out
         (2, 1)
 
         Input data can be provided to both initialization and on call as ordered args
         or keyword kwargs.
         When running the node (or any alias to run like pull, execute, or just calling
         the node), the output of the wrapped function is returned:
 
         >>> plus_minus_1(2, y=3)
         (3, 2)
 
         We can make our node even more sensible by adding type
-        hints (and, optionally, default values) when defining the function that the node
-        wraps.
+        hints (and, optionally, default values) when defining the function that the
+        node wraps.
         The node will automatically figure out defaults and type hints for the IO
         channels from inspection of the wrapped function.
 
         In this example, note the mixture of old-school (`typing.Union`) and new (`|`)
         type hints as well as nested hinting with a union-type inside the tuple for the
         return hint.
         Our treatment of type hints is **not infinitely robust**, but covers a wide
         variety of common use cases.
         Note that getting "good" (i.e. dot-accessible) output labels can be achieved by
         using good variable names and returning those variables instead of using
-        :attr:`output_labels`.
+        :param:`output_labels`.
         If we try to assign a value of the wrong type, it will raise an error:
 
         >>> from typing import Union
         >>>
         >>> def hinted_example(
         ...     x: Union[int, float],
         ...     y: int | float = 1
         ... ) -> tuple[int, int | float]:
         ...     p1, m1 = x+1, y-1
         ...     return p1, m1
         >>>
-        >>> plus_minus_1 = Function(hinted_example)
+        >>> plus_minus_1 = function_node(hinted_example)
         >>> try:
         ...     plus_minus_1.inputs.x =  "not an int or float"
         ... except TypeError as e:
         ...     print("TypeError:", e.args[0])
         TypeError: The channel x cannot take the value `not an int or float` because it is not compliant with the type hint typing.Union[int, float]
 
         We can turn off type hinting with the `strict_hints` boolean property, or just
@@ -203,29 +178,31 @@
         This causes the failure to come earlier because we stop the node from running
         and throwing an error because it sees that the channel (and thus node) is not
         ready:
 
         >>> plus_minus_1.ready, plus_minus_1.inputs.x.ready, plus_minus_1.inputs.y.ready
         (False, False, True)
 
-        In these examples, we've instantiated nodes directly from the base :class:`Function`
-        class, and populated their input directly with data.
+        In these examples, we've instantiated nodes directly from the base
+        :class:`Function` class, and populated their input directly with data.
         In practice, these nodes are meant to be part of complex workflows; that means
         both that you are likely to have particular nodes that get heavily re-used, and
         that you need the nodes to pass data to each other.
 
-        For reusable nodes, we want to create a sub-class of :class:`Function` that fixes some
-        of the node behaviour -- usually the :meth:`node_function` and :attr:`output_labels`.
+        For reusable nodes, we want to create a sub-class of :class:`Function`
+        that fixes some of the node behaviour -- i.e. the :meth:`node_function`.
 
-        This can be done most easily with the :func:`function_node` decorator, which takes a function
-        and returns a node class:
+        This can be done most easily with the :func:`as_function_node` decorator, which
+        takes a function and returns a node class. It also allows us to provide labels
+        for the return values, :param:output_labels, which are otherwise scraped from
+        the text of the function definition:
 
-        >>> from pyiron_workflow.function import function_node
+        >>> from pyiron_workflow.function import as_function_node
         >>>
-        >>> @function_node("p1", "m1")
+        >>> @as_function_node("p1", "m1")
         ... def my_mwe_node(
         ...     x: int | float, y: int | float = 1
         ... ) -> tuple[int | float, int | float]:
         ...     return x+1, y-1
         >>>
         >>> node_instance = my_mwe_node(x=0)
         >>> node_instance(y=0)
@@ -237,42 +214,34 @@
         Because we provided a good initial value for `x`, we get our result right away.
 
         Using the decorator is the recommended way to create new node classes, but this
         magic is just equivalent to creating a child class with the `node_function`
         already defined as a `staticmethod`:
 
         >>> from typing import Literal, Optional
+        >>> from pyiron_workflow.function import Function
         >>>
         >>> class AlphabetModThree(Function):
-        ...     def __init__(
-        ...         self,
-        ...         label: Optional[str] = None,
-        ...         **kwargs
-        ...     ):
-        ...         super().__init__(
-        ...             None,
-        ...             label=label,
-        ...             **kwargs
-        ...         )
         ...
         ...     @staticmethod
         ...     def node_function(i: int) -> Literal["a", "b", "c"]:
         ...         letter = ["a", "b", "c"][i % 3]
         ...         return letter
 
+
         Finally, let's put it all together by using both of these nodes at once.
         Instead of setting input to a particular data value, we'll set it to
         be another node's output channel, thus forming a connection.
         At the end of the day, the graph will also need to know about the execution
         flow, but in most cases (directed acyclic graphs -- DAGs), this can be worked
         out automatically by the topology of data connections.
         Let's put together a couple of nodes and then run in a "pull" paradigm to get
         the final node to run everything "upstream" then run itself:
 
-        >>> @function_node()
+        >>> @as_function_node()
         ... def adder_node(x: int = 0, y: int = 0) -> int:
         ...     sum = x + y
         ...     return sum
         >>>
         >>> adder = adder_node(x=1)
         >>> alpha = AlphabetModThree(i=adder.outputs.sum)
         >>> print(alpha())
@@ -291,15 +260,15 @@
         some syntactic sugar using the `>` operator.
         Then we can use a "push" paradigm with the `run` command to force execution
         forwards through the graph to get an end result.
         This is a bit more verbose, but a necessary tool for more complex situations
         (like cyclic graphs).
         Here's our simple example from above using this other paradigm:
 
-        >>> @function_node()
+        >>> @as_function_node()
         ... def adder_node(x: int = 0, y: int = 0) -> int:
         ...     sum = x + y
         ...     return sum
         >>>
         >>> adder = adder_node()
         >>> alpha = AlphabetModThree(i=adder.outputs.sum)
         >>> _ = adder >> alpha
@@ -322,267 +291,49 @@
 
     Comments:
         Using the `self` argument for function nodes is not fully supported; it will
         raise an error when combined with an executor, and otherwise behaviour is not
         guaranteed.
     """
 
-    def __init__(
-        self,
-        node_function: callable,
-        *args,
-        label: Optional[str] = None,
-        parent: Optional[Composite] = None,
-        overwrite_save: bool = False,
-        run_after_init: bool = False,
-        storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
-        save_after_run: bool = False,
-        output_labels: Optional[str | list[str] | tuple[str]] = None,
-        **kwargs,
-    ):
-        if not callable(node_function):
-            # Children of `Function` may explicitly provide a `node_function` static
-            # method so the node has fixed behaviour.
-            # In this case, the `__init__` signature should be changed so that the
-            # `node_function` argument is just always `None` or some other non-callable.
-            # If a callable `node_function` is not received, you'd better have it as an
-            # attribute already!
-            if not hasattr(self, "node_function"):
-                raise AttributeError(
-                    f"If `None` is provided as a `node_function`, a `node_function` "
-                    f"property must be defined instead, e.g. when making child classes"
-                    f"of `Function` with specific behaviour"
-                )
-            self._type_hints = get_type_hints(self.node_function)
-        else:
-            # If a callable node function is received, use it
-            self.node_function = node_function
-            self._type_hints = get_type_hints(node_function)
-
-        super().__init__(
-            label=label if label is not None else self.node_function.__name__,
-            parent=parent,
-            save_after_run=save_after_run,
-            storage_backend=storage_backend,
-            # **kwargs,
-        )
-
-        self._inputs = None
-        self._outputs = None
-        self._output_labels = self._get_output_labels(output_labels)
-        # TODO: Parse output labels from the node function in case output_labels is None
-
-        self.set_input_values(*args, **kwargs)
-
-    def _get_output_labels(self, output_labels: str | list[str] | tuple[str] | None):
-        """
-        If output labels are provided, turn convert them to a list if passed as a
-        string and return them, else scrape them from the source channel.
-
-        Note: When the user explicitly provides output channels, they are taking
-        responsibility that these are correct, e.g. in terms of quantity, order, etc.
-        """
-        if output_labels is None:
-            return self._scrape_output_labels()
-        elif isinstance(output_labels, str):
-            return [output_labels]
-        else:
-            return output_labels
-
-    def _scrape_output_labels(self):
-        """
-        Inspect the source code to scrape out strings representing the returned values.
-        _Only_ works for functions with a single `return` expression in their body.
-
-        Will return expressions and function calls just fine, thus best practice is to
-        create well-named variables and return those so that the output labels stay
-        dot-accessible.
-        """
-        parsed_outputs = ParseOutput(self.node_function).output
-        return [None] if parsed_outputs is None else parsed_outputs
-
-    @property
-    def _input_args(self):
-        return inspect.signature(self.node_function).parameters
-
-    @property
-    def inputs(self) -> Inputs:
-        if self._inputs is None:
-            self._inputs = Inputs(*self._build_input_channels())
-        return self._inputs
-
-    @property
-    def outputs(self) -> Outputs:
-        if self._outputs is None:
-            self._outputs = Outputs(*self._build_output_channels(*self._output_labels))
-        return self._outputs
-
-    def _build_input_channels(self):
-        channels = []
-        type_hints = self._type_hints
-
-        for ii, (label, value) in enumerate(self._input_args.items()):
-            is_self = False
-            if label == "self":  # `self` is reserved for the node object
-                if ii == 0:
-                    is_self = True
-                else:
-                    warnings.warn(
-                        "`self` is used as an argument but not in the first"
-                        " position, so it is treated as a normal function"
-                        " argument. If it is to be treated as the node object,"
-                        " use it as a first argument"
-                    )
-            if label in self._init_keywords:
-                # We allow users to parse arbitrary kwargs as channel initialization
-                # So don't let them choose bad channel names
-                raise ValueError(
-                    f"The Input channel name {label} is not valid. Please choose a "
-                    f"name _not_ among {self._init_keywords}"
-                )
-
-            try:
-                type_hint = type_hints[label]
-                if is_self:
-                    warnings.warn("type hint for self ignored")
-            except KeyError:
-                type_hint = None
-
-            default = NOT_DATA  # The standard default in DataChannel
-            if value.default is not inspect.Parameter.empty:
-                if is_self:
-                    warnings.warn("default value for self ignored")
-                else:
-                    default = value.default
-
-            if not is_self:
-                channels.append(
-                    InputData(
-                        label=label,
-                        owner=self,
-                        default=default,
-                        type_hint=type_hint,
-                    )
-                )
-        return channels
-
-    @property
-    def _init_keywords(self):
-        return list(inspect.signature(self.__init__).parameters.keys())
-
-    def _build_output_channels(self, *return_labels: str):
-        try:
-            type_hints = self._type_hints["return"]
-            if len(return_labels) > 1:
-                type_hints = get_args(type_hints)
-                if not isinstance(type_hints, tuple):
-                    raise TypeError(
-                        f"With multiple return labels expected to get a tuple of type "
-                        f"hints, but got type {type(type_hints)}"
-                    )
-                if len(type_hints) != len(return_labels):
-                    raise ValueError(
-                        f"Expected type hints and return labels to have matching "
-                        f"lengths, but got {len(type_hints)} hints and "
-                        f"{len(return_labels)} labels: {type_hints}, {return_labels}"
-                    )
-            else:
-                # If there's only one hint, wrap it in a tuple so we can zip it with
-                # *return_labels and iterate over both at once
-                type_hints = (type_hints,)
-        except KeyError:
-            type_hints = [None] * len(return_labels)
-
-        channels = []
-        for label, hint in zip(return_labels, type_hints):
-            channels.append(
-                OutputDataWithInjection(
-                    label=label,
-                    owner=self,
-                    type_hint=hint,
-                )
-            )
-
-        return channels
+    @staticmethod
+    @abstractmethod
+    def node_function(*args, **kwargs) -> callable:
+        """What the node _does_."""
+
+    @classmethod
+    def _io_defining_function(cls) -> callable:
+        return cls.node_function
+
+    @classmethod
+    def _build_outputs_preview(cls) -> dict[str, Any]:
+        preview = super(Function, cls)._build_outputs_preview()
+        return preview if len(preview) > 0 else {"None": type(None)}
+        # If clause facilitates functions with no return value
 
     @property
     def on_run(self):
         return self.node_function
 
     @property
     def run_args(self) -> dict:
         kwargs = self.inputs.to_value_dict()
-        if "self" in self._input_args:
-            if self.executor:
-                raise ValueError(
-                    f"Function node {self.label} uses the `self` argument, but this "
-                    f"can't yet be run with executors"
-                )
-            kwargs["self"] = self
         return kwargs
 
     def process_run_result(self, function_output: Any | tuple) -> Any | tuple:
         """
         Take the results of the node function, and use them to update the node output.
         """
         for out, value in zip(
             self.outputs,
             (function_output,) if len(self.outputs) == 1 else function_output,
         ):
             out.value = value
         return function_output
 
-    def _convert_input_args_and_kwargs_to_input_kwargs(self, *args, **kwargs):
-        reverse_keys = list(self._input_args.keys())[::-1]
-        if len(args) > len(reverse_keys):
-            raise ValueError(
-                f"Received {len(args)} positional arguments, but the node {self.label}"
-                f"only accepts {len(reverse_keys)} inputs."
-            )
-
-        positional_keywords = reverse_keys[-len(args) :] if len(args) > 0 else []  # -0:
-        if len(set(positional_keywords).intersection(kwargs.keys())) > 0:
-            raise ValueError(
-                f"Cannot use {set(positional_keywords).intersection(kwargs.keys())} "
-                f"as both positional _and_ keyword arguments; args {args}, kwargs "
-                f"{kwargs}, reverse_keys {reverse_keys}, positional_keyworkds "
-                f"{positional_keywords}"
-            )
-
-        for arg in args:
-            key = positional_keywords.pop()
-            kwargs[key] = arg
-
-        return kwargs
-
-    def set_input_values(self, *args, **kwargs) -> None:
-        """
-        Match positional and keyword arguments to input channels and update input
-        values.
-
-        Args:
-            *args: Interpreted in the same order as node function arguments.
-            **kwargs: input label - input value (including channels for connection)
-             pairs.
-        """
-        kwargs = self._convert_input_args_and_kwargs_to_input_kwargs(*args, **kwargs)
-        return super().set_input_values(**kwargs)
-
-    def execute(self, *args, **kwargs):
-        kwargs = self._convert_input_args_and_kwargs_to_input_kwargs(*args, **kwargs)
-        return super().execute(**kwargs)
-
-    def pull(self, *args, run_parent_trees_too=False, **kwargs):
-        kwargs = self._convert_input_args_and_kwargs_to_input_kwargs(*args, **kwargs)
-        return super().pull(run_parent_trees_too=run_parent_trees_too, **kwargs)
-
-    def __call__(self, *args, **kwargs) -> None:
-        kwargs = self._convert_input_args_and_kwargs_to_input_kwargs(*args, **kwargs)
-        return super().__call__(**kwargs)
-
     def to_dict(self):
         return {
             "label": self.label,
             "ready": self.ready,
             "connected": self.connected,
             "fully_connected": self.fully_connected,
             "inputs": self.inputs.to_dict(),
@@ -592,50 +343,68 @@
 
     @property
     def color(self) -> str:
         """For drawing the graph"""
         return SeabornColors.green
 
 
-def function_node(*output_labels: str):
+as_function_node = decorated_node_decorator_factory(Function, Function.node_function)
+
+
+def function_node(
+    node_function: callable,
+    *args,
+    label: Optional[str] = None,
+    parent: Optional[Composite] = None,
+    overwrite_save: bool = False,
+    run_after_init: bool = False,
+    storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
+    save_after_run: bool = False,
+    output_labels: Optional[str | tuple[str]] = None,
+    validate_output_labels: bool = True,
+    **kwargs,
+):
     """
-    A decorator for dynamically creating node classes from functions.
+    Dynamically creates a new child of :class:`Function` using the
+    provided :func:`node_function` and returns an instance of that.
+
+    Beyond the standard :class:`Function`, initialization allows the args...
 
-    Decorates a function.
-    Returns a `Function` subclass whose name is the camel-case version of the function
-    node, and whose signature is modified to exclude the node function and output labels
-    (which are explicitly defined in the process of using the decorator).
+    Args:
+        node_function (callable): The function determining the behaviour of the node.
+        output_labels (Optional[str | list[str] | tuple[str]]): A name for each return
+            value of the node function OR a single label. (Default is None, which
+            scrapes output labels automatically from the source code of the wrapped
+            function.) This can be useful when returned values are not well named, e.g.
+            to make the output channel dot-accessible if it would otherwise have a label
+            that requires item-string-based access. Additionally, specifying a _single_
+            label for a wrapped function that returns a tuple of values ensures that a
+            _single_ output channel (holding the tuple) is created, instead of one
+            channel for each return value. The default approach of extracting labels
+            from the function source code also requires that the function body contain
+            _at most_ one `return` expression, so providing explicit labels can be used
+            to circumvent this (at your own risk), or to circumvent un-inspectable
+            source code (e.g. a function that exists only in memory).
     """
-    output_labels = None if len(output_labels) == 0 else output_labels
 
-    # One really subtle thing is that we manually parse the function type hints right
-    # here and include these as a class-level attribute.
-    # This is because on (de)(cloud)pickling a function node, somehow the node function
-    # method attached to it gets its `__globals__` attribute changed; it retains stuff
-    # _inside_ the function, but loses imports it used from the _outside_ -- i.e. type
-    # hints! I (@liamhuber) don't deeply understand _why_ (de)pickling is modifying the
-    # __globals__ in this way, but the result is that type hints cannot be parsed after
-    # the change.
-    # The final piece of the puzzle here is that because the node function is a _class_
-    # level attribute, if you (de)pickle a node, _new_ instances of that node wind up
-    # having their node function's `__globals__` trimmed down in this way!
-    # So to keep the type hint parsing working, we snag and interpret all the type hints
-    # at wrapping time, when we are guaranteed to have all the globals available, and
-    # also slap them on as a class-level attribute. These get safely packed and returned
-    # when (de)pickling so we can keep processing type hints without trouble.
-    def as_node(node_function: callable):
-        return type(
-            node_function.__name__,
-            (Function,),  # Define parentage
-            {
-                "__init__": partialmethod(
-                    Function.__init__,
-                    None,
-                    output_labels=output_labels,
-                ),
-                "node_function": staticmethod(node_function),
-                "_type_hints": get_type_hints(node_function),
-                "__module__": node_function.__module__,
-            },
+    if not callable(node_function):
+        raise AttributeError(
+            f"Expected `node_function` to be callable but got {node_function}"
         )
 
-    return as_node
+    if output_labels is None:
+        output_labels = ()
+    elif isinstance(output_labels, str):
+        output_labels = (output_labels,)
+
+    return as_function_node(
+        *output_labels, validate_output_labels=validate_output_labels
+    )(node_function)(
+        *args,
+        label=label,
+        parent=parent,
+        overwrite_save=overwrite_save,
+        run_after_init=run_after_init,
+        storage_backend=storage_backend,
+        save_after_run=save_after_run,
+        **kwargs,
+    )
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/has_interface_mixins.py` & `pyiron_workflow-0.6.0/pyiron_workflow/has_interface_mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,13 @@
     @abstractmethod
     def channel(self) -> Channel:
         pass
 
 
 class HasRun(ABC):
     """
-    A mixin to guarantee that the :meth:`run` method exists, and can be called without
-    arguments.
+    A mixin to guarantee that the :meth:`run` method exists.
     """
 
     @abstractmethod
-    def run(self, **kwargs):
+    def run(self, *args, **kwargs):
         pass
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/injection.py` & `pyiron_workflow-0.6.0/pyiron_workflow/injection.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, Optional, TYPE_CHECKING
 
-from pyiron_workflow.channels import OutputData, NOT_DATA, InputData
+from pyiron_workflow.channels import OutputData, NOT_DATA
 from pyiron_workflow.has_interface_mixins import HasChannel
 from pyiron_workflow.io import Outputs, HasIO
 
 if TYPE_CHECKING:
     from pyiron_workflow.node import Node
 
 
@@ -40,15 +40,15 @@
     def __init__(
         self,
         label: str,
         owner: Node,
         default: Optional[Any] = NOT_DATA,
         type_hint: Optional[Any] = None,
         strict_hints: bool = True,
-        value_receiver: Optional[InputData] = None,
+        value_receiver: Optional[OutputData] = None,
     ):
         # Override parent method to give the new owner type hint
         super().__init__(
             label=label,
             owner=owner,
             default=default,
             type_hint=type_hint,
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/io.py` & `pyiron_workflow-0.6.0/pyiron_workflow/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 These also support the syntactic sugar of treating value assignments and new
 connections on the same footing.
 """
 
 from __future__ import annotations
 
-import warnings
 from abc import ABC, abstractmethod
 from typing import Any
+import warnings
 
 from pyiron_workflow.channels import (
     Channel,
     DataChannel,
     InputData,
     OutputData,
     SignalChannel,
@@ -383,33 +383,57 @@
     def __lshift__(self, others):
         """
         Connect one or more `ran` signals to `accumulate_and_run` signals like:
         `this << some_object, another_object, or_by_channel.signals.output.ran`
         """
         self.signals.input.accumulate_and_run << others
 
-    def set_input_values(self, **kwargs) -> None:
+    def set_input_values(self, *args, **kwargs) -> None:
         """
         Match keywords to input channels and update their values.
 
         Throws a warning if a keyword is provided that cannot be found among the input
         keys.
 
         Args:
+            *args: values assigned to inputs in order of appearance.
             **kwargs: input key - input value (including channels for connection) pairs.
-        """
+
+        Raises:
+            (ValueError): If more args are received than there are inputs available.
+            (ValueError): If there is any overlap between channels receiving values
+                from `args` and those from `kwargs`.
+            (ValueError): If any of the `kwargs` keys do not match available input
+                labels.
+        """
+        if len(args) > len(self.inputs.labels):
+            raise ValueError(
+                f"Received {len(args)} args, but only have {len(self.inputs.labels)} "
+                f"input channels available"
+            )
+        keyed_args = {label: value for label, value in zip(self.inputs.labels, args)}
+
+        if len(set(keyed_args.keys()).intersection(kwargs.keys())) > 0:
+            raise ValueError(
+                f"n args are interpreted using the first n input channels "
+                f"({self.inputs.labels}), but this conflicted with received kwargs "
+                f"({list(kwargs.keys())}) -- perhaps the input was ordered differently "
+                f"than expected?"
+            )
+
+        kwargs.update(keyed_args)
+
+        if len(set(kwargs.keys()).difference(self.inputs.labels)) > 0:
+            raise ValueError(
+                f"Tried to set input {list(kwargs.keys())}, but one or more label was "
+                f"not found among available inputs: {self.inputs.labels}"
+            )
+
         for k, v in kwargs.items():
-            if k in self.inputs.labels:
-                self.inputs[k] = v
-            else:
-                warnings.warn(
-                    f"The keyword '{k}' was not found among input labels. If you are "
-                    f"trying to update a class instance keyword, please use attribute "
-                    f"assignment directly instead of calling this method"
-                )
+            self.inputs[k] = v
 
     def copy_io(
         self,
         other: HasIO,
         connections_fail_hard: bool = True,
         values_fail_hard: bool = False,
     ) -> None:
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/job.py` & `pyiron_workflow-0.6.0/pyiron_workflow/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/macro.py` & `pyiron_workflow-0.6.0/pyiron_workflow/macro.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 """
 A base class for macro nodes, which are composite like workflows but have a static
 interface and are not intended to be internally modified after instantiation.
 """
 
 from __future__ import annotations
 
-from functools import partialmethod
-import inspect
-from typing import get_type_hints, Literal, Optional, TYPE_CHECKING
+from abc import ABC, abstractmethod
+import re
+from typing import Literal, Optional, TYPE_CHECKING
 
-from bidict import bidict
-
-from pyiron_workflow.channels import InputData, OutputData, NOT_DATA
 from pyiron_workflow.composite import Composite
 from pyiron_workflow.has_interface_mixins import HasChannel
 from pyiron_workflow.io import Outputs, Inputs
-from pyiron_workflow.output_parser import ParseOutput
+from pyiron_workflow.io_preview import DecoratedNode, decorated_node_decorator_factory
 
 if TYPE_CHECKING:
     from pyiron_workflow.channels import Channel
 
 
-class Macro(Composite):
+class Macro(Composite, DecoratedNode, ABC):
     """
     A macro is a composite node that holds a graph with a fixed interface, like a
     pre-populated workflow that is the same every time you instantiate it.
 
     At instantiation, the macro uses a provided callable to build and wire the graph,
     then builds a static IO interface for this graph.
     This callable must use the macro object itself as the first argument (e.g. adding
     nodes to it).
-    As with :class:`Workflow` objects, macros leverage `inputs_map` and `outputs_map` to
-    control macro-level IO access to child IO.
-    As with :class:`Workflow`, default behaviour is to expose all unconnected child IO.
-    The provided callable may optionally specify further args and kwargs, which are used
-    to pre-populate the macro with :class:`UserInput` nodes;
+    The provided callable may optionally specify further args and kwargs; these are
+    used to pre-populate the macro with :class:`UserInput` nodes, although they may
+    later be trimmed if the IO can be connected directly to child node IO without any
+    loss of functionality.
     This can be especially helpful when more than one child node needs access to the
     same input value.
     Similarly, the callable may return any number of child nodes' output channels (or
-    the node itself in the case of single-output nodes) and commensurate
-    :attr:`output_labels` to define macro-level output.
+    the node itself in the case of single-output nodes) as long as a commensurate
+    number of labels for these outputs were provided to the class constructor.
     These function-like definitions of the graph creator callable can be used
-    independently or together.
-    Each that is used switches its IO map to a "whitelist" paradigm, so any I/O _not_
-    provided in the callable signature/return values and output labels will be disabled.
-    Manual modifications of the IO maps inside the callable always take priority over
-    this whitelisting behaviour, so you always retain full control over what IO is
-    exposed, and the whitelisting is only for your convenience.
+    to build only input xor output, or both together.
+    Macro input channel labels are scraped from the signature of the graph creator;
+    for output, output labels can be provided explicitly as a class attribute or, as a
+    fallback, they are scraped from the graph creator code return statement (stripping
+    off the "{first argument}.", where {first argument} is whatever the name of the
+    first argument is.
 
     Macro IO is _value linked_ to the child IO, so that their values stay synchronized,
     but the child nodes of a macro form an isolated sub-graph.
 
     As with function nodes, subclasses of :class:`Macro` may define a method for creating the
     graph.
 
     As with :class:`Workflow``, all DAG macros can determine their execution flow
     automatically, if you have cycles in your data flow, or otherwise want more control
     over the execution, all you need to do is specify the `node.signals.input.run`
     connections and :attr:`starting_nodes` list yourself.
     If only _one_ of these is specified, you'll get an error, but if you've provided
     both then no further checks of their validity/reasonableness are performed, so be
     careful.
-    Unlike :class:`Workflow`, this execution flow automation is set up once at instantiation;
+    Unlike :class:`Workflow`, this execution flow automation is set up once at
+    instantiation;
     If the macro is modified post-facto, you may need to manually re-invoke
     :meth:`configure_graph_execution`.
 
     Promises (in addition parent class promises):
 
     - IO is...
-        - Only built at instantiation, after child node replacement, or at request, so
-            it is "static" for improved efficiency
+        - Statically defined at the class level
         - By value, i.e. the macro has its own IO channel instances and children are
             duly encapsulated inside their own sub-graph
         - Value-linked to the values of their corresponding child nodes' IO -- i.e.
             updating a macro input value changes a child node's input value, and a
             child node updating its output value changes a macro output value (if that
             child's output is regularly included in the macro's output, e.g. because it
             is disconnected or otherwise included in the outputs map)
@@ -82,403 +78,267 @@
     - A default node label can be generated using the name of the callable that builds
         the graph.
 
     Examples:
         Let's consider the simplest case of macros that just consecutively add 1 to
         their input:
 
-        >>> from pyiron_workflow.macro import Macro
+        >>> from pyiron_workflow.macro import macro_node, Macro
         >>>
         >>> def add_one(x):
         ...     result = x + 1
         ...     return result
         >>>
-        >>> def add_three_macro(macro):
-        ...     macro.one = macro.create.Function(add_one)
-        ...     macro.two = macro.create.Function(add_one, macro.one)
-        ...     macro.three = macro.create.Function(add_one, macro.two)
-        ...     macro.one >> macro.two >> macro.three
-        ...     macro.starting_nodes = [macro.one]
+        >>> def add_three_macro(self, one__x):
+        ...     self.one = self.create.function_node(add_one, x=one__x)
+        ...     self.two = self.create.function_node(add_one, self.one)
+        ...     self.three = self.create.function_node(add_one, self.two)
+        ...     self.one >> self.two >> self.three
+        ...     self.starting_nodes = [self.one]
+        ...     return self.three
 
         In this case we had _no need_ to specify the execution order and starting nodes
         --it's just an extremely simple DAG after all! -- but it's done here to
         demonstrate the syntax.
 
         We can make a macro by passing this graph-building function (that takes a macro
         as its first argument, i.e. `self` from the macro's perspective) to the :class:`Macro`
         class. Then, we can use it like a regular node! Just like a workflow, the
         io is constructed from unconnected owned-node IO by combining node and channel
         labels.
 
-        >>> macro = Macro(add_three_macro)
+        >>> macro = macro_node(add_three_macro, output_labels="three__result")
         >>> out = macro(one__x=3)
         >>> out.three__result
         6
 
-        If there's a particular macro we're going to use again and again, we might want
-        to consider making a new child class of :class:`Macro` that overrides the
-        :meth:`graph_creator` arg such that the same graph is always created. We could
-        override `__init__` the normal way, but it's even faster to just use
-        `partialmethod`:
-
-        >>> from functools import partialmethod
-        >>> class AddThreeMacro(Macro):
-        ...     @staticmethod
-        ...     def graph_creator(self):
-        ...         add_three_macro(self)
-        ...
-        ...     __init__ = partialmethod(
-        ...         Macro.__init__,
-        ...         None,  # We directly define the graph creator method on the class
-        ...     )
-        >>>
-        >>> macro = AddThreeMacro()
-        >>> macro(one__x=0).three__result
-        3
-
         We can also nest macros, rename their IO, and provide access to
         internally-connected IO by inputs and outputs maps:
 
-        >>> def nested_macro(macro):
-        ...     macro.a = macro.create.Function(add_one)
-        ...     macro.b = macro.create.Macro(add_three_macro, one__x=macro.a)
-        ...     macro.c = macro.create.Function(
-        ...         add_one, x=macro.b.outputs.three__result
+        >>> def nested_macro(self, inp):
+        ...     self.a = self.create.function_node(add_one, x=inp)
+        ...     self.b = self.create.macro_node(
+        ...         add_three_macro, one__x=self.a, output_labels="three__result"
         ...     )
+        ...     self.c = self.create.function_node(add_one, x=self.b)
+        ...     return self.c, self.b
         >>>
-        >>> macro = Macro(
-        ...     nested_macro,
-        ...     inputs_map={"a__x": "inp"},
-        ...     outputs_map={"c__result": "out", "b__three__result": "intermediate"},
+        >>> macro = macro_node(
+        ...     nested_macro, output_labels=("out", "intermediate")
         ... )
         >>> macro(inp=1)
-        {'intermediate': 5, 'out': 6}
+        {'out': 6, 'intermediate': 5}
 
         Macros and workflows automatically generate execution flows when their data
         is acyclic.
         Let's build a simple macro with two independent tracks:
 
-        >>> def modified_flow_macro(macro):
-        ...     macro.a = macro.create.Function(add_one, x=0)
-        ...     macro.b = macro.create.Function(add_one, x=0)
-        ...     macro.c = macro.create.Function(add_one, x=0)
+        >>> def modified_flow_macro(self, a__x=0, b__x=0):
+        ...     self.a = self.create.function_node(add_one, x=a__x)
+        ...     self.b = self.create.function_node(add_one, x=b__x)
+        ...     self.c = self.create.function_node(add_one, x=self.b)
+        ...     return self.a, self.c
         >>>
-        >>> m = Macro(modified_flow_macro)
-        >>> m(a__x=1, b__x=2, c__x=3)
-        {'a__result': 2, 'b__result': 3, 'c__result': 4}
-
-        We can override which nodes get used to start by specifying the :attr:`starting_nodes`
-        property.
-        If we do this we also need to provide at least one connection among the run
-        signals, but beyond that the code doesn't hold our hands.
+        >>> m = macro_node(modified_flow_macro, output_labels=("a", "c"))
+        >>> m(a__x=1, b__x=2)
+        {'a': 2, 'c': 4}
+
+        We can override which nodes get used to start by specifying the
+        :attr:`starting_nodes` property and (if necessary) reconfiguring the execution
+        signals.
+        Care should be taken here, as macro nodes may be creating extra input
+        nodes that need to be considered.
+        It's advisable to use :meth:`draw()` or to otherwise inspect the macro's
+        children and their connections before manually updating execution flows.
+
         Let's use this and then observe how the `a` sub-node no longer gets run:
 
-        >>> m.starting_nodes = [m.b]  # At least one starting node
-        >>> _ = m.b >> m.c  # At least one run signal
-        >>> # We catch and ignore output -- it's needed for chaining, but screws up
-        >>> # doctests -- you don't normally need to catch it like this!
-        >>> m(a__x=1000, b__x=2000, c__x=3000)
-        {'a__result': 2, 'b__result': 2001, 'c__result': 3001}
+        >>> _ = m.disconnect_run()
+        >>> m.starting_nodes = [m.b]
+        >>> _ = m.b >> m.c
+        >>> m(a__x=1000, b__x=2000)
+        {'a': 2, 'c': 2002}
+
+        (The `_` is just to catch and ignore output for the doctest, you don't
+        typically need this.)
 
         Note how the `a` node is no longer getting run, so the output is not updated!
         Manually controlling execution flow is necessary for cyclic graphs (cf. the
         while loop meta-node), but best to avoid when possible as it's easy to miss
         intended connections in complex graphs.
 
+        If there's a particular macro we're going to use again and again, we might want
+        to consider making a new class for it using the decorator, just like we do for
+        function nodes. If no output labels are explicitly provided, these are scraped
+        from the function return value, just like for function nodes (except the
+        initial `macro.` (or whatever the first argument is named) on any return values
+        is ignored):
+
+        >>> @Macro.wrap.as_macro_node()
+        ... def AddThreeMacro(self, x):
+        ...     add_three_macro(self, one__x=x)
+        ...     # We could also simply have decorated that function to begin with
+        ...     return self.three
+        >>>
+        >>> macro = AddThreeMacro()
+        >>> macro(x=0).three
+        3
+
+        Alternatively (and not recommended) is to make a new child class of
+        :class:`Macro` that overrides the :meth:`graph_creator` arg such that
+        the same graph is always created.
+
+        >>> class AddThreeMacro(Macro):
+        ...     _output_labels = ["three"]
+        ...
+        ...     @staticmethod
+        ...     def graph_creator(self, x):
+        ...         add_three_macro(self, one__x=x)
+        ...         return self.three
+        >>>
+        >>> macro = AddThreeMacro()
+        >>> macro(x=0).three
+        3
+
         We can also modify an existing macro at runtime by replacing nodes within it, as
         long as the replacement has fully compatible IO. There are three syntacic ways
         to do this. Let's explore these by going back to our `add_three_macro` and
         replacing each of its children with a node that adds 2 instead of 1.
 
-        >>> @Macro.wrap_as.function_node()
+        >>> @Macro.wrap.as_function_node()
         ... def add_two(x):
         ...     result = x + 2
         ...     return result
         >>>
-        >>> adds_six_macro = Macro(add_three_macro)
+        >>> adds_six_macro = macro_node(add_three_macro, output_labels="three__result")
         >>> # With the replace method
         >>> # (replacement target can be specified by label or instance,
         >>> # the replacing node can be specified by instance or class)
         >>> replaced = adds_six_macro.replace_child(adds_six_macro.one, add_two())
         >>> # With the replace_with method
         >>> adds_six_macro.two.replace_with(add_two())
         >>> # And by assignment of a compatible class to an occupied node label
         >>> adds_six_macro.three = add_two
         >>> adds_six_macro(one__x=1)
         {'three__result': 7}
 
-        Instead of controlling the IO interface with dictionary maps, we can instead
-        provide a more :class:`Function(Node)`-like definition of the :meth:`graph_creator` by
-        adding args and/or kwargs to the signature (under the hood, this dynamically
-        creates new :class:`UserInput` nodes before running the rest of the graph creation),
-        and/or returning child channels (or whole children in the case of single-output
-        nodes) and providing commensurate :attr:`output_labels`.
-        This process switches us from the :class:`Workflow` default of exposing all
-        unconnected child IO, to a "whitelist" paradigm of _only_ showing the IO that
-        we exposed by our function defintion.
-        (Note: any `.inputs_map` or `.outputs_map` explicitly defined in the
-        :meth:`graph_creator` still takes precedence over this whitelisting! So you always
-        retain full control over what IO gets exposed.)
-        E.g., these two definitions are perfectly equivalent:
-
-        >>> @Macro.wrap_as.macro_node("lout", "n_plus_2")
-        ... def LikeAFunction(macro, lin: list,  n: int = 1):
-        ...     macro.plus_two = n + 2
-        ...     macro.sliced_list = lin[n:macro.plus_two]
-        ...     macro.double_fork = 2 * n
-        ...     # ^ This is vestigial, just to show we don't need to blacklist it in a
-        ...     # whitelist-paradigm
-        ...     return macro.sliced_list, macro.plus_two.channel
-        >>>
-        >>> like_functions = LikeAFunction(lin=[1,2,3,4,5,6], n=2)
-        >>> like_functions()
-        {'n_plus_2': 4, 'lout': [3, 4]}
-
-        >>> @Macro.wrap_as.macro_node()
-        ... def WithIOMaps(macro):
-        ...     macro.list_in = macro.create.standard.UserInput()
-        ...     macro.list_in.inputs.user_input.type_hint = list
-        ...     macro.forked = macro.create.standard.UserInput(2)
-        ...     macro.forked.inputs.user_input.type_hint = int
-        ...     macro.n_plus_2 = macro.forked + 2
-        ...     macro.sliced_list = macro.list_in[macro.forked:macro.n_plus_2]
-        ...     macro.double_fork = 2 * macro.forked
-        ...     macro.inputs_map = {
-        ...         "list_in__user_input": "lin",
-        ...         macro.forked.inputs.user_input.scoped_label: "n",
-        ...         "n_plus_2__other": None,
-        ...         "list_in__user_input_Slice_forked__user_input_n_plus_2__add_None__step": None,
-        ...         macro.double_fork.inputs.other.scoped_label: None,
-        ...     }
-        ...     macro.outputs_map = {
-        ...         macro.sliced_list.outputs.getitem.scoped_label: "lout",
-        ...         macro.n_plus_2.outputs.add.scoped_label: "n_plus_2",
-        ...         "double_fork__rmul": None
-        ...     }
+        It's possible for the macro to hold nodes which are not publicly exposed for
+        data and signal connections, but which will still internally execute and store
+        data, e.g.:
+
+        >>> @Macro.wrap.as_macro_node("lout", "n_plus_2")
+        ... def LikeAFunction(self, lin: list,  n: int = 1):
+        ...     self.plus_two = n + 2
+        ...     self.sliced_list = lin[n:self.plus_two]
+        ...     self.double_fork = 2 * n
+        ...     return self.sliced_list, self.plus_two.channel
         >>>
-        >>> with_maps = WithIOMaps(lin=[1,2,3,4,5,6], n=2)
-        >>> with_maps()
-        {'n_plus_2': 4, 'lout': [3, 4]}
+        >>> like_functions = LikeAFunction(lin=[1,2,3,4,5,6], n=3)
+        >>> sorted(like_functions().items())
+        [('lout', [4, 5]), ('n_plus_2', 5)]
 
-        Here we've leveraged the macro-creating decorator, but this works the same way
-        using the :class:`Macro` class directly.
-    """
+        >>> like_functions.double_fork.value
+        6
 
-    def __init__(
-        self,
-        graph_creator: callable[[Macro], None],
-        label: Optional[str] = None,
-        parent: Optional[Composite] = None,
-        overwrite_save: bool = False,
-        run_after_init: bool = False,
-        storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
-        save_after_run: bool = False,
-        strict_naming: bool = True,
-        inputs_map: Optional[dict | bidict] = None,
-        outputs_map: Optional[dict | bidict] = None,
-        output_labels: Optional[str | list[str] | tuple[str]] = None,
-        **kwargs,
-    ):
-        if not callable(graph_creator):
-            # Children of `Function` may explicitly provide a `node_function` static
-            # method so the node has fixed behaviour.
-            # In this case, the `__init__` signature should be changed so that the
-            # `node_function` argument is just always `None` or some other non-callable.
-            # If a callable `node_function` is not received, you'd better have it as an
-            # attribute already!
-            if not hasattr(self, "graph_creator"):
-                raise AttributeError(
-                    f"If `None` is provided as a `graph_creator`, a `graph_creator` "
-                    f"property must be defined instead, e.g. when making child classes"
-                    f"of `Macro` with specific behaviour"
-                )
-        else:
-            # If a callable graph creator is received, use it
-            self.graph_creator = graph_creator
 
-        super().__init__(
-            label=label if label is not None else self.graph_creator.__name__,
-            parent=parent,
-            save_after_run=save_after_run,
-            storage_backend=storage_backend,
-            strict_naming=strict_naming,
-            inputs_map=inputs_map,
-            outputs_map=outputs_map,
-        )
-        output_labels = self._validate_output_labels(output_labels)
+    """
+
+    def _setup_node(self) -> None:
+        super()._setup_node()
 
         ui_nodes = self._prepopulate_ui_nodes_from_graph_creator_signature(
-            storage_backend=storage_backend
+            storage_backend=self.storage_backend
         )
         returned_has_channel_objects = self.graph_creator(self, *ui_nodes)
-        self._configure_graph_execution()
-
-        # Update IO map(s) if a function-like graph creator interface was used
-        if len(ui_nodes) > 0:
-            self._whitelist_inputs_map(*ui_nodes)
-        if returned_has_channel_objects is not None:
-            if not isinstance(returned_has_channel_objects, tuple):
-                returned_has_channel_objects = (returned_has_channel_objects,)
-            self._whitelist_outputs_map(output_labels, *returned_has_channel_objects)
-
-        self._inputs: Inputs = self._build_inputs()
-        self._outputs: Outputs = self._build_outputs()
+        if returned_has_channel_objects is None:
+            returned_has_channel_objects = ()
+        elif isinstance(returned_has_channel_objects, HasChannel):
+            returned_has_channel_objects = (returned_has_channel_objects,)
+
+        for node in ui_nodes:
+            self.inputs[node.label].value_receiver = node.inputs.user_input
+
+        for node, output_channel_label in zip(
+            returned_has_channel_objects,
+            () if self._output_labels is None else self._output_labels,
+        ):
+            node.channel.value_receiver = self.outputs[output_channel_label]
 
-        self.set_input_values(**kwargs)
+        remaining_ui_nodes = self._purge_single_use_ui_nodes(ui_nodes)
+        self._configure_graph_execution(remaining_ui_nodes)
 
-    def _validate_output_labels(self, output_labels) -> tuple[str]:
-        """
-        Ensure that output_labels, if provided, are commensurate with graph creator
-        return values, if provided, and return them as a tuple.
-        """
-        graph_creator_returns = ParseOutput(self.graph_creator).output
-        output_labels = (
-            (output_labels,) if isinstance(output_labels, str) else output_labels
-        )
-        if graph_creator_returns is not None or output_labels is not None:
-            error_suffix = (
-                f"but {self.label} macro got return values: "
-                f"{graph_creator_returns} and labels: {output_labels}."
-            )
-            try:
-                if len(output_labels) != len(graph_creator_returns):
-                    raise ValueError(
-                        "The number of return values in the graph creator must exactly "
-                        "match the number of output labels provided, " + error_suffix
-                    )
-            except TypeError:
-                raise TypeError(
-                    f"Output labels and graph creator return values must either both "
-                    f"or neither be present, " + error_suffix
+    @staticmethod
+    @abstractmethod
+    def graph_creator(self, *args, **kwargs) -> callable:
+        """Build the graph the node will run."""
+
+    @classmethod
+    def _io_defining_function(cls) -> callable:
+        return cls.graph_creator
+
+    _io_defining_function_uses_self = True
+
+    @classmethod
+    def _scrape_output_labels(cls):
+        scraped_labels = super(Macro, cls)._scrape_output_labels()
+
+        if scraped_labels is not None:
+            # Strip off the first argument, e.g. self.foo just becomes foo
+            self_argument = list(cls._get_input_args().keys())[0]
+            cleaned_labels = [
+                re.sub(r"^" + re.escape(f"{self_argument}."), "", label)
+                for label in scraped_labels
+            ]
+            if any("." in label for label in cleaned_labels):
+                raise ValueError(
+                    f"Tried to scrape cleaned labels for {cls.__name__}, but at least "
+                    f"one of {cleaned_labels} still contains a '.' -- please provide "
+                    f"explicit labels"
                 )
-        return () if output_labels is None else tuple(output_labels)
+            return cleaned_labels
+        else:
+            return scraped_labels
 
     def _prepopulate_ui_nodes_from_graph_creator_signature(
         self, storage_backend: Literal["h5io", "tinybase"]
     ):
-        hints_dict = get_type_hints(self.graph_creator)
-        interface_nodes = ()
-        for i, (arg_name, inspected_value) in enumerate(
-            inspect.signature(self.graph_creator).parameters.items()
-        ):
-            if i == 0:
-                continue  # Skip the macro argument itself, it's like `self` here
-
-            default = (
-                NOT_DATA
-                if inspected_value.default is inspect.Parameter.empty
-                else inspected_value.default
+        ui_nodes = []
+        for label, (type_hint, default) in self.preview_inputs().items():
+            n = self.create.standard.UserInput(
+                default,
+                label=label,
+                parent=self,
+                storage_backend=storage_backend,
             )
-            node = self.create.standard.UserInput(
-                default, label=arg_name, parent=self, storage_backend=storage_backend
-            )
-            node.inputs.user_input.default = default
-            try:
-                node.inputs.user_input.type_hint = hints_dict[arg_name]
-            except KeyError:
-                pass  # If there's no hint that's fine
-            interface_nodes += (node,)
-
-        return interface_nodes
-
-    def _whitelist_inputs_map(self, *ui_nodes) -> None:
-        """
-        Updates the inputs map so each UI node's output channel is available directly
-        under the node label, and updates the map to disable all other input that
-        wasn't explicitly mapped already.
-        """
-        self.inputs_map = self._hide_non_whitelisted_io(
-            self._whitelist_map(
-                self.inputs_map, tuple(n.label for n in ui_nodes), ui_nodes
-            ),
-            "inputs",
-        )
-
-    def _whitelist_outputs_map(
-        self, output_labels: tuple[str], *creator_returns: HasChannel
-    ):
-        """
-        Updates the outputs map so objects returned by the graph creator directly
-        leverage the supplied output labels, and updates the map to disable all other
-        output that wasn't explicitly mapped already.
-        """
-        for new_label, ui_node in zip(output_labels, creator_returns):
-            if not isinstance(ui_node, HasChannel):
-                raise TypeError(
-                    f"Your node `{new_label}` does not have `channel`. There"
-                    + " are following nodes that can be returned:"
-                    + f" {self.node_labels}. More can be found from this page:"
-                    + " https://github.com/pyiron/pyiron_workflow"
-                )
-        self.outputs_map = self._hide_non_whitelisted_io(
-            self._whitelist_map(self.outputs_map, output_labels, creator_returns),
-            "outputs",
-        )
-
-    @staticmethod
-    def _whitelist_map(
-        io_map: bidict, new_labels: tuple[str], has_channel_objects: tuple[HasChannel]
-    ) -> bidict:
-        """
-        Update an IO map to give new labels to the channels of a bunch of :class:`HasChannel`
-        objects.
-        """
-        io_map = bidict({}) if io_map is None else io_map
-        for new_label, ui_node in zip(new_labels, has_channel_objects):
-            # White-list everything not already in the map
-            if ui_node.channel.scoped_label not in io_map.keys():
-                io_map[ui_node.channel.scoped_label] = new_label
-        return io_map
-
-    def _hide_non_whitelisted_io(
-        self, io_map: bidict, i_or_o: Literal["inputs", "outputs"]
-    ) -> dict:
-        """
-        Make a new map dictionary with `None` entries for each channel that isn't
-        already in the provided map bidict. I.e. blacklist things we didn't whitelist.
-        """
-        io_map = dict(io_map)
-        # We do it in two steps like this to leverage the bidict security on the setter
-        # Since bidict can't handle getting `None` (i.e. disable) for multiple keys
-        for node in self.children.values():
-            for channel in getattr(node, i_or_o):
-                if channel.scoped_label not in io_map.keys():
-                    io_map[channel.scoped_label] = None
-        return io_map
-
-    def _get_linking_channel(
-        self,
-        child_reference_channel: InputData | OutputData,
-        composite_io_key: str,
-    ) -> InputData | OutputData:
-        """
-        Build IO by value: create a new channel just like the child's channel.
-
-        In the case of input data, we also form a value link from the composite channel
-        down to the child channel, so that the child will stay up-to-date.
-        """
-        composite_channel = child_reference_channel.__class__(
-            label=composite_io_key,
-            owner=self,
-            default=child_reference_channel.default,
-            type_hint=child_reference_channel.type_hint,
-        )
-        composite_channel.value = child_reference_channel.value
-
-        if isinstance(composite_channel, InputData):
-            composite_channel.strict_hints = child_reference_channel.strict_hints
-            composite_channel.value_receiver = child_reference_channel
-        elif isinstance(composite_channel, OutputData):
-            child_reference_channel.value_receiver = composite_channel
-        else:
-            raise TypeError(
-                "This should not be an accessible state, please contact the developers"
-            )
-
-        return composite_channel
+            n.inputs.user_input.type_hint = type_hint
+            ui_nodes.append(n)
+        return tuple(ui_nodes)
+
+    def _purge_single_use_ui_nodes(self, ui_nodes):
+        """
+        We (may) create UI nodes based on the :meth:`graph_creator` signature;
+        If these are connected to only a single node actually defined in the creator,
+        they are superfluous, and we can remove them -- linking the macro input
+        directly to the child node input.
+        """
+        remaining_ui_nodes = list(ui_nodes)
+        for macro_input in self.inputs:
+            target_node = macro_input.value_receiver.owner
+            if (
+                target_node in ui_nodes  # Value link is a UI node
+                and target_node.channel.value_receiver is None  # That doesn't forward
+                # its value directly to the output
+                and len(target_node.channel.connections) <= 1  # And isn't forked to
+                # multiple children
+            ):
+                if len(target_node.channel.connections) == 1:
+                    macro_input.value_receiver = target_node.channel.connections[0]
+                self.remove_child(target_node)
+                remaining_ui_nodes.remove(target_node)
+        return tuple(remaining_ui_nodes)
 
     @property
     def inputs(self) -> Inputs:
         return self._inputs
 
     @property
     def outputs(self) -> Outputs:
@@ -514,23 +374,27 @@
         channel: Channel, old_connection: Channel, new_connection: Channel
     ):
         """Brute-force replace an old connection in a channel with a new one"""
         channel.connections = [
             c if c is not old_connection else new_connection for c in channel
         ]
 
-    def _configure_graph_execution(self):
+    def _configure_graph_execution(self, ui_nodes):
         run_signals = self.disconnect_run()
 
         has_signals = len(run_signals) > 0
         has_starters = len(self.starting_nodes) > 0
 
         if has_signals and has_starters:
             # Assume the user knows what they're doing
             self._reconnect_run(run_signals)
+            # Then put the UI upstream of the original starting nodes
+            for n in self.starting_nodes:
+                n << ui_nodes
+            self.starting_nodes = ui_nodes if len(ui_nodes) > 0 else self.starting_nodes
         elif not has_signals and not has_starters:
             # Automate construction of the execution graph
             self.set_run_signals_to_dag_execution()
         else:
             raise ValueError(
                 f"The macro '{self.label}' has {len(run_signals)} run signals "
                 f"internally and {len(self.starting_nodes)} starting nodes. Either "
@@ -602,41 +466,78 @@
         for inp, (child, child_inp) in input_links:
             self.inputs[inp].value_receiver = self.children[child].inputs[child_inp]
 
         for (child, child_out), out in output_links:
             self.children[child].outputs[child_out].value_receiver = self.outputs[out]
 
 
-def macro_node(*output_labels, **node_class_kwargs):
+as_macro_node = decorated_node_decorator_factory(
+    Macro,
+    Macro.graph_creator,
+    decorator_docstring_additions="The first argument in the wrapped function is "
+    "`self`-like and will receive the macro instance "
+    "itself, and thus is ignored in the IO.",
+)
+
+
+def macro_node(
+    graph_creator,
+    label: Optional[str] = None,
+    parent: Optional[Composite] = None,
+    overwrite_save: bool = False,
+    run_after_init: bool = False,
+    storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
+    save_after_run: bool = False,
+    strict_naming: bool = True,
+    output_labels: Optional[str | list[str] | tuple[str]] = None,
+    validate_output_labels: bool = True,
+    **kwargs,
+):
     """
-    A decorator for dynamically creating macro classes from graph-creating functions.
+    Creates a new child of :class:`Macro` using the provided
+    :func:`graph_creator` and returns an instance of that.
 
-    Decorates a function.
-    Returns a :class:`Macro` subclass whose name is the camel-case version of the
-    graph-creating function, and whose signature is modified to exclude this function
-    and provided kwargs.
-
-    Optionally takes output labels as args in case the node function uses the
-    like-a-function interface to define its IO. (The number of output labels must match
-    number of channel-like objects returned by the graph creating function _exactly_.)
+    Quacks like a :class:`Composite` for the sake of creating and registering nodes.
 
-    Optionally takes any keyword arguments of :class:`Macro`.
-    """
-    output_labels = None if len(output_labels) == 0 else output_labels
+    Beyond the standard :class:`Macro`, initialization allows the args...
 
-    def as_node(graph_creator: callable[[Macro, ...], Optional[tuple[HasChannel]]]):
-        return type(
-            graph_creator.__name__,
-            (Macro,),  # Define parentage
-            {
-                "__init__": partialmethod(
-                    Macro.__init__,
-                    None,
-                    output_labels=output_labels,
-                    **node_class_kwargs,
-                ),
-                "graph_creator": staticmethod(graph_creator),
-                "__module__": graph_creator.__module__,
-            },
+    Args:
+        graph_creator (callable): The function defining macro's graph.
+        output_labels (Optional[str | list[str] | tuple[str]]): A name for each return
+            value of the node function OR a single label. (Default is None, which
+            scrapes output labels automatically from the source code of the wrapped
+            function.) This can be useful when returned values are not well named, e.g.
+            to make the output channel dot-accessible if it would otherwise have a label
+            that requires item-string-based access. Additionally, specifying a _single_
+            label for a wrapped function that returns a tuple of values ensures that a
+            _single_ output channel (holding the tuple) is created, instead of one
+            channel for each return value. The default approach of extracting labels
+            from the function source code also requires that the function body contain
+            _at most_ one `return` expression, so providing explicit labels can be used
+            to circumvent this (at your own risk), or to circumvent un-inspectable
+            source code (e.g. a function that exists only in memory).
+    """
+    if not callable(graph_creator):
+        # `function_node` quacks like a class, even though it's a function and
+        # dynamically creates children of `Macro` by providing the necessary
+        # callable to the decorator
+        raise AttributeError(
+            f"Expected `graph_creator` to be callable but got {graph_creator}"
         )
 
-    return as_node
+    if output_labels is None:
+        output_labels = ()
+    elif isinstance(output_labels, str):
+        output_labels = (output_labels,)
+
+    return as_macro_node(*output_labels, validate_output_labels=validate_output_labels)(
+        graph_creator
+    )(
+        label=label,
+        parent=parent,
+        overwrite_save=overwrite_save,
+        run_after_init=run_after_init,
+        storage_backend=storage_backend,
+        save_after_run=save_after_run,
+        strict_naming=strict_naming,
+        **kwargs,
+    )
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/meta.py` & `pyiron_workflow-0.6.0/pyiron_workflow/loops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,312 +1,314 @@
-"""
-Meta nodes are callables that create a node class instead of a node instance.
-"""
-
 from __future__ import annotations
 
+import random
+from textwrap import dedent
 from typing import Optional
 
-from pyiron_workflow.function import (
-    Function,
-    function_node,
-)
-from pyiron_workflow.macro import Macro, macro_node
+import pyiron_workflow
+from pyiron_workflow import Workflow
+from pyiron_workflow.function import Function
+from pyiron_workflow.macro import Macro
+from pyiron_workflow.meta import input_to_list, list_to_output
 from pyiron_workflow.node import Node
 
 
-def list_to_output(length: int, **node_class_kwargs) -> type[Function]:
-    """
-    A meta-node that returns a node class with :param:`length` input channels and
-    maps these to a single output channel with type `list`.
-    """
-
-    def _list_to_many(length: int):
-        template = f"""
-def __list_to_many(l: list):
-    {"; ".join([f"out{i} = l[{i}]" for i in range(length)])}
-    return [{", ".join([f"out{i}" for i in range(length)])}]
-        """
-        exec(template)
-        return locals()["__list_to_many"]
-
-    return function_node(**node_class_kwargs)(_list_to_many(length=length))
-
-
-def input_to_list(length: int, **node_class_kwargs) -> type[Function]:
-    """
-    A meta-node that returns a node class with :param:`length` output channels and
-    maps an input list to these.
-    """
-
-    def _many_to_list(length: int):
-        template = f"""
-def __many_to_list({", ".join([f"inp{i}=None" for i in range(length)])}):
-    return [{", ".join([f"inp{i}" for i in range(length)])}]
-        """
-        exec(template)
-        return locals()["__many_to_list"]
-
-    return function_node(**node_class_kwargs)(_many_to_list(length=length))
-
-
 def for_loop(
     loop_body_class: type[Node],
     length: int,
     iterate_on: str | tuple[str] | list[str],
-    # TODO:
 ) -> type[Macro]:
     """
-    An _extremely rough_ first draft of a for-loop meta-node.
+    An _extremely rough_ second draft of a for-loop meta-node.
 
     Takes a node class, how long the loop should be, and which input(s) of the provided
     node class should be looped over (given as strings of the channel labels) and
-    builds a macro that
+    builds a macro that scatters some input and broadcasts the rest, then operates on
+    a zip of all the scattered input (so it had better be the same length).
 
     - Makes copies of the provided node class, i.e. the "body node"
-    - For each input channel specified to "loop over", creates a list-to-many node and
-      connects each of its outputs to their respective body node inputs
-    - For all other inputs, makes a 1:1 node and connects its output to _all_ of the
-      body nodes
-    - Relables the macro IO to match the passed node class IO so that list-ified IO
-      (i.e. the specified input and all output) is all caps
+    - Labels in :param:`iterate_on` must correspond to `loop_body_class` input channels,
+        and the for-loop node then expects list-like input for these with ALL CAPS
+        labeling, and this gets scattered to the children.
+    - All other input simply gets broadcast to each child.
+    - Output channels correspond to input channels, but are lists of the children and
+        labeled in ALL CAPS
+
+    Warnings:
+        The loop body class must be importable. E.g. it can come from a node package or
+        be defined in `__main__`, but not defined inside the scope of some other
+        function.
 
     Examples:
 
         >>> from pyiron_workflow import Workflow
-        >>> from pyiron_workflow.meta import for_loop
-        >>>
-        >>> @Workflow.wrap_as.function_node("div")
-        ... def Divide(numerator, denominator):
-        ...    return numerator / denominator
         >>>
         >>> denominators = list(range(1, 5))
         >>> bulk_loop = Workflow.create.meta.for_loop(
-        ...     Divide,
+        ...     Workflow.create.standard.Divide,
         ...     len(denominators),
-        ...     iterate_on = ("denominator",),
+        ...     iterate_on = ("other",),
         ... )()
-        >>> bulk_loop.inputs.numerator = 1
-        >>> bulk_loop.inputs.DENOMINATOR = denominators
-        >>> bulk_loop().DIV
+        >>> bulk_loop.inputs.obj = 1
+        >>> bulk_loop.inputs.OTHER = denominators
+        >>> bulk_loop().TRUEDIV
         [1.0, 0.5, 0.3333333333333333, 0.25]
 
     TODO:
 
         - Refactor like crazy, it's super hard to read and some stuff is too hard-coded
-        - Give some sort of access to flow control??
         - How to handle passing executors to the children? Maybe this is more
           generically a Macro question?
         - Is it possible to somehow dynamically adapt the held graph depending on the
-          length of the input values being iterated over? Tricky to keep IO well defined
+          length of the input values being iterated over? E.g. rebuilding the graph
+          every run call.
         - Allow a different mode, or make a different meta node, that makes all possible
-          pairs of body nodes given the input being looped over instead of just :param:`length`
+          pairs of body nodes given the input being looped over instead of just
+          :param:`length`
         - Provide enter and exit magic methods so we can `for` or `with` this fancy-like
     """
+    input_preview = loop_body_class.preview_inputs()
+    output_preview = loop_body_class.preview_outputs()
+
+    # Ensure `iterate_on` is in the input
     iterate_on = [iterate_on] if isinstance(iterate_on, str) else iterate_on
+    incommensurate_input = set(iterate_on).difference(input_preview.keys())
+    if len(incommensurate_input) > 0:
+        raise ValueError(
+            f"Cannot loop on {incommensurate_input}, as it is not an input channel "
+            f"of {loop_body_class.__name__}; please choose from among "
+            f"{list(input_preview)}"
+        )
 
-    def make_loop(macro):
-        macro.inputs_map = {}
-        macro.outputs_map = {}
-        body_nodes = []
-
-        # Parallelize over body nodes
-        for n in range(length):
-            body_nodes.append(
-                macro.add_child(
-                    loop_body_class(label=f"{loop_body_class.__name__}_{n}")
+    # Build code components that need an f-string, slash, etc.
+    output_labels = ", ".join(f'"{l.upper()}"' for l in output_preview.keys()).rstrip(
+        " "
+    )
+    macro_args = ", ".join(
+        l.upper() if l in iterate_on else l for l in input_preview.keys()
+    ).rstrip(" ")
+    body_label = 'f"body{n}"'
+    item_access = "[{n}]"
+    body_kwargs = ", ".join(
+        f"{l}={l.upper()}[n]" if l in iterate_on else f"{l}={l}"
+        for l in input_preview.keys()
+    ).rstrip(" ")
+    input_label = 'f"inp{n}"'
+    returns = ", ".join(
+        f'self.children["{label.upper()}"]' for label in output_preview.keys()
+    )
+    node_name = f'{loop_body_class.__name__}For{"".join([l.title() for l in sorted(iterate_on)])}{length}'
+
+    # Assemble components into a decorated for-loop macro
+    for_loop_code = dedent(
+        f"""
+        @Macro.wrap.as_macro_node({output_labels})
+        def {node_name}(self, {macro_args}):
+            from {loop_body_class.__module__} import {loop_body_class.__name__}
+
+            for label in [{output_labels}]:
+                input_to_list({length})(label=label, parent=self)
+
+            for n in range({length}):
+                body_node = {loop_body_class.__name__}(
+                    {body_kwargs},
+                    label={body_label},
+                    parent=self
                 )
-            )
+                for label in {list(output_preview.keys())}:
+                    self.children[label.upper()].inputs[{input_label}] = body_node.outputs[label]
 
-        # Make input interface
-        for label, inp in body_nodes[0].inputs.items():
-            # Don't rely on inp.label directly, since inputs may be a Composite IO
-            # panel that has a different key for this input channel than its label
-
-            # Scatter a list of inputs to each node separately
-            if label in iterate_on:
-                interface = list_to_output(length)(
-                    parent=macro,
-                    label=label.upper(),
-                    output_labels=[
-                        f"{loop_body_class.__name__}__{inp.label}_{i}"
-                        for i in range(length)
-                    ],
-                    l=[inp.default] * length,
-                )
-                # Connect each body node input to the input interface's respective output
-                for body_node, out in zip(body_nodes, interface.outputs):
-                    body_node.inputs[label] = out
-                macro.inputs_map[f"{interface.label}__l"] = interface.label
-                # TODO: Don't hardcode __l
-            # Or distribute the same input to each node equally
-            else:
-                interface = macro.create.standard.UserInput(
-                    label=label,
-                    output_labels=label,
-                    user_input=inp.default,
-                    parent=macro,
-                )
-                for body_node in body_nodes:
-                    body_node.inputs[label] = interface
-                macro.inputs_map[f"{interface.label}__user_input"] = interface.label
-                # TODO: Don't hardcode __user_input
-
-        # Make output interface: outputs to lists
-        for label, out in body_nodes[0].outputs.items():
-            interface = input_to_list(length)(
-                parent=macro,
-                label=label.upper(),
-                output_labels=f"{loop_body_class.__name__}__{label}",
-            )
-            # Connect each body node output to the output interface's respective input
-            for body_node, inp in zip(body_nodes, interface.inputs):
-                inp.connect(body_node.outputs[label])
-                if body_node.executor:
-                    raise NotImplementedError(
-                        "Right now the output interface gets run after each body node,"
-                        "if the body nodes can run asynchronously we need something "
-                        "more clever than that!"
-                    )
-            macro.outputs_map[
-                f"{interface.label}__{loop_body_class.__name__}__{label}"
-            ] = interface.label
-            # TODO: Don't manually copy the output label construction
+            return {returns}
+        """
+    )
 
-    return macro_node()(make_loop)
+    exec(for_loop_code)
+    return locals()[node_name]
 
 
 def while_loop(
     loop_body_class: type[Node],
     condition_class: type[Function],
     internal_connection_map: dict[str, str],
-    inputs_map: Optional[dict[str, str]] = None,
-    outputs_map: Optional[dict[str, str]] = None,
+    inputs_map: Optional[dict[str, str]],
+    outputs_map: Optional[dict[str, str]],
 ) -> type[Macro]:
     """
-    An _extremely rough_ first draft of a for-loop meta-node.
+    An _extremely rough_ second draft of a for-loop meta-node.
 
     Takes body and condition node classes and builds a macro that makes a cyclic signal
     connection between them and an "if" switch, i.e. when the body node finishes it
     runs the condtion, which runs the switch, and as long as the condition result was
     `True`, the switch loops back to run the body again.
     We additionally allow four-tuples of (input node, input channel, output node,
     output channel) labels to wire data connections inside the macro, e.g. to pass data
     from the body to the condition. This is beastly syntax, but it will suffice for now.
     Finally, you can set input and output maps as normal.
 
     Args:
         loop_body_class (type[pyiron_workflow.node.Node]): The class for the
             body of the while-loop.
-        condition_class (type[pyiron_workflow.function.Function]): A single-output
-            function node returning a `bool` controlling the while loop exit condition
-            (exits on False)
+        condition_class (type[pyiron_workflow.function.Function]): A
+            single-output function node returning a `bool` controlling the while loop
+            exit condition (exits on False)
         internal_connection_map (list[tuple[str, str, str, str]]): String tuples
             giving (input node, input channel, output node, output channel) labels
             connecting channel pairs inside the macro.
-        inputs_map Optional[dict[str, str]]: The inputs map as usual for a macro.
-        outputs_map Optional[dict[str, str]]: The outputs map as usual for a macro.
+        inputs_map (dict[str, str]): Define the inputs for the new macro like
+            `{body/condition class name}__{input channel}: {macro input channel name}`
+        outputs_map (dict[str, str]): Define the outputs for the new macro like
+            `{body/condition class name}__{output channel}: {macro output channel name}`
+
+    Warnings:
+        The loop body and condition classes must be importable. E.g. they can come from
+        a node package or be defined in `__main__`, but not defined inside the scope of
+        some other function.
 
     Examples:
 
         >>> from pyiron_workflow import Workflow
         >>>
-        >>> @Workflow.wrap_as.function_node()
-        ... def Add(a, b):
-        ...     print(f"{a} + {b} = {a + b}")
-        ...     return a + b
-        >>>
-        >>> @Workflow.wrap_as.function_node()
-        ... def LessThanTen(value):
-        ...     return value < 10
-        >>>
         >>> AddWhile = Workflow.create.meta.while_loop(
-        ...     loop_body_class=Add,
+        ...     loop_body_class=Workflow.create.standard.Add,
         ...     condition_class=Workflow.create.standard.LessThan,
         ...     internal_connection_map=[
-        ...         ("Add", "a + b", "LessThan", "obj"),
-        ...         ("Add", "a + b", "Add", "a")
+        ...         ("Add", "add", "LessThan", "obj"),
+        ...         ("Add", "add", "Add", "obj")
         ...     ],
-        ...     inputs_map={"Add__a": "a", "Add__b": "b", "LessThan__other": "cap"},
-        ...     outputs_map={"Add__a + b": "total"}
+        ...     inputs_map={
+        ...         "Add__obj": "a",
+        ...         "Add__other": "b",
+        ...         "LessThan__other": "cap"
+        ...     },
+        ...     outputs_map={"Add__add": "total"}
         ... )
         >>>
         >>> wf = Workflow("do_while")
         >>> wf.add_while = AddWhile(cap=10)
         >>>
         >>> wf.inputs_map = {
         ...     "add_while__a": "a",
         ...     "add_while__b": "b"
         ... }
         >>> wf.outputs_map = {"add_while__total": "total"}
         >>>
         >>> print(f"Finally, {wf(a=1, b=2).total}")
-        1 + 2 = 3
-        3 + 2 = 5
-        5 + 2 = 7
-        7 + 2 = 9
-        9 + 2 = 11
         Finally, 11
 
         >>> import random
         >>>
         >>> from pyiron_workflow import Workflow
         >>>
-        >>> random.seed(0)
-        >>>
-        >>> @Workflow.wrap_as.function_node("random")
-        ... def RandomFloat():
-        ...     return random.random()
-        >>>
-        >>> @Workflow.wrap_as.function_node()
-        ... def GreaterThan(x: float, threshold: float):
-        ...     gt = x > threshold
-        ...     symbol = ">" if gt else "<="
-        ...     print(f"{x:.3f} {symbol} {threshold}")
-        ...     return gt
+        >>> random.seed(0)  # Set the seed so the output is consistent and doctest runs
         >>>
         >>> RandomWhile = Workflow.create.meta.while_loop(
-        ...     loop_body_class=RandomFloat,
-        ...     condition_class=GreaterThan,
-        ...     internal_connection_map=[("RandomFloat", "random", "GreaterThan", "x")],
+        ...     loop_body_class=Workflow.create.standard.RandomFloat,
+        ...     condition_class=Workflow.create.standard.GreaterThan,
+        ...     internal_connection_map=[
+        ...         ("RandomFloat", "random", "GreaterThan", "obj")
+        ...     ],
+        ...     inputs_map={"GreaterThan__other": "threshold"},
         ...     outputs_map={"RandomFloat__random": "capped_result"}
         ... )
         >>>
         >>> # Define workflow
         >>>
         >>> wf = Workflow("random_until_small_enough")
         >>>
         >>> ## Wire together the while loop and its condition
         >>>
         >>> wf.random_while = RandomWhile()
         >>>
         >>> ## Give convenient labels
-        >>> wf.inputs_map = {"random_while__GreaterThan__threshold": "threshold"}
+        >>> wf.inputs_map = {"random_while__threshold": "threshold"}
         >>> wf.outputs_map = {"random_while__capped_result": "capped_result"}
         >>>
         >>> # Set a threshold and run
         >>> print(f"Finally {wf(threshold=0.3).capped_result:.3f}")
-        0.844 > 0.3
-        0.758 > 0.3
-        0.421 > 0.3
-        0.259 <= 0.3
         Finally 0.259
     """
 
-    def make_loop(macro):
-        body_node = macro.add_child(loop_body_class(label=loop_body_class.__name__))
-        condition_node = macro.add_child(
-            condition_class(label=condition_class.__name__)
+    # Make sure each dynamic class is getting a unique name
+    io_hash = hash(
+        ",".join(
+            [
+                "_".join(s for conn in internal_connection_map for s in conn),
+                "".join(f"{k}:{v}" for k, v in sorted(inputs_map.items())),
+                "".join(f"{k}:{v}" for k, v in sorted(outputs_map.items())),
+            ]
         )
-        switch = macro.create.standard.If(label="switch", parent=macro)
+    )
+    io_hash = str(io_hash).replace("-", "m")
+    node_name = f"{loop_body_class.__name__}While{condition_class.__name__}_{io_hash}"
+
+    # Build code components that need an f-string, slash, etc.
+    output_labels = ", ".join(f'"{l}"' for l in outputs_map.values()).rstrip(" ")
+    input_args = ", ".join(l for l in inputs_map.values()).rstrip(" ")
+
+    def get_kwargs(io_map: dict[str, str], node_class: type[Node]):
+        return ", ".join(
+            f'{k.split("__")[1]}={v}'
+            for k, v in io_map.items()
+            if k.split("__")[0] == node_class.__name__
+        ).rstrip(" ")
+
+    returns = ", ".join(
+        f'self.{l.split("__")[0]}.outputs.{l.split("__")[1]}'
+        for l in outputs_map.keys()
+    ).rstrip(" ")
+
+    # Assemble components into a decorated while-loop macro
+    while_loop_code = dedent(
+        f"""
+        @Macro.wrap.as_macro_node({output_labels})
+        def {node_name}(self, {input_args}):
+            from {loop_body_class.__module__} import {loop_body_class.__name__}
+            from {condition_class.__module__} import {condition_class.__name__}
+
+            body = self.add_child(
+                {loop_body_class.__name__}(
+                    label="{loop_body_class.__name__}",
+                    {get_kwargs(inputs_map, loop_body_class)}
+                )
+            )
+
+            condition = self.add_child(
+                {condition_class.__name__}(
+                    label="{condition_class.__name__}",
+                    {get_kwargs(inputs_map, condition_class)}
+                )
+            )
 
-        switch.inputs.condition = condition_node
-        for out_n, out_c, in_n, in_c in internal_connection_map:
-            macro.children[in_n].inputs[in_c] = macro.children[out_n].outputs[out_c]
+            self.switch = self.create.standard.If(condition=condition)
 
-        switch.signals.output.true >> body_node >> condition_node >> switch
-        macro.starting_nodes = [body_node]
+            for out_n, out_c, in_n, in_c in {str(internal_connection_map)}:
+                self.children[in_n].inputs[in_c] = self.children[out_n].outputs[out_c]
+
+
+            self.switch.signals.output.true >> body >> condition >> self.switch
+            self.starting_nodes = [body]
+
+            return {returns}
+        """
+    )
 
-        macro.inputs_map = {} if inputs_map is None else inputs_map
-        macro.outputs_map = {} if outputs_map is None else outputs_map
+    exec(while_loop_code)
+    return locals()[node_name]
 
-    return macro_node()(make_loop)
+    # def make_loop(macro):
+    #     body_node = macro.add_child(loop_body_class(label=loop_body_class.__name__))
+    #     condition_node = macro.add_child(
+    #         condition_class(label=condition_class.__name__)
+    #     )
+    #     switch = macro.create.standard.If(label="switch", parent=macro)
+    #
+    #     switch.inputs.condition = condition_node
+    #     for out_n, out_c, in_n, in_c in internal_connection_map:
+    #         macro.children[in_n].inputs[in_c] = macro.children[out_n].outputs[out_c]
+    #
+    #     switch.signals.output.true >> body_node >> condition_node >> switch
+    #     macro.starting_nodes = [body_node]
+    #
+    #     macro.inputs_map = {} if inputs_map is None else inputs_map
+    #     macro.outputs_map = {} if outputs_map is None else outputs_map
+    #
+    # return as_macro_node()(make_loop)
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/node.py` & `pyiron_workflow-0.6.0/pyiron_workflow/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from pyiron_workflow.single_output import ExploitsSingleOutput
 from pyiron_workflow.storage import HasH5ioStorage, HasTinybaseStorage
 from pyiron_workflow.topology import (
     get_nodes_in_data_tree,
     set_run_connections_according_to_linear_dag,
 )
 from pyiron_workflow.snippets.colors import SeabornColors
-from pyiron_workflow.snippets.has_post import AbstractHasPost
 from pyiron_workflow.working import HasWorkingDirectory
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     import graphviz
 
@@ -43,15 +42,14 @@
     Runnable,
     HasIOWithInjection,
     ExploitsSingleOutput,
     HasWorkingDirectory,
     HasH5ioStorage,
     HasTinybaseStorage,
     ABC,
-    metaclass=AbstractHasPost,
 ):
     """
     Nodes are elements of a computational graph.
     They have inputs and outputs to interface with the wider world, and perform some
     operation.
     By connecting multiple nodes' inputs and outputs together, computational graphs can
     be formed.
@@ -132,15 +130,15 @@
             runs.
         - On instantiation, nodes will load automatically if they find saved content.
           - Discovered content can instead be deleted with a kwarg.
           - You can't load saved content _and_ run after instantiation at once.
         - The nodes must be somewhere importable, and the imported object must match
             the type of the node being saved. This basically just rules out one edge
             case where a node class is defined like
-            `SomeFunctionNode = Workflow.wrap_as.function_node()(some_function)`, since
+            `SomeFunctionNode = Workflow.wrap.as_function_node()(some_function)`, since
             then the new class gets the name `some_function`, which when imported is
             the _function_ "some_function" and not the desired class "SomeFunctionNode".
             This is checked for at save-time and will cause a nice early failure.
         - [ALPHA ISSUE] If the source code (cells, `.py` files...) for a saved graph is
             altered between saving and loading the graph, there are no guarantees about
             the loaded state; depending on the nature of the changes everything may
             work fine with the new node definition, the graph may load but silently
@@ -271,54 +269,86 @@
             object is encountered).
         replace_with: If the node belongs to a parent, attempts to replace itself in
             that parent with a new provided node.
         run: Run the node function from :meth:`on_run`. Handles status automatically. Various
             execution options are available as boolean flags.
         set_input_values: Allows input channels' values to be updated without any
             running.
+
+    Note:
+        :meth:`__init__` ends with a routine :meth:`_after_node_setup` that may,
+        depending on instantiation arguments, try to actually execute the node. Since
+        child classes may need to get things done before this point, we want to make
+        sure that this happens _after_ all the other setup. This can be accomplished
+        by children (a) sticking stuff that is independent of `super().__init__` calls
+        before the super call, and (b) overriding :meth:`_setup_node(self)` to do any
+        remaining, parameter-free setup. This latter function gets called prior to any
+        execution.
+
+        Initialization will also try to parse any outstanding `args` and `kwargs` as
+        input to the node's input channels. For node class developers, that means it's
+        also important that `Node` parentage appear to the right-most of the
+        inheritance set in the class definition, so that it's invokation of `__init__`
+        appears as late as possible with the minimal set of args and kwargs.
     """
 
     package_identifier = None
 
     # This isn't nice, just a technical necessity in the current implementation
     # Eventually, of course, this needs to be _at least_ file-format independent
 
     def __init__(
         self,
-        label: str,
         *args,
+        label: Optional[str] = None,
         parent: Optional[Composite] = None,
         overwrite_save: bool = False,
         run_after_init: bool = False,
         storage_backend: Literal["h5io", "tinybase"] | None = "h5io",
         save_after_run: bool = False,
         **kwargs,
     ):
         """
-        A mixin class for objects that can form nodes in the graph representation of a
+        A parent class for objects that can form nodes in the graph representation of a
         computational workflow.
 
         Args:
             label (str): A name for this node.
-            *args: Arguments passed on with `super`.
+            *args: Interpreted as node input data, in order of input channels.
             parent: (Composite|None): The composite node that owns this as a child.
             run_after_init (bool): Whether to run at the end of initialization.
-            **kwargs: Keyword arguments passed on with `super`.
+            **kwargs: Interpreted as node input data, with keys corresponding to
+                channel labels.
         """
         super().__init__(
-            *args,
-            label=label,
+            label=self.__class__.__name__ if label is None else label,
             parent=parent,
             storage_backend=storage_backend,
-            **kwargs,
         )
         self.save_after_run = save_after_run
         self._user_data = {}  # A place for power-users to bypass node-injection
 
-    def __post__(
+        self._setup_node()
+        self._after_node_setup(
+            *args,
+            overwrite_save=overwrite_save,
+            run_after_init=run_after_init,
+            **kwargs,
+        )
+
+    def _setup_node(self) -> None:
+        """
+        Called _before_ :meth:`Node.__init__` finishes.
+
+        Child node classes can use this for any parameter-free node setup that should
+        happen _before_ :meth:`Node._after_node_setup` gets called.
+        """
+        pass
+
+    def _after_node_setup(
         self,
         *args,
         overwrite_save: bool = False,
         run_after_init: bool = False,
         **kwargs,
     ):
         if overwrite_save and sys.version_info >= (3, 11):
@@ -336,20 +366,23 @@
         elif do_load:
             warnings.warn(
                 f"A saved file was found for the node {self.label} -- attempting to "
                 f"load it...(To delete the saved file instead, use "
                 f"`overwrite_save=True`)"
             )
             self.load()
+            self.set_input_values(*args, **kwargs)
         elif run_after_init:
             try:
+                self.set_input_values(*args, **kwargs)
                 self.run()
             except ReadinessError:
                 pass
-        # Else neither loading nor running now -- no action required!
+        else:
+            self.set_input_values(*args, **kwargs)
         self.graph_root.tidy_working_directory()
 
     @property
     def graph_path(self) -> str:
         """
         The path of node labels from the graph root (parent-most node in this semantic
         path) down to this node.
@@ -378,14 +411,15 @@
             f"{self.label} received a run command but is not ready. The node "
             f"should be neither running nor failed, and all input values should"
             f" conform to type hints.\n" + self.readiness_report
         )
 
     def run(
         self,
+        *args,
         run_data_tree: bool = False,
         run_parent_trees_too: bool = False,
         fetch_input: bool = True,
         check_readiness: bool = True,
         force_local_execution: bool = False,
         emit_ran_signal: bool = True,
         **kwargs,
@@ -408,15 +442,18 @@
 
         Args:
             run_data_tree (bool): Whether to first run all upstream nodes in the data
                 graph. (Default is False.)
             run_parent_trees_too (bool): Whether to recursively run the data tree in
                 parent nodes (if any). (Default is False.)
             fetch_input (bool): Whether to first update inputs with the
-                highest-priority connections holding data. (Default is True.)
+                highest-priority connections holding data (i.e. the first valid
+                connection; and the most recently formed connections appear first
+                unless the connections list has been manually tampered with). (Default
+                is True.)
             check_readiness (bool): Whether to raise an exception if the node is not
                 :attr:`ready` to run after fetching new input. (Default is True.)
             force_local_execution (bool): Whether to ignore any executor settings and
                 force the computation to run locally. (Default is False.)
             emit_ran_signal (bool): Whether to fire off all the output `ran` signal
                 afterwards. (Default is True.)
             **kwargs: Keyword arguments matching input channel labels; used to update
@@ -430,22 +467,25 @@
             Running data trees is a pull-based paradigm and only compatible with graphs
             whose data forms a directed acyclic graph (DAG).
 
         Note:
             Kwargs updating input channel values happens _first_ and will get
             overwritten by any subsequent graph-based data manipulation.
         """
-        self.set_input_values(**kwargs)
+        self.set_input_values(*args, **kwargs)
 
         if run_data_tree:
             self.run_data_tree(run_parent_trees_too=run_parent_trees_too)
 
         if fetch_input:
             self.inputs.fetch()
 
+        if self.parent is not None:
+            self.parent.register_child_starting(self)
+
         return super().run(
             check_readiness=check_readiness,
             force_local_execution=force_local_execution,
             _finished_callback=(
                 self._finish_run_and_emit_ran if emit_ran_signal else self._finish_run
             ),
         )
@@ -486,107 +526,151 @@
             # Maybe we could switch a bunch of stuff to rely on the unique ID?
             nodes[modified_label] = node
 
         try:
             disconnected_pairs, starters = set_run_connections_according_to_linear_dag(
                 nodes
             )
-            starter = starters[0]
+            data_tree_starters = list(set(starters).intersection(data_tree_nodes))
         except Exception as e:
             # If the dag setup fails it will repair any connections it breaks before
             # raising the error, but we still need to repair our label changes
             for modified_label, node in nodes.items():
                 node.label = label_map[modified_label]
             raise e
 
-        self.signals.disconnect_run()
-        # Don't let anything upstream trigger this node
-
         try:
-            # If you're the only one in the data tree, there's nothing upstream to run
-            # Otherwise...
-            if starter is not self:
-                starter.run()  # Now push from the top
+            parent_starting_nodes = (
+                self.parent.starting_nodes if self.parent is not None else None
+            )  # We need these for state recovery later, even if we crash
+
+            if len(data_tree_starters) == 1 and data_tree_starters[0] is self:
+                # If you're the only one in the data tree, there's nothing upstream to
+                # run.
+                pass
+            else:
+                for node in set(nodes.values()).difference(data_tree_nodes):
+                    # Disconnect any nodes not in the data tree to avoid unnecessary
+                    # execution
+                    node.signals.disconnect_run()
+
+                self.signals.disconnect_run()
+                # Don't let anything upstream trigger _this_ node
+
+                if self.parent is None:
+                    for starter in data_tree_starters:
+                        starter.run()  # Now push from the top
+                else:
+                    # Run the special exec connections from above with the parent
+
+                    # Workflow parents will attempt to automate execution on run,
+                    # undoing all our careful execution
+                    # This heinous hack breaks in and stops that behaviour
+                    # I recognize this is dirty, but let's be pragmatic about getting
+                    # the features playing together. Workflows and pull are anyhow
+                    # already both very annoying on their own...
+                    from pyiron_workflow.workflow import Workflow
+
+                    if isinstance(self.parent, Workflow):
+                        automated = self.parent.automate_execution
+                        self.parent.automate_execution = False
+
+                    self.parent.starting_nodes = data_tree_starters
+                    self.parent.run()
+
+                    # And revert our workflow hack
+                    if isinstance(self.parent, Workflow):
+                        self.parent.automate_execution = automated
         finally:
             # No matter what, restore the original connections and labels afterwards
             for modified_label, node in nodes.items():
                 node.label = label_map[modified_label]
                 node.signals.disconnect_run()
             for c1, c2 in disconnected_pairs:
                 c1.connect(c2)
+            if self.parent is not None:
+                self.parent.starting_nodes = parent_starting_nodes
 
     def _finish_run(self, run_output: tuple | Future) -> Any | tuple:
         try:
-            return super()._finish_run(run_output=run_output)
+            processed_output = super()._finish_run(run_output=run_output)
+            if self.parent is not None:
+                self.parent.register_child_finished(self)
+            return processed_output
         finally:
             if self.save_after_run:
                 self.save()
 
     def _finish_run_and_emit_ran(self, run_output: tuple | Future) -> Any | tuple:
         processed_output = self._finish_run(run_output)
-        self.signals.output.ran()
+        if self.parent is None:
+            self.signals.output.ran()
+        else:
+            self.parent.register_child_emitting_ran(self)
         return processed_output
 
     _finish_run_and_emit_ran.__doc__ = (
         Runnable._finish_run.__doc__
         + """
 
     Finally, fire the `ran` signal.
     """
     )
 
-    def execute(self, **kwargs):
+    def execute(self, *args, **kwargs):
         """
         A shortcut for :meth:`run` with particular flags.
 
         Run the node with whatever input it currently has (or is given as kwargs here),
         run it on this python process, and don't emit the `ran` signal afterwards.
 
         Intended to be useful for debugging by just forcing the node to do its thing
         right here, right now, and as-is.
         """
         return self.run(
+            *args,
             run_data_tree=False,
             run_parent_trees_too=False,
             fetch_input=False,
             check_readiness=False,
             force_local_execution=True,
             emit_ran_signal=False,
             **kwargs,
         )
 
-    def pull(self, run_parent_trees_too=False, **kwargs):
+    def pull(self, *args, run_parent_trees_too=False, **kwargs):
         """
         A shortcut for :meth:`run` with particular flags.
 
         Runs nodes upstream in the data graph, then runs this node without triggering
         any downstream runs. By default only runs sibling nodes, but can optionally
         require the parent node to pull in its own upstream runs (this is recursive
         up to the parent-most object).
 
         Args:
             run_parent_trees_too (bool): Whether to (recursively) require the parent to
                 first pull.
         """
         return self.run(
+            *args,
             run_data_tree=True,
             run_parent_trees_too=run_parent_trees_too,
             fetch_input=True,
             check_readiness=True,
             force_local_execution=False,
             emit_ran_signal=False,
             **kwargs,
         )
 
-    def __call__(self, **kwargs) -> None:
+    def __call__(self, *args, **kwargs) -> None:
         """
         A shortcut for :meth:`pull` that automatically runs the entire set of upstream data
         dependencies all the way to the parent-most graph object.
         """
-        return self.pull(run_parent_trees_too=True, **kwargs)
+        return self.pull(*args, run_parent_trees_too=True, **kwargs)
 
     @property
     def ready(self) -> bool:
         return super().ready and self.inputs.ready
 
     @property
     def color(self) -> str:
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/calculator.py` & `pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from ase.units import Ry
 
-from pyiron_workflow.function import function_node
+from pyiron_workflow.function import as_function_node
 
 
-@function_node("calculator")
+@as_function_node("calculator")
 def Emt():
     from ase.calculators.emt import EMT
 
     return EMT()
 
 
-@function_node("calculator")
+@as_function_node("calculator")
 def Abinit(
-    label="abinit_evcurve",
+    ase_label="abinit_evcurve",
     nbands=32,
     ecut=10 * Ry,
     kpts=(3, 3, 3),
     toldfe=1.0e-2,
     v8_legacy_format=False,
 ):
     from ase.calculators.abinit import Abinit
 
     return Abinit(
-        label=label,
+        label=ase_label,
         nbands=nbands,
         ecut=ecut,
         kpts=kpts,
         toldfe=toldfe,
         v8_legacy_format=v8_legacy_format,
     )
 
 
-@function_node("calculator")
+@as_function_node("calculator")
 def Gpaw(xc="PBE", encut=300, kpts=(3, 3, 3)):
     from gpaw import GPAW, PW
 
     return GPAW(xc=xc, mode=PW(encut), kpts=kpts)
 
 
-@function_node("calculator")
+@as_function_node("calculator")
 def QuantumEspresso(
     pseudopotentials={"Al": "Al.pbe-n-kjpaw_psl.1.0.0.UPF"},
     tstress=True,
     tprnfor=True,
     kpts=(3, 3, 3),
 ):
     from ase.calculators.espresso import Espresso
@@ -51,57 +51,57 @@
         pseudopotentials=pseudopotentials,
         tstress=tstress,
         tprnfor=tprnfor,
         kpts=kpts,
     )
 
 
-@function_node("calculator")
+@as_function_node("calculator")
 def Siesta(
-    label="siesta",
+    ase_label="siesta",
     xc="PBE",
     mesh_cutoff=200 * Ry,
     energy_shift=0.01 * Ry,
     basis_set="DZ",
     kpts=(5, 5, 5),
     fdf_arguments={"DM.MixingWeight": 0.1, "MaxSCFIterations": 100},
     pseudo_path="",
     pseudo_qualifier="",
 ):
     from ase.calculators.siesta import Siesta
 
     return Siesta(
-        label=label,
+        label=ase_label,
         xc=xc,
         mesh_cutoff=mesh_cutoff,
         energy_shift=energy_shift,
         basis_set=basis_set,
         kpts=kpts,
         fdf_arguments=fdf_arguments,
         pseudo_path=pseudo_path,
         pseudo_qualifier=pseudo_qualifier,
     )
 
 
-@function_node("energy_dict")
+@as_function_node("energy_dict")
 def CalcWithCalculator(task_dict, calculator):
     from atomistics.calculators.ase import evaluate_with_ase
 
     return evaluate_with_ase(task_dict=task_dict, ase_calculator=calculator)
 
 
-@function_node("lammps_potential_dataframe")
+@as_function_node("lammps_potential_dataframe")
 def LammpsPotential(potential_name, structure, resource_path):
     from atomistics.calculators.lammps import get_potential_dataframe
 
     df_pot = get_potential_dataframe(structure=structure, resource_path=resource_path)
     return df_pot[df_pot.Name == potential_name].iloc[0]
 
 
-@function_node("energy_dict")
+@as_function_node("energy_dict")
 def Lammps(task_dict, potential_dataframe):
     from atomistics.calculators.lammps import evaluate_with_lammps
 
     return evaluate_with_lammps(
         task_dict=task_dict,
         potential_dataframe=potential_dataframe,
     )
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/task.py` & `pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from phonopy.units import VaspToTHz
-from pyiron_workflow.function import function_node
+from pyiron_workflow.function import as_function_node
 
 
-@function_node("task_generator")
+@as_function_node("task_generator")
 def ElasticMatrixTaskGenerator(
     structure, num_of_point=5, eps_range=0.05, sqrt_eta=True, fit_order=2
 ):
     from atomistics.workflows.elastic.workflow import ElasticMatrixWorkflow
 
     return ElasticMatrixWorkflow(
         structure=structure,
         num_of_point=num_of_point,
         eps_range=eps_range,
         sqrt_eta=sqrt_eta,
         fit_order=fit_order,
     )
 
 
-@function_node("task_generator")
+@as_function_node("task_generator")
 def EvcurveTaskGenerator(
     structure,
     num_points=11,
     fit_type="polynomial",
     fit_order=3,
     vol_range=0.05,
     axes=["x", "y", "z"],
@@ -36,15 +36,15 @@
         fit_order=fit_order,
         vol_range=vol_range,
         axes=axes,
         strains=strains,
     )
 
 
-@function_node("task_generator")
+@as_function_node("task_generator")
 def PhononsTaskGenerator(
     structure,
     interaction_range=10,
     factor=VaspToTHz,
     displacement=0.01,
     dos_mesh=20,
     primitive_matrix=None,
@@ -59,25 +59,25 @@
         displacement=displacement,
         dos_mesh=dos_mesh,
         primitive_matrix=primitive_matrix,
         number_of_snapshots=number_of_snapshots,
     )
 
 
-@function_node("result_dict")
+@as_function_node("result_dict")
 def AnalyseStructures(instance, output_dict):
     return instance.analyse_structures(output_dict=output_dict)
 
 
-@function_node("task_dict")
+@as_function_node("task_dict")
 def GenerateStructures(instance):
     return instance.generate_structures()
 
 
-@function_node("structure")
+@as_function_node("structure")
 def Bulk(element):
     from ase.build import bulk
 
     return bulk(element)
 
 
 nodes = [
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/node_library/pyiron_atomistics.py` & `pyiron_workflow-0.6.0/pyiron_workflow/node_library/pyiron_atomistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from typing import Literal, Optional
 
 from pyiron_atomistics import Project, _StructureFactory
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 from pyiron_atomistics.lammps.lammps import Lammps as LammpsJob
 
-from pyiron_workflow.function import function_node
+from pyiron_workflow.function import as_function_node
 
 
-Bulk = function_node("structure")(_StructureFactory().bulk)
+Bulk = as_function_node("structure")(_StructureFactory().bulk)
 Bulk.__name__ = "Bulk"
+Bulk.__module__ = __name__
 
 
-@function_node("job")
+@as_function_node("job")
 def Lammps(structure: Optional[Atoms] = None) -> LammpsJob:
     pr = Project(".")
     job = pr.atomistics.job.Lammps("NOTAREALNAME")
     job.structure = structure if structure is not None else _StructureFactory().bulk()
     job.potential = job.list_potentials()[0]
     return job
 
@@ -80,51 +81,53 @@
         temperature,
         total_displacements,
         unwrapped_positions,
         volume,
     )
 
 
-@function_node(
+@as_function_node(
     "cells",
     "displacements",
     "energy_pot",
     "energy_tot",
     "force_max",
     "forces",
     "indices",
     "positions",
     "pressures",
     "steps",
     "temperature",
     "total_displacements",
     "unwrapped_positions",
     "volume",
+    validate_output_labels=False,
 )
 def CalcStatic(
     job: AtomisticGenericJob,
 ):
     return _run_and_remove_job(job=job)
 
 
-@function_node(
+@as_function_node(
     "cells",
     "displacements",
     "energy_pot",
     "energy_tot",
     "force_max",
     "forces",
     "indices",
     "positions",
     "pressures",
     "steps",
     "temperature",
     "total_displacements",
     "unwrapped_positions",
     "volume",
+    validate_output_labels=False,
 )
 def CalcMd(
     job: AtomisticGenericJob,
     n_ionic_steps: int = 1000,
     n_print: int = 100,
     temperature: int | float = 300.0,
     pressure: (
@@ -149,28 +152,29 @@
         n_ionic_steps=n_ionic_steps,
         n_print=n_print,
         temperature=temperature,
         pressure=pressure,
     )
 
 
-@function_node(
+@as_function_node(
     "cells",
     "displacements",
     "energy_pot",
     "energy_tot",
     "force_max",
     "forces",
     "indices",
     "positions",
     "pressures",
     "steps",
     "total_displacements",
     "unwrapped_positions",
     "volume",
+    validate_output_labels=False,
 )
 def CalcMin(
     job: AtomisticGenericJob,
     n_ionic_steps: int = 1000,
     n_print: int = 100,
     pressure: (
         float
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/node_library/standard.py` & `pyiron_workflow-0.6.0/pyiron_workflow/node_library/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 """
 Common-use nodes relying only on the standard library
 """
 
 from __future__ import annotations
 
-from inspect import isclass
+import random
 
 from pyiron_workflow.channels import NOT_DATA, OutputSignal
-from pyiron_workflow.function import Function, function_node
+from pyiron_workflow.function import Function, as_function_node
 
 
-@function_node()
+@as_function_node()
 def UserInput(user_input):
     return user_input
 
 
 class If(Function):
     """
     Has two extra signal channels: true and false. Evaluates the input as obj otheroolean and
     fires the corresponding output signal after running.
     """
 
     def __init__(self, **kwargs):
-        super().__init__(self.if_, output_labels="truth", **kwargs)
+        super().__init__(**kwargs)
         self.signals.output.true = OutputSignal("true", self)
         self.signals.output.false = OutputSignal("false", self)
 
     @staticmethod
-    def if_(condition):
+    def node_function(condition):
         if condition is NOT_DATA:
             raise TypeError(
                 f"Logic 'If' node expected data other but got NOT_DATA as input."
             )
-        return bool(condition)
+        truth = bool(condition)
+        return truth
 
     def process_run_result(self, function_output):
         """
         Process the output as usual, then fire signals accordingly.
         """
         super().process_run_result(function_output)
 
         if self.outputs.truth.value:
             self.signals.output.true()
         else:
             self.signals.output.false()
 
 
-@function_node("slice")
+@as_function_node("random")
+def RandomFloat():
+    return random.random()
+
+
+@as_function_node("slice")
 def Slice(start=None, stop=NOT_DATA, step=None):
     if start is None:
         if stop is None:
             raise ValueError(
                 "Slice must define at least start or stop, but both are None"
             )
         elif step is not None:
@@ -64,193 +70,193 @@
     return s
 
 
 # A bunch of (but not all) standard operators
 # Return values based on dunder methods, where available
 
 
-@function_node("str")
+@as_function_node("str")
 def String(obj):
     return str(obj)
 
 
-@function_node("bytes")
+@as_function_node("bytes")
 def Bytes(obj):
     return bytes(obj)
 
 
-@function_node("lt")
+@as_function_node("lt")
 def LessThan(obj, other):
     return obj < other
 
 
-@function_node("le")
+@as_function_node("le")
 def LessThanEquals(obj, other):
     return obj <= other
 
 
-@function_node("eq")
+@as_function_node("eq")
 def Equals(obj, other):
     return obj == other
 
 
-@function_node("neq")
+@as_function_node("neq")
 def NotEquals(obj, other):
     return obj != other
 
 
-@function_node("gt")
+@as_function_node("gt")
 def GreaterThan(obj, other):
     return obj > other
 
 
-@function_node("ge")
+@as_function_node("ge")
 def GreaterThanEquals(obj, other):
     return obj >= other
 
 
-@function_node("hash")
+@as_function_node("hash")
 def Hash(obj):
     return hash(obj)
 
 
-@function_node("bool")
+@as_function_node("bool")
 def Bool(obj):
     return bool(obj)
 
 
-@function_node("getattr")
+@as_function_node("getattr")
 def GetAttr(obj, name):
     return getattr(obj, name)
 
 
 # These are not idempotent and thus not encouraged
-# @function_node("none")
+# @as_function_node("none")
 # def SetAttr(obj, name, value):
 #     setattr(obj, name, value)
 #     return None
 #
 #
-# @function_node("none")
+# @as_function_node("none")
 # def DelAttr(obj, name):
 #     delattr(obj, name)
 #     return None
 
 
-@function_node("getitem")
+@as_function_node("getitem")
 def GetItem(obj, item):
     return obj[item]
 
 
-@function_node("dir")
+@as_function_node("dir")
 def Dir(obj):
     return dir(obj)
 
 
-@function_node("len")
+@as_function_node("len")
 def Length(obj):
     return len(obj)
 
 
-@function_node("in")
+@as_function_node("in")
 def Contains(obj, other):
     return other in obj
 
 
-@function_node("add")
+@as_function_node("add")
 def Add(obj, other):
     return obj + other
 
 
-@function_node("sub")
+@as_function_node("sub")
 def Subtract(obj, other):
     return obj - other
 
 
-@function_node("mul")
+@as_function_node("mul")
 def Multiply(obj, other):
     return obj * other
 
 
-@function_node("rmul")
+@as_function_node("rmul")
 def RightMultiply(obj, other):
     return other * obj
 
 
-@function_node("matmul")
+@as_function_node("matmul")
 def MatrixMultiply(obj, other):
     return obj @ other
 
 
-@function_node("truediv")
+@as_function_node("truediv")
 def Divide(obj, other):
     return obj / other
 
 
-@function_node("floordiv")
+@as_function_node("floordiv")
 def FloorDivide(obj, other):
     return obj // other
 
 
-@function_node("mod")
+@as_function_node("mod")
 def Modulo(obj, other):
     return obj % other
 
 
-@function_node("pow")
+@as_function_node("pow")
 def Power(obj, other):
     return obj**other
 
 
-@function_node("and")
+@as_function_node("and")
 def And(obj, other):
     return obj & other
 
 
-@function_node("xor")
+@as_function_node("xor")
 def XOr(obj, other):
     return obj ^ other
 
 
-@function_node("or")
+@as_function_node("or")
 def Or(obj, other):
     return obj ^ other
 
 
-@function_node("neg")
+@as_function_node("neg")
 def Negative(obj):
     return -obj
 
 
-@function_node("pos")
+@as_function_node("pos")
 def Positive(obj):
     return +obj
 
 
-@function_node("abs")
+@as_function_node("abs")
 def Absolute(obj):
     return abs(obj)
 
 
-@function_node("invert")
+@as_function_node("invert")
 def Invert(obj):
     return ~obj
 
 
-@function_node("int")
+@as_function_node("int")
 def Int(obj):
     return int(obj)
 
 
-@function_node("float")
+@as_function_node("float")
 def Float(obj):
     return float(obj)
 
 
-@function_node("round")
+@as_function_node("round")
 def Round(obj):
     return round(obj)
 
 
 nodes = [
     Absolute,
     Add,
@@ -278,14 +284,15 @@
     Modulo,
     Multiply,
     Negative,
     NotEquals,
     Or,
     Positive,
     Power,
+    RandomFloat,
     RightMultiply,
     Round,
     Slice,
     String,
     Subtract,
     UserInput,
     XOr,
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/node_package.py` & `pyiron_workflow-0.6.0/pyiron_workflow/node_package.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/output_parser.py` & `pyiron_workflow-0.6.0/pyiron_workflow/output_parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/run.py` & `pyiron_workflow-0.6.0/pyiron_workflow/run.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/semantics.py` & `pyiron_workflow-0.6.0/pyiron_workflow/semantics.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/single_output.py` & `pyiron_workflow-0.6.0/pyiron_workflow/single_output.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/colors.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/colors.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/dotdict.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/files.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/has_post.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/has_post.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/logger.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/singleton.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/snippets/testcase.py` & `pyiron_workflow-0.6.0/pyiron_workflow/snippets/testcase.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/storage.py` & `pyiron_workflow-0.6.0/pyiron_workflow/storage.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/topology.py` & `pyiron_workflow-0.6.0/pyiron_workflow/topology.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/type_hinting.py` & `pyiron_workflow-0.6.0/pyiron_workflow/type_hinting.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow/working.py` & `pyiron_workflow-0.6.0/pyiron_workflow/working.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow.egg-info/PKG-INFO` & `pyiron_workflow-0.6.0/pyiron_workflow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.5.0
+Version: 0.6.0
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
@@ -15,22 +15,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: bidict>=0.23.1
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: graphviz>=0.20.3
 Requires-Dist: h5io>=0.2.2
-Requires-Dist: h5io_browser>=0.0.10
-Requires-Dist: matplotlib>=3.8.3
-Requires-Dist: pyiron_base>=0.8.0
+Requires-Dist: h5io_browser>=0.0.12
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: pyiron_base>=0.8.2
 Requires-Dist: pyiron_contrib>=0.1.16
 Requires-Dist: pympipool>=0.7.17
 Requires-Dist: toposort>=1.10
 Requires-Dist: typeguard>=4.2.1
 Provides-Extra: node-library
 Requires-Dist: ase>=3.22.1; extra == "node-library"
-Requires-Dist: atomistics>=0.1.24; extra == "node-library"
+Requires-Dist: atomistics>=0.1.27; extra == "node-library"
 Requires-Dist: numpy>=1.26.4; extra == "node-library"
 Requires-Dist: phonopy>=2.22.1; extra == "node-library"
-Requires-Dist: pyiron_atomistics>=0.5.0; extra == "node-library"
+Requires-Dist: pyiron_atomistics>=0.5.3; extra == "node-library"
 
 http://pyiron.org
```

### Comparing `pyiron_workflow-0.5.0/pyiron_workflow.egg-info/SOURCES.txt` & `pyiron_workflow-0.6.0/pyiron_workflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 pyiron_workflow/create.py
 pyiron_workflow/draw.py
 pyiron_workflow/function.py
 pyiron_workflow/has_interface_mixins.py
 pyiron_workflow/has_to_dict.py
 pyiron_workflow/injection.py
 pyiron_workflow/io.py
+pyiron_workflow/io_preview.py
 pyiron_workflow/job.py
+pyiron_workflow/loops.py
 pyiron_workflow/macro.py
 pyiron_workflow/meta.py
 pyiron_workflow/node.py
 pyiron_workflow/node_package.py
 pyiron_workflow/output_parser.py
 pyiron_workflow/run.py
 pyiron_workflow/semantics.py
```

### Comparing `pyiron_workflow-0.5.0/setup.py` & `pyiron_workflow-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'bidict>=0.23.1',
         'cloudpickle>=3.0.0',
         'graphviz>=0.20.3',
         'h5io>=0.2.2',
-        'h5io_browser>=0.0.10',
-        'matplotlib>=3.8.3',
-        'pyiron_base>=0.8.0',
+        'h5io_browser>=0.0.12',
+        'matplotlib>=3.8.4',
+        'pyiron_base>=0.8.2',
         'pyiron_contrib>=0.1.16',
         'pympipool>=0.7.17',
         'toposort>=1.10',
         'typeguard>=4.2.1',
     ],
     extras_require={
         "node_library": [
             'ase>=3.22.1',
-            'atomistics>=0.1.24',
+            'atomistics>=0.1.27',
             'numpy>=1.26.4',
             'phonopy>=2.22.1',
-            'pyiron_atomistics>=0.5.0',
+            'pyiron_atomistics>=0.5.3',
         ],
     },
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron_workflow-0.5.0/versioneer.py` & `pyiron_workflow-0.6.0/versioneer.py`

 * *Files identical despite different names*

