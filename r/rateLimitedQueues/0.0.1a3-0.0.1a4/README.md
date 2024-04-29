# Comparing `tmp/ratelimitedqueues-0.0.1a3.tar.gz` & `tmp/ratelimitedqueues-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratelimitedqueues-0.0.1a3.tar", last modified: Sun Apr 28 14:45:47 2024, max compression
+gzip compressed data, was "ratelimitedqueues-0.0.1a4.tar", last modified: Sun Apr 28 16:54:14 2024, max compression
```

## Comparing `ratelimitedqueues-0.0.1a3.tar` & `ratelimitedqueues-0.0.1a4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:45:47.045887 ratelimitedqueues-0.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 14:45:47.041887 ratelimitedqueues-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-28 14:45:42.000000 ratelimitedqueues-0.0.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-28 14:45:42.000000 ratelimitedqueues-0.0.1a3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 14:45:47.041887 ratelimitedqueues-0.0.1a3/rateLimitedQueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 14:45:47.000000 ratelimitedqueues-0.0.1a3/rateLimitedQueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-28 14:45:47.000000 ratelimitedqueues-0.0.1a3/rateLimitedQueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 14:45:47.000000 ratelimitedqueues-0.0.1a3/rateLimitedQueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 14:45:47.000000 ratelimitedqueues-0.0.1a3/rateLimitedQueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-28 14:45:42.000000 ratelimitedqueues-0.0.1a3/rateLimitedQueues.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 14:45:47.045887 ratelimitedqueues-0.0.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:54:14.498387 ratelimitedqueues-0.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 16:54:14.494387 ratelimitedqueues-0.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-28 16:54:09.000000 ratelimitedqueues-0.0.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-28 16:54:09.000000 ratelimitedqueues-0.0.1a4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:54:14.494387 ratelimitedqueues-0.0.1a4/rateLimitedQueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 16:54:14.000000 ratelimitedqueues-0.0.1a4/rateLimitedQueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-28 16:54:14.000000 ratelimitedqueues-0.0.1a4/rateLimitedQueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:54:14.000000 ratelimitedqueues-0.0.1a4/rateLimitedQueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 16:54:14.000000 ratelimitedqueues-0.0.1a4/rateLimitedQueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-28 16:54:09.000000 ratelimitedqueues-0.0.1a4/rateLimitedQueues.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:54:14.498387 ratelimitedqueues-0.0.1a4/setup.cfg
```

### Comparing `ratelimitedqueues-0.0.1a3/PKG-INFO` & `ratelimitedqueues-0.0.1a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rateLimitedQueues
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 Maintainer-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/rateLimitedQueues
 Keywords: thread,threaded,task,threaded task,queue,queues,queued tasks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# rateLimitedQueues v0.0.1a3
+# rateLimitedQueues v0.0.1a4
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install:
```

### Comparing `ratelimitedqueues-0.0.1a3/README.md` & `ratelimitedqueues-0.0.1a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# rateLimitedQueues v0.0.1a3
+# rateLimitedQueues v0.0.1a4
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install:
```

### Comparing `ratelimitedqueues-0.0.1a3/pyproject.toml` & `ratelimitedqueues-0.0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateLimitedQueues"
-version = "0.0.1a3"
+version = "0.0.1a4"
 description = "A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence."
 readme = "README.md"
 maintainers = [{ name = "Bhindi", email = "bhaskarpanja93@gmail.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `ratelimitedqueues-0.0.1a3/rateLimitedQueues.egg-info/PKG-INFO` & `ratelimitedqueues-0.0.1a4/rateLimitedQueues.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rateLimitedQueues
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 Maintainer-email: Bhindi <bhaskarpanja93@gmail.com>
 Project-URL: Homepage, https://github.com/BhaskarPanja93/rateLimitedQueues
 Keywords: thread,threaded,task,threaded task,queue,queues,queued tasks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# rateLimitedQueues v0.0.1a3
+# rateLimitedQueues v0.0.1a4
 
 ```pip install rateLimitedQueues --upgrade```
 
 
 ###### <br>A well maintained program to execute functions in queue as if only 1 worker is executing them one by one (High priority first). Works wonders when a series of time consuming tasks has to be performed but they need to be in sequence.
 
 <br>To install:
```

### Comparing `ratelimitedqueues-0.0.1a3/rateLimitedQueues.py` & `ratelimitedqueues-0.0.1a4/rateLimitedQueues.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1a3"
+__version__ = "0.0.1a4"
 __packagename__ = "rateLimitedQueues"
 
 
 def updatePackage():
     from time import sleep
     from json import loads
     import http.client
@@ -49,31 +49,36 @@
         :return:
         """
         if self.__workerIdle: self.__workerIdle = False
         else: return
         while self.__tasks:
             topPriorityTasks = self.__tasks.pop(max(self.__tasks))
             for task in topPriorityTasks:
-                mainFunction, postFunction, args, kwargs, executeThreaded = task
+                mainFunction, args, kwargs, executeThreaded, postFunction, postArgs, postKwArgs = task
+                if postKwArgs is None: postKwArgs = {}
+                if postArgs is None: postArgs = ()
                 if self.maxRateLimitWaitDuration >= self.minRateLimitWaitDuration: Imports.sleep(self.maxRateLimitWaitDuration)
-                if not executeThreaded:
-                    if postFunction is not None: Imports.Thread(target=postFunction, args=args, kwargs={"functionResponse":mainFunction(*args, **kwargs)}.update(kwargs)).start()
-                    else: mainFunction(*args, **kwargs)
-                else: Imports.Thread(target=mainFunction, args=args, kwargs=kwargs).start()
+                if executeThreaded: Imports.Thread(target=mainFunction, args=args, kwargs=kwargs).start()
+                else: postKwArgs.update({"functionResponse": mainFunction(*args, **kwargs)})
+                if postFunction is not None: Imports.Thread(target=postFunction, args=postArgs, kwargs=postKwArgs).start()
         self.__workerIdle = True
 
 
-    def queueAction(self, mainFunction, executePriority:int=0, executeThreaded: bool = False, postFunction = None, *args, **kwargs):
+    def queueAction(self, mainFunction, executePriority:int=0, executeThreaded: bool = False, postFunction = None, postArgs:tuple = None, postKwArgs:dict = None, *args, **kwargs):
         """
         Queue a new function to be executed
+        :param postKwArgs:
+        :param postArgs:
         :param postFunction:
         :param mainFunction:
         :param executePriority:
         :param executeThreaded:
         :return:
         """
         if not callable(mainFunction): return print("Please pass a callable object as the `mainFunction` parameter...")
         if postFunction is not None and not callable(postFunction): return print("Please pass a callable object as the `postFunction` parameter...")
-        execList = [mainFunction, postFunction, args, kwargs, executeThreaded]
+        if postArgs is not None and type(postArgs)!=tuple: return print("Please pass a tuple as postArgs...")
+        if postKwArgs is not None and type(postKwArgs)!=dict: return print("Please pass a dictionary as postKwArgs...")
+        execList = [mainFunction, args, kwargs, executeThreaded, postFunction, postArgs, postKwArgs]
         if executePriority in self.__tasks: self.__tasks[executePriority].append(execList)
         else: self.__tasks[executePriority] = [execList]
         Imports.Thread(target=self.__startExecution).start()
```

