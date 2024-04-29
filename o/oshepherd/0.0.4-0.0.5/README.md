# Comparing `tmp/oshepherd-0.0.4.tar.gz` & `tmp/oshepherd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oshepherd-0.0.4.tar", last modified: Mon Apr 29 13:18:58 2024, max compression
+gzip compressed data, was "oshepherd-0.0.5.tar", last modified: Mon Apr 29 13:18:14 2024, max compression
```

## Comparing `oshepherd-0.0.4.tar` & `oshepherd-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:58.947168 oshepherd-0.0.4/
--rw-r--r--   0 raulpino   (501) staff       (20)     1064 2024-04-09 19:32:21.000000 oshepherd-0.0.4/LICENSE
--rw-r--r--   0 raulpino   (501) staff       (20)       47 2024-04-09 19:47:56.000000 oshepherd-0.0.4/MANIFEST.in
--rw-r--r--   0 raulpino   (501) staff       (20)     3459 2024-04-29 13:18:58.946951 oshepherd-0.0.4/PKG-INFO
--rw-r--r--   0 raulpino   (501) staff       (20)     2425 2024-04-28 14:19:44.000000 oshepherd-0.0.4/README.md
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:58.944226 oshepherd-0.0.4/oshepherd/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 01:40:19.000000 oshepherd-0.0.4/oshepherd/__init__.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:58.945477 oshepherd-0.0.4/oshepherd/api/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.4/oshepherd/api/__init__.py
--rw-r--r--   0 raulpino   (501) staff       (20)      932 2024-04-08 01:56:54.000000 oshepherd-0.0.4/oshepherd/api/app.py
--rw-r--r--   0 raulpino   (501) staff       (20)      353 2024-04-08 03:25:51.000000 oshepherd-0.0.4/oshepherd/api/config.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:58.945834 oshepherd-0.0.4/oshepherd/api/generate/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.4/oshepherd/api/generate/__init__.py
--rw-r--r--   0 raulpino   (501) staff       (20)      847 2024-04-09 03:21:09.000000 oshepherd-0.0.4/oshepherd/api/generate/models.py
--rw-r--r--   0 raulpino   (501) staff       (20)     1262 2024-04-08 03:36:28.000000 oshepherd-0.0.4/oshepherd/api/generate/routes.py
--rw-r--r--   0 raulpino   (501) staff       (20)      304 2024-04-07 02:37:24.000000 oshepherd-0.0.4/oshepherd/api/utils.py
--rw-r--r--   0 raulpino   (501) staff       (20)     1208 2024-04-08 03:34:21.000000 oshepherd-0.0.4/oshepherd/cli.py
--rw-r--r--   0 raulpino   (501) staff       (20)      665 2024-04-08 03:21:10.000000 oshepherd-0.0.4/oshepherd/lib.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:58.946348 oshepherd-0.0.4/oshepherd/worker/
--rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:47:11.000000 oshepherd-0.0.4/oshepherd/worker/__init__.py
--rw-r--r--   0 raulpino   (501) staff       (20)     1170 2024-04-29 13:18:50.000000 oshepherd-0.0.4/oshepherd/worker/app.py
--rw-r--r--   0 raulpino   (501) staff       (20)      290 2024-04-29 13:18:50.000000 oshepherd-0.0.4/oshepherd/worker/config.py
--rw-r--r--   0 raulpino   (501) staff       (20)      684 2024-04-29 13:18:50.000000 oshepherd-0.0.4/oshepherd/worker/tasks.py
-drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:58.946506 oshepherd-0.0.4/oshepherd.egg-info/
--rw-r--r--   0 raulpino   (501) staff       (20)     3459 2024-04-29 13:18:58.000000 oshepherd-0.0.4/oshepherd.egg-info/PKG-INFO
--rw-r--r--   0 raulpino   (501) staff       (20)      610 2024-04-29 13:18:58.000000 oshepherd-0.0.4/oshepherd.egg-info/SOURCES.txt
--rw-r--r--   0 raulpino   (501) staff       (20)        1 2024-04-29 13:18:58.000000 oshepherd-0.0.4/oshepherd.egg-info/dependency_links.txt
--rw-r--r--   0 raulpino   (501) staff       (20)       49 2024-04-29 13:18:58.000000 oshepherd-0.0.4/oshepherd.egg-info/entry_points.txt
--rw-r--r--   0 raulpino   (501) staff       (20)      142 2024-04-29 13:18:58.000000 oshepherd-0.0.4/oshepherd.egg-info/requires.txt
--rw-r--r--   0 raulpino   (501) staff       (20)       16 2024-04-29 13:18:58.000000 oshepherd-0.0.4/oshepherd.egg-info/top_level.txt
--rw-r--r--   0 raulpino   (501) staff       (20)      870 2024-04-29 13:18:50.000000 oshepherd-0.0.4/pyproject.toml
--rw-r--r--   0 raulpino   (501) staff       (20)       38 2024-04-29 13:18:58.947209 oshepherd-0.0.4/setup.cfg
--rw-r--r--   0 raulpino   (501) staff       (20)     1271 2024-04-29 13:18:50.000000 oshepherd-0.0.4/setup.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.352509 oshepherd-0.0.5/
+-rw-r--r--   0 raulpino   (501) staff       (20)     1064 2024-04-09 19:32:21.000000 oshepherd-0.0.5/LICENSE
+-rw-r--r--   0 raulpino   (501) staff       (20)       47 2024-04-09 19:47:56.000000 oshepherd-0.0.5/MANIFEST.in
+-rw-r--r--   0 raulpino   (501) staff       (20)     3459 2024-04-29 13:18:14.352329 oshepherd-0.0.5/PKG-INFO
+-rw-r--r--   0 raulpino   (501) staff       (20)     2425 2024-04-28 14:19:44.000000 oshepherd-0.0.5/README.md
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.347523 oshepherd-0.0.5/oshepherd/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 01:40:19.000000 oshepherd-0.0.5/oshepherd/__init__.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.350284 oshepherd-0.0.5/oshepherd/api/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.5/oshepherd/api/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      932 2024-04-08 01:56:54.000000 oshepherd-0.0.5/oshepherd/api/app.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      353 2024-04-08 03:25:51.000000 oshepherd-0.0.5/oshepherd/api/config.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.350905 oshepherd-0.0.5/oshepherd/api/generate/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:37:24.000000 oshepherd-0.0.5/oshepherd/api/generate/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      847 2024-04-09 03:21:09.000000 oshepherd-0.0.5/oshepherd/api/generate/models.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1262 2024-04-08 03:36:28.000000 oshepherd-0.0.5/oshepherd/api/generate/routes.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      304 2024-04-07 02:37:24.000000 oshepherd-0.0.5/oshepherd/api/utils.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1208 2024-04-08 03:34:21.000000 oshepherd-0.0.5/oshepherd/cli.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      665 2024-04-08 03:21:10.000000 oshepherd-0.0.5/oshepherd/lib.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.351656 oshepherd-0.0.5/oshepherd/worker/
+-rw-r--r--   0 raulpino   (501) staff       (20)        0 2024-04-07 02:47:11.000000 oshepherd-0.0.5/oshepherd/worker/__init__.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     1236 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/app.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      459 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/config.py
+-rw-r--r--   0 raulpino   (501) staff       (20)     2302 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/ollama_task.py
+-rw-r--r--   0 raulpino   (501) staff       (20)      877 2024-04-29 13:18:02.000000 oshepherd-0.0.5/oshepherd/worker/tasks.py
+drwxr-xr-x   0 raulpino   (501) staff       (20)        0 2024-04-29 13:18:14.351881 oshepherd-0.0.5/oshepherd.egg-info/
+-rw-r--r--   0 raulpino   (501) staff       (20)     3459 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/PKG-INFO
+-rw-r--r--   0 raulpino   (501) staff       (20)      642 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/SOURCES.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)        1 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/dependency_links.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)       49 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/entry_points.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)      142 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/requires.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)       16 2024-04-29 13:18:14.000000 oshepherd-0.0.5/oshepherd.egg-info/top_level.txt
+-rw-r--r--   0 raulpino   (501) staff       (20)      870 2024-04-29 13:18:02.000000 oshepherd-0.0.5/pyproject.toml
+-rw-r--r--   0 raulpino   (501) staff       (20)       38 2024-04-29 13:18:14.352552 oshepherd-0.0.5/setup.cfg
+-rw-r--r--   0 raulpino   (501) staff       (20)     1271 2024-04-29 13:18:02.000000 oshepherd-0.0.5/setup.py
```

### Comparing `oshepherd-0.0.4/LICENSE` & `oshepherd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/PKG-INFO` & `oshepherd-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oshepherd
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Oshepherd guiding the Ollama(s) inference orchestration.
 Author: mnemonica.ai
 Author-email: "mnemonica.ai" <info@mnemonica.ai>
 Project-URL: Homepage, https://github.com/mnemonica-ai/oshepherd
 Project-URL: Issues, https://github.com/mnemonica-ai/oshepherd/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `oshepherd-0.0.4/README.md` & `oshepherd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/oshepherd/api/app.py` & `oshepherd-0.0.5/oshepherd/api/app.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/oshepherd/api/generate/models.py` & `oshepherd-0.0.5/oshepherd/api/generate/models.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/oshepherd/api/generate/routes.py` & `oshepherd-0.0.5/oshepherd/api/generate/routes.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/oshepherd/cli.py` & `oshepherd-0.0.5/oshepherd/cli.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/oshepherd/lib.py` & `oshepherd-0.0.5/oshepherd/lib.py`

 * *Files identical despite different names*

