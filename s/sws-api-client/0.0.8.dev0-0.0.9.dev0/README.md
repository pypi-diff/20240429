# Comparing `tmp/sws_api_client-0.0.8.dev0.tar.gz` & `tmp/sws_api_client-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sws_api_client-0.0.8.dev0.tar", last modified: Mon Apr 29 07:10:36 2024, max compression
+gzip compressed data, was "sws_api_client-0.0.9.dev0.tar", last modified: Mon Apr 29 08:40:20 2024, max compression
```

## Comparing `sws_api_client-0.0.8.dev0.tar` & `sws_api_client-0.0.9.dev0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 07:10:36.598048 sws_api_client-0.0.8.dev0/
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1073 2024-02-29 08:07:44.000000 sws_api_client-0.0.8.dev0/LICENSE
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-04-29 07:10:36.597595 sws_api_client-0.0.8.dev0/PKG-INFO
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 08:07:44.000000 sws_api_client-0.0.8.dev0/README.md
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)       38 2024-04-29 07:10:36.598147 sws_api_client-0.0.8.dev0/setup.cfg
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1175 2024-04-29 07:08:34.000000 sws_api_client-0.0.8.dev0/setup.py
-drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 07:10:36.594175 sws_api_client-0.0.8.dev0/sws_api_client/
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      232 2024-02-29 11:45:11.000000 sws_api_client-0.0.8.dev0/sws_api_client/__init__.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      431 2024-02-29 10:31:01.000000 sws_api_client-0.0.8.dev0/sws_api_client/datasets.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 12:02:55.000000 sws_api_client-0.0.8.dev0/sws_api_client/discover.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3420 2024-03-01 16:39:27.000000 sws_api_client-0.0.8.dev0/sws_api_client/sws_api_client.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      609 2024-02-29 10:50:25.000000 sws_api_client-0.0.8.dev0/sws_api_client/tags.py
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     6777 2024-04-29 07:06:00.000000 sws_api_client-0.0.8.dev0/sws_api_client/tasks.py
-drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 07:10:36.597072 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/PKG-INFO
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)      376 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)        1 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)       34 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/requires.txt
--rw-r--r--   0 matteoterrinoni   (501) staff       (20)       15 2024-04-29 07:10:36.000000 sws_api_client-0.0.8.dev0/sws_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 08:40:20.754734 sws_api_client-0.0.9.dev0/
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1073 2024-02-29 08:07:44.000000 sws_api_client-0.0.9.dev0/LICENSE
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-04-29 08:40:20.754289 sws_api_client-0.0.9.dev0/PKG-INFO
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 08:07:44.000000 sws_api_client-0.0.9.dev0/README.md
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)       38 2024-04-29 08:40:20.754823 sws_api_client-0.0.9.dev0/setup.cfg
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     1175 2024-04-29 08:39:25.000000 sws_api_client-0.0.9.dev0/setup.py
+drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 08:40:20.751002 sws_api_client-0.0.9.dev0/sws_api_client/
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      232 2024-02-29 11:45:11.000000 sws_api_client-0.0.9.dev0/sws_api_client/__init__.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      431 2024-02-29 10:31:01.000000 sws_api_client-0.0.9.dev0/sws_api_client/datasets.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     2258 2024-02-29 12:02:55.000000 sws_api_client-0.0.9.dev0/sws_api_client/discover.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3420 2024-03-01 16:39:27.000000 sws_api_client-0.0.9.dev0/sws_api_client/sws_api_client.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      609 2024-02-29 10:50:25.000000 sws_api_client-0.0.9.dev0/sws_api_client/tags.py
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     7056 2024-04-29 08:34:39.000000 sws_api_client-0.0.9.dev0/sws_api_client/tasks.py
+drwxr-xr-x   0 matteoterrinoni   (501) staff       (20)        0 2024-04-29 08:40:20.753707 sws_api_client-0.0.9.dev0/sws_api_client.egg-info/
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)     3039 2024-04-29 08:40:20.000000 sws_api_client-0.0.9.dev0/sws_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)      376 2024-04-29 08:40:20.000000 sws_api_client-0.0.9.dev0/sws_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)        1 2024-04-29 08:40:20.000000 sws_api_client-0.0.9.dev0/sws_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)       34 2024-04-29 08:40:20.000000 sws_api_client-0.0.9.dev0/sws_api_client.egg-info/requires.txt
+-rw-r--r--   0 matteoterrinoni   (501) staff       (20)       15 2024-04-29 08:40:20.000000 sws_api_client-0.0.9.dev0/sws_api_client.egg-info/top_level.txt
```

### Comparing `sws_api_client-0.0.8.dev0/LICENSE` & `sws_api_client-0.0.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.8.dev0/PKG-INFO` & `sws_api_client-0.0.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sws_api_client
-Version: 0.0.8.dev0
+Version: 0.0.9.dev0
 Summary: A Python client to easily interact with the FAO SWS REST APIs
 Home-page: https://bitbucket.org/cioapps/sws-it-python-api-client/src/main/
 Author: Mansillo, Daniele (CSI)
 Author-email: <daniele.mansillo@fao.com>
 Keywords: python,fao,sws,rest,api,client
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `sws_api_client-0.0.8.dev0/README.md` & `sws_api_client-0.0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.8.dev0/setup.py` & `sws_api_client-0.0.9.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.8-dev"
+VERSION = "0.0.9-dev"
 
 # Setting up
 setup(
     name="sws_api_client",
     version=VERSION,
     author="Mansillo, Daniele (CSI)",
     author_email="<daniele.mansillo@fao.com>",
```

