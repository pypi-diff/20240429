# Comparing `tmp/telemetrx-0.1.2.tar.gz` & `tmp/telemetrx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemetrx-0.1.2.tar", last modified: Mon Apr 29 11:02:35 2024, max compression
+gzip compressed data, was "telemetrx-0.1.3.tar", last modified: Mon Apr 29 11:05:35 2024, max compression
```

## Comparing `telemetrx-0.1.2.tar` & `telemetrx-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-29 11:02:35.098189 telemetrx-0.1.2/
--rw-r--r--   0 anpapath   (501) staff       (20)     1617 2024-04-11 11:37:58.000000 telemetrx-0.1.2/LICENSE
--rw-r--r--   0 anpapath   (501) staff       (20)     2202 2024-04-29 11:02:35.097802 telemetrx-0.1.2/PKG-INFO
--rw-r--r--   0 anpapath   (501) staff       (20)     1790 2024-04-11 13:41:26.000000 telemetrx-0.1.2/README.md
--rw-r--r--   0 anpapath   (501) staff       (20)      456 2024-04-29 11:02:18.000000 telemetrx-0.1.2/pyproject.toml
--rw-r--r--   0 anpapath   (501) staff       (20)       38 2024-04-29 11:02:35.098282 telemetrx-0.1.2/setup.cfg
-drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-29 11:02:35.094608 telemetrx-0.1.2/telemetrx/
--rw-r--r--   0 anpapath   (501) staff       (20)     6635 2024-04-29 10:58:33.000000 telemetrx-0.1.2/telemetrx/TelemetrX.py
--rw-r--r--   0 anpapath   (501) staff       (20)       37 2024-04-11 12:55:25.000000 telemetrx-0.1.2/telemetrx/__init__.py
-drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-29 11:02:35.097358 telemetrx-0.1.2/telemetrx.egg-info/
--rw-r--r--   0 anpapath   (501) staff       (20)     2202 2024-04-29 11:02:35.000000 telemetrx-0.1.2/telemetrx.egg-info/PKG-INFO
--rw-r--r--   0 anpapath   (501) staff       (20)      241 2024-04-29 11:02:35.000000 telemetrx-0.1.2/telemetrx.egg-info/SOURCES.txt
--rw-r--r--   0 anpapath   (501) staff       (20)        1 2024-04-29 11:02:35.000000 telemetrx-0.1.2/telemetrx.egg-info/dependency_links.txt
--rw-r--r--   0 anpapath   (501) staff       (20)       22 2024-04-29 11:02:35.000000 telemetrx-0.1.2/telemetrx.egg-info/requires.txt
--rw-r--r--   0 anpapath   (501) staff       (20)       10 2024-04-29 11:02:35.000000 telemetrx-0.1.2/telemetrx.egg-info/top_level.txt
+drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-29 11:05:35.315147 telemetrx-0.1.3/
+-rw-r--r--   0 anpapath   (501) staff       (20)     1617 2024-04-11 11:37:58.000000 telemetrx-0.1.3/LICENSE
+-rw-r--r--   0 anpapath   (501) staff       (20)     2202 2024-04-29 11:05:35.314650 telemetrx-0.1.3/PKG-INFO
+-rw-r--r--   0 anpapath   (501) staff       (20)     1790 2024-04-29 11:05:29.000000 telemetrx-0.1.3/README.md
+-rw-r--r--   0 anpapath   (501) staff       (20)      456 2024-04-29 11:05:29.000000 telemetrx-0.1.3/pyproject.toml
+-rw-r--r--   0 anpapath   (501) staff       (20)       38 2024-04-29 11:05:35.315260 telemetrx-0.1.3/setup.cfg
+drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-29 11:05:35.311179 telemetrx-0.1.3/telemetrx/
+-rw-r--r--   0 anpapath   (501) staff       (20)     6635 2024-04-29 10:58:33.000000 telemetrx-0.1.3/telemetrx/TelemetrX.py
+-rw-r--r--   0 anpapath   (501) staff       (20)       37 2024-04-11 12:55:25.000000 telemetrx-0.1.3/telemetrx/__init__.py
+drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-29 11:05:35.314042 telemetrx-0.1.3/telemetrx.egg-info/
+-rw-r--r--   0 anpapath   (501) staff       (20)     2202 2024-04-29 11:05:35.000000 telemetrx-0.1.3/telemetrx.egg-info/PKG-INFO
+-rw-r--r--   0 anpapath   (501) staff       (20)      241 2024-04-29 11:05:35.000000 telemetrx-0.1.3/telemetrx.egg-info/SOURCES.txt
+-rw-r--r--   0 anpapath   (501) staff       (20)        1 2024-04-29 11:05:35.000000 telemetrx-0.1.3/telemetrx.egg-info/dependency_links.txt
+-rw-r--r--   0 anpapath   (501) staff       (20)       22 2024-04-29 11:05:35.000000 telemetrx-0.1.3/telemetrx.egg-info/requires.txt
+-rw-r--r--   0 anpapath   (501) staff       (20)       10 2024-04-29 11:05:35.000000 telemetrx-0.1.3/telemetrx.egg-info/top_level.txt
```

### Comparing `telemetrx-0.1.2/LICENSE` & `telemetrx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telemetrx-0.1.2/PKG-INFO` & `telemetrx-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: telemetrx
-Version: 0.1.2
+Version: 0.1.3
 Summary: a package for sending app telemetry data to the TelemetrX backend.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: python-dotenv
 
-# telemetrx-0.1.1
+# telemetrx-0.1.3
 
 telemetrx is a Python library which facilitates the sending of App telemetry data to the TelemetrX platform, leveraging the TelemetrX API. 
 
 ## Features
 
 The library features the function send_telemetrx() which helps app owners to send telemetry data to the TelemetrX platform with a single line of code.
```

### Comparing `telemetrx-0.1.2/README.md` & `telemetrx-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# telemetrx-0.1.1
+# telemetrx-0.1.3
 
 telemetrx is a Python library which facilitates the sending of App telemetry data to the TelemetrX platform, leveraging the TelemetrX API. 
 
 ## Features
 
 The library features the function send_telemetrx() which helps app owners to send telemetry data to the TelemetrX platform with a single line of code.
```

### Comparing `telemetrx-0.1.2/telemetrx/TelemetrX.py` & `telemetrx-0.1.3/telemetrx/TelemetrX.py`

 * *Files identical despite different names*

### Comparing `telemetrx-0.1.2/telemetrx.egg-info/PKG-INFO` & `telemetrx-0.1.3/telemetrx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: telemetrx
-Version: 0.1.2
+Version: 0.1.3
 Summary: a package for sending app telemetry data to the TelemetrX backend.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: python-dotenv
 
-# telemetrx-0.1.1
+# telemetrx-0.1.3
 
 telemetrx is a Python library which facilitates the sending of App telemetry data to the TelemetrX platform, leveraging the TelemetrX API. 
 
 ## Features
 
 The library features the function send_telemetrx() which helps app owners to send telemetry data to the TelemetrX platform with a single line of code.
```

