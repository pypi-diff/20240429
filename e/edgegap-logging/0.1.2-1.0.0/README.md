# Comparing `tmp/edgegap_logging-0.1.2.tar.gz` & `tmp/edgegap_logging-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-0.1.2.tar", max compression
+gzip compressed data, was "edgegap_logging-1.0.0.tar", max compression
```

## Comparing `edgegap_logging-0.1.2.tar` & `edgegap_logging-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.379038 edgegap_logging-0.1.2/LICENSE
--rw-r--r--   0        0        0     2216 2024-04-29 14:47:02.453948 edgegap_logging-0.1.2/README.md
--rw-r--r--   0        0        0      221 2024-04-29 15:27:47.515968 edgegap_logging-0.1.2/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      417 2024-04-29 15:27:47.519183 edgegap_logging-0.1.2/edgegap_logging/_format.py
--rw-r--r--   0        0        0     4077 2024-04-25 13:10:38.954195 edgegap_logging-0.1.2/edgegap_logging/_logging.py
--rw-r--r--   0        0        0      494 2024-04-29 15:27:51.400518 edgegap_logging-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 edgegap_logging-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:13:42.710660 edgegap_logging-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2216 2024-04-29 18:13:42.710660 edgegap_logging-1.0.0/README.md
+-rw-r--r--   0        0        0      221 2024-04-29 18:13:42.710660 edgegap_logging-1.0.0/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-29 18:13:42.710660 edgegap_logging-1.0.0/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     4077 2024-04-29 18:13:42.710660 edgegap_logging-1.0.0/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0      494 2024-04-29 18:14:10.530809 edgegap_logging-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 edgegap_logging-1.0.0/PKG-INFO
```

### Comparing `edgegap_logging-0.1.2/LICENSE` & `edgegap_logging-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-0.1.2/README.md` & `edgegap_logging-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-0.1.2/edgegap_logging/_logging.py` & `edgegap_logging-1.0.0/edgegap_logging/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-0.1.2/PKG-INFO` & `edgegap_logging-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 0.1.2
+Version: 1.0.0
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Logging Library
 
 This is the README for the Edgegap Logging Helper, which is part of the Edgegap suite of helpers.
```

