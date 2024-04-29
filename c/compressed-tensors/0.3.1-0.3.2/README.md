# Comparing `tmp/compressed-tensors-0.3.1.tar.gz` & `tmp/compressed-tensors-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressed-tensors-0.3.1.tar", last modified: Thu Apr 25 16:42:58 2024, max compression
+gzip compressed data, was "compressed-tensors-0.3.2.tar", last modified: Mon Apr 29 14:01:33 2024, max compression
```

## Comparing `compressed-tensors-0.3.1.tar` & `compressed-tensors-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/
--rw-rw-r--   0 damian    (1006) damian    (1007)    11357 2024-04-25 16:30:47.000000 compressed-tensors-0.3.1/LICENSE
--rw-rw-r--   0 damian    (1006) damian    (1007)     3472 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/PKG-INFO
--rw-rw-r--   0 damian    (1006) damian    (1007)     3078 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/README.md
--rw-rw-r--   0 damian    (1006) damian    (1007)       56 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/pyproject.toml
--rw-rw-r--   0 damian    (1006) damian    (1007)      388 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/setup.cfg
--rw-rw-r--   0 damian    (1006) damian    (1007)     1838 2024-04-25 16:42:40.000000 compressed-tensors-0.3.1/setup.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.675947 compressed-tensors-0.3.1/src/
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.675947 compressed-tensors-0.3.1/src/compressed_tensors/
--rw-rw-r--   0 damian    (1006) damian    (1007)      789 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)      717 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/base.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.675947 compressed-tensors-0.3.1/src/compressed_tensors/compressors/
--rw-rw-r--   0 damian    (1006) damian    (1007)      898 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/compressors/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2936 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/compressors/base.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1263 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/compressors/dense.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     6421 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/compressors/helpers.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     8639 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/compressors/sparse_bitmask.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.675947 compressed-tensors-0.3.1/src/compressed_tensors/config/
--rw-rw-r--   0 damian    (1006) damian    (1007)      704 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/config/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1373 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/config/base.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1311 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/config/dense.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1284 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/config/sparse_bitmask.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.675947 compressed-tensors-0.3.1/src/compressed_tensors/quantization/
--rw-rw-r--   0 damian    (1006) damian    (1007)      760 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/__init__.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/
--rw-rw-r--   0 damian    (1006) damian    (1007)      772 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     6651 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/apply.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1776 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/calibration.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     4599 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/forward.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1596 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/frozen.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     3578 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/initialize.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/
--rw-rw-r--   0 damian    (1006) damian    (1007)      745 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2786 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/base.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2109 2024-04-25 14:00:11.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/helpers.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1848 2024-04-25 14:00:11.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/memoryless.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2439 2024-04-25 14:00:11.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/min_max.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2742 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/quant_args.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     6650 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/quant_config.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1480 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/quant_scheme.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/src/compressed_tensors/quantization/utils/
--rw-rw-r--   0 damian    (1006) damian    (1007)      656 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/utils/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     3694 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/quantization/utils/helpers.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/src/compressed_tensors/registry/
--rw-rw-r--   0 damian    (1006) damian    (1007)      658 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/registry/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)    11890 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/src/compressed_tensors/registry/registry.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/src/compressed_tensors/utils/
--rw-rw-r--   0 damian    (1006) damian    (1007)      665 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/utils/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     8502 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/src/compressed_tensors/utils/safetensors_load.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.675947 compressed-tensors-0.3.1/src/compressed_tensors.egg-info/
--rw-r--r--   0 damian    (1006) damian    (1007)     3472 2024-04-25 16:42:58.000000 compressed-tensors-0.3.1/src/compressed_tensors.egg-info/PKG-INFO
--rw-rw-r--   0 damian    (1006) damian    (1007)     1911 2024-04-25 16:42:58.000000 compressed-tensors-0.3.1/src/compressed_tensors.egg-info/SOURCES.txt
--rw-rw-r--   0 damian    (1006) damian    (1007)        1 2024-04-25 16:42:58.000000 compressed-tensors-0.3.1/src/compressed_tensors.egg-info/dependency_links.txt
--rw-rw-r--   0 damian    (1006) damian    (1007)      139 2024-04-25 16:42:58.000000 compressed-tensors-0.3.1/src/compressed_tensors.egg-info/requires.txt
--rw-rw-r--   0 damian    (1006) damian    (1007)       19 2024-04-25 16:42:58.000000 compressed-tensors-0.3.1/src/compressed_tensors.egg-info/top_level.txt
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-25 16:42:58.679947 compressed-tensors-0.3.1/tests/
--rw-rw-r--   0 damian    (1006) damian    (1007)     4322 2024-04-19 09:24:17.000000 compressed-tensors-0.3.1/tests/test_bitmask.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1662 2024-04-25 13:53:48.000000 compressed-tensors-0.3.1/tests/test_registry.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/
+-rw-rw-r--   0 damian    (1006) damian    (1007)    11357 2024-04-25 16:30:47.000000 compressed-tensors-0.3.2/LICENSE
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3682 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/PKG-INFO
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3288 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/README.md
+-rw-rw-r--   0 damian    (1006) damian    (1007)       56 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/pyproject.toml
+-rw-rw-r--   0 damian    (1006) damian    (1007)      388 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/setup.cfg
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1838 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/setup.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      789 2024-04-29 09:32:10.000000 compressed-tensors-0.3.2/src/compressed_tensors/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)      717 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/base.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/compressors/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      841 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3902 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/base.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1271 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/dense.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     5458 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/helpers.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     8647 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/sparse_bitmask.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/config/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      704 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1373 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/base.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1311 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/dense.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1284 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/sparse_bitmask.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      760 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/__init__.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      772 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     6651 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/apply.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1776 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/calibration.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     4941 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/forward.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1606 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/frozen.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3697 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/initialize.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      745 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     2786 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/base.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     2109 2024-04-25 14:00:11.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/helpers.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1859 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/memoryless.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     2439 2024-04-25 14:00:11.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/min_max.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3371 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_args.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     6650 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_config.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1480 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_scheme.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      656 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3694 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/helpers.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/registry/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      658 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/registry/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)    11890 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/registry/registry.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/utils/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      665 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/utils/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     8502 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/utils/safetensors_load.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/
+-rw-r--r--   0 damian    (1006) damian    (1007)     3682 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/PKG-INFO
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1911 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/SOURCES.txt
+-rw-rw-r--   0 damian    (1006) damian    (1007)        1 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/dependency_links.txt
+-rw-rw-r--   0 damian    (1006) damian    (1007)      139 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/requires.txt
+-rw-rw-r--   0 damian    (1006) damian    (1007)       19 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/top_level.txt
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/tests/
+-rw-rw-r--   0 damian    (1006) damian    (1007)     4322 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/tests/test_bitmask.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1662 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/tests/test_registry.py
```

### Comparing `compressed-tensors-0.3.1/LICENSE` & `compressed-tensors-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/PKG-INFO` & `compressed-tensors-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressed-tensors
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for utilization of compressed safetensors of neural network models
 Home-page: https://github.com/neuralmagic/compressed-tensors
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -90,8 +90,11 @@
 # save compressed model weights
 save_compressed_model(model, "compressed_model.safetensors", compression_format=compression_config.format)
 
 # load compressed model weights (`dict` turns generator into a dictionary)
 state_dict = dict(load_compressed("compressed_model.safetensors", compression_config))
 ```
 
+For more in-depth tutorial on bitmask compression, refer to the [notebook](https://github.com/neuralmagic/compressed-tensors/blob/d707c5b84bc3fef164aebdcd97cb6eaa571982f8/examples/bitmask_compression.ipynb).
+
+
```

