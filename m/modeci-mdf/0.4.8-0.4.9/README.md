# Comparing `tmp/modeci-mdf-0.4.8.tar.gz` & `tmp/modeci-mdf-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeci-mdf-0.4.8.tar", last modified: Fri Sep 15 17:39:22 2023, max compression
+gzip compressed data, was "modeci-mdf-0.4.9.tar", last modified: Wed Mar  6 16:27:22 2024, max compression
```

## Comparing `modeci-mdf-0.4.8.tar` & `modeci-mdf-0.4.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.531869 modeci-mdf-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-15 17:39:12.000000 modeci-mdf-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2023-09-15 17:39:22.531869 modeci-mdf-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2023-09-15 17:39:12.000000 modeci-mdf-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-09-15 17:39:22.535869 modeci-mdf-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.523869 modeci-mdf-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.523869 modeci-mdf-0.4.8/src/modeci_mdf/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50376 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/full_translator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.523869 modeci-mdf-0.4.8/src/modeci_mdf/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.523869 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/dm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/ddm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/functions/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/actr/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/actr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/actr/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/graphviz/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/graphviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19462 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/graphviz/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/keras/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/neuroml/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/neuroml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/neuroml/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/onnx/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15306 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/onnx/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    19682 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20391 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/mdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/src/modeci_mdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.523869 modeci-mdf-0.4.8/src/modeci_mdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2023-09-15 17:39:22.000000 modeci-mdf-0.4.8/src/modeci_mdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-09-15 17:39:22.000000 modeci-mdf-0.4.8/src/modeci_mdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 17:39:22.000000 modeci-mdf-0.4.8/src/modeci_mdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-09-15 17:39:22.000000 modeci-mdf-0.4.8/src/modeci_mdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-15 17:39:22.000000 modeci-mdf-0.4.8/src/modeci_mdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 17:39:22.527869 modeci-mdf-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_mdf_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_onnx_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2023-09-15 17:39:13.000000 modeci-mdf-0.4.8/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.874997 modeci-mdf-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-06 16:27:17.000000 modeci-mdf-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-03-06 16:27:22.874997 modeci-mdf-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-03-06 16:27:17.000000 modeci-mdf-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-06 16:27:22.874997 modeci-mdf-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.862997 modeci-mdf-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.862997 modeci-mdf-0.4.9/src/modeci_mdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50376 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/full_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/functions/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/actr/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/actr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/actr/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/graphviz/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/graphviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19462 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/graphviz/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/keras/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/neuroml/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/neuroml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/neuroml/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.866997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/onnx/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/onnx/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.870997 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19682 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20776 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/mdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/src/modeci_mdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.870997 modeci-mdf-0.4.9/src/modeci_mdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-03-06 16:27:22.000000 modeci-mdf-0.4.9/src/modeci_mdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-06 16:27:22.000000 modeci-mdf-0.4.9/src/modeci_mdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 16:27:22.000000 modeci-mdf-0.4.9/src/modeci_mdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-06 16:27:22.000000 modeci-mdf-0.4.9/src/modeci_mdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-06 16:27:22.000000 modeci-mdf-0.4.9/src/modeci_mdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:27:22.870997 modeci-mdf-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_mdf_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_onnx_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-03-06 16:27:18.000000 modeci-mdf-0.4.9/tests/test_scheduler.py
```

### Comparing `modeci-mdf-0.4.8/LICENSE` & `modeci-mdf-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/PKG-INFO` & `modeci-mdf-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 Metadata-Version: 2.1
 Name: modeci-mdf
-Version: 0.4.8
+Version: 0.4.9
 Summary: ModECI (Model Exchange and Convergence Initiative) Model Description Format
 Home-page: https://www.modeci.org
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: ModECI contributors
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_compat; python_version < "3.8"
 Requires-Dist: dataclasses; python_version < "3.7"
-Requires-Dist: graph_scheduler>=1.1.1
+Requires-Dist: graph_scheduler<1.2.0,>=1.1.1
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: graphviz
 Requires-Dist: h5py
