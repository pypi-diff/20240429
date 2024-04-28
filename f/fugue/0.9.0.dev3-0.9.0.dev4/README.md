# Comparing `tmp/fugue-0.9.0.dev3.tar.gz` & `tmp/fugue-0.9.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.9.0.dev3.tar", last modified: Sun Jan 21 08:21:10 2024, max compression
+gzip compressed data, was "fugue-0.9.0.dev4.tar", last modified: Sun Apr 28 23:32:42 2024, max compression
```

## Comparing `fugue-0.9.0.dev3.tar` & `fugue-0.9.0.dev4.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.593243 fugue-0.9.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-01-21 08:21:10.593243 fugue-0.9.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.569243 fugue-0.9.0.dev3/fugue/
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.569243 fugue-0.9.0.dev3/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.569243 fugue-0.9.0.dev3/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.573243 fugue-0.9.0.dev3/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17257 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.573243 fugue-0.9.0.dev3/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17391 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.573243 fugue-0.9.0.dev3/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.573243 fugue-0.9.0.dev3/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.573243 fugue-0.9.0.dev3/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39818 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47506 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14236 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.573243 fugue-0.9.0.dev3/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14545 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.577243 fugue-0.9.0.dev3/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33844 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.581243 fugue-0.9.0.dev3/fugue/test/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/test/pandas_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/test/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.581243 fugue-0.9.0.dev3/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    88219 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.569243 fugue-0.9.0.dev3/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-01-21 08:21:10.000000 fugue-0.9.0.dev3/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-01-21 08:21:10.000000 fugue-0.9.0.dev3/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 08:21:10.000000 fugue-0.9.0.dev3/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-21 08:21:10.000000 fugue-0.9.0.dev3/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-21 08:21:10.000000 fugue-0.9.0.dev3/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-21 08:21:10.000000 fugue-0.9.0.dev3/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.581243 fugue-0.9.0.dev3/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.581243 fugue-0.9.0.dev3/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.581243 fugue-0.9.0.dev3/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.581243 fugue-0.9.0.dev3/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13471 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_dask/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.585243 fugue-0.9.0.dev3/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20389 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_duckdb/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.585243 fugue-0.9.0.dev3/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ibis/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    18366 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ibis/execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.585243 fugue-0.9.0.dev3/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.585243 fugue-0.9.0.dev3/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.585243 fugue-0.9.0.dev3/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.589243 fugue-0.9.0.dev3/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.589243 fugue-0.9.0.dev3/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_ray/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.589243 fugue-0.9.0.dev3/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.589243 fugue-0.9.0.dev3/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    33048 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_spark/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.589243 fugue-0.9.0.dev3/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.593243 fugue-0.9.0.dev3/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    77940 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    19029 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    47969 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_test/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 08:21:10.593243 fugue-0.9.0.dev3/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-21 08:21:10.593243 fugue-0.9.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-01-21 08:19:07.000000 fugue-0.9.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.675008 fugue-0.9.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-04-28 23:32:42.675008 fugue-0.9.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.655008 fugue-0.9.0.dev4/fugue/
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.655008 fugue-0.9.0.dev4/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.655008 fugue-0.9.0.dev4/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.655008 fugue-0.9.0.dev4/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17257 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.655008 fugue-0.9.0.dev4/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17391 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.659008 fugue-0.9.0.dev4/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.659008 fugue-0.9.0.dev4/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.659008 fugue-0.9.0.dev4/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39818 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47506 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14236 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.659008 fugue-0.9.0.dev4/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.659008 fugue-0.9.0.dev4/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14545 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33844 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.663008 fugue-0.9.0.dev4/fugue/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/test/pandas_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/test/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.667008 fugue-0.9.0.dev4/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88219 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.655008 fugue-0.9.0.dev4/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-04-28 23:32:42.000000 fugue-0.9.0.dev4/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-28 23:32:42.000000 fugue-0.9.0.dev4/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 23:32:42.000000 fugue-0.9.0.dev4/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-28 23:32:42.000000 fugue-0.9.0.dev4/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-28 23:32:42.000000 fugue-0.9.0.dev4/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-28 23:32:42.000000 fugue-0.9.0.dev4/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.667008 fugue-0.9.0.dev4/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.667008 fugue-0.9.0.dev4/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.667008 fugue-0.9.0.dev4/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.667008 fugue-0.9.0.dev4/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13471 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_dask/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.667008 fugue-0.9.0.dev4/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20389 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_duckdb/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ibis/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ibis/execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_ray/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33048 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_spark/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.671008 fugue-0.9.0.dev4/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.675008 fugue-0.9.0.dev4/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77960 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48646 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_test/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:32:42.675008 fugue-0.9.0.dev4/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-28 23:32:42.675008 fugue-0.9.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-28 23:30:22.000000 fugue-0.9.0.dev4/setup.py
```

### Comparing `fugue-0.9.0.dev3/LICENSE` & `fugue-0.9.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/PKG-INFO` & `fugue-0.9.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.9.0.dev3
+Version: 0.9.0.dev4
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.9.0.dev3/README.md` & `fugue-0.9.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/__init__.py` & `fugue-0.9.0.dev4/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/_utils/display.py` & `fugue-0.9.0.dev4/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/_utils/exception.py` & `fugue-0.9.0.dev4/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/_utils/interfaceless.py` & `fugue-0.9.0.dev4/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/_utils/io.py` & `fugue-0.9.0.dev4/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/_utils/misc.py` & `fugue-0.9.0.dev4/fugue/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/api.py` & `fugue-0.9.0.dev4/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/bag/array_bag.py` & `fugue-0.9.0.dev4/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/bag/bag.py` & `fugue-0.9.0.dev4/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/collections/partition.py` & `fugue-0.9.0.dev4/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/collections/sql.py` & `fugue-0.9.0.dev4/fugue/collections/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _TEMP_TABLE_EXPR_SUFFIX = ">"
 
 
 class TempTableName:
     """Generating a temporary, random and globaly unique table name"""
 
     def __init__(self):
