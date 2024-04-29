# Comparing `tmp/sws_api_client-0.0.7.dev0.tar.gz` & `tmp/sws_api_client-0.0.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sws_api_client-0.0.7.dev0.tar", last modified: Sun Mar  3 14:23:23 2024, max compression
+gzip compressed data, was "sws_api_client-0.0.8.dev0.tar", last modified: Mon Apr 29 07:10:36 2024, max compression
```

## Comparing `sws_api_client-0.0.7.dev0.tar` & `sws_api_client-0.0.8.dev0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-03-03 14:23:23.692315 sws_api_client-0.0.7.dev0/
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1073 2024-02-29 08:07:44.000000 sws_api_client-0.0.7.dev0/LICENSE
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-03-03 14:23:23.691350 sws_api_client-0.0.7.dev0/PKG-INFO
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 08:07:44.000000 sws_api_client-0.0.7.dev0/README.md
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)       38 2024-03-03 14:23:23.692502 sws_api_client-0.0.7.dev0/setup.cfg
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1175 2024-03-03 14:21:47.000000 sws_api_client-0.0.7.dev0/setup.py
-drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-03-03 14:23:23.685327 sws_api_client-0.0.7.dev0/sws_api_client/
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      232 2024-02-29 11:45:11.000000 sws_api_client-0.0.7.dev0/sws_api_client/__init__.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      431 2024-02-29 10:31:01.000000 sws_api_client-0.0.7.dev0/sws_api_client/datasets.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 12:02:55.000000 sws_api_client-0.0.7.dev0/sws_api_client/discover.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3420 2024-03-01 16:39:27.000000 sws_api_client-0.0.7.dev0/sws_api_client/sws_api_client.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      609 2024-02-29 10:50:25.000000 sws_api_client-0.0.7.dev0/sws_api_client/tags.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     6545 2024-03-03 14:16:04.000000 sws_api_client-0.0.7.dev0/sws_api_client/tasks.py
-drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-03-03 14:23:23.690300 sws_api_client-0.0.7.dev0/sws_api_client.egg-info/
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-03-03 14:23:23.000000 sws_api_client-0.0.7.dev0/sws_api_client.egg-info/PKG-INFO
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      376 2024-03-03 14:23:23.000000 sws_api_client-0.0.7.dev0/sws_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)        1 2024-03-03 14:23:23.000000 sws_api_client-0.0.7.dev0/sws_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)       34 2024-03-03 14:23:23.000000 sws_api_client-0.0.7.dev0/sws_api_client.egg-info/requires.txt
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)       15 2024-03-03 14:23:23.000000 sws_api_client-0.0.7.dev0/sws_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 07:10:36.598048 sws_api_client-0.0.8.dev0/
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1073 2024-02-29 08:07:44.000000 sws_api_client-0.0.8.dev0/LICENSE
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-04-29 07:10:36.597595 sws_api_client-0.0.8.dev0/PKG-INFO
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 08:07:44.000000 sws_api_client-0.0.8.dev0/README.md
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)       38 2024-04-29 07:10:36.598147 sws_api_client-0.0.8.dev0/setup.cfg
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1175 2024-04-29 07:08:34.000000 sws_api_client-0.0.8.dev0/setup.py
+drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 07:10:36.594175 sws_api_client-0.0.8.dev0/sws_api_client/
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      232 2024-02-29 11:45:11.000000 sws_api_client-0.0.8.dev0/sws_api_client/__init__.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      431 2024-02-29 10:31:01.000000 sws_api_client-0.0.8.dev0/sws_api_client/datasets.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 12:02:55.000000 sws_api_client-0.0.8.dev0/sws_api_client/discover.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3420 2024-03-01 16:39:27.000000 sws_api_client-0.0.8.dev0/sws_api_client/sws_api_client.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      609 2024-02-29 10:50:25.000000 sws_api_client-0.0.8.dev0/sws_api_client/tags.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     6777 2024-04-29 07:06:00.000000 sws_api_client-0.0.8.dev0/sws_api_client/tasks.py
+drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 07:10:36.597072 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      376 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)        1 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)       34 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/requires.txt
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)       15 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/top_level.txt
```

### Comparing `sws_api_client-0.0.7.dev0/LICENSE` & `sws_api_client-0.0.8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.7.dev0/PKG-INFO` & `sws_api_client-0.0.8.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sws_api_client
-Version: 0.0.7.dev0
+Version: 0.0.8.dev0
 Summary: A Python client to easily interact with the FAO SWS REST APIs
 Home-page: https://bitbucket.org/cioapps/sws-it-python-api-client/src/main/
 Author: Mansillo, Daniele (CSI)
 Author-email: <daniele.mansillo@fao.com>
 Keywords: python,fao,sws,rest,api,client
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `sws_api_client-0.0.7.dev0/README.md` & `sws_api_client-0.0.8.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.7.dev0/setup.py` & `sws_api_client-0.0.8.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.7-dev"
+VERSION = "0.0.8-dev"
 
 # Setting up
 setup(
     name="sws_api_client",
     version=VERSION,
     author="Mansillo, Daniele (CSI)",
     author_email="<daniele.mansillo@fao.com>",
```

