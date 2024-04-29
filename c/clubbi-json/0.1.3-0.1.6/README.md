# Comparing `tmp/clubbi_json-0.1.3.tar.gz` & `tmp/clubbi_json-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clubbi_json-0.1.3.tar", last modified: Fri Apr 12 18:04:29 2024, max compression
+gzip compressed data, was "clubbi_json-0.1.6.tar", last modified: Mon Apr 29 18:44:10 2024, max compression
```

## Comparing `clubbi_json-0.1.3.tar` & `clubbi_json-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:04:29.599408 clubbi_json-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 18:04:29.599408 clubbi_json-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:04:29.595409 clubbi_json-0.1.3/clubbi_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/clubbi_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/clubbi_json/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:04:29.599408 clubbi_json-0.1.3/clubbi_json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 18:04:29.000000 clubbi_json-0.1.3/clubbi_json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 18:04:29.000000 clubbi_json-0.1.3/clubbi_json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:04:29.000000 clubbi_json-0.1.3/clubbi_json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 18:04:29.000000 clubbi_json-0.1.3/clubbi_json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-12 18:04:29.599408 clubbi_json-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:04:29.599408 clubbi_json-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/tests/test_default_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 18:04:04.000000 clubbi_json-0.1.3/tests/test_orjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:44:10.759357 clubbi_json-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 18:44:10.759357 clubbi_json-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:44:10.759357 clubbi_json-0.1.6/clubbi_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/clubbi_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/clubbi_json/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:44:10.759357 clubbi_json-0.1.6/clubbi_json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 18:44:10.000000 clubbi_json-0.1.6/clubbi_json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 18:44:10.000000 clubbi_json-0.1.6/clubbi_json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:44:10.000000 clubbi_json-0.1.6/clubbi_json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 18:44:10.000000 clubbi_json-0.1.6/clubbi_json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-29 18:44:10.759357 clubbi_json-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:44:10.759357 clubbi_json-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/tests/test_default_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-29 18:43:51.000000 clubbi_json-0.1.6/tests/test_orjson.py
```

### Comparing `clubbi_json-0.1.3/LICENSE` & `clubbi_json-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clubbi_json-0.1.3/clubbi_json/json.py` & `clubbi_json-0.1.6/clubbi_json/json.py`

 * *Files identical despite different names*

### Comparing `clubbi_json-0.1.3/setup.cfg` & `clubbi_json-0.1.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [metadata]
 name = clubbi-json
-version = 0.1.3
-long_description = Several helper functions, decorators and layers
-long_description_content_type = text/plain
-description-file = README.md
+version = 0.1.6
 license_file = LICENSE
+long_description = Este pacote tem como finalidade facilitar a serialização e desserialização de JSON
+long_description_content_type = text/plain
 
 [options.package_data]
 clubbi_json = py.typed
 
 [tool:pytest]
 addopts = -p no:warnings
 testpaths = tests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clubbi_json-0.1.3/tests/test_default_json.py` & `clubbi_json-0.1.6/tests/test_default_json.py`

 * *Files identical despite different names*