-        self.key = "_" + str(uuid4())[:5]
+        self.key = "_" + str(uuid4())[:5].upper()
 
     def __repr__(self) -> str:
         return _TEMP_TABLE_EXPR_PREFIX + self.key + _TEMP_TABLE_EXPR_SUFFIX
 
 
 @fugue_plugin
 def transpile_sql(
```

### Comparing `fugue-0.9.0.dev3/fugue/collections/yielded.py` & `fugue-0.9.0.dev4/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/column/expressions.py` & `fugue-0.9.0.dev4/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/column/functions.py` & `fugue-0.9.0.dev4/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/column/sql.py` & `fugue-0.9.0.dev4/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/constants.py` & `fugue-0.9.0.dev4/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/__init__.py` & `fugue-0.9.0.dev4/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/api.py` & `fugue-0.9.0.dev4/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/array_dataframe.py` & `fugue-0.9.0.dev4/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/arrow_dataframe.py` & `fugue-0.9.0.dev4/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/dataframe.py` & `fugue-0.9.0.dev4/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.9.0.dev4/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/dataframes.py` & `fugue-0.9.0.dev4/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/function_wrapper.py` & `fugue-0.9.0.dev4/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/iterable_dataframe.py` & `fugue-0.9.0.dev4/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/pandas_dataframe.py` & `fugue-0.9.0.dev4/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataframe/utils.py` & `fugue-0.9.0.dev4/fugue/dataframe/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,39 +17,24 @@
 
 # For backward compatibility, TODO: remove!
 get_dataframe_column_names = get_column_names
 normalize_dataframe_column_names = normalize_column_names
 rename_dataframe_column_names = rename
 
 
-def _pa_type_eq(t1: pa.DataType, t2: pa.DataType) -> bool:
-    # should ignore the name difference of list
-    # e.g. list<item: string> == list<l: string>
-    if pa.types.is_list(t1) and pa.types.is_list(t2):  # pragma: no cover
-        return _pa_type_eq(t1.value_type, t2.value_type)
-    return t1 == t2
-
-
-def _schema_eq(s1: Schema, s2: Schema) -> bool:
-    if s1 == s2:
-        return True
-    return s1.names == s2.names and all(
-        _pa_type_eq(f1.type, f2.type) for f1, f2 in zip(s1.fields, s2.fields)
-    )
-
-
 def _df_eq(
     df: DataFrame,
     data: Any,
     schema: Any = None,
     digits=8,
     check_order: bool = False,
     check_schema: bool = True,
     check_content: bool = True,
     no_pandas: bool = False,
+    equal_type_groups: Optional[List[List[Any]]] = None,
     throw=False,
 ) -> bool:
     """Compare if two dataframes are equal. Is for internal, unit test
     purpose only. It will convert both dataframes to
     :class:`~fugue.dataframe.dataframe.LocalBoundedDataFrame`, so it assumes
     both dataframes are small and fast enough to convert. DO NOT use it
     on critical or expensive tasks.
@@ -62,28 +47,29 @@
     :param digits: precision on float number comparison, defaults to 8
     :param check_order: if to compare the row orders, defaults to False
     :param check_schema: if compare schemas, defaults to True
     :param check_content: if to compare the row values, defaults to True
     :param no_pandas: if true, it will compare the string representations of the
       dataframes, otherwise, it will convert both to pandas dataframe to compare,
       defaults to False
+    :param equal_type_groups: the groups to treat as equal types, defaults to None.
     :param throw: if to throw error if not equal, defaults to False
     :return: if they equal
     """
     df1 = as_fugue_df(df).as_local_bounded()
     if schema is not None:
         df2 = as_fugue_df(data, schema=schema).as_local_bounded()
     else:
         df2 = as_fugue_df(data).as_local_bounded()
     try:
         assert (
             df1.count() == df2.count()
         ), f"count mismatch {df1.count()}, {df2.count()}"
-        assert not check_schema or _schema_eq(
-            df.schema, df2.schema
+        assert not check_schema or df.schema.is_like(
+            df2.schema, equal_groups=equal_type_groups
         ), f"schema mismatch {df.schema.pa_schema}, {df2.schema.pa_schema}"
         if not check_content:
             return True
         cols: Any = df1.columns
         if no_pandas:
             dd1 = [[x.__repr__()] for x in df1.as_array_iterable(type_safe=True)]
             dd2 = [[x.__repr__()] for x in df2.as_array_iterable(type_safe=True)]
```

### Comparing `fugue-0.9.0.dev3/fugue/dataset/api.py` & `fugue-0.9.0.dev4/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dataset/dataset.py` & `fugue-0.9.0.dev4/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/dev.py` & `fugue-0.9.0.dev4/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/exceptions.py` & `fugue-0.9.0.dev4/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/execution/api.py` & `fugue-0.9.0.dev4/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/execution/execution_engine.py` & `fugue-0.9.0.dev4/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/execution/factory.py` & `fugue-0.9.0.dev4/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/execution/native_execution_engine.py` & `fugue-0.9.0.dev4/fugue/execution/native_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/__init__.py` & `fugue-0.9.0.dev4/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/_builtins/__init__.py` & `fugue-0.9.0.dev4/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/_builtins/creators.py` & `fugue-0.9.0.dev4/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/_builtins/outputters.py` & `fugue-0.9.0.dev4/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/_builtins/processors.py` & `fugue-0.9.0.dev4/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/_utils.py` & `fugue-0.9.0.dev4/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/context.py` & `fugue-0.9.0.dev4/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/creator/convert.py` & `fugue-0.9.0.dev4/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/creator/creator.py` & `fugue-0.9.0.dev4/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/outputter/convert.py` & `fugue-0.9.0.dev4/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/outputter/outputter.py` & `fugue-0.9.0.dev4/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/processor/convert.py` & `fugue-0.9.0.dev4/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/processor/processor.py` & `fugue-0.9.0.dev4/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/transformer/convert.py` & `fugue-0.9.0.dev4/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/extensions/transformer/transformer.py` & `fugue-0.9.0.dev4/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/plugins.py` & `fugue-0.9.0.dev4/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/registry.py` & `fugue-0.9.0.dev4/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/rpc/base.py` & `fugue-0.9.0.dev4/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/rpc/flask.py` & `fugue-0.9.0.dev4/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/sql/_utils.py` & `fugue-0.9.0.dev4/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/sql/_visitors.py` & `fugue-0.9.0.dev4/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/sql/api.py` & `fugue-0.9.0.dev4/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/sql/workflow.py` & `fugue-0.9.0.dev4/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/test/pandas_tester.py` & `fugue-0.9.0.dev4/fugue/test/pandas_tester.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/test/plugins.py` & `fugue-0.9.0.dev4/fugue/test/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Type
-
+from fugue.dataframe.utils import _df_eq
 from triad import assert_or_throw, run_once
 from triad.utils.entry_points import load_entry_point
 
 try:
     import pytest
 
     _HAS_PYTEST = True
@@ -156,14 +156,15 @@
                 def test_spark(self):
                     # test spark
                     pass
     """
 
     backend: Any
     tmp_path: Path
+    equal_type_groups: Any = None
 
     __test__ = False
     _test_context: Any = None
 
     if _HAS_PYTEST:
 
         @pytest.fixture(autouse=True)
@@ -176,14 +177,23 @@
         return self._test_context
 
     @property
     def engine(self) -> Any:
         """The engine object inside the ``FugueTestContext``"""
         return self.context.engine
 
+    def get_equal_type_groups(self) -> Optional[List[List[Any]]]:
+        return None  # pragma: no cover
+
+    def df_eq(self, *args: Any, **kwargs: Any) -> bool:
+        """A wrapper of :func:`~fugue.dataframe.utils.df_eq`"""
+        if "equal_type_groups" not in kwargs:
+            kwargs["equal_type_groups"] = self.equal_type_groups
+        return _df_eq(*args, **kwargs)
+
 
 def fugue_test_suite(backend: Any, mark_test: Optional[bool] = None) -> Any:
     def deco(cls: Type["FugueTestSuite"]) -> Type["FugueTestSuite"]:
         import pytest
 
         assert_or_throw(
             issubclass(cls, FugueTestSuite),
```

### Comparing `fugue-0.9.0.dev3/fugue/workflow/_checkpoint.py` & `fugue-0.9.0.dev4/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/workflow/_tasks.py` & `fugue-0.9.0.dev4/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/workflow/_workflow_context.py` & `fugue-0.9.0.dev4/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/workflow/api.py` & `fugue-0.9.0.dev4/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/workflow/module.py` & `fugue-0.9.0.dev4/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue/workflow/workflow.py` & `fugue-0.9.0.dev4/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue.egg-info/PKG-INFO` & `fugue-0.9.0.dev4/fugue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.9.0.dev3
+Version: 0.9.0.dev4
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.9.0.dev3/fugue.egg-info/SOURCES.txt` & `fugue-0.9.0.dev4/fugue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue.egg-info/requires.txt` & `fugue-0.9.0.dev4/fugue.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-triad>=0.9.4
+triad>=0.9.6
 adagio>=0.2.4
 
 [all]
 qpd>=0.4.4
 fugue-sql-antlr>=0.2.0
 sqlglot
 jinja2
 pyspark>=3.1.1
 dask[dataframe,distributed]>=2023.5.0
 dask-sql
-ray[data]>=2.4.0
+ray[data]>=2.5.0
 notebook
 jupyterlab
 ipython>=7.10.0
 duckdb>=0.5.0
 pyarrow>=6.0.1
 pandas<2.2,>=2.0.2
 ibis-framework
@@ -23,41 +23,45 @@
 fugue-sql-antlr[cpp]>=0.2.0
 
 [dask]
 dask[dataframe,distributed]>=2023.5.0
 pyarrow>=7.0.0
 pandas>=2.0.2
 
+[dask:python_version >= "3.11.9"]
+dask[dataframe,distributed]>=2024.4.0
+
 [duckdb]
 qpd>=0.4.4
 fugue-sql-antlr>=0.2.0
 sqlglot
 jinja2
 duckdb>=0.5.0
 numpy
 
 [ibis]
 qpd>=0.4.4
 fugue-sql-antlr>=0.2.0
 sqlglot
 jinja2
 ibis-framework
+pandas<2.2
 
 [notebook]
 notebook
 jupyterlab
 ipython>=7.10.0
 
 [polars]
 polars
 
 [ray]
-ray[data]>=2.4.0
+ray[data]>=2.5.0
 duckdb>=0.5.0
-pyarrow>=6.0.1
+pyarrow>=7.0.0
 pandas<2.2
 
 [spark]
 pyspark>=3.1.1
 
 [sql]
 qpd>=0.4.4
```

### Comparing `fugue-0.9.0.dev3/fugue_contrib/seaborn/__init__.py` & `fugue-0.9.0.dev4/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_contrib/viz/__init__.py` & `fugue-0.9.0.dev4/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_contrib/viz/_ext.py` & `fugue-0.9.0.dev4/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_dask/_io.py` & `fugue-0.9.0.dev4/fugue_dask/_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 from dask import dataframe as dd
 from fsspec import AbstractFileSystem
 from triad.collections.dict import ParamDict
 from triad.collections.schema import Schema
 from triad.utils.assertion import assert_or_throw
-from triad.utils.io import join, makedirs, url_to_fs
+from triad.utils.io import isfile, join, makedirs, url_to_fs
 
 from fugue._utils.io import FileParser, _get_single_files
 from fugue_dask.dataframe import DaskDataFrame
 
 from ._utils import DASK_UTILS
 
 
@@ -96,17 +96,19 @@
     makedirs(p.path, exist_ok=True)
     df.native.to_csv(
         p.join("*.csv").path, **{"index": False, "header": False, **kwargs}
     )
 
 
 def _safe_load_csv(path: str, **kwargs: Any) -> dd.DataFrame:
+    if not isfile(path):
+        return dd.read_csv(join(path, "*.csv"), **kwargs)
     try:
         return dd.read_csv(path, **kwargs)
-    except (IsADirectoryError, PermissionError):
+    except (IsADirectoryError, PermissionError):  # pragma: no cover
         return dd.read_csv(join(path, "*.csv"), **kwargs)
 
 
 def _load_csv(  # noqa: C901
     p: FileParser, columns: Any = None, **kwargs: Any
 ) -> Tuple[dd.DataFrame, Any]:
     kw = ParamDict(kwargs)
@@ -144,19 +146,20 @@
 
 def _save_json(df: DaskDataFrame, p: FileParser, **kwargs: Any) -> None:
     makedirs(p.path, exist_ok=True)
     df.native.to_json(p.join("*.json").path, **kwargs)
 
 
 def _safe_load_json(path: str, **kwargs: Any) -> dd.DataFrame:
+    if not isfile(path):
+        return dd.read_json(join(path, "*.json"), **kwargs)
     try:
         return dd.read_json(path, **kwargs)
-    except (IsADirectoryError, PermissionError):
-        x = dd.read_json(join(path, "*.json"), **kwargs)
-        return x
+    except (IsADirectoryError, PermissionError):  # pragma: no cover
+        return dd.read_json(join(path, "*.json"), **kwargs)
 
 
 def _load_json(
     p: FileParser, columns: Any = None, **kwargs: Any
 ) -> Tuple[dd.DataFrame, Any]:
     pdf = _safe_load_json(p.path, **kwargs).reset_index(drop=True)
     if columns is None:
```

### Comparing `fugue-0.9.0.dev3/fugue_dask/_utils.py` & `fugue-0.9.0.dev4/fugue_dask/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :param cols: columns to hash, if empty, all columns will be used
 
     :return: repartitioned dataframe
     """
     if num < 1:
         return df
     if num == 1:
-        return df.repartition(1)
+        return df.repartition(npartitions=1)
     df = df.reset_index(drop=True).clear_divisions()
     idf, ct = _add_hash_index(df, num, cols)
     return _postprocess(idf, ct, num)
 
 
 def even_repartition(df: dd.DataFrame, num: int, cols: List[Any]) -> dd.DataFrame:
     """Repartition the dataframe by evenly distributing the given columns
@@ -72,15 +72,15 @@
 
         When cols is empty, the dataframe will be evenly repartitioned by ``num``.
         When cols is not empty, the dataframe will be evenly repartitioned by the
         groups of the given columns. When cols is not empty, if ``num<=0``,
         the number of partitions will be the number of groups.
     """
     if num == 1:
-        return df.repartition(1)
+        return df.repartition(npartitions=1)
     if len(cols) == 0 and num <= 0:
         return df
     df = df.reset_index(drop=True).clear_divisions()
     if len(cols) == 0:
         idf, ct = _add_continuous_index(df)
     else:
         idf, ct = _add_group_index(df, cols, shuffle=False)
@@ -107,28 +107,28 @@
         When cols is empty, the dataframe will be randomly shuffled and
         repartitioned by ``num``. When cols is not empty, the dataframe will be
         grouped and then randomly shuffled by groups.
     """
     if num < 1:
         return df
     if num == 1:
-        return df.repartition(1)
+        return df.repartition(npartitions=1)
     df = df.reset_index(drop=True).clear_divisions()
     if len(cols) == 0:
         idf, ct = _add_random_index(df, num=num, seed=seed)
     else:
         idf, ct = _add_group_index(df, cols, shuffle=True, seed=seed)
         # when cols are set and num is not set, we use the number of groups
     return _postprocess(idf, ct, num)
 
 
 def _postprocess(idf: dd.DataFrame, ct: int, num: int) -> dd.DataFrame:
     parts = min(ct, num)
     if parts <= 1:
-        return idf.repartition(1)
+        return idf.repartition(npartitions=1)
     divisions = list(np.arange(ct, step=math.ceil(ct / parts)))
     divisions.append(ct - 1)
     return idf.repartition(divisions=divisions, force=True)
 
 
 def _add_group_index(
     df: dd.DataFrame, cols: List[str], shuffle: bool, seed: Any = None
```

### Comparing `fugue-0.9.0.dev3/fugue_dask/dataframe.py` & `fugue-0.9.0.dev4/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_dask/execution_engine.py` & `fugue-0.9.0.dev4/fugue_dask/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_dask/registry.py` & `fugue-0.9.0.dev4/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_dask/tester.py` & `fugue-0.9.0.dev4/fugue_dask/tester.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/_io.py` & `fugue-0.9.0.dev4/fugue_duckdb/_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
                 query = f"SELECT * FROM read_csv_auto({pm})"
                 tdf = DuckDataFrame(self._con.from_query(query))
                 rn = dict(zip(tdf.columns, columns))
                 return tdf.rename(rn)  # type: ignore
         else:
             if header:
                 kw["ALL_VARCHAR"] = 1
+                kw["auto_detect"] = 1
                 if columns is None:
                     cols = "*"
                 elif isinstance(columns, list):
                     cols = ", ".join(encode_column_names(columns))
                 else:
                     cols = "*"
                 for k, v in kw.items():
```

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/_utils.py` & `fugue-0.9.0.dev4/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/dask.py` & `fugue-0.9.0.dev4/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/dataframe.py` & `fugue-0.9.0.dev4/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/execution_engine.py` & `fugue-0.9.0.dev4/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/registry.py` & `fugue-0.9.0.dev4/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_duckdb/tester.py` & `fugue-0.9.0.dev4/fugue_duckdb/tester.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ibis/_utils.py` & `fugue-0.9.0.dev4/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ibis/dataframe.py` & `fugue-0.9.0.dev4/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ibis/execution_engine.py` & `fugue-0.9.0.dev4/fugue_ibis/execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from fugue.dataframe.utils import get_join_schemas
 from fugue.execution.execution_engine import ExecutionEngine, MapEngine, SQLEngine
 
 from ._compat import IbisTable
 from ._utils import to_ibis_schema
 from .dataframe import IbisDataFrame
 
-_JOIN_RIGHT_SUFFIX = "_ibis_y__"
-_GEN_TABLE_NAMES = (f"_fugue_temp_table_{i:d}" for i in itertools.count())
+_JOIN_RIGHT_SUFFIX = "_ibis_y__".upper()
+_GEN_TABLE_NAMES = (f"_fugue_temp_table_{i:d}".upper() for i in itertools.count())
 
 
 class IbisSQLEngine(SQLEngine):
     """Ibis SQL backend base implementation.
 
     :param execution_engine: the execution engine this sql engine will run on
     """
@@ -220,26 +220,27 @@
             ValueError("n needs to be an integer"),
         )
 
         if presort is not None and presort != "":
             _presort = parse_presort_exp(presort)
         else:
             _presort = partition_spec.presort
-        tbn = "_temp"
+        tbn = "_TEMP"
         idf = self.to_df(df)
 
         if len(_presort) == 0:
             if len(partition_spec.partition_by) == 0:
                 return self.to_df(idf.native.head(n), schema=df.schema)
             pcols = ", ".join(
                 self.encode_column_name(x) for x in partition_spec.partition_by
             )
+            dummy_order_by = self._dummy_window_order_by()
             sql = (
                 f"SELECT * FROM ("
-                f"SELECT *, ROW_NUMBER() OVER (PARTITION BY {pcols}) "
+                f"SELECT *, ROW_NUMBER() OVER (PARTITION BY {pcols} {dummy_order_by}) "
                 f"AS __fugue_take_param FROM {tbn}"
                 f") WHERE __fugue_take_param<={n}"
             )
             tb = self.query_to_table(sql, {tbn: idf})
             return self.to_df(tb[df.columns], schema=df.schema)
 
         sorts: List[str] = []
@@ -286,14 +287,20 @@
             self.backend.create_table(
                 table, df.as_pandas(), schema=to_ibis_schema(df.schema)
             )
 
     def load_table(self, table: str, **kwargs: Any) -> DataFrame:
         return self.to_df(self.backend.table(table))
 
+    def _dummy_window_order_by(self) -> str:
+        """Return a dummy window order by clause, this is required for
+        some SQL backends when there is no real order by clause in window
+        """
+        return ""
+
 
 class IbisMapEngine(MapEngine):
     """IbisExecutionEngine's MapEngine, it is a wrapper of the map engine
     of :meth:`~.IbisExecutionEngine.non_ibis_engine`
 
     :param execution_engine: the execution engine this map engine will run on
     """
```

### Comparing `fugue-0.9.0.dev3/fugue_notebook/__init__.py` & `fugue-0.9.0.dev4/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_notebook/env.py` & `fugue-0.9.0.dev4/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_notebook/nbextension/main.js` & `fugue-0.9.0.dev4/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_polars/polars_dataframe.py` & `fugue-0.9.0.dev4/fugue_polars/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_polars/registry.py` & `fugue-0.9.0.dev4/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ray/_constants.py` & `fugue-0.9.0.dev4/fugue_ray/_constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Any, Dict
 
 import ray
+from packaging import version
 
 FUGUE_RAY_CONF_SHUFFLE_PARTITIONS = "fugue.ray.shuffle.partitions"
 FUGUE_RAY_DEFAULT_PARTITIONS = "fugue.ray.default.partitions"
 FUGUE_RAY_DEFAULT_BATCH_SIZE = "fugue.ray.default.batch_size"
 FUGUE_RAY_ZERO_COPY = "fugue.ray.zero_copy"
 
 FUGUE_RAY_DEFAULT_CONF: Dict[str, Any] = {
     FUGUE_RAY_CONF_SHUFFLE_PARTITIONS: -1,
     FUGUE_RAY_DEFAULT_PARTITIONS: 0,
     FUGUE_RAY_ZERO_COPY: True,
 }
+RAY_VERSION = version.parse(ray.__version__)
 
-if ray.__version__ >= "2.3":
-    _ZERO_COPY: Dict[str, Any] = {"zero_copy_batch": True}
-else:  # pragma: no cover
-    _ZERO_COPY = {}
+_ZERO_COPY: Dict[str, Any] = {"zero_copy_batch": True}
```

### Comparing `fugue-0.9.0.dev3/fugue_ray/_utils/cluster.py` & `fugue-0.9.0.dev4/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ray/_utils/dataframe.py` & `fugue-0.9.0.dev4/fugue_ray/_utils/dataframe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pickle
 from typing import Any, Dict, List, Optional, Tuple
 
 import pandas as pd
 import pyarrow as pa
-import ray
 import ray.data as rd
 from triad import Schema
 
 from .._constants import _ZERO_COPY
 
 _RAY_NULL_REPR = "__RAY_NULL__"
 
@@ -27,39 +26,29 @@
     return df
 
 
 def get_dataset_format(df: rd.Dataset) -> Tuple[Optional[str], rd.Dataset]:
     df = materialize(df)
     if df.count() == 0:
         return None, df
-    if ray.__version__ < "2.5.0":  # pragma: no cover
-        if hasattr(df, "_dataset_format"):  # pragma: no cover
-            return df._dataset_format(), df  # ray<2.2
-        ctx = rd.context.DatasetContext.get_current()
-        ctx.use_streaming_executor = False
-        return df.dataset_format(), df  # ray>=2.2
-    else:
-        schema = df.schema(fetch_if_missing=True)
-        if schema is None:  # pragma: no cover
-            return None, df
-        if isinstance(schema.base_schema, pa.Schema):
-            return "arrow", df
-        return "pandas", df
+    schema = df.schema(fetch_if_missing=True)
+    if schema is None:  # pragma: no cover
+        return None, df
+    if isinstance(schema.base_schema, pa.Schema):
+        return "arrow", df
+    return "pandas", df
 
 
 def to_schema(schema: Any) -> Schema:  # pragma: no cover
     if isinstance(schema, pa.Schema):
         return Schema(schema)
-    if ray.__version__ >= "2.5.0":
-        if isinstance(schema, rd.Schema):
-            if hasattr(schema, "base_schema") and isinstance(
-                schema.base_schema, pa.Schema
-            ):
-                return Schema(schema.base_schema)
-            return Schema(list(zip(schema.names, schema.types)))
+    if isinstance(schema, rd.Schema):
+        if hasattr(schema, "base_schema") and isinstance(schema.base_schema, pa.Schema):
+            return Schema(schema.base_schema)
+        return Schema(list(zip(schema.names, schema.types)))
     raise ValueError(f"{schema} is not supported")
 
 
 def build_empty(schema: Schema) -> rd.Dataset:
     return rd.from_arrow(schema.create_empty_arrow_table())
```

### Comparing `fugue-0.9.0.dev3/fugue_ray/_utils/io.py` & `fugue-0.9.0.dev4/fugue_ray/_utils/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 import pathlib
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 import pyarrow as pa
-import ray
 import ray.data as rd
+from packaging import version
 from pyarrow import csv as pacsv
 from pyarrow import json as pajson
 from ray.data.datasource import FileExtensionFilter
 from triad.collections import Schema
 from triad.collections.dict import ParamDict
 from triad.utils.assertion import assert_or_throw
-from triad.utils.io import exists, makedirs, rm
+from triad.utils.io import exists, makedirs, rm, isfile
 
 from fugue import ExecutionEngine
 from fugue._utils.io import FileParser, save_df
 from fugue.collections.partition import PartitionSpec
 from fugue.dataframe import DataFrame
 from fugue_ray.dataframe import RayDataFrame
 
+from .._constants import RAY_VERSION
+
 
 class RayIO(object):
     def __init__(self, engine: ExecutionEngine):
         self._engine = engine
         self._logger = engine.log
         self._loads: Dict[str, Callable[..., DataFrame]] = {
             "csv": self._load_csv,
@@ -145,24 +147,34 @@
         infer_schema = kw.get("infer_schema", False)
         read_options: Dict[str, Any] = {"use_threads": False}
         parse_options: Dict[str, Any] = {}
         convert_options: Dict[str, Any] = {}
         if infer_schema and columns is not None and not isinstance(columns, list):
             raise ValueError("can't set columns as a schema when infer schema is true")
 
+        if RAY_VERSION >= version.parse("2.10"):
+            if len(p) == 1 and isfile(p[0]):  # TODO: very hacky
+                params: Dict[str, Any] = {}
+            else:
+                params = {"file_extensions": ["csv"]}
+        else:  # pragma: no cover
+            params = {
+                "partition_filter": _FileFiler(
+                    file_extensions=["csv"], exclude=["_SUCCESS"]
+                ),
+            }
+
         def _read_csv(to_str: bool) -> RayDataFrame:
             res = rd.read_csv(
                 p,
                 ray_remote_args=self._remote_args(),
                 read_options=pacsv.ReadOptions(**read_options),
                 parse_options=pacsv.ParseOptions(**parse_options),
                 convert_options=pacsv.ConvertOptions(**convert_options),
-                partition_filter=_FileFiler(
-                    file_extensions=["csv"], exclude=["_SUCCESS"]
-                ),
+                **params,
             )
             if to_str:
                 _schema = res.schema(fetch_if_missing=True)
                 str_schema = Schema([(x, pa.string()) for x in _schema.names]).pa_schema
                 return RayDataFrame(res, schema=str_schema)
             else:
                 return RayDataFrame(res)
@@ -192,28 +204,39 @@
         else:  # pragma: no cover
             raise NotImplementedError(f"{header} is not supported")
 
     def _load_json(self, p: List[str], columns: Any = None, **kwargs: Any) -> DataFrame:
         read_options: Dict[str, Any] = {"use_threads": False}
         parse_options: Dict[str, Any] = {}
 
-        def _read_json() -> RayDataFrame:
-            if ray.__version__ >= "2.9":
-                params: Dict[str, Any] = {"file_extensions": None}
+        def _read_json() -> RayDataFrame:  # pragma: no cover
+            if RAY_VERSION >= version.parse("2.10"):
+                if len(p) == 1 and isfile(p[0]):  # TODO: very hacky
+                    params: Dict[str, Any] = {"file_extensions": None}
+                else:
+                    params = {"file_extensions": ["json"]}
+            elif RAY_VERSION >= version.parse("2.9"):  # pragma: no cover
+                params = {
+                    "file_extensions": None,
+                    "partition_filter": _FileFiler(
+                        file_extensions=["json"], exclude=["_SUCCESS"]
+                    ),
+                }
             else:  # pragma: no cover
-                params = {}
+                params = {
+                    "partition_filter": _FileFiler(
+                        file_extensions=["json"], exclude=["_SUCCESS"]
+                    ),
+                }
             return RayDataFrame(
                 rd.read_json(
                     p,
                     ray_remote_args=self._remote_args(),
                     read_options=pajson.ReadOptions(**read_options),
                     parse_options=pajson.ParseOptions(**parse_options),
-                    partition_filter=_FileFiler(
-                        file_extensions=["json"], exclude=["_SUCCESS"]
-                    ),
                     **params,
                 )
             )
 
         if columns is None or isinstance(columns, list):
             rdf = _read_json()
             if isinstance(columns, list):  # column names
@@ -223,15 +246,15 @@
             schema = Schema(columns)
             return _read_json()[schema.names].alter_columns(schema)
 
     def _remote_args(self) -> Dict[str, Any]:
         return {"num_cpus": 1}
 
 
-class _FileFiler(FileExtensionFilter):
+class _FileFiler(FileExtensionFilter):  # pragma: no cover
     def __init__(self, file_extensions: Union[str, List[str]], exclude: Iterable[str]):
         super().__init__(file_extensions, allow_if_no_extension=True)
         self._exclude = set(exclude)
 
     def _is_valid(self, path: str) -> bool:
         return pathlib.Path(
             path
```

### Comparing `fugue-0.9.0.dev3/fugue_ray/dataframe.py` & `fugue-0.9.0.dev4/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ray/execution_engine.py` & `fugue-0.9.0.dev4/fugue_ray/execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,15 @@
                     rdf, PartitionSpec(num=n)
                 )
         mb_args: Dict[str, Any] = {}
         if FUGUE_RAY_DEFAULT_BATCH_SIZE in self.conf:
             mb_args["batch_size"] = self.conf.get_or_throw(
                 FUGUE_RAY_DEFAULT_BATCH_SIZE, int
             )
-        if ray.__version__ >= "2.3":
-            mb_args["zero_copy_batch"] = self.conf.get(FUGUE_RAY_ZERO_COPY, True)
+        mb_args["zero_copy_batch"] = self.conf.get(FUGUE_RAY_ZERO_COPY, True)
         sdf = rdf.native.map_batches(
             _udf,
             batch_format="pyarrow",
             **mb_args,
             **self.execution_engine._get_remote_args(),  # type: ignore
         )
         return RayDataFrame(sdf, schema=output_schema, internal_schema=True)
```

### Comparing `fugue-0.9.0.dev3/fugue_ray/registry.py` & `fugue-0.9.0.dev4/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_ray/tester.py` & `fugue-0.9.0.dev4/fugue_ray/tester.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/_utils/convert.py` & `fugue-0.9.0.dev4/fugue_spark/_utils/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/_utils/io.py` & `fugue-0.9.0.dev4/fugue_spark/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/_utils/misc.py` & `fugue-0.9.0.dev4/fugue_spark/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/_utils/partition.py` & `fugue-0.9.0.dev4/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/dataframe.py` & `fugue-0.9.0.dev4/fugue_spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/execution_engine.py` & `fugue-0.9.0.dev4/fugue_spark/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/registry.py` & `fugue-0.9.0.dev4/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_spark/tester.py` & `fugue-0.9.0.dev4/fugue_spark/tester.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_test/__init__.py` & `fugue-0.9.0.dev4/fugue_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_test/bag_suite.py` & `fugue-0.9.0.dev4/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/fugue_test/builtin_suite.py` & `fugue-0.9.0.dev4/fugue_test/builtin_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     register_processor,
     register_transformer,
     transformer,
 )
 from fugue.column import col
 from fugue.column import functions as ff
 from fugue.column import lit
-from fugue.dataframe.utils import _df_eq as df_eq
 from fugue.exceptions import (
     FugueInterfacelessError,
     FugueWorkflowCompileError,
     FugueWorkflowCompileValidationError,
     FugueWorkflowError,
     FugueWorkflowRuntimeValidationError,
 )
@@ -77,15 +76,15 @@
     Whenever you add method to FugueWorkflow and WorkflowDataFrame, you should
     add correspondent tests here
     """
 
     class Tests(ft.FugueTestSuite):
         def test_workflows(self):
             a = FugueWorkflow().df([[0]], "a:int")
-            df_eq(a.compute(self.engine), [[0]], "a:int")
+            self.df_eq(a.compute(self.engine), [[0]], "a:int")
 
         def test_create_show(self):
             with FugueWorkflow() as dag:
                 dag.df([[0]], "a:int").persist().partition(num=2).show()
                 dag.df(dag.df([[0]], "a:int")).persist().broadcast().show(title="t")
             dag.run(self.engine)
 
@@ -1686,15 +1685,15 @@
                     """
                 TRANSFORM x USING tr(n=2) SCHEMA *
                 YIELD LOCAL DATAFRAME AS res
                 PRINT sdf1
                 """,
                     x=sdf3,
                 ).run()
-                df_eq(
+                self.df_eq(
                     res["res"],
                     [[3, 4, 13]],
                     schema="a:long,b:int,c:long",
                     check_schema=False,
                     throw=True,
                 )
 
@@ -1719,58 +1718,58 @@
             def tr(df: pd.DataFrame) -> pd.DataFrame:
                 return df.assign(**{"c *": 2})
 
             with fa.engine_context(self.engine):
                 df1 = pd.DataFrame([[0, 1], [2, 3]], columns=["a b", " "])
                 df2 = pd.DataFrame([[0, 10], [20, 3]], columns=["a b", "d"])
                 r = fa.inner_join(df1, df2, as_fugue=True)
-                df_eq(r, [[0, 1, 10]], "`a b`:long,` `:long,d:long", throw=True)
+                self.df_eq(r, [[0, 1, 10]], "`a b`:long,` `:long,d:long", throw=True)
                 r = fa.transform(r, tr)
-                df_eq(
+                self.df_eq(
                     r,
                     [[0, 1, 10, 2]],
                     "`a b`:long,` `:long,d:long,`c *`:long",
                     throw=True,
                 )
                 r = fa.alter_columns(r, "`c *`:str")
                 r = fa.select(
                     r,
                     col("a b").alias("a b "),
                     col(" ").alias("x y"),
                     col("d"),
                     col("c *").cast(int),
                 )
-                df_eq(
+                self.df_eq(
                     r,
                     [[0, 1, 10, 2]],
                     "`a b `:long,`x y`:long,d:long,`c *`:long",
                     throw=True,
                 )
                 r = fa.rename(r, {"a b ": "a b"})
                 fa.save(r, f_csv, header=True, force_single=True)
                 fa.save(r, f_parquet)
-                df_eq(
+                self.df_eq(
                     fa.load(f_parquet, columns=["x y", "d", "c *"], as_fugue=True),
                     [[1, 10, 2]],
                     "`x y`:long,d:long,`c *`:long",
                     throw=True,
                 )
-                df_eq(
+                self.df_eq(
                     fa.load(
                         f_csv,
                         header=True,
                         infer_schema=False,
                         columns=["d", "c *"],
                         as_fugue=True,
                     ),
                     [["10", "2"]],
                     "d:str,`c *`:str",
                     throw=True,
                 )
-                df_eq(
+                self.df_eq(
                     fa.load(
                         f_csv,
                         header=True,
                         columns="`a b`:long,`x y`:long,d:long,`c *`:long",
                         as_fugue=True,
                     ),
                     [[0, 1, 10, 2]],
@@ -1782,34 +1781,34 @@
                     """
                 df1 = CREATE [[0, 1], [2, 3]] SCHEMA `a b`:long,` `:long
                 df2 = CREATE [[0, 10], [20, 3]] SCHEMA `a b`:long,d:long
                 SELECT df1.*,d FROM df1 INNER JOIN df2 ON df1.`a b`=df2.`a b`
                 """,
                     as_fugue=True,
                 )
-                df_eq(r, [[0, 1, 10]], "`a b`:long,` `:long,d:long", throw=True)
+                self.df_eq(r, [[0, 1, 10]], "`a b`:long,` `:long,d:long", throw=True)
                 r = fa.fugue_sql(
                     """
                 TRANSFORM r USING tr SCHEMA *,`c *`:long
                 """,
                     as_fugue=True,
                 )
-                df_eq(
+                self.df_eq(
                     r,
                     [[0, 1, 10, 2]],
                     "`a b`:long,` `:long,d:long,`c *`:long",
                     throw=True,
                 )
                 r = fa.fugue_sql(
                     """
                 ALTER COLUMNS `c *`:long FROM r
                 """,
                     as_fugue=True,
                 )
-                df_eq(
+                self.df_eq(
                     r,
                     [[0, 1, 10, 2]],
                     "`a b`:long,` `:long,d:long,`c *`:long",
                     throw=True,
                 )
                 res = fa.fugue_sql_flow(
                     """
@@ -1822,27 +1821,27 @@
                 LOAD "{{f_csv}}"(header=TRUE,infer_schema=FALSE)
                 COLUMNS `a b`:long,`x y`:long,d:long,`c *`:long
                 YIELD LOCAL DATAFRAME AS r3
                 """,
                     f_parquet=f_parquet,
                     f_csv=f_csv,
                 ).run()
-                df_eq(
+                self.df_eq(
                     res["r1"],
                     [[1, 10, 2]],
                     "`x y`:long,d:long,`c *`:long",
                     throw=True,
                 )
-                df_eq(
+                self.df_eq(
                     res["r2"],
                     [["1", "10", "2"]],
                     "`x y`:str,d:str,`c *`:str",
                     throw=True,
                 )
-                df_eq(
+                self.df_eq(
                     res["r3"],
                     [[0, 1, 10, 2]],
                     "`a b`:long,`x y`:long,d:long,`c *`:long",
                     throw=True,
                 )
```

### Comparing `fugue-0.9.0.dev3/fugue_test/dataframe_suite.py` & `fugue-0.9.0.dev4/fugue_test/dataframe_suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy as np
 import pandas as pd
 from pytest import raises
 
 import fugue.api as fi
 import fugue.test as ft
 from fugue.dataframe import ArrowDataFrame, DataFrame
-from fugue.dataframe.utils import _df_eq as df_eq
 from fugue.exceptions import FugueDataFrameOperationError, FugueDatasetEmptyError
 
 
 class DataFrameTests(object):
     """DataFrame level general test suite.
     All new DataFrame types should pass this test suite.
     """
@@ -117,32 +116,32 @@
             )  # not existed
             raises(
                 FugueDataFrameOperationError, lambda: fi.select_columns(df, ["a"])
             )  # empty
             assert [[1]] == fi.as_array(df, type_safe=True)
 
             df = self.df([["a", 1, 2]], "a:str,b:int,c:int")
-            df_eq(
+            self.df_eq(
                 fi.as_fugue_df(fi.select_columns(df, ["c", "a"])),
                 [[2, "a"]],
                 "a:str,c:int",
             )
 
         def test_rename(self):
             for data in [[["a", 1]], []]:
                 df = self.df(data, "a:str,b:int")
                 df2 = fi.rename(df, columns=dict(a="aa"))
                 assert fi.get_schema(df) == "a:str,b:int"
-                df_eq(fi.as_fugue_df(df2), data, "aa:str,b:int", throw=True)
+                self.df_eq(fi.as_fugue_df(df2), data, "aa:str,b:int", throw=True)
 
             for data in [[["a", 1]], []]:
                 df = self.df(data, "a:str,b:int")
                 df3 = fi.rename(df, columns={})
                 assert fi.get_schema(df3) == "a:str,b:int"
-                df_eq(fi.as_fugue_df(df3), data, "a:str,b:int", throw=True)
+                self.df_eq(fi.as_fugue_df(df3), data, "a:str,b:int", throw=True)
 
         def test_rename_invalid(self):
             df = self.df([["a", 1]], "a:str,b:int")
             raises(
                 FugueDataFrameOperationError,
                 lambda: fi.rename(df, columns=dict(aa="ab")),
             )
```

### Comparing `fugue-0.9.0.dev3/fugue_test/execution_suite.py` & `fugue-0.9.0.dev4/fugue_test/execution_suite.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     ArrayDataFrame,
     DataFrame,
     DataFrames,
     PandasDataFrame,
     PartitionSpec,
 )
 from fugue.column import all_cols, col, lit
-from fugue.dataframe.utils import _df_eq as df_eq
 from fugue.execution.native_execution_engine import NativeExecutionEngine
 
 
 class ExecutionEngineTests(object):
     """ExecutionEngine level general test suite.
     Any new :class:`~fugue.execution.execution_engine.ExecutionEngine`
     should pass this test suite.
@@ -52,119 +51,119 @@
             e = self.engine
             o = ArrayDataFrame(
                 [[1.1, 2.2], [3.3, 4.4]],
                 "a:double,b:double",
             )
             # all engines should accept these types of inputs
             # should take fugue.DataFrame
-            df_eq(o, fa.as_fugue_engine_df(e, o), throw=True)
+            self.df_eq(o, fa.as_fugue_engine_df(e, o), throw=True)
             # should take array, shema
-            df_eq(
+            self.df_eq(
                 o,
                 fa.as_fugue_engine_df(e, [[1.1, 2.2], [3.3, 4.4]], "a:double,b:double"),
                 throw=True,
             )
             # should take pandas dataframe
             pdf = pd.DataFrame([[1.1, 2.2], [3.3, 4.4]], columns=["a", "b"])
-            df_eq(o, fa.as_fugue_engine_df(e, pdf), throw=True)
+            self.df_eq(o, fa.as_fugue_engine_df(e, pdf), throw=True)
 
             # should convert string to datetime in to_df
-            df_eq(
+            self.df_eq(
                 fa.as_fugue_engine_df(e, [["2020-01-01"]], "a:datetime"),
                 [[datetime(2020, 1, 1)]],
                 "a:datetime",
                 throw=True,
             )
 
             # should handle empty pandas dataframe
             o = ArrayDataFrame([], "a:double,b:str")
             pdf = pd.DataFrame([[0.1, "a"]], columns=["a", "b"])
             pdf = pdf[pdf.a < 0]
-            df_eq(o, fa.as_fugue_engine_df(e, pdf), throw=True)
+            self.df_eq(o, fa.as_fugue_engine_df(e, pdf), throw=True)
 
         @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_filter(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]],
                 "a:double,b:int",
             )
             b = fa.filter(a, col("a").not_null())
-            df_eq(b, [[1, 2], [3, 4]], "a:double,b:int", throw=True)
+            self.df_eq(b, [[1, 2], [3, 4]], "a:double,b:int", throw=True)
             c = fa.filter(a, col("a").not_null() & (col("b") < 3))
-            df_eq(c, [[1, 2]], "a:double,b:int", throw=True)
+            self.df_eq(c, [[1, 2]], "a:double,b:int", throw=True)
             c = fa.filter(a, col("a") + col("b") == 3)
-            df_eq(c, [[1, 2]], "a:double,b:int", throw=True)
+            self.df_eq(c, [[1, 2]], "a:double,b:int", throw=True)
 
         @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_select(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]], "a:double,b:int"
             )
 
             # simple
             b = fa.select(a, col("b"), (col("b") + 1).alias("c").cast(str))
-            df_eq(
+            self.df_eq(
                 b,
                 [[2, "3"], [2, "3"], [1, "2"], [4, "5"], [4, "5"]],
                 "b:int,c:str",
                 throw=True,
             )
 
             # with distinct
             b = fa.select(
                 a, col("b"), (col("b") + 1).alias("c").cast(str), distinct=True
             )
-            df_eq(
+            self.df_eq(
                 b,
                 [[2, "3"], [1, "2"], [4, "5"]],
                 "b:int,c:str",
                 throw=True,
             )
 
             # wildcard
             b = fa.select(a, all_cols(), where=col("a") + col("b") == 3)
-            df_eq(b, [[1, 2]], "a:double,b:int", throw=True)
+            self.df_eq(b, [[1, 2]], "a:double,b:int", throw=True)
 
             # aggregation
             b = fa.select(a, col("a"), ff.sum(col("b")).cast(float).alias("b"))
-            df_eq(b, [[1, 2], [3, 4], [None, 7]], "a:double,b:double", throw=True)
+            self.df_eq(b, [[1, 2], [3, 4], [None, 7]], "a:double,b:double", throw=True)
 
             # having
             # https://github.com/fugue-project/fugue/issues/222
             col_b = ff.sum(col("b"))
             b = fa.select(
                 a,
                 col("a"),
                 col_b.cast(float).alias("c"),
                 having=(col_b >= 7) | (col("a") == 1),
             )
-            df_eq(b, [[1, 2], [None, 7]], "a:double,c:double", throw=True)
+            self.df_eq(b, [[1, 2], [None, 7]], "a:double,c:double", throw=True)
 
             # literal + alias inference
             # https://github.com/fugue-project/fugue/issues/222
             col_b = ff.sum(col("b"))
             b = fa.select(
                 a,
                 col("a"),
                 lit(1, "o").cast(str),
                 col_b.cast(float).alias("c"),
                 having=(col_b >= 7) | (col("a") == 1),
             )
-            df_eq(
+            self.df_eq(
                 b, [[1, "1", 2], [None, "1", 7]], "a:double,o:str,c:double", throw=True
             )
 
         @pytest.mark.skipif(not HAS_QPD, reason="qpd not working")
         def test_assign(self):
             a = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]], "a:double,b:int"
             )
 
             b = fa.assign(a, x=1, b=col("b").cast(str), c=(col("b") + 1).cast(int))
-            df_eq(
+            self.df_eq(
                 b,
                 [
                     [1, "2", 1, 3],
                     [None, "2", 1, 3],
                     [None, "1", 1, 2],
                     [3, "4", 1, 5],
                     [None, "4", 1, 5],
@@ -180,23 +179,23 @@
             )
 
             b = fa.aggregate(
                 df=a,
                 b=ff.max(col("b")),
                 c=(ff.max(col("b")) * 2).cast("int32").alias("c"),
             )
-            df_eq(b, [[4, 8]], "b:int,c:int", throw=True)
+            self.df_eq(b, [[4, 8]], "b:int,c:int", throw=True)
 
             b = fa.aggregate(
                 a,
                 "a",
                 b=ff.max(col("b")),
                 c=(ff.max(col("b")) * 2).cast("int32").alias("c"),
             )
-            df_eq(
+            self.df_eq(
                 b,
                 [[None, 4, 8], [1, 2, 4], [3, 4, 8]],
                 "a:double,b:int,c:int",
                 throw=True,
             )
 
             with raises(ValueError):
@@ -217,47 +216,47 @@
             e = self.engine
             o = ArrayDataFrame(
                 [[1, 2], [None, 2], [None, 1], [3, 4], [None, 4]], "a:double,b:int"
             )
             a = fa.as_fugue_engine_df(e, o)
             # no partition
             c = e.map_engine.map_dataframe(a, noop, a.schema, PartitionSpec())
-            df_eq(c, o, throw=True)
+            self.df_eq(c, o, throw=True)
             # with key partition
             c = e.map_engine.map_dataframe(
                 a, noop, a.schema, PartitionSpec(by=["a"], presort="b")
             )
-            df_eq(c, o, throw=True)
+            self.df_eq(c, o, throw=True)
             # select top
             c = e.map_engine.map_dataframe(
                 a, select_top, a.schema, PartitionSpec(by=["a"], presort="b")
             )
-            df_eq(c, [[None, 1], [1, 2], [3, 4]], "a:double,b:int", throw=True)
+            self.df_eq(c, [[None, 1], [1, 2], [3, 4]], "a:double,b:int", throw=True)
             # select top with another order
             c = e.map_engine.map_dataframe(
                 a,
                 select_top,
                 a.schema,
                 PartitionSpec(partition_by=["a"], presort="b DESC"),
             )
-            df_eq(
+            self.df_eq(
                 c,
                 [[None, 4], [1, 2], [3, 4]],
                 "a:double,b:int",
                 throw=True,
             )
             # add num_partitions, on_init should not matter
             c = e.map_engine.map_dataframe(
                 a,
                 select_top,
                 a.schema,
                 PartitionSpec(partition_by=["a"], presort="b DESC", num_partitions=3),
                 on_init=on_init,
             )
-            df_eq(c, [[None, 4], [1, 2], [3, 4]], "a:double,b:int", throw=True)
+            self.df_eq(c, [[None, 4], [1, 2], [3, 4]], "a:double,b:int", throw=True)
 
         def test_map_with_special_values(self):
             def with_nat(cursor, data):
                 df = data.as_pandas()
                 df["nat"] = pd.NaT
                 schema = data.schema + "nat:datetime"
                 return PandasDataFrame(df, schema)
@@ -266,15 +265,15 @@
             # test with multiple key with null values
             o = ArrayDataFrame(
                 [[1, None, 1], [1, None, 0], [None, None, 2]], "a:double,b:double,c:int"
             )
             c = e.map_engine.map_dataframe(
                 o, select_top, o.schema, PartitionSpec(by=["a", "b"], presort="c")
             )
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, None, 0], [None, None, 2]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             # test datetime with nat
             dt = datetime.now()
@@ -287,69 +286,69 @@
                     [None, 4, None],
                 ],
                 "a:datetime,b:int,c:double",
             )
             c = e.map_engine.map_dataframe(
                 o, select_top, o.schema, PartitionSpec(by=["a", "c"], presort="b DESC")
             )
-            df_eq(
+            self.df_eq(
                 c,
                 [[None, 4, None], [dt, 5, 1]],
                 "a:datetime,b:int,c:double",
                 throw=True,
             )
             d = e.map_engine.map_dataframe(
                 c, with_nat, "a:datetime,b:int,c:double,nat:datetime", PartitionSpec()
             )
-            df_eq(
+            self.df_eq(
                 d,
                 [[None, 4, None, None], [dt, 5, 1, None]],
                 "a:datetime,b:int,c:double,nat:datetime",
                 throw=True,
             )
             # test list
             o = ArrayDataFrame([[dt, [1, 2]]], "a:datetime,b:[int]")
             c = e.map_engine.map_dataframe(
                 o, select_top, o.schema, PartitionSpec(by=["a"])
             )
-            df_eq(c, o, check_order=True, throw=True)
+            self.df_eq(c, o, check_order=True, throw=True)
 
         def test_map_with_dict_col(self):
             e = self.engine
             dt = datetime.now()
             # test dict
             o = PandasDataFrame([[dt, dict(a=1)]], "a:datetime,b:{a:long}")
             c = e.map_engine.map_dataframe(
                 o, select_top, o.schema, PartitionSpec(by=["a"])
             )
-            df_eq(c, o, no_pandas=True, check_order=True, throw=True)
+            self.df_eq(c, o, no_pandas=True, check_order=True, throw=True)
 
             # input has dict, output doesn't
             def mp2(cursor, data):
                 return data[["a"]]
 
             c = e.map_engine.map_dataframe(
                 o, mp2, "a:datetime", PartitionSpec(by=["a"])
             )
-            df_eq(
+            self.df_eq(
                 c,
                 PandasDataFrame([[dt]], "a:datetime"),
                 no_pandas=True,
                 check_order=True,
                 throw=True,
             )
 
             # input doesn't have dict, output has
             def mp3(cursor, data):
                 return PandasDataFrame([[dt, dict(a=1)]], "a:datetime,b:{a:long}")
 
             c = e.map_engine.map_dataframe(
                 c, mp3, "a:datetime,b:{a:long}", PartitionSpec(by=["a"])
             )
-            df_eq(c, o, no_pandas=True, check_order=True, throw=True)
+            self.df_eq(c, o, no_pandas=True, check_order=True, throw=True)
 
         def test_map_with_binary(self):
             e = self.engine
             o = ArrayDataFrame(
                 [[pickle.dumps(BinaryObject("a"))], [pickle.dumps(BinaryObject("b"))]],
                 "a:bytes",
             )
@@ -357,211 +356,219 @@
             expected = ArrayDataFrame(
                 [
                     [pickle.dumps(BinaryObject("ax"))],
                     [pickle.dumps(BinaryObject("bx"))],
                 ],
                 "a:bytes",
             )
-            df_eq(expected, c, no_pandas=True, check_order=True, throw=True)
+            self.df_eq(expected, c, no_pandas=True, check_order=False, throw=True)
 
         def test_join_multiple(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[1, 20], [3, 40]], "a:int,c:int")
             c = fa.as_fugue_engine_df(e, [[1, 200], [3, 400]], "a:int,d:int")
             d = fa.inner_join(a, b, c)
-            df_eq(
+            self.df_eq(
                 d,
                 [[1, 2, 20, 200], [3, 4, 40, 400]],
                 "a:int,b:int,c:int,d:int",
                 throw=True,
             )
 
         def test__join_cross(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6], [7]], "c:int")
             c = fa.join(a, b, how="Cross")
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, 2, 6], [1, 2, 7], [3, 4, 6], [3, 4, 7]],
                 "a:int,b:int,c:int",
                 throw=True,
             )
 
             b = fa.as_fugue_engine_df(e, [], "c:int")
             c = fa.cross_join(a, b)
-            df_eq(c, [], "a:int,b:int,c:int", throw=True)
+            self.df_eq(c, [], "a:int,b:int,c:int", throw=True)
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [], "c:int")
             c = fa.join(a, b, how="Cross")
-            df_eq(c, [], "a:int,b:int,c:int", throw=True)
+            self.df_eq(c, [], "a:int,b:int,c:int", throw=True)
 
         def test__join_inner(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             c = fa.join(a, b, how="INNER", on=["a"])
-            df_eq(c, [[1, 2, 6]], "a:int,b:int,c:int", throw=True)
+            self.df_eq(c, [[1, 2, 6]], "a:int,b:int,c:int", throw=True)
             c = fa.inner_join(b, a)
-            df_eq(c, [[6, 1, 2]], "c:int,a:int,b:int", throw=True)
+            self.df_eq(c, [[6, 1, 2]], "c:int,a:int,b:int", throw=True)
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [], "c:int,a:int")
             c = fa.join(a, b, how="INNER", on=["a"])
-            df_eq(c, [], "a:int,b:int,c:int", throw=True)
+            self.df_eq(c, [], "a:int,b:int,c:int", throw=True)
 
         def test__join_outer(self):
             e = self.engine
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [], "c:str,a:int")
             c = fa.left_outer_join(a, b)
-            df_eq(c, [], "a:int,b:int,c:str", throw=True)
+            self.df_eq(c, [], "a:int,b:int,c:str", throw=True)
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [], "c:int,a:int")
             c = fa.right_outer_join(a, b)
-            df_eq(c, [], "a:int,b:str,c:int", throw=True)
+            self.df_eq(c, [], "a:int,b:str,c:int", throw=True)
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [], "c:str,a:int")
             c = fa.full_outer_join(a, b)
-            df_eq(c, [], "a:int,b:str,c:str", throw=True)
+            self.df_eq(c, [], "a:int,b:str,c:str", throw=True)
 
             a = fa.as_fugue_engine_df(e, [[1, "2"], [3, "4"]], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [["6", 1], ["2", 7]], "c:str,a:int")
             c = fa.join(a, b, how="left_OUTER", on=["a"])
-            df_eq(c, [[1, "2", "6"], [3, "4", None]], "a:int,b:str,c:str", throw=True)
+            self.df_eq(
+                c, [[1, "2", "6"], [3, "4", None]], "a:int,b:str,c:str", throw=True
+            )
             c = fa.join(b, a, how="left_outer", on=["a"])
-            df_eq(c, [["6", 1, "2"], ["2", 7, None]], "c:str,a:int,b:str", throw=True)
+            self.df_eq(
+                c, [["6", 1, "2"], ["2", 7, None]], "c:str,a:int,b:str", throw=True
+            )
 
             a = fa.as_fugue_engine_df(e, [[1, "2"], [3, "4"]], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:double,a:int")
             c = fa.join(a, b, how="left_OUTER", on=["a"])
-            df_eq(
+            self.df_eq(
                 c, [[1, "2", 6.0], [3, "4", None]], "a:int,b:str,c:double", throw=True
             )
             c = fa.join(b, a, how="left_outer", on=["a"])
             # assert c.as_pandas().values.tolist()[1][2] is None
-            df_eq(
+            self.df_eq(
                 c, [[6.0, 1, "2"], [2.0, 7, None]], "c:double,a:int,b:str", throw=True
             )
 
             a = fa.as_fugue_engine_df(e, [[1, "2"], [3, "4"]], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [["6", 1], ["2", 7]], "c:str,a:int")
             c = fa.join(a, b, how="right_outer", on=["a"])
             # assert c.as_pandas().values.tolist()[1][1] is None
-            df_eq(c, [[1, "2", "6"], [7, None, "2"]], "a:int,b:str,c:str", throw=True)
+            self.df_eq(
+                c, [[1, "2", "6"], [7, None, "2"]], "a:int,b:str,c:str", throw=True
+            )
 
             c = fa.join(a, b, how="full_outer", on=["a"])
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, "2", "6"], [3, "4", None], [7, None, "2"]],
                 "a:int,b:str,c:str",
                 throw=True,
             )
 
         def test__join_outer_pandas_incompatible(self):
             e = self.engine
 
             a = fa.as_fugue_engine_df(e, [[1, "2"], [3, "4"]], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             c = fa.join(a, b, how="left_OUTER", on=["a"])
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, "2", 6], [3, "4", None]],
                 "a:int,b:str,c:int",
                 throw=True,
             )
             c = fa.join(b, a, how="left_outer", on=["a"])
-            df_eq(c, [[6, 1, "2"], [2, 7, None]], "c:int,a:int,b:str", throw=True)
+            self.df_eq(c, [[6, 1, "2"], [2, 7, None]], "c:int,a:int,b:str", throw=True)
 
             a = fa.as_fugue_engine_df(e, [[1, "2"], [3, "4"]], "a:int,b:str")
             b = fa.as_fugue_engine_df(e, [[True, 1], [False, 7]], "c:bool,a:int")
             c = fa.join(a, b, how="left_OUTER", on=["a"])
-            df_eq(c, [[1, "2", True], [3, "4", None]], "a:int,b:str,c:bool", throw=True)
+            self.df_eq(
+                c, [[1, "2", True], [3, "4", None]], "a:int,b:str,c:bool", throw=True
+            )
             c = fa.join(b, a, how="left_outer", on=["a"])
-            df_eq(
+            self.df_eq(
                 c, [[True, 1, "2"], [False, 7, None]], "c:bool,a:int,b:str", throw=True
             )
 
         def test__join_semi(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             c = fa.join(a, b, how="semi", on=["a"])
-            df_eq(c, [[1, 2]], "a:int,b:int", throw=True)
+            self.df_eq(c, [[1, 2]], "a:int,b:int", throw=True)
             c = fa.semi_join(b, a)
-            df_eq(c, [[6, 1]], "c:int,a:int", throw=True)
+            self.df_eq(c, [[6, 1]], "c:int,a:int", throw=True)
 
             b = fa.as_fugue_engine_df(e, [], "c:int,a:int")
             c = fa.join(a, b, how="semi", on=["a"])
-            df_eq(c, [], "a:int,b:int", throw=True)
+            self.df_eq(c, [], "a:int,b:int", throw=True)
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [], "c:int,a:int")
             c = fa.join(a, b, how="semi", on=["a"])
-            df_eq(c, [], "a:int,b:int", throw=True)
+            self.df_eq(c, [], "a:int,b:int", throw=True)
 
         def test__join_anti(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             c = fa.join(a, b, how="anti", on=["a"])
-            df_eq(c, [[3, 4]], "a:int,b:int", throw=True)
+            self.df_eq(c, [[3, 4]], "a:int,b:int", throw=True)
             c = fa.anti_join(b, a)
-            df_eq(c, [[2, 7]], "c:int,a:int", throw=True)
+            self.df_eq(c, [[2, 7]], "c:int,a:int", throw=True)
 
             b = fa.as_fugue_engine_df(e, [], "c:int,a:int")
             c = fa.join(a, b, how="anti", on=["a"])
-            df_eq(c, [[1, 2], [3, 4]], "a:int,b:int", throw=True)
+            self.df_eq(c, [[1, 2], [3, 4]], "a:int,b:int", throw=True)
 
             a = fa.as_fugue_engine_df(e, [], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [], "c:int,a:int")
             c = fa.join(a, b, how="anti", on=["a"])
-            df_eq(c, [], "a:int,b:int", throw=True)
+            self.df_eq(c, [], "a:int,b:int", throw=True)
 
         def test__join_with_null_keys(self):
             # SQL will not match null values
             e = self.engine
             a = fa.as_fugue_engine_df(
                 e, [[1, 2, 3], [4, None, 6]], "a:double,b:double,c:int"
             )
             b = fa.as_fugue_engine_df(
                 e, [[1, 2, 33], [4, None, 63]], "a:double,b:double,d:int"
             )
             c = fa.join(a, b, how="INNER")
-            df_eq(c, [[1, 2, 3, 33]], "a:double,b:double,c:int,d:int", throw=True)
+            self.df_eq(c, [[1, 2, 3, 33]], "a:double,b:double,c:int,d:int", throw=True)
 
         def test_union(self):
             e = self.engine
             a = fa.as_fugue_engine_df(
                 e, [[1, 2, 3], [4, None, 6]], "a:double,b:double,c:int"
             )
             b = fa.as_fugue_engine_df(
                 e, [[1, 2, 33], [4, None, 6]], "a:double,b:double,c:int"
             )
             c = fa.union(a, b)
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, 2, 3], [4, None, 6], [1, 2, 33]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             c = fa.union(a, b, distinct=False)
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, 2, 3], [4, None, 6], [1, 2, 33], [4, None, 6]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             d = fa.union(a, b, c, distinct=False)
-            df_eq(
+            self.df_eq(
                 d,
                 [
                     [1, 2, 3],
                     [4, None, 6],
                     [1, 2, 33],
                     [4, None, 6],
                     [1, 2, 3],
@@ -578,32 +585,32 @@
             a = fa.as_fugue_engine_df(
                 e, [[1, 2, 3], [1, 2, 3], [4, None, 6]], "a:double,b:double,c:int"
             )
             b = fa.as_fugue_engine_df(
                 e, [[1, 2, 33], [4, None, 6]], "a:double,b:double,c:int"
             )
             c = fa.subtract(a, b)
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, 2, 3]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             x = fa.as_fugue_engine_df(e, [[1, 2, 33]], "a:double,b:double,c:int")
             y = fa.as_fugue_engine_df(e, [[4, None, 6]], "a:double,b:double,c:int")
             z = fa.subtract(a, x, y)
-            df_eq(
+            self.df_eq(
                 z,
                 [[1, 2, 3]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             # TODO: EXCEPT ALL is not implemented (QPD issue)
             # c = fa.subtract(a, b, distinct=False)
-            # df_eq(
+            # self.df_eq(
             #     c,
             #     [[1, 2, 3], [1, 2, 3]],
             #     "a:double,b:double,c:int",
             #     throw=True,
             # )
 
         def test_intersect(self):
@@ -613,15 +620,15 @@
             )
             b = fa.as_fugue_engine_df(
                 e,
                 [[1, 2, 33], [4, None, 6], [4, None, 6], [4, None, 6]],
                 "a:double,b:double,c:int",
             )
             c = fa.intersect(a, b)
-            df_eq(
+            self.df_eq(
                 c,
                 [[4, None, 6]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             x = fa.as_fugue_engine_df(
                 e,
@@ -630,36 +637,36 @@
             )
             y = fa.as_fugue_engine_df(
                 e,
                 [[4, None, 6], [4, None, 6], [4, None, 6]],
                 "a:double,b:double,c:int",
             )
             z = fa.intersect(a, x, y)
-            df_eq(
+            self.df_eq(
                 z,
                 [],
                 "a:double,b:double,c:int",
                 throw=True,
             )
             # TODO: INTERSECT ALL is not implemented (QPD issue)
             # c = fa.intersect(a, b, distinct=False)
-            # df_eq(
+            # self.df_eq(
             #     c,
             #     [[4, None, 6], [4, None, 6]],
             #     "a:double,b:double,c:int",
             #     throw=True,
             # )
 
         def test_distinct(self):
             e = self.engine
             a = fa.as_fugue_engine_df(
                 e, [[4, None, 6], [1, 2, 3], [4, None, 6]], "a:double,b:double,c:int"
             )
             c = fa.distinct(a)
-            df_eq(
+            self.df_eq(
                 c,
                 [[4, None, 6], [1, 2, 3]],
                 "a:double,b:double,c:int",
                 throw=True,
             )
 
         def test_dropna(self):
@@ -670,33 +677,33 @@
                 "a:double,b:double,c:double",
             )
             c = fa.dropna(a)  # default
             d = fa.dropna(a, how="all")
             f = fa.dropna(a, how="any", thresh=2)
             g = fa.dropna(a, how="any", subset=["a", "c"])
             h = fa.dropna(a, how="any", thresh=1, subset=["a", "c"])
-            df_eq(
+            self.df_eq(
                 c,
                 [[1, 2, 3]],
                 "a:double,b:double,c:double",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 d,
                 [[4, None, 6], [1, 2, 3], [4, None, None]],
                 "a:double,b:double,c:double",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 f, [[4, None, 6], [1, 2, 3]], "a:double,b:double,c:double", throw=True
             )
-            df_eq(
+            self.df_eq(
                 g, [[4, None, 6], [1, 2, 3]], "a:double,b:double,c:double", throw=True
             )
-            df_eq(
+            self.df_eq(
                 h,
                 [[4, None, 6], [1, 2, 3], [4, None, None]],
                 "a:double,b:double,c:double",
                 throw=True,
             )
 
         def test_fillna(self):
@@ -706,33 +713,33 @@
                 [[4, None, 6], [1, 2, 3], [4, None, None]],
                 "a:double,b:double,c:double",
             )
             c = fa.fillna(a, value=1)
             d = fa.fillna(a, {"b": 99, "c": -99})
             f = fa.fillna(a, value=-99, subset=["c"])
             g = fa.fillna(a, {"b": 99, "c": -99}, subset=["c"])  # subset ignored
-            df_eq(
+            self.df_eq(
                 c,
                 [[4, 1, 6], [1, 2, 3], [4, 1, 1]],
                 "a:double,b:double,c:double",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 d,
                 [[4, 99, 6], [1, 2, 3], [4, 99, -99]],
                 "a:double,b:double,c:double",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 f,
                 [[4, None, 6], [1, 2, 3], [4, None, -99]],
                 "a:double,b:double,c:double",
                 throw=True,
             )
-            df_eq(g, d, throw=True)
+            self.df_eq(g, d, throw=True)
             raises(ValueError, lambda: fa.fillna(a, {"b": None, c: "99"}))
             raises(ValueError, lambda: fa.fillna(a, None))
             # raises(ValueError, lambda: fa.fillna(a, ["b"]))
 
         def test_sample(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[x] for x in range(100)], "a:int")
@@ -743,17 +750,17 @@
                 fa.sample(a, n=90, frac=0.9)  # can't set both
 
             f = fa.sample(a, frac=0.8, replace=False)
             g = fa.sample(a, frac=0.8, replace=True)
             h = fa.sample(a, frac=0.8, seed=1)
             h2 = fa.sample(a, frac=0.8, seed=1)
             i = fa.sample(a, frac=0.8, seed=2)
-            assert not df_eq(f, g, throw=False)
-            df_eq(h, h2, throw=True)
-            assert not df_eq(h, i, throw=False)
+            assert not self.df_eq(f, g, throw=False)
+            self.df_eq(h, h2, throw=True)
+            assert not self.df_eq(h, i, throw=False)
             assert abs(len(i.as_array()) - 80) < 10
 
         def test_take(self):
             e = self.engine
             ps = dict(by=["a"], presort="b DESC,c DESC")
             ps2 = dict(by=["c"], presort="b ASC")
             a = fa.as_fugue_engine_df(
@@ -770,45 +777,45 @@
             )
             b = fa.take(a, n=1, presort="b desc")
             c = fa.take(a, n=2, presort="a desc", na_position="first")
             d = fa.take(a, n=1, presort="a asc, b desc", partition=ps)
             f = fa.take(a, n=1, presort=None, partition=ps2)
             g = fa.take(a, n=2, presort="a desc", na_position="last")
             h = fa.take(a, n=2, presort="a", na_position="first")
-            df_eq(
+            self.df_eq(
                 b,
                 [[None, 4, 2]],
                 "a:str,b:int,c:long",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 c,
                 [[None, 4, 2], [None, 2, 1]],
                 "a:str,b:int,c:long",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 d,
                 [["a", 3, 4], ["b", 2, 2], [None, 4, 2]],
                 "a:str,b:int,c:long",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 f,
                 [["a", 2, 3], ["a", 3, 4], ["b", 1, 2], [None, 2, 1]],
                 "a:str,b:int,c:long",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 g,
                 [["b", 1, 2], ["b", 2, 2]],
                 "a:str,b:int,c:long",
                 throw=True,
             )
-            df_eq(
+            self.df_eq(
                 h,
                 [
                     [None, 4, 2],
                     [None, 2, 1],
                 ],
                 "a:str,b:int,c:long",
                 throw=True,
@@ -819,35 +826,35 @@
                     ["a", 2, 3],
                     [None, 4, 2],
                     [None, 2, 1],
                 ],
                 "a:str,b:int,c:long",
             )
             i = fa.take(a, n=1, partition="a", presort=None)
-            case1 = df_eq(
+            case1 = self.df_eq(
                 i,
                 [
                     ["a", 2, 3],
                     [None, 4, 2],
                 ],
                 "a:str,b:int,c:long",
                 throw=False,
             )
-            case2 = df_eq(
+            case2 = self.df_eq(
                 i,
                 [
                     ["a", 2, 3],
                     [None, 2, 1],
                 ],
                 "a:str,b:int,c:long",
                 throw=False,
             )
             assert case1 or case2
             j = fa.take(a, n=2, partition="a", presort=None)
-            df_eq(
+            self.df_eq(
                 j,
                 [
                     ["a", 2, 3],
                     [None, 4, 2],
                     [None, 2, 1],
                 ],
                 "a:str,b:int,c:long",
@@ -860,17 +867,17 @@
             a = fa.as_fugue_engine_df(e, [[x] for x in range(100)], "a:int")
 
             b = fa.sample(a, n=90, replace=False)
             c = fa.sample(a, n=90, replace=True)
             d = fa.sample(a, n=90, seed=1)
             d2 = fa.sample(a, n=90, seed=1)
             e = fa.sample(a, n=90, seed=2)
-            assert not df_eq(b, c, throw=False)
-            df_eq(d, d2, throw=True)
-            assert not df_eq(d, e, throw=False)
+            assert not self.df_eq(b, c, throw=False)
+            self.df_eq(d, d2, throw=True)
+            assert not self.df_eq(d, e, throw=False)
             assert abs(len(e.as_array()) - 90) < 2
 
         def test_comap(self):
             ps = PartitionSpec(presort="b,c")
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4], [1, 5]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
@@ -918,38 +925,38 @@
             res = e.comap(
                 z1,
                 comap,
                 "a:int,v:str",
                 PartitionSpec(),
                 on_init=on_init,
             )
-            df_eq(res, [[1, "_02,_11"]], "a:int,v:str", throw=True)
+            self.df_eq(res, [[1, "_02,_11"]], "a:int,v:str", throw=True)
 
             # for outer joins, the NULL will be filled with empty dataframe
             res = e.comap(z2, comap, "a:int,v:str", PartitionSpec())
-            df_eq(
+            self.df_eq(
                 res,
                 [[1, "_02,_11"], [3, "_01,_10"]],
                 "a:int,v:str",
                 throw=True,
             )
 
             res = e.comap(z3, comap, "a:int,v:str", PartitionSpec())
-            df_eq(
+            self.df_eq(
                 res,
                 [[1, "_01,_12"], [3, "_00,_11"]],
                 "a:int,v:str",
                 throw=True,
             )
 
             res = e.comap(z4, comap, "v:str", PartitionSpec())
-            df_eq(res, [["_03,_12"]], "v:str", throw=True)
+            self.df_eq(res, [["_03,_12"]], "v:str", throw=True)
 
             res = e.comap(z5, comap, "a:int,v:str", PartitionSpec())
-            df_eq(
+            self.df_eq(
                 res,
                 [[1, "_02,_11"], [3, "_01,_10"], [7, "_00,_11"]],
                 "a:int,v:str",
                 throw=True,
             )
 
         def test_comap_with_key(self):
@@ -979,102 +986,102 @@
             res = e.comap(
                 z1,
                 comap,
                 "a:int,v:str",
                 PartitionSpec(),
                 on_init=on_init,
             )
-            df_eq(res, [[1, "x2,y1"]], "a:int,v:str", throw=True)
+            self.df_eq(res, [[1, "x2,y1"]], "a:int,v:str", throw=True)
 
             res = e.comap(
                 z2,
                 comap,
                 "a:int,v:str",
                 PartitionSpec(),
                 on_init=on_init,
             )
-            df_eq(res, [[1, "x2,y1,z1"]], "a:int,v:str", throw=True)
+            self.df_eq(res, [[1, "x2,y1,z1"]], "a:int,v:str", throw=True)
 
             res = e.comap(
                 z3,
                 comap,
                 "a:int,v:str",
                 PartitionSpec(),
                 on_init=on_init,
             )
-            df_eq(res, [[1, "z1"]], "a:int,v:str", throw=True)
+            self.df_eq(res, [[1, "z1"]], "a:int,v:str", throw=True)
 
         @pytest.fixture(autouse=True)
         def init_tmpdir(self, tmpdir):
             self.tmpdir = tmpdir
 
         def test_save_single_and_load_parquet(self):
             b = ArrayDataFrame([[6, 1], [2, 7]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             makedirs(path, exist_ok=True)
             # over write folder with single file
             fa.save(b, path, format_hint="parquet", force_single=True)
             assert isfile(path)
             c = fa.load(path, format_hint="parquet", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2]], "a:long,c:int", throw=True)
+            self.df_eq(c, [[1, 6], [7, 2]], "a:long,c:int", throw=True)
 
             # overwirte single with folder (if applicable)
             b = ArrayDataFrame([[60, 1], [20, 7]], "c:int,a:long")
             fa.save(b, path, format_hint="parquet", mode="overwrite")
             c = fa.load(path, format_hint="parquet", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 60], [7, 20]], "a:long,c:int", throw=True)
+            self.df_eq(c, [[1, 60], [7, 20]], "a:long,c:int", throw=True)
 
         def test_save_and_load_parquet(self):
             b = ArrayDataFrame([[6, 1], [2, 7]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             fa.save(b, path, format_hint="parquet")
             c = fa.load(path, format_hint="parquet", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2]], "a:long,c:int", throw=True)
+            self.df_eq(c, [[1, 6], [7, 2]], "a:long,c:int", throw=True)
 
         def test_load_parquet_folder(self):
             native = NativeExecutionEngine()
             a = ArrayDataFrame([[6, 1]], "c:int,a:long")
             b = ArrayDataFrame([[2, 7], [4, 8]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             fa.save(a, os.path.join(path, "a.parquet"), engine=native)
             fa.save(b, os.path.join(path, "b.parquet"), engine=native)
             touch(os.path.join(path, "_SUCCESS"))
             c = fa.load(path, format_hint="parquet", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2], [8, 4]], "a:long,c:int", throw=True)
+            self.df_eq(c, [[1, 6], [7, 2], [8, 4]], "a:long,c:int", throw=True)
 
         def test_load_parquet_files(self):
             native = NativeExecutionEngine()
             a = ArrayDataFrame([[6, 1]], "c:int,a:long")
             b = ArrayDataFrame([[2, 7], [4, 8]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             f1 = os.path.join(path, "a.parquet")
             f2 = os.path.join(path, "b.parquet")
             fa.save(a, f1, engine=native)
             fa.save(b, f2, engine=native)
             c = fa.load(
                 [f1, f2], format_hint="parquet", columns=["a", "c"], as_fugue=True
             )
-            df_eq(c, [[1, 6], [7, 2], [8, 4]], "a:long,c:int", throw=True)
+            self.df_eq(c, [[1, 6], [7, 2], [8, 4]], "a:long,c:int", throw=True)
 
         def test_save_single_and_load_csv(self):
             b = ArrayDataFrame([[6.1, 1.1], [2.1, 7.1]], "c:double,a:double")
             path = os.path.join(self.tmpdir, "a", "b")
             makedirs(path, exist_ok=True)
             # over write folder with single file
             fa.save(b, path, format_hint="csv", header=True, force_single=True)
             assert isfile(path)
             c = fa.load(
                 path, format_hint="csv", header=True, infer_schema=False, as_fugue=True
             )
-            df_eq(c, [["6.1", "1.1"], ["2.1", "7.1"]], "c:str,a:str", throw=True)
+            self.df_eq(c, [["6.1", "1.1"], ["2.1", "7.1"]], "c:str,a:str", throw=True)
 
             c = fa.load(
                 path, format_hint="csv", header=True, infer_schema=True, as_fugue=True
             )
-            df_eq(c, [[6.1, 1.1], [2.1, 7.1]], "c:double,a:double", throw=True)
+            self.df_eq(c, [[6.1, 1.1], [2.1, 7.1]], "c:double,a:double", throw=True)
 
             with raises(ValueError):
                 c = fa.load(
                     path,
                     format_hint="csv",
                     header=True,
                     infer_schema=True,
@@ -1086,38 +1093,38 @@
                 path,
                 format_hint="csv",
                 header=True,
                 infer_schema=False,
                 columns=["a", "c"],
                 as_fugue=True,
             )
-            df_eq(c, [["1.1", "6.1"], ["7.1", "2.1"]], "a:str,c:str", throw=True)
+            self.df_eq(c, [["1.1", "6.1"], ["7.1", "2.1"]], "a:str,c:str", throw=True)
 
             c = fa.load(
                 path,
                 format_hint="csv",
                 header=True,
                 infer_schema=False,
                 columns="a:double,c:double",
                 as_fugue=True,
             )
-            df_eq(c, [[1.1, 6.1], [7.1, 2.1]], "a:double,c:double", throw=True)
+            self.df_eq(c, [[1.1, 6.1], [7.1, 2.1]], "a:double,c:double", throw=True)
 
             # overwirte single with folder (if applicable)
             b = ArrayDataFrame([[60.1, 1.1], [20.1, 7.1]], "c:double,a:double")
             fa.save(b, path, format_hint="csv", header=True, mode="overwrite")
             c = fa.load(
                 path,
                 format_hint="csv",
                 header=True,
                 infer_schema=False,
                 columns=["a", "c"],
                 as_fugue=True,
             )
-            df_eq(c, [["1.1", "60.1"], ["7.1", "20.1"]], "a:str,c:str", throw=True)
+            self.df_eq(c, [["1.1", "60.1"], ["7.1", "20.1"]], "a:str,c:str", throw=True)
 
         def test_save_single_and_load_csv_no_header(self):
             b = ArrayDataFrame([[6.1, 1.1], [2.1, 7.1]], "c:double,a:double")
             path = os.path.join(self.tmpdir, "a", "b")
             makedirs(path, exist_ok=True)
             # over write folder with single file
             fa.save(b, path, format_hint="csv", header=False, force_single=True)
@@ -1125,37 +1132,37 @@
 
             with raises(ValueError):
                 c = fa.load(
                     path,
                     format_hint="csv",
                     header=False,
                     infer_schema=False,
-                    as_fugue=True
+                    as_fugue=True,
                     # when header is False, must set columns
                 )
 
             c = fa.load(
                 path,
                 format_hint="csv",
                 header=False,
                 infer_schema=False,
                 columns=["c", "a"],
                 as_fugue=True,
             )
-            df_eq(c, [["6.1", "1.1"], ["2.1", "7.1"]], "c:str,a:str", throw=True)
+            self.df_eq(c, [["6.1", "1.1"], ["2.1", "7.1"]], "c:str,a:str", throw=True)
 
             c = fa.load(
                 path,
                 format_hint="csv",
                 header=False,
                 infer_schema=True,
                 columns=["c", "a"],
                 as_fugue=True,
             )
-            df_eq(c, [[6.1, 1.1], [2.1, 7.1]], "c:double,a:double", throw=True)
+            self.df_eq(c, [[6.1, 1.1], [2.1, 7.1]], "c:double,a:double", throw=True)
 
             with raises(ValueError):
                 c = fa.load(
                     path,
                     format_hint="csv",
                     header=False,
                     infer_schema=True,
@@ -1167,29 +1174,29 @@
                 path,
                 format_hint="csv",
                 header=False,
                 infer_schema=False,
                 columns="c:double,a:str",
                 as_fugue=True,
             )
-            df_eq(c, [[6.1, "1.1"], [2.1, "7.1"]], "c:double,a:str", throw=True)
+            self.df_eq(c, [[6.1, "1.1"], [2.1, "7.1"]], "c:double,a:str", throw=True)
 
         def test_save_and_load_csv(self):
             b = ArrayDataFrame([[6.1, 1.1], [2.1, 7.1]], "c:double,a:double")
             path = os.path.join(self.tmpdir, "a", "b")
             fa.save(b, path, format_hint="csv", header=True)
             c = fa.load(
                 path,
                 format_hint="csv",
                 header=True,
                 infer_schema=True,
                 columns=["a", "c"],
                 as_fugue=True,
             )
-            df_eq(c, [[1.1, 6.1], [7.1, 2.1]], "a:double,c:double", throw=True)
+            self.df_eq(c, [[1.1, 6.1], [7.1, 2.1]], "a:double,c:double", throw=True)
 
         def test_load_csv_folder(self):
             native = NativeExecutionEngine()
             a = ArrayDataFrame([[6.1, 1.1]], "c:double,a:double")
             b = ArrayDataFrame([[2.1, 7.1], [4.1, 8.1]], "c:double,a:double")
             path = os.path.join(self.tmpdir, "a", "b")
             fa.save(
@@ -1211,71 +1218,71 @@
                 path,
                 format_hint="csv",
                 header=True,
                 infer_schema=True,
                 columns=["a", "c"],
                 as_fugue=True,
             )
-            df_eq(
+            self.df_eq(
                 c, [[1.1, 6.1], [7.1, 2.1], [8.1, 4.1]], "a:double,c:double", throw=True
             )
 
         def test_save_single_and_load_json(self):
             b = ArrayDataFrame([[6, 1], [2, 7]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             makedirs(path, exist_ok=True)
             # over write folder with single file
             fa.save(b, path, format_hint="json", force_single=True)
             assert isfile(path)
             c = fa.load(path, format_hint="json", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2]], "a:long,c:long", throw=True)
+            self.df_eq(c, [[1, 6], [7, 2]], "a:long,c:long", throw=True)
 
             # overwirte single with folder (if applicable)
             b = ArrayDataFrame([[60, 1], [20, 7]], "c:long,a:long")
             fa.save(b, path, format_hint="json", mode="overwrite")
             c = fa.load(path, format_hint="json", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 60], [7, 20]], "a:long,c:long", throw=True)
+            self.df_eq(c, [[1, 60], [7, 20]], "a:long,c:long", throw=True)
 
         def test_save_and_load_json(self):
             e = self.engine
             b = ArrayDataFrame([[6, 1], [3, 4], [2, 7], [4, 8], [6, 7]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             fa.save(
                 e.repartition(fa.as_fugue_engine_df(e, b), PartitionSpec(num=2)),
                 path,
                 format_hint="json",
             )
             c = fa.load(path, format_hint="json", columns=["a", "c"], as_fugue=True)
-            df_eq(
+            self.df_eq(
                 c, [[1, 6], [7, 2], [4, 3], [8, 4], [7, 6]], "a:long,c:long", throw=True
             )
 
         def test_load_json_folder(self):
             native = NativeExecutionEngine()
             a = ArrayDataFrame([[6, 1], [3, 4]], "c:int,a:long")
             b = ArrayDataFrame([[2, 7], [4, 8]], "c:int,a:long")
             path = os.path.join(self.tmpdir, "a", "b")
             fa.save(a, os.path.join(path, "a.json"), format_hint="json", engine=native)
             fa.save(b, os.path.join(path, "b.json"), format_hint="json", engine=native)
             touch(os.path.join(path, "_SUCCESS"))
             c = fa.load(path, format_hint="json", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2], [8, 4], [4, 3]], "a:long,c:long", throw=True)
+            self.df_eq(c, [[1, 6], [7, 2], [8, 4], [4, 3]], "a:long,c:long", throw=True)
 
         def test_engine_api(self):
             # complimentary tests not covered by the other tests
             with fa.engine_context(self.engine):
                 df1 = fa.as_fugue_df([[0, 1], [2, 3]], schema="a:long,b:long")
                 df1 = fa.repartition(df1, {"num": 2})
                 df1 = fa.get_native_as_df(fa.broadcast(df1))
                 df2 = pd.DataFrame([[0, 1], [2, 3]], columns=["a", "b"])
                 df3 = fa.union(df1, df2, as_fugue=False)
                 assert fa.is_df(df3) and not isinstance(df3, DataFrame)
                 df4 = fa.union(df1, df2, as_fugue=True)
                 assert isinstance(df4, DataFrame)
-                df_eq(df4, fa.as_pandas(df3), throw=True)
+                self.df_eq(df4, fa.as_pandas(df3), throw=True)
 
 
 def select_top(cursor, data):
     return ArrayDataFrame([cursor.row], cursor.row_schema)
 
 
 class BinaryObject(object):
```

### Comparing `fugue-0.9.0.dev3/fugue_test/fixtures.py` & `fugue-0.9.0.dev4/fugue_test/fixtures.py`

 * *Files identical despite different names*

### Comparing `fugue-0.9.0.dev3/setup.cfg` & `fugue-0.9.0.dev4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 omit = 
 	fugue_sql/_antlr/*
 	fugue_test/plugins/*
 	fugue_test/fixtures.py
 	fugue_test/__init__.py
 
 [flake8]
-ignore = E24,E203,W503,C401,C408,A001,A003,W504,C407,C405,B023,B028
+ignore = E24,E203,W503,C401,C408,A001,A003,A005,W504,C407,C405,B023,B028
 max-line-length = 88
 format = pylint
 exclude = .svc,CVS,.bzr,.hg,.git,__pycache__,venv,tests/*,docs/*
 max-complexity = 10
 
 [egg_info]
 tag_build =
```

### Comparing `fugue-0.9.0.dev3/setup.py` & `fugue-0.9.0.dev4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,52 +34,53 @@
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="distributed spark dask ray sql dsl domain specific language",
     url="http://github.com/fugue-project/fugue",
     install_requires=[
-        "triad>=0.9.4",
+        "triad>=0.9.6",
         "adagio>=0.2.4",
     ],
     extras_require={
         "sql": SQL_DEPENDENCIES,
         "cpp_sql_parser": ["fugue-sql-antlr[cpp]>=0.2.0"],
         "spark": ["pyspark>=3.1.1"],
         "dask": [
             "dask[distributed,dataframe]>=2023.5.0",
+            "dask[distributed,dataframe]>=2024.4.0;python_version>='3.11.9'",
             "pyarrow>=7.0.0",
             "pandas>=2.0.2",
         ],
         "ray": [
-            "ray[data]>=2.4.0",
+            "ray[data]>=2.5.0",
             "duckdb>=0.5.0",
-            "pyarrow>=6.0.1",
+            "pyarrow>=7.0.0",
             "pandas<2.2",
         ],
         "duckdb": SQL_DEPENDENCIES
         + [
             "duckdb>=0.5.0",
             "numpy",
         ],
         "polars": ["polars"],
-        "ibis": SQL_DEPENDENCIES + ["ibis-framework"],
+        "ibis": SQL_DEPENDENCIES + ["ibis-framework", "pandas<2.2"],
         "notebook": ["notebook", "jupyterlab", "ipython>=7.10.0"],
         "all": SQL_DEPENDENCIES
         + [
             "pyspark>=3.1.1",
             "dask[distributed,dataframe]>=2023.5.0",
             "dask-sql",
-            "ray[data]>=2.4.0",
+            "ray[data]>=2.5.0",
             "notebook",
             "jupyterlab",
             "ipython>=7.10.0",
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
-            "pandas>=2.0.2,<2.2",  # because of Ray
+            "pandas>=2.0.2,<2.2",  # because of Ray and ibis
             "ibis-framework",
             "polars",
         ],
     },
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 5 - Production/Stable",
```