### Comparing `oshepherd-0.0.4/oshepherd/worker/app.py` & `oshepherd-0.0.5/oshepherd/worker/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     global celery_app
 
     celery_app = Celery(
         TASKS_MODULE, broker=config.RABBITMQ_URL, backend=config.REDIS_URL
     )
     celery_app.conf.update(
         result_expires=config.RESULTS_EXPIRES,
+        broker_transport_options=config.BROKER_TRANSPORT_OPTIONS,
     )
     celery_app.autodiscover_tasks([TASKS_MODULE])
 
     return celery_app
 
 
 def create_celery_app_for_flask(flask_app):
```

### Comparing `oshepherd-0.0.4/oshepherd/worker/tasks.py` & `oshepherd-0.0.5/oshepherd/worker/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import json
 import ollama
 from oshepherd.worker.app import celery_app
+from oshepherd.worker.ollama_task import OllamaCeleryTask
 
 
-@celery_app.task(name="oshepherd.worker.tasks.make_generate_request")
-def make_generate_request(request_str: str):
+@celery_app.task(
+    name="oshepherd.worker.tasks.make_generate_request",
+    bind=True,
+    base=OllamaCeleryTask,
+)
+def make_generate_request(self, request_str: str):
     try:
         request = json.loads(request_str)
         print(f"# make_generate_request request {request}")
 
         response = ollama.generate(**request)
         print(f"  $ success {response}")
     except Exception as error:
