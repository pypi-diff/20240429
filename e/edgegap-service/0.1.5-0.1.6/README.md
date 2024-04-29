# Comparing `tmp/edgegap_service-0.1.5.tar.gz` & `tmp/edgegap_service-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-0.1.5.tar", max compression
+gzip compressed data, was "edgegap_service-0.1.6.tar", max compression
```

## Comparing `edgegap_service-0.1.5.tar` & `edgegap_service-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.5/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.5/README.md
--rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.5/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.5/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.5/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.5/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.5/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.5/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7668 2024-04-29 17:47:56.892279 edgegap_service-0.1.5/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.5/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.5/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.5/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.5/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.5/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.5/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.5/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.5/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.5/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.5/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-04-29 17:44:05.347132 edgegap_service-0.1.5/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      739 2024-04-29 17:48:00.507726 edgegap_service-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.6/README.md
+-rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.6/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.6/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.6/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.6/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.6/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.6/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7668 2024-04-29 17:47:56.892279 edgegap_service-0.1.6/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.6/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.6/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.6/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.6/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.6/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.6/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.6/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.6/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.6/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1880 2024-04-29 17:49:57.082015 edgegap_service-0.1.6/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-04-29 17:44:05.347132 edgegap_service-0.1.6/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      739 2024-04-29 17:50:19.314967 edgegap_service-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.6/PKG-INFO
```

### Comparing `edgegap_service-0.1.5/LICENSE` & `edgegap_service-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/README.md` & `edgegap_service-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_configuration.py` & `edgegap_service-0.1.6/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_documentation.py` & `edgegap_service-0.1.6/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_environment.py` & `edgegap_service-0.1.6/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_logging.py` & `edgegap_service-0.1.6/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_scheduling.py` & `edgegap_service-0.1.6/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_service.py` & `edgegap_service-0.1.6/edgegap_service/_service.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/_templating.py` & `edgegap_service-0.1.6/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/health/_health.py` & `edgegap_service-0.1.6/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/health/checks/_consul.py` & `edgegap_service-0.1.6/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/health/checks/_database.py` & `edgegap_service-0.1.6/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/health/checks/_interface.py` & `edgegap_service-0.1.6/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/edgegap_service/static/html/index.html` & `edgegap_service-0.1.6/edgegap_service/static/html/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 <html>
 <head>
     <meta charset="utf-8">
     <meta content="width=device-width, initial-scale=1" name="viewport">
 
     <title>{{ title }}</title>
 
+    <link rel="icon" type="image/x-icon" href="/static/images/favicon.ico">
+
     <!-- Fonts -->
     <link href="https://fonts.googleapis.com/css?family=Nunito:200,600" rel="stylesheet">
 
     <!-- Styles -->
     <style>
         html, body {
             background-color: #fff;
```

### Comparing `edgegap_service-0.1.5/edgegap_service/static/images/favicon.ico` & `edgegap_service-0.1.6/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.5/pyproject.toml` & `edgegap_service-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "0.1.5"
+version = "0.1.6"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-0.1.5/PKG-INFO` & `edgegap_service-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 0.1.5
+Version: 0.1.6
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