-Requires-Dist: onnxruntime==1.13.1
-Requires-Dist: onnx==1.12.0
-Requires-Dist: skl2onnx==1.14.0
+Requires-Dist: onnxruntime
+Requires-Dist: onnx
+Requires-Dist: skl2onnx
 Requires-Dist: attrs>=21.1.0
 Requires-Dist: cattrs
 Requires-Dist: modelspec<0.4,>=0.3.0
 Requires-Dist: glom
 Provides-Extra: psyneulink
 Requires-Dist: grpcio-tools==1.42.0; extra == "psyneulink"
 Requires-Dist: psyneulink; extra == "psyneulink"
 Provides-Extra: neuroml
 Requires-Dist: pyNeuroML>=1.0.10; extra == "neuroml"
 Requires-Dist: neuromllite>=0.5.6; extra == "neuroml"
 Requires-Dist: PyNN==0.10.1; extra == "neuroml"
 Provides-Extra: tensorflow
-Requires-Dist: tensorflow; extra == "tensorflow"
+Requires-Dist: tensorflow>=2.11.0; extra == "tensorflow"
 Requires-Dist: keras_visualizer; extra == "tensorflow"
 Requires-Dist: pydot; extra == "tensorflow"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-benchmark; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: typing_extensions; python_version < "3.8" and extra == "test"
@@ -68,21 +68,21 @@
 Requires-Dist: sphinx_markdown_tables; extra == "optional"
 Requires-Dist: sphinx-autoapi; extra == "optional"
 Requires-Dist: pytorch-sphinx-theme==0.0.19; extra == "optional"
 Requires-Dist: sphinxcontrib-versioning; extra == "optional"
 Requires-Dist: Jinja2<3.1; extra == "optional"
 Requires-Dist: torchviz; extra == "optional"
 Requires-Dist: netron; extra == "optional"
-Requires-Dist: torch>=1.11.0; extra == "optional"
-Requires-Dist: torchvision<=0.12.0; extra == "optional"
+Requires-Dist: torch<2.2.0,>=1.11.0; extra == "optional"
+Requires-Dist: torchvision; extra == "optional"
 Requires-Dist: h5py; extra == "optional"
 Provides-Extra: all-except-psyneulink
+Requires-Dist: modeci-mdf[tensorflow]; extra == "all-except-psyneulink"
 Requires-Dist: modeci-mdf[optional]; extra == "all-except-psyneulink"
 Requires-Dist: modeci-mdf[neuroml]; extra == "all-except-psyneulink"
-Requires-Dist: modeci-mdf[tensorflow]; extra == "all-except-psyneulink"
 Provides-Extra: all
 Requires-Dist: modeci-mdf[all_except_psyneulink]; extra == "all"
 Requires-Dist: modeci-mdf[psyneulink]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: modeci-mdf[test]; extra == "dev"
 
 <p align="center">
```

### Comparing `modeci-mdf-0.4.8/README.md` & `modeci-mdf-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/pyproject.toml` & `modeci-mdf-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/setup.cfg` & `modeci-mdf-0.4.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 license = LGPLv3
 license_file = LICENSE
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Natural Language :: English
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.8
 	Topic :: Scientific/Engineering
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Topic :: Software Development
 	Typing :: Typed
 
 [options]
 packages = find:
 install_requires = 
 	typing_compat;python_version<'3.8'
 	dataclasses;python_version<'3.7'
-	graph_scheduler>=1.1.1
+	graph_scheduler<1.2.0,>=1.1.1
 	numpy
 	matplotlib
 	graphviz
 	h5py
-	onnxruntime==1.13.1
-	onnx==1.12.0
-	skl2onnx==1.14.0
+	onnxruntime
+	onnx
+	skl2onnx
 	attrs>=21.1.0
 	cattrs
 	modelspec<0.4,>=0.3.0
 	glom
 python_requires = >=3.7
 include_package_data = True
 package_dir = 