### Comparing `compressed-tensors-0.3.1/README.md` & `compressed-tensors-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,7 +76,10 @@
 
 # save compressed model weights
 save_compressed_model(model, "compressed_model.safetensors", compression_format=compression_config.format)
 
 # load compressed model weights (`dict` turns generator into a dictionary)
 state_dict = dict(load_compressed("compressed_model.safetensors", compression_config))
 ```
+
+For more in-depth tutorial on bitmask compression, refer to the [notebook](https://github.com/neuralmagic/compressed-tensors/blob/d707c5b84bc3fef164aebdcd97cb6eaa571982f8/examples/bitmask_compression.ipynb).
+
```

### Comparing `compressed-tensors-0.3.1/setup.py` & `compressed-tensors-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return ["torch>=1.7.0", "transformers<4.41", "pydantic<2.7"]
 
 def _setup_extras() -> Dict:
     return {"dev": ["black==22.12.0", "isort==5.8.0", "wheel>=0.36.2", "flake8>=3.8.3", "pytest>=6.0.0", "nbconvert>=7.16.3"]}
 
 setup(
     name="compressed-tensors",
-    version="0.3.1",
+    version="0.3.2",
     author="Neuralmagic, Inc.",
     author_email="support@neuralmagic.com",
     license="Apache 2.0",
     description="Library for utilization of compressed safetensors of neural network models",
     long_description=_setup_long_description()[0],
     long_description_content_type=_setup_long_description()[1],
     url="https://github.com/neuralmagic/compressed-tensors",
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/base.py` & `compressed-tensors-0.3.2/src/compressed_tensors/base.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/compressors/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/config/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,10 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # flake8: noqa
-
-from .base import ModelCompressor
-from .dense import DenseCompressor
-from .helpers import (
-    infer_compressor_from_model_config,
-    load_compressed,
-    save_compressed,
-    save_compressed_model,
-)
-from .sparse_bitmask import BitmaskCompressor, BitmaskTensor
+from .base import *
+from .dense import *
+from .sparse_bitmask import *
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/compressors/base.py` & `compressed-tensors-0.3.2/src/compressed_tensors/compressors/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,40 +18,64 @@
 from compressed_tensors.base import SPARSITY_CONFIG_NAME
 from compressed_tensors.config import CompressionConfig
 from compressed_tensors.registry import RegistryMixin
 from compressed_tensors.utils import get_safetensors_folder
 from torch import Tensor
 from torch.nn import Module, Parameter
 from tqdm import tqdm
+from transformers import AutoConfig
 
 
 __all__ = ["ModelCompressor"]
 
 
 class ModelCompressor(RegistryMixin):
     """
     Base class representing a model compression algorithm.
 
     :param config: config specifying compression parameters
     """
 
+    @classmethod
+    def from_pretrained(
+        cls, pretrained_model_name_or_path: str
+    ) -> Optional["ModelCompressor"]:
+        """
+        Given a path to a model config, extract a sparsity config if it exists and
+        return the associated ModelCompressor
+
+        :param pretrained_model_name_or_path: path to model config on disk or HF hub
+        :return: matching compressor if config contains a sparsity config
+        """
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
+        sparsity_config = getattr(config, SPARSITY_CONFIG_NAME, None)
+        if sparsity_config is None:
+            return None
+
+        format = sparsity_config.get("format")
+        sparsity_config = CompressionConfig.load_from_registry(
+            format, **sparsity_config
+        )
+        compressor = cls.load_from_registry(format, config=sparsity_config)
+        return compressor
+
     def __init__(self, config: Optional[CompressionConfig] = None):
         self.config = config
 
     def compress(self, model_state: Dict[str, Tensor]) -> Dict[str, Tensor]:
         """
         Compresses a dense state dict
 
         :param model_state: state dict of uncompressed model
         :return: compressed state dict
         """
         raise NotImplementedError()
 
     def decompress(
-        self, path_to_model_or_tensors: str
+        self, path_to_model_or_tensors: str, device: str = "cpu"
     ) -> Generator[Tuple[str, Tensor], None, None]:
         """
         Reads a compressed state dict located at path_to_model_or_tensors
         and returns a generator for sequentially decompressing back to a
         dense state dict
 
         :param model_path: path to compressed safetensors model (directory with
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/compressors/dense.py` & `compressed-tensors-0.3.2/src/compressed_tensors/compressors/dense.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,10 @@
     Identity compressor for dense models, returns the original state_dict
     """
 
     def compress(self, model_state: Dict[str, Tensor]) -> Dict[str, Tensor]:
         return model_state
 
     def decompress(
-        self, path_to_model_or_tensors: str, device: str
+        self, path_to_model_or_tensors: str, device: str = "cpu"
     ) -> Generator[Tuple[str, Tensor], None, None]:
         return iter([])
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/compressors/helpers.py` & `compressed-tensors-0.3.2/src/compressed_tensors/compressors/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,53 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
 from typing import Dict, Generator, Optional, Tuple, Union
 
 import torch
-from compressed_tensors.base import SPARSITY_CONFIG_NAME
 from compressed_tensors.compressors import ModelCompressor
 from compressed_tensors.config import CompressionConfig, CompressionFormat
 from compressed_tensors.utils.safetensors_load import get_weight_mappings
 from safetensors import safe_open
 from safetensors.torch import save_file
 from torch import Tensor
-from transformers import AutoConfig
 
 
 __all__ = [
-    "infer_compressor_from_model_config",
     "load_compressed",
     "save_compressed",
     "save_compressed_model",
 ]
 
 
-def infer_compressor_from_model_config(
-    pretrained_model_name_or_path: str,
-) -> Optional[ModelCompressor]:
-    """
-    Given a path to a model config, extract a sparsity config if it exists and return
-    the associated ModelCompressor
-
-    :param pretrained_model_name_or_path: path to model config on disk or HF hub
-    :return: matching compressor if config contains a sparsity config
-    """
-    config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
-    sparsity_config = getattr(config, SPARSITY_CONFIG_NAME, None)
-    if sparsity_config is None:
-        return None
-
-    format = sparsity_config.get("format")
-    sparsity_config = CompressionConfig.load_from_registry(format, **sparsity_config)
-    compressor = ModelCompressor.load_from_registry(format, config=sparsity_config)
-    return compressor
-
-
 def save_compressed(
     tensors: Dict[str, Tensor],
     save_path: Union[str, Path],
     compression_format: Optional[CompressionFormat] = None,
 ):
     """
     Save compressed tensors to disk. If tensors are not compressed,
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/compressors/sparse_bitmask.py` & `compressed-tensors-0.3.2/src/compressed_tensors/compressors/sparse_bitmask.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,17 @@
 
         return compressed_dict
 
     def decompress(
         self, path_to_model_or_tensors: str, device: str = "cpu"
     ) -> Generator[Tuple[str, Tensor], None, None]:
         """
-        Reads a bitmask compressed state dict located at path_to_model_or_tensors
-        and returns a generator for sequentially decompressing back to a dense state dict
+        Reads a bitmask compressed state dict located
+        at path_to_model_or_tensors and returns a generator
+        for sequentially decompressing back to a dense state dict
 
         :param model_path: path to compressed safetensors model (directory with
             one or more safetensors files) or compressed tensors file
         :param device: device to load decompressed weights onto
         :return: iterator for generating decompressed weights
         """
         weight_mappings = get_nested_weight_mappings(
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/config/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,10 +9,14 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # flake8: noqa
-from .base import *
-from .dense import *
-from .sparse_bitmask import *
+# isort: skip_file
+
+from .calibration import *
+from .forward import *
+from .frozen import *
+from .initialize import *
+from .apply import *
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/config/base.py` & `compressed-tensors-0.3.2/src/compressed_tensors/config/base.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/config/dense.py` & `compressed-tensors-0.3.2/src/compressed_tensors/config/dense.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/config/sparse_bitmask.py` & `compressed-tensors-0.3.2/src/compressed_tensors/config/sparse_bitmask.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,12 +11,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # flake8: noqa
 # isort: skip_file
 
-from .calibration import *
-from .forward import *
-from .frozen import *
-from .initialize import *
-from .apply import *
+from .helpers import *
+from .base import *
+from .memoryless import *
+from .min_max import *
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/apply.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/apply.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/calibration.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/calibration.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/forward.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/forward.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,30 +107,36 @@
     # bind wrapped forward to module class so reference to `self` is correct
     bound_wrapped_forward = wrapped_forward.__get__(module, module.__class__)
     # set forward to wrapped forward
     setattr(module, "forward", bound_wrapped_forward)
 
 
 def _maybe_calibrate_or_quantize(
-    module: Module, value: Module, base_name: str, args: "QuantizationArgs"
+    module: Module, value: torch.Tensor, base_name: str, args: "QuantizationArgs"
 ) -> torch.Tensor:
     # only run quantized for the included stages
     if module.quantization_status not in {
         QuantizationStatus.CALIBRATION,
         QuantizationStatus.FROZEN,
     }:
         return value
 
-    device = next(module.parameters()).device
-    scale = getattr(module, f"{base_name}_scale")
-    zero_point = getattr(module, f"{base_name}_zero_point")
-
-    if module.quantization_status == QuantizationStatus.CALIBRATION:
-        # get observer and get new quant params from observation
+    if args.dynamic:
+        # dynamic quantization - get scale and zero point directly from observer
         observer = getattr(module, f"{base_name}_observer")
-        updated_scale, updated_zero_point = observer(value)
-
-        # update scale and zero point
-        scale.data = updated_scale.to(device)
-        zero_point.data = updated_zero_point.to(device)
+        scale, zero_point = observer(value)
+    else:
+        # static quantization - get previous scale and zero point from layer
+        scale = getattr(module, f"{base_name}_scale")
+        zero_point = getattr(module, f"{base_name}_zero_point")
+
+        if module.quantization_status == QuantizationStatus.CALIBRATION:
+            # calibration mode - get new quant params from observer
+            observer = getattr(module, f"{base_name}_observer")
+            updated_scale, updated_zero_point = observer(value)
+
+            # update scale and zero point
+            device = next(module.parameters()).device
+            scale.data = updated_scale.to(device)
+            zero_point.data = updated_zero_point.to(device)
 
     return fake_quantize(value, scale, zero_point, args)
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/lifecycle/initialize.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,21 +76,24 @@
     # wrap forward call of module to perform quantized actions based on calltime status
     wrap_module_forward_quantized(module, scheme)
 
 
 def _initialize_scale_zero_point_observer(
     module: Module, base_name: str, quantization_args: QuantizationArgs
 ):
+    # initialize observer module and attach as submodule
+    observer = quantization_args.get_observer()
+    module.register_module(f"{base_name}_observer", observer)
+
+    if quantization_args.dynamic:
+        return  # no need to register a scale and zero point for a dynamic observer
+
     device = next(module.parameters()).device
 
     # initializes empty scale and zero point parameters for the module
     init_scale = Parameter(torch.empty(0, device=device), requires_grad=False)
     module.register_parameter(f"{base_name}_scale", init_scale)
 
     init_zero_point = Parameter(
         torch.empty(0, device=device, dtype=int), requires_grad=False
     )
     module.register_parameter(f"{base_name}_zero_point", init_zero_point)
-
-    # initialize observer module and attach as submodule
-    observer = quantization_args.get_observer()
-    module.register_module(f"{base_name}_observer", observer)
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,10 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 # flake8: noqa
-# isort: skip_file
 
-from .helpers import *
-from .base import *
-from .memoryless import *
-from .min_max import *
+from .safetensors_load import *
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/base.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/base.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/helpers.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/helpers.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/memoryless.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/memoryless.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from compressed_tensors.quantization.observers.helpers import calculate_qparams
 from torch import FloatTensor, IntTensor, Tensor
 
 
 __all__ = ["MemorylessObserver"]
 
 
-@Observer.register("memoryless")
+@Observer.register("memoryless", alias=["dynamic"])
 class MemorylessObserver(Observer):
     """
-    Implements a dynamic quantization observer that sets the scale and
+    Implements a quantization observer that sets the scale and
     zero point based on the latest observed value without tracking state
     """
 
     def calculate_qparams(self, observed: Tensor) -> Tuple[FloatTensor, IntTensor]:
         """
         Returns the min and max values of observed
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/observers/min_max.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/min_max.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/quant_args.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,22 +49,28 @@
     :param num_bits: quantization bit depth
     :param type: dtype to quantized to, either int or float
     :param symmetric: whether or not quantization scale is symmetric about zero-point
     :param strategy: string id determining the scope of scale/zero-point to apply
     :param group_size: group length to use for the group strategy
     :param block_structure: 2d block structure to use for the block strategy, must be
     of the format "2x4", "8x16", etc.
+    :param dynamic: set True to perform dynamic quantization - values will not be
+        calibrated during calibration phase, instead during inference new quantization
+        ranges will be observed with every sample. Defaults to False for static
+        quantization. Note that enabling dynamic quantization will change the default
+        observer to a memoryless one
     """
 
     num_bits: int = 8
     type: QuantizationType = QuantizationType.INT
     symmetric: bool = True
     strategy: QuantizationStrategy = QuantizationStrategy.TENSOR
     group_size: Optional[int] = None
     block_structure: Optional[str] = None
+    dynamic: bool = False
     observer: str = Field(
         default="minmax",
         description=(
             "The class to use to compute the quantization param - "
             "scale and zero-point'"
         ),
     )
@@ -78,8 +84,13 @@
 
     def get_observer(self):
         """
         :return: torch quantization FakeQuantize built based on these QuantizationArgs
         """
         from compressed_tensors.quantization.observers.base import Observer
 
+        if self.observer == "minmax" and self.dynamic:
+            # override defualt observer for dynamic, you never want minmax which
+            # keeps state across samples for dynamic
+            self.observer = "memoryless"
+
         return Observer.load_from_registry(self.observer, quantization_args=self)
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/quant_config.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_config.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/quant_scheme.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_scheme.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/utils/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/quantization/utils/helpers.py` & `compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/registry/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/registry/registry.py` & `compressed-tensors-0.3.2/src/compressed_tensors/registry/registry.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/utils/__init__.py` & `compressed-tensors-0.3.2/src/compressed_tensors/compressors/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,10 +7,14 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 # flake8: noqa
 
-from .safetensors_load import *
+from .base import ModelCompressor
+from .dense import DenseCompressor
+from .helpers import load_compressed, save_compressed, save_compressed_model
+from .sparse_bitmask import BitmaskCompressor, BitmaskTensor
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors/utils/safetensors_load.py` & `compressed-tensors-0.3.2/src/compressed_tensors/utils/safetensors_load.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors.egg-info/PKG-INFO` & `compressed-tensors-0.3.2/src/compressed_tensors.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressed-tensors
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for utilization of compressed safetensors of neural network models
 Home-page: https://github.com/neuralmagic/compressed-tensors
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -90,8 +90,11 @@
 # save compressed model weights
 save_compressed_model(model, "compressed_model.safetensors", compression_format=compression_config.format)
 
 # load compressed model weights (`dict` turns generator into a dictionary)
 state_dict = dict(load_compressed("compressed_model.safetensors", compression_config))
 ```
 
+For more in-depth tutorial on bitmask compression, refer to the [notebook](https://github.com/neuralmagic/compressed-tensors/blob/d707c5b84bc3fef164aebdcd97cb6eaa571982f8/examples/bitmask_compression.ipynb).
+
+
```

### Comparing `compressed-tensors-0.3.1/src/compressed_tensors.egg-info/SOURCES.txt` & `compressed-tensors-0.3.2/src/compressed_tensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/tests/test_bitmask.py` & `compressed-tensors-0.3.2/tests/test_bitmask.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.1/tests/test_registry.py` & `compressed-tensors-0.3.2/tests/test_registry.py`

 * *Files identical despite different names*

