# Comparing `tmp/aau_ais_dipaal-0.1.1.tar.gz` & `tmp/aau_ais_dipaal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_dipaal-0.1.1.tar", last modified: Mon Apr 29 09:53:01 2024, max compression
+gzip compressed data, was "aau_ais_dipaal-0.1.2.tar", last modified: Mon Apr 29 09:57:13 2024, max compression
```

## Comparing `aau_ais_dipaal-0.1.1.tar` & `aau_ais_dipaal-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      139 2024-04-18 10:19:07.540695 aau_ais_dipaal-0.1.1/README.md
--rw-r--r--   0        0        0      670 2024-04-29 09:53:01.166226 aau_ais_dipaal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:59:12.781590 aau_ais_dipaal-0.1.1/src/dipaal/__init__.py
--rw-r--r--   0        0        0      244 2024-04-17 14:41:48.579028 aau_ais_dipaal-0.1.1/src/dipaal/convert/__init__.py
--rw-r--r--   0        0        0     1207 2024-04-25 09:28:54.746754 aau_ais_dipaal-0.1.1/src/dipaal/convert/callsign.py
--rw-r--r--   0        0        0     1544 2024-04-29 09:09:13.050378 aau_ais_dipaal-0.1.1/src/dipaal/convert/converter.py
--rw-r--r--   0        0        0     1177 2024-04-25 09:28:54.789569 aau_ais_dipaal-0.1.1/src/dipaal/convert/imo.py
--rw-r--r--   0        0        0     1187 2024-04-25 09:28:54.736736 aau_ais_dipaal-0.1.1/src/dipaal/convert/mmsi.py
--rw-r--r--   0        0        0      152 2024-04-23 11:19:37.881658 aau_ais_dipaal-0.1.1/src/dipaal/export/__init__.py
--rw-r--r--   0        0        0     5913 2024-04-24 11:38:06.792730 aau_ais_dipaal-0.1.1/src/dipaal/export/exporter.py
--rw-r--r--   0        0        0     4077 2024-04-24 12:04:56.635681 aau_ais_dipaal-0.1.1/src/dipaal/export/map_exporter.py
--rw-r--r--   0        0        0        0 2024-04-23 14:21:24.000145 aau_ais_dipaal-0.1.1/src/dipaal/export/sql/map_exporter/exists/enc.sql
--rw-r--r--   0        0        0        0 2024-04-23 14:21:52.095786 aau_ais_dipaal-0.1.1/src/dipaal/export/sql/map_exporter/exists/ship_type.sql
--rw-r--r--   0        0        0      401 2024-04-29 09:31:48.467158 aau_ais_dipaal-0.1.1/src/dipaal/settings.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      139 2024-04-18 10:19:07.540695 aau_ais_dipaal-0.1.2/README.md
+-rw-r--r--   0        0        0      670 2024-04-29 09:57:13.169032 aau_ais_dipaal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:59:12.781590 aau_ais_dipaal-0.1.2/src/dipaal/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-17 14:41:48.579028 aau_ais_dipaal-0.1.2/src/dipaal/convert/__init__.py
+-rw-r--r--   0        0        0     1207 2024-04-25 09:28:54.746754 aau_ais_dipaal-0.1.2/src/dipaal/convert/callsign.py
+-rw-r--r--   0        0        0     1544 2024-04-29 09:09:13.050378 aau_ais_dipaal-0.1.2/src/dipaal/convert/converter.py
+-rw-r--r--   0        0        0     1177 2024-04-25 09:28:54.789569 aau_ais_dipaal-0.1.2/src/dipaal/convert/imo.py
+-rw-r--r--   0        0        0     1187 2024-04-25 09:28:54.736736 aau_ais_dipaal-0.1.2/src/dipaal/convert/mmsi.py
+-rw-r--r--   0        0        0      152 2024-04-23 11:19:37.881658 aau_ais_dipaal-0.1.2/src/dipaal/export/__init__.py
+-rw-r--r--   0        0        0     5913 2024-04-24 11:38:06.792730 aau_ais_dipaal-0.1.2/src/dipaal/export/exporter.py
+-rw-r--r--   0        0        0     4077 2024-04-24 12:04:56.635681 aau_ais_dipaal-0.1.2/src/dipaal/export/map_exporter.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:21:24.000145 aau_ais_dipaal-0.1.2/src/dipaal/export/sql/map_exporter/exists/enc.sql
+-rw-r--r--   0        0        0        0 2024-04-23 14:21:52.095786 aau_ais_dipaal-0.1.2/src/dipaal/export/sql/map_exporter/exists/ship_type.sql
+-rw-r--r--   0        0        0      401 2024-04-29 09:31:48.467158 aau_ais_dipaal-0.1.2/src/dipaal/settings.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.2/PKG-INFO
```

### Comparing `aau_ais_dipaal-0.1.1/pyproject.toml` & `aau_ais_dipaal-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aau-ais-dipaal"
-version = "0.1.1"
+version = "0.1.2"
 description = "TODO: Add a description of your project."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "aau-ais-utilities==0.1.*",
     "pydantic==2.7.*",
```

### Comparing `aau_ais_dipaal-0.1.1/src/dipaal/convert/callsign.py` & `aau_ais_dipaal-0.1.2/src/dipaal/convert/callsign.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.1/src/dipaal/convert/converter.py` & `aau_ais_dipaal-0.1.2/src/dipaal/convert/converter.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.1/src/dipaal/convert/imo.py` & `aau_ais_dipaal-0.1.2/src/dipaal/convert/imo.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.1/src/dipaal/convert/mmsi.py` & `aau_ais_dipaal-0.1.2/src/dipaal/convert/mmsi.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.1/src/dipaal/export/exporter.py` & `aau_ais_dipaal-0.1.2/src/dipaal/export/exporter.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.1/src/dipaal/export/map_exporter.py` & `aau_ais_dipaal-0.1.2/src/dipaal/export/map_exporter.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.1/PKG-INFO` & `aau_ais_dipaal-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aau-ais-dipaal
-Version: 0.1.1
+Version: 0.1.2
 Summary: TODO: Add a description of your project.
 Author-Email: Mikael Vind Mikkelsen <mvmi@cs.aau.dk>
 License: MIT
 Requires-Python: ==3.12.*
 Requires-Dist: aau-ais-utilities==0.1.*
 Requires-Dist: pydantic==2.7.*
 Requires-Dist: pydantic-settings==2.2.*
```