@@ -57,15 +57,15 @@
 	grpcio-tools==1.42.0
 	psyneulink
 neuroml = 
 	pyNeuroML>=1.0.10
 	neuromllite>=0.5.6
 	PyNN==0.10.1
 tensorflow = 
-	tensorflow
+	tensorflow>=2.11.0
 	keras_visualizer
 	pydot
 test = 
 	pytest
 	pytest-benchmark
 	pytest-mock
 	typing_extensions;python_version<'3.8'
@@ -79,21 +79,21 @@
 	sphinx_markdown_tables
 	sphinx-autoapi
 	pytorch-sphinx-theme==0.0.19
 	sphinxcontrib-versioning
 	Jinja2<3.1
 	torchviz
 	netron
-	torch>=1.11.0
-	torchvision<=0.12.0
+	torch<2.2.0,>=1.11.0
+	torchvision
 	h5py
 all_except_psyneulink = 
+	modeci-mdf[tensorflow]
 	modeci-mdf[optional]
 	modeci-mdf[neuroml]
-	modeci-mdf[tensorflow]
 all = 
 	modeci-mdf[all_except_psyneulink]
 	modeci-mdf[psyneulink]
 dev = 
 	modeci-mdf[test]
 
 [options.packages.find]
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/__init__.py` & `modeci-mdf-0.4.9/src/modeci_mdf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 widely-used programming environments in a range of disciplines, and for easily extending these to other environments.
 """
 
 # Version of the specification for MDF
 MODECI_MDF_VERSION = "0.4"
 
 # Version of the Python module.
-__version__ = "0.4.8"
+__version__ = "0.4.9"
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/execution_engine.py` & `modeci-mdf-0.4.9/src/modeci_mdf/execution_engine.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/full_translator.py` & `modeci-mdf-0.4.9/src/modeci_mdf/full_translator.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/__init__.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/__init__.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/__init__.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/buffer.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/buffer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/dm.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/dm.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/logger.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/logger.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/model.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/model.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/pattern.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/pattern.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/actr/ccm/scheduler.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/actr/ccm/scheduler.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/ddm.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/ddm.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/onnx.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,20 @@
     inputs = {k: convert_type(v) for k, v in inputs.items()}
 
     # In the case of the Pad operator, if constant_value argument is passed with different dtype
     # to the data, cast it.
     if op_name == "Pad":
         if "constant_value" in inputs:
             cval = inputs["constant_value"]
-            data = list(inputs.values())[0]
-            if cval.dtype != data.dtype:
-                inputs["constant_value"] = cval.astype(data.dtype)
+            if cval is None:
+                inputs.pop("constant_value")
+            else:
+                data = list(inputs.values())[0]
+                if cval.dtype != data.dtype:
+                    inputs["constant_value"] = cval.astype(data.dtype)
 
     # SkLearn ONNX doesn't seem to support ConcatFromSequence, see
     # https://github.com/onnx/sklearn-onnx/issues/710
     # Let us just use this implemetation I found in ONNX backend test.
     if op_name == "ConcatFromSequence":
         from onnx.backend.test.case.model.sequence import ConcatFromSequenceImpl
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/functions/standard.py` & `modeci-mdf-0.4.9/src/modeci_mdf/functions/standard.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/actr/importer.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/actr/importer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/graphviz/exporter.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/graphviz/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/keras/importer.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/keras/importer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/neuroml/exporter.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/neuroml/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/onnx/exporter.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/onnx/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from modeci_mdf.execution_engine import EvaluableGraph
 
 import onnx
 from onnx import helper, shape_inference
 from onnx import AttributeProto, TensorProto, GraphProto
 from onnx.defs import get_schema
 
+import onnxruntime
+
 from ast import literal_eval
 
 import argparse
 import os
 
 import numpy
 
@@ -40,15 +42,22 @@
 
         # print(nodenames_in_execution_order, graph.nodes, graph.edges)
 
         # Generate onnx graph
         onnx_graph = generate_onnx_graph(graph, nodenames_in_execution_order)
 
         # Make an onnx model from graph
-        onnx_model = helper.make_model(onnx_graph)
+
+        # Check to see if onnxruntime version is less than 1.15, if so ir_version should
+        # be 8 for now. See: https://github.com/microsoft/onnxruntime/issues/15874
+        make_model_kwargs = {}
+        if onnxruntime.__version__ < "1.15":
+            make_model_kwargs = {"ir_version": 8}
+
+        onnx_model = helper.make_model(onnx_graph, **make_model_kwargs)
 
         # Infer shapes
         onnx_model = shape_inference.infer_shapes(onnx_model)
 
         # Check model
         onnx.checker.check_model(onnx_model)
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/onnx/importer.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/onnx/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 
 from modeci_mdf.mdf import *
 
 
 def id_to_port(id: str):
     """Turn unique ONNX output and input value names into valid MDF input and outport names"""
 
+    # Get rid of periods in names
     new_name = str(id).replace(".", "_")
 
+    # Get rid of slashes in names
+    new_name = str(id).replace("/", "_")
+
     # Get rid of double colon in id names, this causes issues with execution engine.
     new_name = new_name.replace("::", "_")
 
     # If the first character is a digit, precede with an underscore so this can never be interpreted
     # as number down the line.
     if new_name[0].isdigit():
         new_name = "_" + new_name
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/builtins.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/builtins.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/exporter.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/importer.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,26 @@
 import logging
 
 from typing import Union, Dict, Any, Tuple, List, Callable
 import onnx.defs
 
 import torch
 
+# We need to monkey patch the torch._C.Node class to add a __getitem__ method
+# This is for torch 2.0
+# From https://github.com/openai/CLIP/issues/79#issuecomment-1624202950
+def _node_get(node: torch._C.Node, key: str):
+    """Gets attributes of a node which is polymorphic over return type."""
+    sel = node.kindOf(key)
+    return getattr(node, sel)(key)
+
+
+torch._C.Node.__getitem__ = _node_get
+
+
 from modeci_mdf.mdf import Model, Graph, Node, Edge, InputPort, OutputPort, Parameter
 from modeci_mdf.functions.onnx import onnx_opset_version as modeci_onnx_opset_version
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -289,23 +301,23 @@
 
     Returns:
         The MDF node for this TorchScript node. prim::Constant nodes are excluded from the MDF graph and are
         instead placed as parameters. In this case, return None.
     """
     op = node.kind()
 
