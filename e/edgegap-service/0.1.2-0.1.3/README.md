# Comparing `tmp/edgegap_service-0.1.2.tar.gz` & `tmp/edgegap_service-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-0.1.2.tar", max compression
+gzip compressed data, was "edgegap_service-0.1.3.tar", max compression
```

## Comparing `edgegap_service-0.1.2.tar` & `edgegap_service-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.2/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.2/README.md
--rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.2/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-29 15:06:35.271621 edgegap_service-0.1.2/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      720 2024-04-25 13:10:38.955686 edgegap_service-0.1.2/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.2/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.2/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.2/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7152 2024-04-29 17:20:13.848056 edgegap_service-0.1.2/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.2/edgegap_service/_templating.py
--rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.2/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.2/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.2/edgegap_service/health/_model.py
--rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.2/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.2/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.2/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.2/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.2/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.2/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0      739 2024-04-29 17:20:45.716086 edgegap_service-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.383589 edgegap_service-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 14:44:49.935599 edgegap_service-0.1.3/README.md
+-rw-r--r--   0        0        0      164 2024-04-25 13:10:38.955511 edgegap_service-0.1.3/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-29 17:27:57.365982 edgegap_service-0.1.3/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 17:29:47.933632 edgegap_service-0.1.3/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 15:06:35.269908 edgegap_service-0.1.3/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 15:06:35.277810 edgegap_service-0.1.3/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 15:00:46.983361 edgegap_service-0.1.3/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7510 2024-04-29 17:29:47.929627 edgegap_service-0.1.3/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-25 13:10:38.956290 edgegap_service-0.1.3/edgegap_service/_templating.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:10:38.956384 edgegap_service-0.1.3/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-25 13:10:38.956471 edgegap_service-0.1.3/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-25 13:10:38.956554 edgegap_service-0.1.3/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0      234 2024-04-25 13:10:38.956640 edgegap_service-0.1.3/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 15:06:35.265857 edgegap_service-0.1.3/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 15:06:35.268102 edgegap_service-0.1.3/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-25 13:10:38.956902 edgegap_service-0.1.3/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-25 13:10:38.956988 edgegap_service-0.1.3/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1803 2024-04-25 13:10:38.958326 edgegap_service-0.1.3/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0      739 2024-04-29 17:30:06.246972 edgegap_service-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-0.1.3/PKG-INFO
```

### Comparing `edgegap_service-0.1.2/LICENSE` & `edgegap_service-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/README.md` & `edgegap_service-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/_configuration.py` & `edgegap_service-0.1.3/edgegap_service/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     model_config = ConfigDict(arbitrary_types_allowed=True)
     name: str = Field(..., description="The name of the Service")
     version: str = Field(..., description="The version of the Service")
     description: str = Field(..., description="The description of the Service")
     routers: list[APIRouter] = Field([], description="The FastAPI routers")
     root_dir: str = Field(..., description="The Root Directory of the Service")
     static_dir: str = Field(default="static", description="The Static Directory of the Service")
+    html_index_path: str | None = Field(default=None, description="The full path to the html index file")
     checks: list[type(CheckInterface)] = Field([], description="The list of Checks to run on the Service")
     depend: Optional[Callable] = Field(default=None, description="The Base Depend Attribute for DB Session")
     port: int = Field(default=8000, description="The Port of the Service")
     host: str = Field(default="0.0.0.0", description="The Host of the Service")
     workers: int = Field(default=1, description="Numbers of Workers, (if you use the scheduler, keep to 1)")
     timeout: int = Field(default=300, description="Default Timeout for Connection")
     worker_class: str = Field(default="uvicorn.workers.UvicornWorker", description="The worker class for ASGI")
```

### Comparing `edgegap_service-0.1.2/edgegap_service/_documentation.py` & `edgegap_service-0.1.3/edgegap_service/_documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from fastapi import FastAPI, templating, Request, responses
 
 
 class DocumentationRoute:
     @staticmethod
-    def init_documentation(app: FastAPI, templates: templating.Jinja2Templates):
+    def init_documentation(app: FastAPI, file_name: str, templates: templating.Jinja2Templates):
         @app.get("/", response_class=responses.HTMLResponse, include_in_schema=False)
         async def root(request: Request):
             urls = {
                 "Docs": f"{request.base_url}docs",
                 "Redoc": f"{request.base_url}redoc",
             }
 
             return templates.TemplateResponse(
-                name="index.html",
+                name=file_name,
                 context={
                     "request": request,
                     "urls": urls,
                     "title": getattr(app, 'title')
                 }
             )
```

### Comparing `edgegap_service-0.1.2/edgegap_service/_environment.py` & `edgegap_service-0.1.3/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/_logging.py` & `edgegap_service-0.1.3/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/_scheduling.py` & `edgegap_service-0.1.3/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/_service.py` & `edgegap_service-0.1.3/edgegap_service/_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 
         for router in self.__configuration.routers:
             self.__app.include_router(router)
 
         self.__app.mount(
             "/static",
             staticfiles.StaticFiles(
-                directory=self.__static_folder,
-                packages=[("edgegap_service", "static")]
+                directory=self.__static_folder
             ), name="static"
         )
 
         self.__logger = self.__init_logging()
 
         service_string = f"{self.__configuration.name} ({self.__configuration.version})"
         self.__logger.info(
@@ -64,17 +63,25 @@
         self.__init_startup_functions()
         self.__init_scheduling()
         self.__init_sigterm()
 
         return self.__app
 
     def __init_root(self):
-        folder = f"{current_dir}/html"
+        is_defined = isinstance(self.__configuration.html_index_path, str)
+
+        if is_defined and os.path.isfile(self.__configuration.html_index_path):
+            folder = os.path.dirname(os.path.abspath(self.__configuration.html_index_path))
+            file_name = os.path.basename(self.__configuration.html_index_path)
+        else:
+            folder = os.path.join(current_dir, "static", "html")
+            file_name = "index.html"
+
         templates = templating.Jinja2Templates(directory=folder)
-        DocumentationRoute.init_documentation(self.__app, templates)
+        DocumentationRoute.init_documentation(self.__app, file_name, templates)
         self.__logger.info(
             f"Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}"
         )
 
     def __init_health(self):
         health_check = HealthCheck(
             title=self.__configuration.name,
```

### Comparing `edgegap_service-0.1.2/edgegap_service/_templating.py` & `edgegap_service-0.1.3/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/health/_health.py` & `edgegap_service-0.1.3/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/health/checks/_consul.py` & `edgegap_service-0.1.3/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/health/checks/_database.py` & `edgegap_service-0.1.3/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/health/checks/_interface.py` & `edgegap_service-0.1.3/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/edgegap_service/static/html/index.html` & `edgegap_service-0.1.3/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-0.1.2/pyproject.toml` & `edgegap_service-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "0.1.2"
+version = "0.1.3"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-0.1.2/PKG-INFO` & `edgegap_service-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

