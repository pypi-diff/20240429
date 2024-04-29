# Comparing `tmp/edgegap_service-0.1.4.tar.gz` & `tmp/edgegap_service-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-0.1.4.tar", max compression
+gzip compressed data, was "edgegap_service-0.1.5.tar", max compression
```

## Comparing `edgegap_service-0.1.4.tar` & `edgegap_service-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.4/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.4/README.md
--rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.4/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.4/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.4/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.4/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.4/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.4/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7514 2024-04-29 17:35:49.173091 edgegap_service-0.1.4/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.4/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.4/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.4/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.4/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.4/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.4/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.4/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.4/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.4/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.4/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0      739 2024-04-29 17:36:52.490348 edgegap_service-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.5/README.md
+-rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.5/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.5/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.5/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.5/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.5/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.5/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7668 2024-04-29 17:47:56.892279 edgegap_service-0.1.5/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.5/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.5/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.5/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.5/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.5/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.5/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.5/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.5/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.5/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.5/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-04-29 17:44:05.347132 edgegap_service-0.1.5/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      739 2024-04-29 17:48:00.507726 edgegap_service-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.5/PKG-INFO
```

### Comparing `edgegap_service-0.1.4/LICENSE` & `edgegap_service-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/README.md` & `edgegap_service-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/_configuration.py` & `edgegap_service-0.1.5/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/_documentation.py` & `edgegap_service-0.1.5/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/_environment.py` & `edgegap_service-0.1.5/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/_logging.py` & `edgegap_service-0.1.5/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/_scheduling.py` & `edgegap_service-0.1.5/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/_service.py` & `edgegap_service-0.1.5/edgegap_service/_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import inspect
 import logging
 import os
 from logging.config import dictConfig
+from pathlib import Path
 
 from edgegap_logging import Color, Format
 from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings
 from elasticapm.contrib.starlette import make_apm_client, ElasticAPM
 from fastapi import (
     FastAPI,
@@ -35,21 +36,24 @@
         self.__app = FastAPI(
             title=self.__configuration.name,
             description=self.__configuration.description,
             configuration=self.__configuration,
             openapi_tags=self.__configuration.tags_definition
         )
 
+        Path(self.__static_folder).mkdir(parents=True, exist_ok=True)
+
         for router in self.__configuration.routers:
             self.__app.include_router(router)
 
         self.__app.mount(
             "/static",
             staticfiles.StaticFiles(
-                directory=self.__static_folder
+                directory=self.__static_folder,
+                packages=[("edgegap_service", "static")]
             ), name="static"
         )
 
         self.__logger = self.__init_logging()
 
         service_string = f"{self.__configuration.name} ({self.__configuration.version})"
         self.__logger.info(
```

### Comparing `edgegap_service-0.1.4/edgegap_service/_templating.py` & `edgegap_service-0.1.5/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/health/_health.py` & `edgegap_service-0.1.5/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/health/checks/_consul.py` & `edgegap_service-0.1.5/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/health/checks/_database.py` & `edgegap_service-0.1.5/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/health/checks/_interface.py` & `edgegap_service-0.1.5/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/edgegap_service/static/html/index.html` & `edgegap_service-0.1.5/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.4/PKG-INFO` & `edgegap_service-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 0.1.4
+Version: 0.1.5
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

