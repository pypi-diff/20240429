# Comparing `tmp/aau_ais_utilities-0.1.0.tar.gz` & `tmp/aau_ais_utilities-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_utilities-0.1.0.tar", last modified: Wed Apr 24 12:48:52 2024, max compression
+gzip compressed data, was "aau_ais_utilities-0.1.1.tar", last modified: Mon Apr 29 09:56:48 2024, max compression
```

## Comparing `aau_ais_utilities-0.1.0.tar` & `aau_ais_utilities-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      145 2024-04-19 08:48:38.959957 aau_ais_utilities-0.1.0/README.md
--rw-r--r--   0        0        0      596 2024-04-24 12:48:52.671266 aau_ais_utilities-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 12:04:56.661628 aau_ais_utilities-0.1.0/src/aau_ais_utilities/__init__.py
--rw-r--r--   0        0        0       93 2024-04-24 09:00:02.991569 aau_ais_utilities-0.1.0/src/aau_ais_utilities/connections/__init__.py
--rw-r--r--   0        0        0     1762 2024-04-17 12:06:39.000000 aau_ais_utilities-0.1.0/src/aau_ais_utilities/connections/postgresql_connection.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:29.563946 aau_ais_utilities-0.1.0/src/aau_ais_utilities/lookup/__init__.py
--rw-r--r--   0        0        0    18270 2024-04-24 11:56:27.025069 aau_ais_utilities-0.1.0/src/aau_ais_utilities/lookup/mmsi.py
--rw-r--r--   0        0        0      111 2024-04-17 06:44:56.872198 aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-17 06:44:56.873437 aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/imo.py
--rw-r--r--   0        0        0     1136 2024-04-17 06:44:56.873437 aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/mmsi.py
--rw-r--r--   0        0        0     1253 2024-04-17 06:44:56.874519 aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/validator.py
--rw-r--r--   0        0        0     1534 2024-04-24 11:56:27.052662 aau_ais_utilities-0.1.0/tests/validate/test_imo.py
--rw-r--r--   0        0        0        0 2024-04-10 14:19:47.264802 aau_ais_utilities-0.1.0/tests/validate/test_mmsi.py
--rw-r--r--   0        0        0        0 2024-04-17 06:44:56.878541 aau_ais_utilities-0.1.0/tests/validate/test_validator.py
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 aau_ais_utilities-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      145 2024-04-19 08:48:38.959957 aau_ais_utilities-0.1.1/README.md
+-rw-r--r--   0        0        0      628 2024-04-29 09:56:48.375833 aau_ais_utilities-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 12:04:56.661628 aau_ais_utilities-0.1.1/src/aau_ais_utilities/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-25 09:08:00.197116 aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/__init__.py
+-rw-r--r--   0        0        0      504 2024-04-29 09:43:50.319740 aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/engine_settings.py
+-rw-r--r--   0        0        0     1762 2024-04-17 12:06:39.000000 aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/postgresql_connection.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:29.563946 aau_ais_utilities-0.1.1/src/aau_ais_utilities/lookup/__init__.py
+-rw-r--r--   0        0        0    18270 2024-04-24 11:56:27.025069 aau_ais_utilities-0.1.1/src/aau_ais_utilities/lookup/mmsi.py
+-rw-r--r--   0        0        0      111 2024-04-17 06:44:56.872198 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-17 06:44:56.873437 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/imo.py
+-rw-r--r--   0        0        0     1136 2024-04-17 06:44:56.873437 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/mmsi.py
+-rw-r--r--   0        0        0     1253 2024-04-17 06:44:56.874519 aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/validator.py
+-rw-r--r--   0        0        0     1534 2024-04-24 11:56:27.052662 aau_ais_utilities-0.1.1/tests/validate/test_imo.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:19:47.264802 aau_ais_utilities-0.1.1/tests/validate/test_mmsi.py
+-rw-r--r--   0        0        0        0 2024-04-17 06:44:56.878541 aau_ais_utilities-0.1.1/tests/validate/test_validator.py
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 aau_ais_utilities-0.1.1/PKG-INFO
```

### Comparing `aau_ais_utilities-0.1.0/pyproject.toml` & `aau_ais_utilities-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "aau-ais-utilities"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utilities for working with the AAU AIS database."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "sqlalchemy==2.0.*",
+    "pydantic-settings==2.2.*",
 ]
 requires-python = "==3.12.*"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `aau_ais_utilities-0.1.0/src/aau_ais_utilities/connections/postgresql_connection.py` & `aau_ais_utilities-0.1.1/src/aau_ais_utilities/connections/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.0/src/aau_ais_utilities/lookup/mmsi.py` & `aau_ais_utilities-0.1.1/src/aau_ais_utilities/lookup/mmsi.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/imo.py` & `aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/imo.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/mmsi.py` & `aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/mmsi.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.0/src/aau_ais_utilities/validate/validator.py` & `aau_ais_utilities-0.1.1/src/aau_ais_utilities/validate/validator.py`

 * *Files identical despite different names*

### Comparing `aau_ais_utilities-0.1.0/tests/validate/test_imo.py` & `aau_ais_utilities-0.1.1/tests/validate/test_imo.py`

 * *Files identical despite different names*

