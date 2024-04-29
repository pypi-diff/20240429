# Comparing `tmp/edgegap_consul-0.1.0.tar.gz` & `tmp/edgegap_consul-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_consul-0.1.0.tar", max compression
+gzip compressed data, was "edgegap_consul-1.0.0.tar", max compression
```

## Comparing `edgegap_consul-0.1.0.tar` & `edgegap_consul-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.381361 edgegap_consul-0.1.0/LICENSE
--rw-r--r--   0        0        0     2152 2024-04-29 14:44:44.636670 edgegap_consul-0.1.0/README.md
--rw-r--r--   0        0        0      256 2024-04-29 14:26:08.858675 edgegap_consul-0.1.0/edgegap_consul/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-25 13:10:38.952731 edgegap_consul-0.1.0/edgegap_consul/_client.py
--rw-r--r--   0        0        0      399 2024-04-25 13:10:38.952817 edgegap_consul-0.1.0/edgegap_consul/_configuration.py
--rw-r--r--   0        0        0     1298 2024-04-25 13:10:38.952904 edgegap_consul-0.1.0/edgegap_consul/_factory.py
--rw-r--r--   0        0        0     1471 2024-04-29 14:26:08.851323 edgegap_consul-0.1.0/edgegap_consul/_reader.py
--rw-r--r--   0        0        0      519 2024-04-29 14:48:34.028276 edgegap_consul-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 edgegap_consul-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2152 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/README.md
+-rw-r--r--   0        0        0      256 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/edgegap_consul/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/edgegap_consul/_client.py
+-rw-r--r--   0        0        0      399 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/edgegap_consul/_configuration.py
+-rw-r--r--   0        0        0     1298 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/edgegap_consul/_factory.py
+-rw-r--r--   0        0        0     1471 2024-04-29 18:13:42.710660 edgegap_consul-1.0.0/edgegap_consul/_reader.py
+-rw-r--r--   0        0        0      519 2024-04-29 18:13:48.778693 edgegap_consul-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.0.0/PKG-INFO
```

### Comparing `edgegap_consul-0.1.0/LICENSE` & `edgegap_consul-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_consul-0.1.0/README.md` & `edgegap_consul-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_consul-0.1.0/edgegap_consul/_client.py` & `edgegap_consul-1.0.0/edgegap_consul/_client.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-0.1.0/edgegap_consul/_factory.py` & `edgegap_consul-1.0.0/edgegap_consul/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-0.1.0/edgegap_consul/_reader.py` & `edgegap_consul-1.0.0/edgegap_consul/_reader.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-0.1.0/pyproject.toml` & `edgegap_consul-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-consul"
-version = "0.1.0"
+version = "1.0.0"
 description = "The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_consul-0.1.0/PKG-INFO` & `edgegap_consul-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-consul
-Version: 0.1.0
+Version: 1.0.0
 Summary: The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp[speedups] (>=3.9.5,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: python-consul (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Consul Library
```

