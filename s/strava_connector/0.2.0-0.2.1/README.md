# Comparing `tmp/strava_connector-0.2.0.tar.gz` & `tmp/strava_connector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strava_connector-0.2.0.tar", max compression
+gzip compressed data, was "strava_connector-0.2.1.tar", max compression
```

## Comparing `strava_connector-0.2.0.tar` & `strava_connector-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-04-29 09:03:24.918761 strava_connector-0.2.0/LICENSE
--rw-r--r--   0        0        0     1108 2024-04-29 18:10:20.657421 strava_connector-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1438 2024-04-29 17:01:42.375758 strava_connector-0.2.0/strava_connector/__init__.py
--rw-r--r--   0        0        0     3600 2024-04-29 10:33:43.309077 strava_connector-0.2.0/strava_connector/authenticator.py
--rw-r--r--   0        0        0    15144 2024-04-29 18:06:29.122919 strava_connector-0.2.0/strava_connector/connector.py
--rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 strava_connector-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-29 09:03:24.918761 strava_connector-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3491 2024-04-29 18:09:26.007046 strava_connector-0.2.1/README.md
+-rw-r--r--   0        0        0     1168 2024-04-29 18:17:52.762884 strava_connector-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1438 2024-04-29 17:01:42.375758 strava_connector-0.2.1/strava_connector/__init__.py
+-rw-r--r--   0        0        0     3600 2024-04-29 10:33:43.309077 strava_connector-0.2.1/strava_connector/authenticator.py
+-rw-r--r--   0        0        0    15144 2024-04-29 18:06:29.122919 strava_connector-0.2.1/strava_connector/connector.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 strava_connector-0.2.1/PKG-INFO
```

### Comparing `strava_connector-0.2.0/LICENSE` & `strava_connector-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strava_connector-0.2.0/pyproject.toml` & `strava_connector-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "strava_connector"
-version = "0.2.0"
-description = ""
+version = "0.2.1"
+description = "Simple Strava client written in Python"
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
+readme = "README.md"
+
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `strava_connector-0.2.0/strava_connector/__init__.py` & `strava_connector-0.2.1/strava_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `strava_connector-0.2.0/strava_connector/authenticator.py` & `strava_connector-0.2.1/strava_connector/authenticator.py`

 * *Files identical despite different names*

### Comparing `strava_connector-0.2.0/strava_connector/connector.py` & `strava_connector-0.2.1/strava_connector/connector.py`

 * *Files identical despite different names*