### Comparing `sws_api_client-0.0.7.dev0/sws_api_client/discover.py` & `sws_api_client-0.0.8.dev0/sws_api_client/discover.py`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.7.dev0/sws_api_client/sws_api_client.py` & `sws_api_client-0.0.8.dev0/sws_api_client/sws_api_client.py`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.7.dev0/sws_api_client/tags.py` & `sws_api_client-0.0.8.dev0/sws_api_client/tags.py`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.7.dev0/sws_api_client/tasks.py` & `sws_api_client-0.0.8.dev0/sws_api_client/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,18 @@
     status: Status
 
 @dataclass
 class TaskResponse:
     task_id: str
     info: TaskInfo
 
+@dataclass
+class TaskCreateResponse:
+    task_id: str
+
 class TaskManager:
 
     def __init__(self, sws_client: SwsApiClient, endpoint: str = 'task_manager_api') -> None:
         self.sws_client = sws_client
         self.endpoint = endpoint
 
     def update_current(self, progress: Optional[int] = None):
@@ -71,15 +75,15 @@
             pluginId:str,
             slow:bool,
             payload: PluginPayload,
             description: Optional[str],
             group: Optional[str] = None,
             parentTaskId: Optional[str] = None,
             user:Optional[str] = None
-        ) -> TaskResponse:
+        ) -> TaskCreateResponse:
         
         path = 'task/create'
 
         data = {
             "user": user,
             "context": "IS",
             "type": "RUN_PLUGIN",
@@ -96,15 +100,15 @@
         }
 
         if group:
             data['group'] = group
 
         response = self.sws_client.discoverable.post(self.endpoint, path, data=data)
         if response:
-            return self.get_task_response(response)
+            return self.get_task_create_response(response)
         else:
             return None
 
     def get_task_response(self, task: Dict) -> TaskResponse:
         return TaskResponse(
             task_id=task['taskId'],
             info=TaskInfo(
@@ -122,14 +126,19 @@
                 progress=task['info'].get('progress'),
                 user=task['info'].get('user'),
                 outcome=task['info'].get('outcome'),
                 status=task['info'].get('status'),
                 group=task['info'].get('group')
             )
         )
+    
+    def get_task_create_response(self, task: Dict) -> TaskCreateResponse:
+        return TaskCreateResponse(
+            task_id=task['taskId']
+        )
 
 
     def get_task(self, task_id: str) -> Optional[TaskResponse]:
         path = f'/task/{task_id}'
         response = self.sws_client.discoverable.get(self.endpoint, path)
 
         if response:
@@ -183,8 +192,9 @@
         completed_tasks = []
         while True:
             tasks_response = self.get_tasks_by_ids(task_ids)
             completed_tasks = [task for task in tasks_response if task.info.detail_status == 'ENDED']
             if len(completed_tasks) == len(task_ids):
                 return completed_tasks
 
-            time.sleep(poll_interval)
+            time.sleep(poll_interval)
+
```

### Comparing `sws_api_client-0.0.7.dev0/sws_api_client.egg-info/PKG-INFO` & `sws_api_client-0.0.8.dev0/sws_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sws_api_client
-Version: 0.0.7.dev0
+Version: 0.0.8.dev0
 Summary: A Python client to easily interact with the FAO SWS REST APIs
 Home-page: https://bitbucket.org/cioapps/sws-it-python-api-client/src/main/
 Author: Mansillo, Daniele (CSI)
 Author-email: <daniele.mansillo@fao.com>
 Keywords: python,fao,sws,rest,api,client
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

