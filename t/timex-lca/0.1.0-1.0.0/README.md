# Comparing `tmp/timex_lca-0.1.0.tar.gz` & `tmp/timex_lca-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timex_lca-0.1.0.tar", last modified: Mon Apr 29 12:31:02 2024, max compression
+gzip compressed data, was "timex_lca-1.0.0.tar", last modified: Mon Apr 29 12:14:13 2024, max compression
```

## Comparing `timex_lca-0.1.0.tar` & `timex_lca-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:31:02.719095 timex_lca-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-29 12:30:59.000000 timex_lca-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-29 12:31:02.719095 timex_lca-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-29 12:30:59.000000 timex_lca-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:31:02.715095 timex_lca-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 12:30:59.000000 timex_lca-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-29 12:30:59.000000 timex_lca-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:31:02.719095 timex_lca-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 12:30:59.000000 timex_lca-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:31:02.715095 timex_lca-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-29 12:30:59.000000 timex_lca-0.1.0/tests/test_amounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-29 12:30:59.000000 timex_lca-0.1.0/tests/test_bioflows.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 12:30:59.000000 timex_lca-0.1.0/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-04-29 12:30:59.000000 timex_lca-0.1.0/tests/test_temporal_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-04-29 12:30:59.000000 timex_lca-0.1.0/tests/test_temporal_groupings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:31:02.715095 timex_lca-0.1.0/timex_lca/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:31:02.715095 timex_lca-0.1.0/timex_lca/data/
--rw-r--r--   0 runner    (1001) docker     (127)    69114 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/data/hodnebrog20.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/dynamic_biosphere_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    31708 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/dynamic_characterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/edge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/matrix_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/remapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/timeline_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    35961 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/timex_lca.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-29 12:30:59.000000 timex_lca-0.1.0/timex_lca/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:31:02.719095 timex_lca-0.1.0/timex_lca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-29 12:31:02.000000 timex_lca-0.1.0/timex_lca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-29 12:31:02.000000 timex_lca-0.1.0/timex_lca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:31:02.000000 timex_lca-0.1.0/timex_lca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-29 12:31:02.000000 timex_lca-0.1.0/timex_lca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 12:31:02.000000 timex_lca-0.1.0/timex_lca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:14:13.004068 timex_lca-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-29 12:14:05.000000 timex_lca-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-29 12:14:13.004068 timex_lca-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-29 12:14:05.000000 timex_lca-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:14:13.000068 timex_lca-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 12:14:05.000000 timex_lca-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-29 12:14:06.000000 timex_lca-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:14:13.004068 timex_lca-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 12:14:06.000000 timex_lca-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:14:13.000068 timex_lca-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-29 12:14:06.000000 timex_lca-1.0.0/tests/test_amounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-29 12:14:06.000000 timex_lca-1.0.0/tests/test_bioflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 12:14:06.000000 timex_lca-1.0.0/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-04-29 12:14:06.000000 timex_lca-1.0.0/tests/test_temporal_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-04-29 12:14:06.000000 timex_lca-1.0.0/tests/test_temporal_groupings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:14:13.000068 timex_lca-1.0.0/timex_lca/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:14:13.000068 timex_lca-1.0.0/timex_lca/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    69114 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/data/hodnebrog20.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/dynamic_biosphere_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31708 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/dynamic_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/edge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/matrix_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/remapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/timeline_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35961 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/timex_lca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-29 12:14:06.000000 timex_lca-1.0.0/timex_lca/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:14:13.004068 timex_lca-1.0.0/timex_lca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-29 12:14:12.000000 timex_lca-1.0.0/timex_lca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-29 12:14:12.000000 timex_lca-1.0.0/timex_lca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:14:12.000000 timex_lca-1.0.0/timex_lca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-29 12:14:12.000000 timex_lca-1.0.0/timex_lca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 12:14:12.000000 timex_lca-1.0.0/timex_lca.egg-info/top_level.txt
```

### Comparing `timex_lca-0.1.0/LICENSE` & `timex_lca-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/PKG-INFO` & `timex_lca-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timex_lca
-Version: 0.1.0
+Version: 1.0.0
 Summary: Time-explicit Life Cycle Assessment
 Author: Amelie Müller, Arthur Jakobs
 Author-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Maintainer: Amelie Müller
 Maintainer-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Project-URL: source, https://github.com/TimoDiepers/timex
 Project-URL: homepage, https://github.com/TimoDiepers/timex
```

### Comparing `timex_lca-0.1.0/README.md` & `timex_lca-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/pyproject.toml` & `timex_lca-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/tests/test_amounts.py` & `timex_lca-1.0.0/tests/test_amounts.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/tests/test_bioflows.py` & `timex_lca-1.0.0/tests/test_bioflows.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/tests/test_temporal_distributions.py` & `timex_lca-1.0.0/tests/test_temporal_distributions.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/tests/test_temporal_groupings.py` & `timex_lca-1.0.0/tests/test_temporal_groupings.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/data/hodnebrog20.csv` & `timex_lca-1.0.0/timex_lca/data/hodnebrog20.csv`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/dynamic_biosphere_builder.py` & `timex_lca-1.0.0/timex_lca/dynamic_biosphere_builder.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/dynamic_characterization.py` & `timex_lca-1.0.0/timex_lca/dynamic_characterization.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/edge_extractor.py` & `timex_lca-1.0.0/timex_lca/edge_extractor.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/matrix_modifier.py` & `timex_lca-1.0.0/timex_lca/matrix_modifier.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/remapping.py` & `timex_lca-1.0.0/timex_lca/remapping.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/timeline_builder.py` & `timex_lca-1.0.0/timex_lca/timeline_builder.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/timex_lca.py` & `timex_lca-1.0.0/timex_lca/timex_lca.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca/utils.py` & `timex_lca-1.0.0/timex_lca/utils.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.0/timex_lca.egg-info/PKG-INFO` & `timex_lca-1.0.0/timex_lca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timex_lca
-Version: 0.1.0
+Version: 1.0.0
 Summary: Time-explicit Life Cycle Assessment
 Author: Amelie Müller, Arthur Jakobs
 Author-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Maintainer: Amelie Müller
 Maintainer-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Project-URL: source, https://github.com/TimoDiepers/timex
 Project-URL: homepage, https://github.com/TimoDiepers/timex
```

### Comparing `timex_lca-0.1.0/timex_lca.egg-info/SOURCES.txt` & `timex_lca-1.0.0/timex_lca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

