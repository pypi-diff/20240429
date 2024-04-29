# Comparing `tmp/edgegap_service-1.0.1.tar.gz` & `tmp/edgegap_service-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.0.1.tar", max compression
+gzip compressed data, was "edgegap_service-1.0.2.tar", max compression
```

## Comparing `edgegap_service-1.0.1.tar` & `edgegap_service-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/README.md
--rw-r--r--   0        0        0      164 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7668 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1880 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-04-29 18:21:35.343371 edgegap_service-1.0.1/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      739 2024-04-29 18:21:56.875541 edgegap_service-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 edgegap_service-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/README.md
+-rw-r--r--   0        0        0      164 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7668 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1880 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-04-29 18:23:33.441036 edgegap_service-1.0.2/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      739 2024-04-29 18:23:37.545055 edgegap_service-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 edgegap_service-1.0.2/PKG-INFO
```

### Comparing `edgegap_service-1.0.1/LICENSE` & `edgegap_service-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/README.md` & `edgegap_service-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_configuration.py` & `edgegap_service-1.0.2/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_documentation.py` & `edgegap_service-1.0.2/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_environment.py` & `edgegap_service-1.0.2/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_logging.py` & `edgegap_service-1.0.2/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_scheduling.py` & `edgegap_service-1.0.2/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_service.py` & `edgegap_service-1.0.2/edgegap_service/_service.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/_templating.py` & `edgegap_service-1.0.2/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/health/_health.py` & `edgegap_service-1.0.2/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.0.2/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/health/checks/_database.py` & `edgegap_service-1.0.2/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.0.2/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/static/html/index.html` & `edgegap_service-1.0.2/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.0.2/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.1/pyproject.toml` & `edgegap_service-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.0.1"
+version = "1.0.2"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.110.2"
 pydantic = "^2.7.1"
 pydantic-settings = "^2.2.1"
 colorama = "^0.4.6"
 elastic-apm = "^6.22.0"
 jinja2 = "^3.1.3"
-edgegap-consul = "^0.1.0"
-edgegap-database = "^0.1.0"
-edgegap-settings = "^0.1.0"
-edgegap-scheduling = "^0.1.0"
-edgegap-logging = "^0.1.0"
+edgegap-consul = "^1.0.0"
+edgegap-database = "^1.0.0"
+edgegap-settings = "^1.0.0"
+edgegap-scheduling = "^1.0.0"
+edgegap-logging = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edgegap_service-1.0.1/PKG-INFO` & `edgegap_service-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: edgegap-consul (>=0.1.0,<0.2.0)
-Requires-Dist: edgegap-database (>=0.1.0,<0.2.0)
-Requires-Dist: edgegap-logging (>=0.1.0,<0.2.0)
-Requires-Dist: edgegap-scheduling (>=0.1.0,<0.2.0)
-Requires-Dist: edgegap-settings (>=0.1.0,<0.2.0)
+Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
+Requires-Dist: edgegap-database (>=1.0.0,<2.0.0)
+Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
+Requires-Dist: edgegap-scheduling (>=1.0.0,<2.0.0)
+Requires-Dist: edgegap-settings (>=1.0.0,<2.0.0)
 Requires-Dist: elastic-apm (>=6.22.0,<7.0.0)
 Requires-Dist: fastapi (>=0.110.2,<0.111.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
```