@@ -16,8 +21,11 @@
         response = {
             "error": {"type": str(error.__class__.__name__), "message": str(error)}
         }
         print(
             f"    * error response {response}",
         )
 
+        # Rethrow exception in order to be handled by base class
+        raise
+
     return response
```

### Comparing `oshepherd-0.0.4/oshepherd.egg-info/PKG-INFO` & `oshepherd-0.0.5/oshepherd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oshepherd
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Oshepherd guiding the Ollama(s) inference orchestration.
 Author: mnemonica.ai
 Author-email: "mnemonica.ai" <info@mnemonica.ai>
 Project-URL: Homepage, https://github.com/mnemonica-ai/oshepherd
 Project-URL: Issues, https://github.com/mnemonica-ai/oshepherd/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `oshepherd-0.0.4/oshepherd.egg-info/SOURCES.txt` & `oshepherd-0.0.5/oshepherd.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 oshepherd/api/utils.py
 oshepherd/api/generate/__init__.py
 oshepherd/api/generate/models.py
 oshepherd/api/generate/routes.py
 oshepherd/worker/__init__.py
 oshepherd/worker/app.py
 oshepherd/worker/config.py
+oshepherd/worker/ollama_task.py
 oshepherd/worker/tasks.py
```

### Comparing `oshepherd-0.0.4/pyproject.toml` & `oshepherd-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "oshepherd"
-version = "0.0.4"
+version = "0.0.5"
 description = "The Oshepherd guiding the Ollama(s) inference orchestration."
 readme = "README.md"
 authors = [
     {name = "mnemonica.ai", email = "info@mnemonica.ai"},
 ]
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `oshepherd-0.0.4/setup.py` & `oshepherd-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="oshepherd",
-    version="0.0.4",
+    version="0.0.5",
     description="The Oshepherd guiding the Ollama(s) inference orchestration.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="mnemonica.ai",
     author_email="info@mnemonica.ai",
     packages=find_packages(),
     python_requires=">=3.8",
```

