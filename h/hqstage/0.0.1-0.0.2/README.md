# Comparing `tmp/hqstage-0.0.1.tar.gz` & `tmp/hqstage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqstage-0.0.1.tar", last modified: Mon Apr 29 14:40:37 2024, max compression
+gzip compressed data, was "hqstage-0.0.2.tar", last modified: Mon Apr 29 14:53:59 2024, max compression
```

## Comparing `hqstage-0.0.1.tar` & `hqstage-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.157738 hqstage-0.0.1/
--rw-r--r--   0 hqs       (4242) hqs       (4242)      646 2024-04-29 14:40:37.153738 hqstage-0.0.1/PKG-INFO
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      108 2024-04-29 13:12:50.000000 hqstage-0.0.1/README.md
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      265 2024-04-29 14:40:07.000000 hqstage-0.0.1/README_pypi_org.md
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)     2935 2024-04-29 14:40:07.000000 hqstage-0.0.1/pyproject.toml
--rw-r--r--   0 hqs       (4242) hqs       (4242)       38 2024-04-29 14:40:37.157738 hqstage-0.0.1/setup.cfg
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)     1208 2024-04-29 13:12:50.000000 hqstage-0.0.1/setup.py
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.153738 hqstage-0.0.1/src/
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.153738 hqstage-0.0.1/src/hqstage/
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      175 2024-04-29 13:12:50.000000 hqstage-0.0.1/src/hqstage/__init__.py
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      629 2024-04-29 13:12:50.000000 hqstage-0.0.1/src/hqstage/cli.py
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.153738 hqstage-0.0.1/src/hqstage.egg-info/
--rw-r--r--   0 hqs       (4242) hqs       (4242)      646 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/PKG-INFO
--rw-r--r--   0 hqs       (4242) hqs       (4242)      273 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/SOURCES.txt
--rw-r--r--   0 hqs       (4242) hqs       (4242)        1 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/dependency_links.txt
--rw-r--r--   0 hqs       (4242) hqs       (4242)       45 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/entry_points.txt
--rw-r--r--   0 hqs       (4242) hqs       (4242)        8 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/top_level.txt
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:53:59.394239 hqstage-0.0.2/
+-rw-r--r--   0 hqs       (4242) hqs       (4242)      646 2024-04-29 14:53:59.394239 hqstage-0.0.2/PKG-INFO
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      108 2024-04-29 12:55:33.000000 hqstage-0.0.2/README.md
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      265 2024-04-29 14:39:47.000000 hqstage-0.0.2/README_pypi_org.md
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)     2935 2024-04-29 13:36:44.000000 hqstage-0.0.2/pyproject.toml
+-rw-r--r--   0 hqs       (4242) hqs       (4242)       38 2024-04-29 14:53:59.394239 hqstage-0.0.2/setup.cfg
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      759 2024-04-29 14:51:42.000000 hqstage-0.0.2/setup.py
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:53:59.394239 hqstage-0.0.2/src/
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:53:59.394239 hqstage-0.0.2/src/hqstage/
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      175 2024-04-29 13:10:18.000000 hqstage-0.0.2/src/hqstage/__init__.py
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      629 2024-04-29 13:14:17.000000 hqstage-0.0.2/src/hqstage/cli.py
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:53:59.394239 hqstage-0.0.2/src/hqstage.egg-info/
+-rw-r--r--   0 hqs       (4242) hqs       (4242)      646 2024-04-29 14:53:59.000000 hqstage-0.0.2/src/hqstage.egg-info/PKG-INFO
+-rw-r--r--   0 hqs       (4242) hqs       (4242)      273 2024-04-29 14:53:59.000000 hqstage-0.0.2/src/hqstage.egg-info/SOURCES.txt
+-rw-r--r--   0 hqs       (4242) hqs       (4242)        1 2024-04-29 14:53:59.000000 hqstage-0.0.2/src/hqstage.egg-info/dependency_links.txt
+-rw-r--r--   0 hqs       (4242) hqs       (4242)       45 2024-04-29 14:53:59.000000 hqstage-0.0.2/src/hqstage.egg-info/entry_points.txt
+-rw-r--r--   0 hqs       (4242) hqs       (4242)        8 2024-04-29 14:53:59.000000 hqstage-0.0.2/src/hqstage.egg-info/top_level.txt
```

### Comparing `hqstage-0.0.1/PKG-INFO` & `hqstage-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hqstage
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dummy package for hqstage - For the real package please refer to https://docs.cloud.quantumsimulations.de/
 Author-email: HQS Quantum Simulations GmbH <info@quantumsimulations.de>
 Maintainer-email: Sebastian Lehmann <sebastian.lehmann@quantumsimulations.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # HQStage Dummy Package
```

### Comparing `hqstage-0.0.1/pyproject.toml` & `hqstage-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hqstage-0.0.1/src/hqstage/cli.py` & `hqstage-0.0.2/src/hqstage/cli.py`

 * *Files identical despite different names*

### Comparing `hqstage-0.0.1/src/hqstage.egg-info/PKG-INFO` & `hqstage-0.0.2/src/hqstage.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hqstage
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dummy package for hqstage - For the real package please refer to https://docs.cloud.quantumsimulations.de/
 Author-email: HQS Quantum Simulations GmbH <info@quantumsimulations.de>
 Maintainer-email: Sebastian Lehmann <sebastian.lehmann@quantumsimulations.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # HQStage Dummy Package
```

