# Comparing `tmp/anemoi-datasets-0.1.2.tar.gz` & `tmp/anemoi-datasets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi-datasets-0.1.2.tar", last modified: Thu Apr 25 10:30:50 2024, max compression
+gzip compressed data, was "anemoi-datasets-0.1.4.tar", last modified: Mon Apr 29 09:36:45 2024, max compression
```

## Comparing `anemoi-datasets-0.1.2.tar` & `anemoi-datasets-0.1.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.263010 anemoi-datasets-0.1.2/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.263010 anemoi-datasets-0.1.2/anemoi/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.263010 anemoi-datasets-0.1.2/anemoi/datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.263010 anemoi-datasets-0.1.2/anemoi/datasets/commands/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/inspect/zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/commands/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.267010 anemoi-datasets-0.1.2/anemoi/datasets/create/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.267010 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.267010 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/accumulations.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/tendencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.267010 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/rotate_winds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/unrotate_winds.py
--rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    20490 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/loaders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/create/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/anemoi/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/forewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/masked.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/data/unchecked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/anemoi/datasets/dates/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/dates/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/anemoi/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/anemoi/datasets/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:30:50.000000 anemoi-datasets-0.1.2/anemoi_datasets.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:30:50.271010 anemoi-datasets-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-25 10:30:40.000000 anemoi-datasets-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.441787 anemoi-datasets-0.1.4/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.445787 anemoi-datasets-0.1.4/anemoi/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.445787 anemoi-datasets-0.1.4/anemoi/datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.445787 anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/commands/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/accumulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/tendencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.449787 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rotate_winds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/unrotate_winds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20490 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/loaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/create/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/forewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/masked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/data/unchecked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi/datasets/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/dates/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/anemoi/datasets/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:36:45.000000 anemoi-datasets-0.1.4/anemoi_datasets.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:36:45.453787 anemoi-datasets-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-29 09:36:32.000000 anemoi-datasets-0.1.4/setup.py
```

### Comparing `anemoi-datasets-0.1.2/LICENSE` & `anemoi-datasets-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/PKG-INFO` & `anemoi-datasets-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-datasets
-Version: 0.1.2
+Version: 0.1.4
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Home-page: https://github.com/ecmwf/anemoi-datasets
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `anemoi-datasets-0.1.2/README.md` & `anemoi-datasets-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # nor does it submit to any jurisdiction.
 
 from .data import MissingDateError
 from .data import add_dataset_path
 from .data import add_named_dataset
 from .data import open_dataset
 
-__version__ = "0.1.2"
+__version__ = "0.1.4"
 
 __all__ = [
     "open_dataset",
     "MissingDateError",
     "add_dataset_path",
     "add_named_dataset",
 ]
```

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/__main__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/compare.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/compare.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/copy.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/copy.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/create.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/create.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/inspect/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/inspect/zarr.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/inspect/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/commands/scan.py` & `anemoi-datasets-0.1.4/anemoi/datasets/commands/scan.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/check.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/check.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/config.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/config.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/accumulations.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/accumulations.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/constants.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/constants.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/forcings.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/forcings.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/grib.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/mars.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/mars.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/netcdf.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/netcdf.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/opendap.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/opendap.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/perturbations.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/perturbations.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/source.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/source.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/actions/tendencies.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/actions/tendencies.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/empty.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/empty.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/rename.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rename.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/rotate_winds.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/rotate_winds.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/functions/filters/unrotate_winds.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/functions/filters/unrotate_winds.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/input.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/input.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/loaders.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/loaders.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/patch.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/patch.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/statistics.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     raise ValueError("Negative variance")
 
 
 def compute_statistics(array, check_variables_names=None, allow_nan=False):
     nvars = array.shape[1]
 
-    LOG.info(f"Stats {nvars}, {array.shape}, {check_variables_names}")
+    LOG.info("Stats %s", (nvars, array.shape, check_variables_names))
     if check_variables_names:
         assert nvars == len(check_variables_names), (nvars, check_variables_names)
     stats_shape = (array.shape[0], nvars)
 
     count = np.zeros(stats_shape, dtype=np.int64)
     sums = np.zeros(stats_shape, dtype=np.float64)
     squares = np.zeros(stats_shape, dtype=np.float64)
```

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/template.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/template.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/utils.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/utils.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/writer.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/writer.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/create/zarr.py` & `anemoi-datasets-0.1.4/anemoi/datasets/create/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/concat.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/concat.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/dataset.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/dataset.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/debug.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/debug.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/ensemble.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/ensemble.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/forewards.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/forewards.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/grids.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/grids.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/indexing.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/indexing.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/join.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/join.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/masked.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/masked.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/misc.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/misc.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/select.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/select.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/statistics.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class Statistics(Forwards):
     def __init__(self, dataset, statistic):
         super().__init__(dataset)
-        self._statistic = open_dataset(statistic)
+        self._statistic = open_dataset(statistic, select=dataset.variables)
         # TODO: relax that check to allow for a subset of variables
         if dataset.variables != self._statistic.variables:
             raise ValueError(
                 f"Incompatible variables: {dataset.variables} and {self._statistic.variables} ({dataset} {self._statistic})"
             )
 
     @cached_property
```

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/stores.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/stores.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/subset.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/subset.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/data/unchecked.py` & `anemoi-datasets-0.1.4/anemoi/datasets/data/unchecked.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/dates/__init__.py` & `anemoi-datasets-0.1.4/anemoi/datasets/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/dates/groups.py` & `anemoi-datasets-0.1.4/anemoi/datasets/dates/groups.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi/datasets/grids.py` & `anemoi-datasets-0.1.4/anemoi/datasets/grids.py`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi_datasets.egg-info/PKG-INFO` & `anemoi-datasets-0.1.4/anemoi_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-datasets
-Version: 0.1.2
+Version: 0.1.4
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Home-page: https://github.com/ecmwf/anemoi-datasets
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `anemoi-datasets-0.1.2/anemoi_datasets.egg-info/SOURCES.txt` & `anemoi-datasets-0.1.4/anemoi_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/anemoi_datasets.egg-info/requires.txt` & `anemoi-datasets-0.1.4/anemoi_datasets.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `anemoi-datasets-0.1.2/setup.py` & `anemoi-datasets-0.1.4/setup.py`

 * *Files identical despite different names*

