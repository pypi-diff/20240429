# Comparing `tmp/hqstage-0.0.0.tar.gz` & `tmp/hqstage-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqstage-0.0.0.tar", last modified: Mon Apr 29 13:31:42 2024, max compression
+gzip compressed data, was "hqstage-0.0.1.tar", last modified: Mon Apr 29 14:40:37 2024, max compression
```

## Comparing `hqstage-0.0.0.tar` & `hqstage-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 13:31:42.355516 hqstage-0.0.0/
--rw-r--r--   0 hqs       (4242) hqs       (4242)      397 2024-04-29 13:31:42.355516 hqstage-0.0.0/PKG-INFO
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      108 2024-04-29 12:55:33.000000 hqstage-0.0.0/README.md
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)     2952 2024-04-29 13:04:34.000000 hqstage-0.0.0/pyproject.toml
--rw-r--r--   0 hqs       (4242) hqs       (4242)       38 2024-04-29 13:31:42.355516 hqstage-0.0.0/setup.cfg
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)     1208 2024-04-29 13:14:17.000000 hqstage-0.0.0/setup.py
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 13:31:42.351516 hqstage-0.0.0/src/
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 13:31:42.355516 hqstage-0.0.0/src/hqstage/
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      175 2024-04-29 13:10:18.000000 hqstage-0.0.0/src/hqstage/__init__.py
--rw-rw-rw-   0 hqs       (4242) hqs       (4242)      629 2024-04-29 13:14:17.000000 hqstage-0.0.0/src/hqstage/cli.py
-drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 13:31:42.355516 hqstage-0.0.0/src/hqstage.egg-info/
--rw-r--r--   0 hqs       (4242) hqs       (4242)      397 2024-04-29 13:31:42.000000 hqstage-0.0.0/src/hqstage.egg-info/PKG-INFO
--rw-r--r--   0 hqs       (4242) hqs       (4242)      254 2024-04-29 13:31:42.000000 hqstage-0.0.0/src/hqstage.egg-info/SOURCES.txt
--rw-r--r--   0 hqs       (4242) hqs       (4242)        1 2024-04-29 13:31:42.000000 hqstage-0.0.0/src/hqstage.egg-info/dependency_links.txt
--rw-r--r--   0 hqs       (4242) hqs       (4242)       45 2024-04-29 13:31:42.000000 hqstage-0.0.0/src/hqstage.egg-info/entry_points.txt
--rw-r--r--   0 hqs       (4242) hqs       (4242)        8 2024-04-29 13:31:42.000000 hqstage-0.0.0/src/hqstage.egg-info/top_level.txt
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.157738 hqstage-0.0.1/
+-rw-r--r--   0 hqs       (4242) hqs       (4242)      646 2024-04-29 14:40:37.153738 hqstage-0.0.1/PKG-INFO
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      108 2024-04-29 13:12:50.000000 hqstage-0.0.1/README.md
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      265 2024-04-29 14:40:07.000000 hqstage-0.0.1/README_pypi_org.md
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)     2935 2024-04-29 14:40:07.000000 hqstage-0.0.1/pyproject.toml
+-rw-r--r--   0 hqs       (4242) hqs       (4242)       38 2024-04-29 14:40:37.157738 hqstage-0.0.1/setup.cfg
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)     1208 2024-04-29 13:12:50.000000 hqstage-0.0.1/setup.py
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.153738 hqstage-0.0.1/src/
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.153738 hqstage-0.0.1/src/hqstage/
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      175 2024-04-29 13:12:50.000000 hqstage-0.0.1/src/hqstage/__init__.py
+-rw-rw-rw-   0 hqs       (4242) hqs       (4242)      629 2024-04-29 13:12:50.000000 hqstage-0.0.1/src/hqstage/cli.py
+drwxr-xr-x   0 hqs       (4242) hqs       (4242)        0 2024-04-29 14:40:37.153738 hqstage-0.0.1/src/hqstage.egg-info/
+-rw-r--r--   0 hqs       (4242) hqs       (4242)      646 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/PKG-INFO
+-rw-r--r--   0 hqs       (4242) hqs       (4242)      273 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/SOURCES.txt
+-rw-r--r--   0 hqs       (4242) hqs       (4242)        1 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/dependency_links.txt
+-rw-r--r--   0 hqs       (4242) hqs       (4242)       45 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/entry_points.txt
+-rw-r--r--   0 hqs       (4242) hqs       (4242)        8 2024-04-29 14:40:37.000000 hqstage-0.0.1/src/hqstage.egg-info/top_level.txt
```

### Comparing `hqstage-0.0.0/pyproject.toml` & `hqstage-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 maintainers = [
     {name="Sebastian Lehmann", email="sebastian.lehmann@quantumsimulations.de"}
 ]
 requires-python = ">=3.9"
 dynamic = ["version"]
 dependencies = []
-description = "Dummy package for hqstage - For the real package please refer to https://docs.cloud.quantumsimulations.de/installation.html"
+description = "Dummy package for hqstage - For the real package please refer to https://docs.cloud.quantumsimulations.de/"
 readme = "README_pypi_org.md"
 
 
 [build-system]
 # requires = ["setuptools", "setuptools-scm", "toml", "wheel", "nuitka"]
 # build-backend = "nuitka.distutils.Build"
 requires = ["setuptools", "setuptools-scm"]
```

### Comparing `hqstage-0.0.0/setup.py` & `hqstage-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `hqstage-0.0.0/src/hqstage/cli.py` & `hqstage-0.0.1/src/hqstage/cli.py`

 * *Files identical despite different names*

