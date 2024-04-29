# Comparing `tmp/edgegap_service-0.1.1.tar.gz` & `tmp/edgegap_service-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-0.1.1.tar", max compression
+gzip compressed data, was "edgegap_service-0.1.2.tar", max compression
```

## Comparing `edgegap_service-0.1.1.tar` & `edgegap_service-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.1/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.1/README.md
--rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.1/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-29 15:06:35.271621 edgegap_service-0.1.1/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      720 2024-04-25 13:10:38.955686 edgegap_service-0.1.1/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.1/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.1/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.1/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7063 2024-04-29 15:34:07.317892 edgegap_service-0.1.1/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.1/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.1/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.1/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.1/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.1/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.1/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.1/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.1/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.1/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.1/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0      739 2024-04-29 15:34:21.664682 edgegap_service-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.2/README.md
+-rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.2/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-29 15:06:35.271621 edgegap_service-0.1.2/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      720 2024-04-25 13:10:38.955686 edgegap_service-0.1.2/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.2/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.2/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.2/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7152 2024-04-29 17:20:13.848056 edgegap_service-0.1.2/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.2/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.2/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.2/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.2/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.2/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.2/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.2/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.2/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.2/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.2/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0      739 2024-04-29 17:20:45.716086 edgegap_service-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.2/PKG-INFO
```

### Comparing `edgegap_service-0.1.1/LICENSE` & `edgegap_service-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/README.md` & `edgegap_service-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/_configuration.py` & `edgegap_service-0.1.2/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/_documentation.py` & `edgegap_service-0.1.2/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/_environment.py` & `edgegap_service-0.1.2/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/_logging.py` & `edgegap_service-0.1.2/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/_scheduling.py` & `edgegap_service-0.1.2/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/_service.py` & `edgegap_service-0.1.2/edgegap_service/_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import asyncio
 import inspect
 import logging
 import os
 from logging.config import dictConfig
 
 from edgegap_logging import Color, Format
+from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings
 from elasticapm.contrib.starlette import make_apm_client, ElasticAPM
 from fastapi import (
     FastAPI,
     staticfiles,
     templating
 )
 
-from edgegap_scheduling import Scheduler
 from ._configuration import ServiceConfiguration
 from ._documentation import DocumentationRoute
 from ._scheduling import SchedulingAPI
 from ._templating import TemplateRenderer
 from .health import HealthCheck
 
+current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
+
 
 class ServiceFactory:
 
     def __init__(self, configuration: ServiceConfiguration) -> None:
         self.__configuration = configuration
         self.__static_folder = os.path.join(self.__configuration.root_dir, self.__configuration.static_dir)
         self.__logger: logging.Logger | None = None
@@ -62,19 +64,20 @@
         self.__init_startup_functions()
         self.__init_scheduling()
         self.__init_sigterm()
 
         return self.__app
 
     def __init_root(self):
-        folder = f"{self.__static_folder}/html"
+        folder = f"{current_dir}/html"
         templates = templating.Jinja2Templates(directory=folder)
         DocumentationRoute.init_documentation(self.__app, templates)
         self.__logger.info(
-            f"Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}")
+            f"Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}"
+        )
 
     def __init_health(self):
         health_check = HealthCheck(
             title=self.__configuration.name,
             version=self.__configuration.version,
             checks=self.__configuration.checks,
             depend=self.__configuration.depend
```

### Comparing `edgegap_service-0.1.1/edgegap_service/_templating.py` & `edgegap_service-0.1.2/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/health/_health.py` & `edgegap_service-0.1.2/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/health/checks/_consul.py` & `edgegap_service-0.1.2/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/health/checks/_database.py` & `edgegap_service-0.1.2/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/health/checks/_interface.py` & `edgegap_service-0.1.2/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/edgegap_service/static/html/index.html` & `edgegap_service-0.1.2/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.1/PKG-INFO` & `edgegap_service-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

