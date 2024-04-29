# Comparing `tmp/json_advanced-0.3.0.tar.gz` & `tmp/json_advanced-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_advanced-0.3.0.tar", last modified: Mon Apr 29 14:32:30 2024, max compression
+gzip compressed data, was "json_advanced-0.4.0.tar", last modified: Mon Apr 29 14:34:33 2024, max compression
```

## Comparing `json_advanced-0.3.0.tar` & `json_advanced-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:32:30.239394 json_advanced-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 14:32:26.000000 json_advanced-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-29 14:32:30.239394 json_advanced-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-29 14:32:26.000000 json_advanced-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:32:30.235394 json_advanced-0.3.0/json-advanced/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 14:32:26.000000 json_advanced-0.3.0/json-advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-29 14:32:26.000000 json_advanced-0.3.0/json-advanced/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-29 14:32:26.000000 json_advanced-0.3.0/json-advanced/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:32:30.239394 json_advanced-0.3.0/json_advanced.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-29 14:32:30.000000 json_advanced-0.3.0/json_advanced.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 14:32:30.000000 json_advanced-0.3.0/json_advanced.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:32:30.000000 json_advanced-0.3.0/json_advanced.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:32:30.000000 json_advanced-0.3.0/json_advanced.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 14:32:30.000000 json_advanced-0.3.0/json_advanced.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:32:30.239394 json_advanced-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-29 14:32:26.000000 json_advanced-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:34:33.975018 json_advanced-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 14:34:27.000000 json_advanced-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-29 14:34:33.975018 json_advanced-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-29 14:34:27.000000 json_advanced-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:34:33.975018 json_advanced-0.4.0/json-advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 14:34:27.000000 json_advanced-0.4.0/json-advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-29 14:34:27.000000 json_advanced-0.4.0/json-advanced/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-29 14:34:27.000000 json_advanced-0.4.0/json-advanced/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:34:33.975018 json_advanced-0.4.0/json_advanced.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-29 14:34:33.000000 json_advanced-0.4.0/json_advanced.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 14:34:33.000000 json_advanced-0.4.0/json_advanced.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:34:33.000000 json_advanced-0.4.0/json_advanced.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:34:33.000000 json_advanced-0.4.0/json_advanced.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 14:34:33.000000 json_advanced-0.4.0/json_advanced.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:34:33.975018 json_advanced-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-29 14:34:27.000000 json_advanced-0.4.0/setup.py
```

### Comparing `json_advanced-0.3.0/LICENSE` & `json_advanced-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_advanced-0.3.0/PKG-INFO` & `json_advanced-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-advanced
-Version: 0.3.0
+Version: 0.4.0
 Summary: This Python package provides an extended JSON encoder class, `JSONSerializer`, that enables encoding of complex Python data types such as `datetime.datetime`, `datetime.date`, `datetime.time`, `bytes` and `uuid`. It also supports objects that have a `to_json` method, allowing for customizable JSON encoding.
 Home-page: https://github.com/mahdikiani/json-advanced
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: MIT License
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `json_advanced-0.3.0/README.md` & `json_advanced-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `json_advanced-0.3.0/json-advanced/json_encoder.py` & `json_advanced-0.4.0/json-advanced/json_encoder.py`

 * *Files identical despite different names*

### Comparing `json_advanced-0.3.0/json-advanced/test.py` & `json_advanced-0.4.0/json-advanced/test.py`

 * *Files identical despite different names*

### Comparing `json_advanced-0.3.0/json_advanced.egg-info/PKG-INFO` & `json_advanced-0.4.0/json_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-advanced
-Version: 0.3.0
+Version: 0.4.0
 Summary: This Python package provides an extended JSON encoder class, `JSONSerializer`, that enables encoding of complex Python data types such as `datetime.datetime`, `datetime.date`, `datetime.time`, `bytes` and `uuid`. It also supports objects that have a `to_json` method, allowing for customizable JSON encoding.
 Home-page: https://github.com/mahdikiani/json-advanced
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: MIT License
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `json_advanced-0.3.0/setup.py` & `json_advanced-0.4.0/setup.py`

 * *Files identical despite different names*