### Comparing `sws_api_client-0.0.8.dev0/sws_api_client/discover.py` & `sws_api_client-0.0.9.dev0/sws_api_client/discover.py`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.8.dev0/sws_api_client/sws_api_client.py` & `sws_api_client-0.0.9.dev0/sws_api_client/sws_api_client.py`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.8.dev0/sws_api_client/tags.py` & `sws_api_client-0.0.9.dev0/sws_api_client/tags.py`

 * *Files identical despite different names*

### Comparing `sws_api_client-0.0.8.dev0/sws_api_client/tasks.py` & `sws_api_client-0.0.9.dev0/sws_api_client/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,30 +108,30 @@
         else:
             return None
 
     def get_task_response(self, task: Dict) -> TaskResponse:
         return TaskResponse(
             task_id=task['taskId'],
             info=TaskInfo(
-                detail_status=task['info'].get('detailStatus'),
-                ended_on=task['info'].get('endedOn'),
-                description=task['info'].get('description'),
-                updated_on=task['info'].get('updatedOn'),
-                created_on=task['info'].get('createdOn'),
-                service_user=task['info'].get('serviceUser'),
-                tags=task['info'].get('tags'),
-                output=task['info'].get('output'),
-                input=json.loads(task['info'].get('input', '{}')),  # Default to an empty dictionary if 'input' is missing
-                task_type=task['info'].get('taskType'),
-                context=task['info'].get('context'),
-                progress=task['info'].get('progress'),
-                user=task['info'].get('user'),
-                outcome=task['info'].get('outcome'),
-                status=task['info'].get('status'),
-                group=task['info'].get('group')
+                detail_status=task.get('info').get('detailStatus'),
+                ended_on=task.get('info').get('endedOn'),
+                description=task.get('info').get('description'),
+                updated_on=task.get('info').get('updatedOn'),
+                created_on=task.get('info').get('createdOn'),
+                service_user=task.get('info').get('serviceUser'),
+                tags=task.get('info').get('tags'),
+                output=task.get('info').get('output'),
+                input=json.loads(task.get('info').get('input', '{}')),  # Default to an empty dictionary if 'input' is missing
+                task_type=task.get('info').get('taskType'),
+                context=task.get('info').get('context'),
+                progress=task.get('info').get('progress'),
+                user=task.get('info').get('user'),
+                outcome=task.get('info').get('outcome'),
+                status=task.get('info').get('status'),
+                group=task.get('group')
             )
         )
     
     def get_task_create_response(self, task: Dict) -> TaskCreateResponse:
         return TaskCreateResponse(
             task_id=task['taskId']
         )
@@ -161,26 +161,31 @@
         Args:
             task_id (str): The ID of the task.
             poll_interval (int, optional): The interval (in seconds) between status checks. Defaults to 10.
 
         Returns:
             str: The final outcome of the task.
         """
+        not_created_counter = 0
         while True:
             task_response = self.get_task(task_id)
 
-            if not task_response:
+            if not task_response and not_created_counter > 5:
                 raise ValueError(f"Task with ID {task_id} not found.")
+            elif not task_response:
+                not_created_counter += 1
+            else:
+                not_created_counter = 0
+            
+                task_status = task_response.info.detail_status
+                print(f"Task {task_id} status: {task_status}")
+                if task_status == 'ENDED':
+                    return task_response
 
-            task_status = task_response.info.detail_status
-            print(f"Task {task_id} status: {task_status}")
-            if task_status == 'ENDED':
-                return task_response
-
-            time.sleep(poll_interval)
+                time.sleep(poll_interval)
 
     def wait_completion_by_ids(self, task_ids: List[str], poll_interval: int = 10) -> List[TaskResponse]:
         """
         Wait for a list of tasks to reach the 'ENDED' status and return the task outcomes.
 
         Args:
             task_ids (List[str]): The IDs of the tasks.
```

### Comparing `sws_api_client-0.0.8.dev0/sws_api_client.egg-info/PKG-INFO` & `sws_api_client-0.0.9.dev0/sws_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sws_api_client
-Version: 0.0.8.dev0
+Version: 0.0.9.dev0
 Summary: A Python client to easily interact with the FAO SWS REST APIs
 Home-page: https://bitbucket.org/cioapps/sws-it-python-api-client/src/main/
 Author: Mansillo, Daniele (CSI)
 Author-email: <daniele.mansillo@fao.com>
 Keywords: python,fao,sws,rest,api,client
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

