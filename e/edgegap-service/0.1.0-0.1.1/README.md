# Comparing `tmp/edgegap_service-0.1.0.tar.gz` & `tmp/edgegap_service-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-0.1.0.tar", max compression
+gzip compressed data, was "edgegap_service-0.1.1.tar", max compression
```

## Comparing `edgegap_service-0.1.0.tar` & `edgegap_service-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.0/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.0/README.md
--rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.0/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-29 15:06:35.271621 edgegap_service-0.1.0/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      720 2024-04-25 13:10:38.955686 edgegap_service-0.1.0/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.0/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.0/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.0/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7037 2024-04-29 15:06:35.273848 edgegap_service-0.1.0/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.0/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.0/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.0/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.0/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.0/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.0/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.0/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.0/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.0/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.0/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0      739 2024-04-29 15:12:14.811208 edgegap_service-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.1/README.md
+-rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.1/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-29 15:06:35.271621 edgegap_service-0.1.1/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      720 2024-04-25 13:10:38.955686 edgegap_service-0.1.1/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.1/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.1/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.1/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7063 2024-04-29 15:34:07.317892 edgegap_service-0.1.1/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.1/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.1/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.1/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.1/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.1/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.1/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.1/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.1/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.1/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.1/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0      739 2024-04-29 15:34:21.664682 edgegap_service-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.1/PKG-INFO
```

### Comparing `edgegap_service-0.1.0/LICENSE` & `edgegap_service-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/README.md` & `edgegap_service-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/_configuration.py` & `edgegap_service-0.1.1/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/_documentation.py` & `edgegap_service-0.1.1/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/_environment.py` & `edgegap_service-0.1.1/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/_logging.py` & `edgegap_service-0.1.1/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/_scheduling.py` & `edgegap_service-0.1.1/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/_service.py` & `edgegap_service-0.1.1/edgegap_service/_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import inspect
 import logging
 import os
 from logging.config import dictConfig
 
-from colorama import Fore
-from edgegap_scheduling import Scheduler, Format
+from edgegap_logging import Color, Format
 from edgegap_settings import ProjectBaseSettings
 from elasticapm.contrib.starlette import make_apm_client, ElasticAPM
 from fastapi import (
     FastAPI,
     staticfiles,
     templating
 )
 
+from edgegap_scheduling import Scheduler
 from ._configuration import ServiceConfiguration
 from ._documentation import DocumentationRoute
 from ._scheduling import SchedulingAPI
 from ._templating import TemplateRenderer
 from .health import HealthCheck
 
 
@@ -48,15 +48,15 @@
             ), name="static"
         )
 
         self.__logger = self.__init_logging()
 
         service_string = f"{self.__configuration.name} ({self.__configuration.version})"
         self.__logger.info(
-            f"Service {Format.squared(service_string, Fore.GREEN)} is initializing"
+            f"Service {Format.squared(service_string, Color.GREEN)} is initializing"
         )
 
         self.__init_root()
         self.__init_health()
         self.__init_template_renderer()
         self.__init_apm()
         self.__init_startup_functions()
@@ -65,40 +65,41 @@
 
         return self.__app
 
     def __init_root(self):
         folder = f"{self.__static_folder}/html"
         templates = templating.Jinja2Templates(directory=folder)
         DocumentationRoute.init_documentation(self.__app, templates)
-        self.__logger.info(f"Initialized root path and documentation with folder: {Format.squared(folder, Fore.GREEN)}")
+        self.__logger.info(
+            f"Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}")
 
     def __init_health(self):
         health_check = HealthCheck(
             title=self.__configuration.name,
             version=self.__configuration.version,
             checks=self.__configuration.checks,
             depend=self.__configuration.depend
         )
         health_check.init_health_check(self.__app)
 
-        self.__logger.info(f"Initialized Health route at {Format.squared('/health', Fore.GREEN)}")
+        self.__logger.info(f"Initialized Health route at {Format.squared('/health', Color.GREEN)}")
 
     def __init_template_renderer(self):
         assert isinstance(
             TemplateRenderer.get_templates(configuration=self.__configuration),
             templating.Jinja2Templates
         )
         self.__logger.info("Initialized Template Renderer")
 
     def __init_logging(self) -> logging.Logger:
         self.__init_logstash()
 
         dictConfig(self.__configuration.log_config.model_dump())
         logger = logging.getLogger(self.__configuration.name)
-        logger.info(f"Logging for service {Format.squared(self.__configuration.name, Fore.GREEN)} is configured")
+        logger.info(f"Logging for service {Format.squared(self.__configuration.name, Color.GREEN)} is configured")
 
         if self.__configuration.settings and self.__configuration.settings.logstash.enabled:
             logger.info(f"Logstash is enabled")
 
         return logger
 
     def __init_apm(self):
@@ -153,15 +154,15 @@
                 SchedulingAPI().init_scheduling_api(self.__app)
                 asyncio.create_task(self.__configuration.scheduler.start_all())
 
     def __init_sigterm(self):
         @self.__app.on_event("shutdown")
         def handle():
             try:
-                self.__logger.info(f"Shutting down {Format.squared(self.__configuration.name, Fore.GREEN)}")
+                self.__logger.info(f"Shutting down {Format.squared(self.__configuration.name, Color.GREEN)}")
 
                 if isinstance(self.__configuration.scheduler, Scheduler):
                     asyncio.ensure_future(self.__configuration.scheduler.stop_all())
             except Exception as e:
                 self.__logger.exception(e)
 
     def __init_startup_functions(self):
```

### Comparing `edgegap_service-0.1.0/edgegap_service/_templating.py` & `edgegap_service-0.1.1/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/health/_health.py` & `edgegap_service-0.1.1/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/health/checks/_consul.py` & `edgegap_service-0.1.1/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/health/checks/_database.py` & `edgegap_service-0.1.1/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/health/checks/_interface.py` & `edgegap_service-0.1.1/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/edgegap_service/static/html/index.html` & `edgegap_service-0.1.1/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.0/pyproject.toml` & `edgegap_service-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "0.1.0"
+version = "0.1.1"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-0.1.0/PKG-INFO` & `edgegap_service-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

