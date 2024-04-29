# Comparing `tmp/edgegap_service-0.1.3.tar.gz` & `tmp/edgegap_service-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-0.1.3.tar", max compression
+gzip compressed data, was "edgegap_service-0.1.4.tar", max compression
```

## Comparing `edgegap_service-0.1.3.tar` & `edgegap_service-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.3/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.3/README.md
--rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.3/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.3/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.3/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.3/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.3/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.3/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7510 2024-04-29 17:29:47.929627 edgegap_service-0.1.3/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.3/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.3/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.3/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.3/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.3/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.3/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.3/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.3/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.3/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.3/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0      739 2024-04-29 17:30:06.246972 edgegap_service-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.4/README.md
+-rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.4/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.4/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.4/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.4/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.4/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.4/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7514 2024-04-29 17:35:49.173091 edgegap_service-0.1.4/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.4/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.4/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.4/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.4/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.4/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.4/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.4/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.4/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.4/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.4/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0      739 2024-04-29 17:36:52.490348 edgegap_service-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.4/PKG-INFO
```

### Comparing `edgegap_service-0.1.3/LICENSE` & `edgegap_service-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/README.md` & `edgegap_service-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/_configuration.py` & `edgegap_service-0.1.4/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/_documentation.py` & `edgegap_service-0.1.4/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/_environment.py` & `edgegap_service-0.1.4/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/_logging.py` & `edgegap_service-0.1.4/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/_scheduling.py` & `edgegap_service-0.1.4/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/_service.py` & `edgegap_service-0.1.4/edgegap_service/_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,18 +64,19 @@
         self.__init_scheduling()
         self.__init_sigterm()
 
         return self.__app
 
     def __init_root(self):
         is_defined = isinstance(self.__configuration.html_index_path, str)
+        full_path = os.path.join(self.__configuration.root_dir, self.__configuration.html_index_path)
 
-        if is_defined and os.path.isfile(self.__configuration.html_index_path):
-            folder = os.path.dirname(os.path.abspath(self.__configuration.html_index_path))
-            file_name = os.path.basename(self.__configuration.html_index_path)
+        if is_defined and os.path.isfile(full_path):
+            folder = os.path.dirname(full_path)
+            file_name = os.path.basename(full_path)
         else:
             folder = os.path.join(current_dir, "static", "html")
             file_name = "index.html"
 
         templates = templating.Jinja2Templates(directory=folder)
         DocumentationRoute.init_documentation(self.__app, file_name, templates)
         self.__logger.info(
```

### Comparing `edgegap_service-0.1.3/edgegap_service/_templating.py` & `edgegap_service-0.1.4/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/health/_health.py` & `edgegap_service-0.1.4/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/health/checks/_consul.py` & `edgegap_service-0.1.4/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/health/checks/_database.py` & `edgegap_service-0.1.4/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/health/checks/_interface.py` & `edgegap_service-0.1.4/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/edgegap_service/static/html/index.html` & `edgegap_service-0.1.4/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.3/pyproject.toml` & `edgegap_service-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "0.1.3"
+version = "0.1.4"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-0.1.3/PKG-INFO` & `edgegap_service-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

