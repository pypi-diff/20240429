# Comparing `tmp/clidapp4rhino-0.0.1.tar.gz` & `tmp/clidapp4rhino-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidapp4rhino-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "clidapp4rhino-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `clidapp4rhino-0.0.1.tar` & `clidapp4rhino-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      228 2024-04-25 18:44:24.896765 clidapp4rhino-0.0.1/README.md
--rw-r--r--   0        0        0      795 2024-04-25 19:24:50.765280 clidapp4rhino-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0  7665296 2024-04-25 18:41:17.947977 clidapp4rhino-0.0.1/src/CliDApp4Rhino/CliDApp4Rhino
--rw-r--r--   0        0        0        0 2024-04-25 18:38:22.496959 clidapp4rhino-0.0.1/src/CliDApp4Rhino/__init__.py
--rw-r--r--   0        0        0      178 2024-04-25 19:23:01.643410 clidapp4rhino-0.0.1/src/CliDApp4Rhino/run_executable.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 clidapp4rhino-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3146 2024-04-29 18:37:05.305419 clidapp4rhino-0.0.2/README.md
+-rw-r--r--   0        0        0      797 2024-04-29 13:44:45.153783 clidapp4rhino-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0  7665296 2024-04-25 18:41:17.947977 clidapp4rhino-0.0.2/src/CliDApp4Rhino/CliDApp4Rhino
+-rw-r--r--   0        0        0        0 2024-04-25 18:38:22.496959 clidapp4rhino-0.0.2/src/CliDApp4Rhino/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-29 18:05:13.790965 clidapp4rhino-0.0.2/src/CliDApp4Rhino/run_executable.py
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 clidapp4rhino-0.0.2/PKG-INFO
```

### Comparing `clidapp4rhino-0.0.1/pyproject.toml` & `clidapp4rhino-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "CliDApp4Rhino"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Elizabeth Consulting International Inc.", email="info@ec-intl.com" },
 ]
-description = "CliDApp4Rhino is a command line interface for the Rhino 3D CAD software."
+description = "CliDApp4Rhino is a graphical user interface for the Rhino 3D CAD software."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `clidapp4rhino-0.0.1/src/CliDApp4Rhino/CliDApp4Rhino` & `clidapp4rhino-0.0.2/src/CliDApp4Rhino/CliDApp4Rhino`

 * *Files identical despite different names*

