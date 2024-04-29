# Comparing `tmp/edgegap_service-1.0.2.tar.gz` & `tmp/edgegap_service-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.0.2.tar", max compression
+gzip compressed data, was "edgegap_service-1.0.3.tar", max compression
```

## Comparing `edgegap_service-1.0.2.tar` & `edgegap_service-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/README.md
--rw-r--r--   0        0        0      164 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7668 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1880 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      739 2024-04-29 18:23:37.545055 edgegap_service-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 edgegap_service-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:44:21.838079 edgegap_service-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 18:44:21.838508 edgegap_service-1.0.3/README.md
+-rw-r--r--   0        0        0       17 2024-04-29 18:44:21.838719 edgegap_service-1.0.3/edgegap_service/BUILD
+-rw-r--r--   0        0        0      164 2024-04-29 18:44:21.838942 edgegap_service-1.0.3/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-29 18:44:21.839143 edgegap_service-1.0.3/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 18:44:21.839287 edgegap_service-1.0.3/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 18:44:21.839491 edgegap_service-1.0.3/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 18:44:21.839668 edgegap_service-1.0.3/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 18:44:21.839844 edgegap_service-1.0.3/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7671 2024-04-29 18:45:11.326263 edgegap_service-1.0.3/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-29 18:44:21.840414 edgegap_service-1.0.3/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-04-29 18:44:21.840524 edgegap_service-1.0.3/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      101 2024-04-29 18:44:21.841176 edgegap_service-1.0.3/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-29 18:44:21.841466 edgegap_service-1.0.3/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-29 18:44:21.841701 edgegap_service-1.0.3/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-04-29 18:44:21.841786 edgegap_service-1.0.3/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      234 2024-04-29 18:44:21.842102 edgegap_service-1.0.3/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 18:44:21.842322 edgegap_service-1.0.3/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 18:44:21.842578 edgegap_service-1.0.3/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-29 18:44:21.842920 edgegap_service-1.0.3/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-29 18:44:21.843236 edgegap_service-1.0.3/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1880 2024-04-29 18:44:21.843536 edgegap_service-1.0.3/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-04-29 18:44:21.843888 edgegap_service-1.0.3/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      739 2024-04-29 18:45:35.096052 edgegap_service-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-1.0.3/PKG-INFO
```

### Comparing `edgegap_service-1.0.2/LICENSE` & `edgegap_service-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/README.md` & `edgegap_service-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/_configuration.py` & `edgegap_service-1.0.3/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/_documentation.py` & `edgegap_service-1.0.3/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/_environment.py` & `edgegap_service-1.0.3/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/_logging.py` & `edgegap_service-1.0.3/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/_scheduling.py` & `edgegap_service-1.0.3/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/_service.py` & `edgegap_service-1.0.3/edgegap_service/_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,23 +67,24 @@
         self.__init_startup_functions()
         self.__init_scheduling()
         self.__init_sigterm()
 
         return self.__app
 
     def __init_root(self):
+        folder = os.path.join(current_dir, "static", "html")
+        file_name = "index.html"
         is_defined = isinstance(self.__configuration.html_index_path, str)
-        full_path = os.path.join(self.__configuration.root_dir, self.__configuration.html_index_path)
 
-        if is_defined and os.path.isfile(full_path):
-            folder = os.path.dirname(full_path)
-            file_name = os.path.basename(full_path)
-        else:
-            folder = os.path.join(current_dir, "static", "html")
-            file_name = "index.html"
+        if is_defined:
+            full_path = os.path.join(self.__configuration.root_dir, self.__configuration.html_index_path)
+
+            if os.path.isfile(full_path):
+                folder = os.path.dirname(full_path)
+                file_name = os.path.basename(full_path)
 
         templates = templating.Jinja2Templates(directory=folder)
         DocumentationRoute.init_documentation(self.__app, file_name, templates)
         self.__logger.info(
             f"Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}"
         )
```

### Comparing `edgegap_service-1.0.2/edgegap_service/_templating.py` & `edgegap_service-1.0.3/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/health/_health.py` & `edgegap_service-1.0.3/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.0.3/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/health/checks/_database.py` & `edgegap_service-1.0.3/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.0.3/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/static/html/index.html` & `edgegap_service-1.0.3/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.0.3/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.2/pyproject.toml` & `edgegap_service-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.0.2"
+version = "1.0.3"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.0.2/PKG-INFO` & `edgegap_service-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-database (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-scheduling (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-settings (>=1.0.0,<2.0.0)
 Requires-Dist: elastic-apm (>=6.22.0,<7.0.0)
```