-    # Lookup the schema. For some reason we cannot just call node.schema(), it returns "(no schema)", huh?
-    # We need to do this the hard way.
-    schema = onnx.defs.get_schema(op.replace("onnx::", ""), modeci_onnx_opset_version)
-
     # Exclude constants (as nodes) from the MDF graph. We will instead insert them as parameters to the nodes that
     # they project to.
     if op in ("prim::Constant", "onnx::Constant"):
         return None
 
+    # Lookup the schema. For some reason we cannot just call node.schema(), it returns "(no schema)", huh?
+    # We need to do this the hard way.
+    schema = onnx.defs.get_schema(op.replace("onnx::", ""), modeci_onnx_opset_version)
+
     # If we are dealing with a loop node, we need to recursively create a sub-graph for the loop body
     if op == "onnx::Loop":
         sub_mdf_graph = Graph(id=f"LoopSubgraph{make_node_id(node)}")
         block_graph = list(node.blocks())[0]
         translate_graph(
             graph=block_graph,
             mdf_graph=sub_mdf_graph,
@@ -500,15 +512,15 @@
             jit_model = torch.jit.script(model)
             graph = jit_model.graph
         else:
             # If the user wants to trace, _model_to_graph below will take care of that for us.
             graph = None
 
     if use_onnx_ops:
-        operator_export_type = torch._C._onnx.OperatorExportTypes.ONNX_ATEN_FALLBACK
+        operator_export_type = torch._C._onnx.OperatorExportTypes.ONNX
     else:
         operator_export_type = torch._C._onnx.OperatorExportTypes.RAW
 
     # Call out to a part of the ONNX exporter that simiplifies the graph before ONNX export.
     from torch.onnx.utils import _model_to_graph
     from torch.onnx import TrainingMode
     from torch.onnx.symbolic_helper import _set_opset_version
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py` & `modeci-mdf-0.4.9/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/mdf.py` & `modeci-mdf-0.4.9/src/modeci_mdf/mdf.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf/utils.py` & `modeci-mdf-0.4.9/src/modeci_mdf/utils.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf.egg-info/PKG-INFO` & `modeci-mdf-0.4.9/src/modeci_mdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 Metadata-Version: 2.1
 Name: modeci-mdf
-Version: 0.4.8
+Version: 0.4.9
 Summary: ModECI (Model Exchange and Convergence Initiative) Model Description Format
 Home-page: https://www.modeci.org
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: ModECI contributors
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_compat; python_version < "3.8"
 Requires-Dist: dataclasses; python_version < "3.7"
-Requires-Dist: graph_scheduler>=1.1.1
+Requires-Dist: graph_scheduler<1.2.0,>=1.1.1
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: graphviz
 Requires-Dist: h5py
-Requires-Dist: onnxruntime==1.13.1
-Requires-Dist: onnx==1.12.0
-Requires-Dist: skl2onnx==1.14.0
+Requires-Dist: onnxruntime
+Requires-Dist: onnx
+Requires-Dist: skl2onnx
 Requires-Dist: attrs>=21.1.0
 Requires-Dist: cattrs
 Requires-Dist: modelspec<0.4,>=0.3.0
 Requires-Dist: glom
 Provides-Extra: psyneulink
 Requires-Dist: grpcio-tools==1.42.0; extra == "psyneulink"
 Requires-Dist: psyneulink; extra == "psyneulink"
 Provides-Extra: neuroml
 Requires-Dist: pyNeuroML>=1.0.10; extra == "neuroml"
 Requires-Dist: neuromllite>=0.5.6; extra == "neuroml"
 Requires-Dist: PyNN==0.10.1; extra == "neuroml"
 Provides-Extra: tensorflow
-Requires-Dist: tensorflow; extra == "tensorflow"
+Requires-Dist: tensorflow>=2.11.0; extra == "tensorflow"
 Requires-Dist: keras_visualizer; extra == "tensorflow"
 Requires-Dist: pydot; extra == "tensorflow"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-benchmark; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: typing_extensions; python_version < "3.8" and extra == "test"
@@ -68,21 +68,21 @@
 Requires-Dist: sphinx_markdown_tables; extra == "optional"
 Requires-Dist: sphinx-autoapi; extra == "optional"
 Requires-Dist: pytorch-sphinx-theme==0.0.19; extra == "optional"
 Requires-Dist: sphinxcontrib-versioning; extra == "optional"
 Requires-Dist: Jinja2<3.1; extra == "optional"
 Requires-Dist: torchviz; extra == "optional"
 Requires-Dist: netron; extra == "optional"
-Requires-Dist: torch>=1.11.0; extra == "optional"
-Requires-Dist: torchvision<=0.12.0; extra == "optional"
+Requires-Dist: torch<2.2.0,>=1.11.0; extra == "optional"
+Requires-Dist: torchvision; extra == "optional"
 Requires-Dist: h5py; extra == "optional"
 Provides-Extra: all-except-psyneulink
+Requires-Dist: modeci-mdf[tensorflow]; extra == "all-except-psyneulink"
 Requires-Dist: modeci-mdf[optional]; extra == "all-except-psyneulink"
 Requires-Dist: modeci-mdf[neuroml]; extra == "all-except-psyneulink"
-Requires-Dist: modeci-mdf[tensorflow]; extra == "all-except-psyneulink"
 Provides-Extra: all
 Requires-Dist: modeci-mdf[all_except_psyneulink]; extra == "all"
 Requires-Dist: modeci-mdf[psyneulink]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: modeci-mdf[test]; extra == "dev"
 
 <p align="center">
```

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf.egg-info/SOURCES.txt` & `modeci-mdf-0.4.9/src/modeci_mdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/src/modeci_mdf.egg-info/requires.txt` & `modeci-mdf-0.4.9/src/modeci_mdf.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-graph_scheduler>=1.1.1
+graph_scheduler<1.2.0,>=1.1.1
 numpy
 matplotlib
 graphviz
 h5py
-onnxruntime==1.13.1
-onnx==1.12.0
-skl2onnx==1.14.0
+onnxruntime
+onnx
+skl2onnx
 attrs>=21.1.0
 cattrs
 modelspec<0.4,>=0.3.0
 glom
 
 [:python_version < "3.7"]
 dataclasses
@@ -18,17 +18,17 @@
 typing_compat
 
 [all]
 modeci-mdf[all_except_psyneulink]
 modeci-mdf[psyneulink]
 
 [all_except_psyneulink]
+modeci-mdf[tensorflow]
 modeci-mdf[optional]
 modeci-mdf[neuroml]
-modeci-mdf[tensorflow]
 
 [dev]
 modeci-mdf[test]
 
 [neuroml]
 pyNeuroML>=1.0.10
 neuromllite>=0.5.6
@@ -44,24 +44,24 @@
 sphinx_markdown_tables
 sphinx-autoapi
 pytorch-sphinx-theme==0.0.19
 sphinxcontrib-versioning
 Jinja2<3.1
 torchviz
 netron
-torch>=1.11.0
-torchvision<=0.12.0
+torch<2.2.0,>=1.11.0
+torchvision
 h5py
 
 [psyneulink]
 grpcio-tools==1.42.0
 psyneulink
 
 [tensorflow]
-tensorflow
+tensorflow>=2.11.0
 keras_visualizer
 pydot
 
 [test]
 pytest
 pytest-benchmark
 pytest-mock
```

### Comparing `modeci-mdf-0.4.8/tests/test_examples.py` & `modeci-mdf-0.4.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/tests/test_execution.py` & `modeci-mdf-0.4.9/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/tests/test_helpers.py` & `modeci-mdf-0.4.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/tests/test_mdf_functions.py` & `modeci-mdf-0.4.9/tests/test_mdf_functions.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/tests/test_model.py` & `modeci-mdf-0.4.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/tests/test_onnx_functions.py` & `modeci-mdf-0.4.9/tests/test_onnx_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,7 +102,12 @@
 
 def test_maxpool():
     """Test ONNX Concat function. This is a variable number of inputs operator."""
     out = onnx_ops.maxpool(
         np.ones((1, 3, 32, 32)).astype(np.float32), kernel_shape=[2, 2]
     )
     assert True
+
+
+def test_randomuniform():
+    """Test ONNX randomuniform function."""
+    out = onnx_ops.randomuniform(low=-1.0, high=1.0, seed=0.0, shape=(1, 1))
```

### Comparing `modeci-mdf-0.4.8/tests/test_parameters.py` & `modeci-mdf-0.4.9/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.8/tests/test_scheduler.py` & `modeci-mdf-0.4.9/tests/test_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     array_format = FORMAT_NUMPY
 
     for mdf_format in mdf_formats:
 
         eg = modeci_mdf.execution_engine.main(
             "examples/ONNX/ab.%s" % mdf_format, array_format=array_format
         )
-        output = eg.enodes["Mul_3"].evaluable_outputs["_4"].curr_value
+        output = eg.enodes["/B/Mul"].evaluable_outputs["_4"].curr_value
         assert np.array_equal(output, np.full((2, 3), 5))
 
 
 _abc_conditions_expected_output = [
     {"A"},
     {"A"},
     {"B"},
```

