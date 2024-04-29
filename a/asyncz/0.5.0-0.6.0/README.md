# Comparing `tmp/asyncz-0.5.0.tar.gz` & `tmp/asyncz-0.6.0.tar.gz`

## Comparing `asyncz-0.5.0.tar` & `asyncz-0.6.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/_mapping.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/datastructures.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/enums.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/py.typed
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/state.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/typing.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/esmerald/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/esmerald/decorator.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/esmerald/scheduler.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/events/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/events/base.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/events/constants.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/asyncio.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/base.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/debug.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/pool.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/types.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/__init__.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/asyncio.py
--rw-r--r--   0        0        0    39885 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/base.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/datastructures.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/types.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/__init__.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/base.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/memory.py
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/mongo.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/redis.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/types.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/tasks/__init__.py
--rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/tasks/base.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/tasks/types.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/__init__.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/base.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/combination.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/date.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/interval.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/types.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/constants.py
--rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/expressions.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/fields.py
--rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/trigger.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/types.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.5.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.5.0/LICENSE
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.5.0/README.md
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 asyncz-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 asyncz-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/_mapping.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/datastructures.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/enums.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/py.typed
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/state.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/typing.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/contrib/esmerald/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/contrib/esmerald/decorator.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/contrib/esmerald/scheduler.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/events/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/events/base.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/events/constants.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/executors/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/executors/asyncio.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/executors/base.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/executors/debug.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/executors/pool.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/executors/types.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/schedulers/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/schedulers/asyncio.py
+-rw-r--r--   0        0        0    39885 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/schedulers/base.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/schedulers/datastructures.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/schedulers/types.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/schedulers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/stores/__init__.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/stores/base.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/stores/memory.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/stores/mongo.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/stores/redis.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/stores/types.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/tasks/__init__.py
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/tasks/base.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/tasks/types.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/__init__.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/base.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/combination.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/date.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/interval.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/types.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/cron/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/cron/constants.py
+-rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/cron/expressions.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/cron/fields.py
+-rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/cron/trigger.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.6.0/asyncz/triggers/cron/types.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.6.0/README.md
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 asyncz-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 asyncz-0.6.0/PKG-INFO
```

### Comparing `asyncz-0.5.0/asyncz/_mapping.py` & `asyncz-0.6.0/asyncz/_mapping.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/datastructures.py` & `asyncz-0.6.0/asyncz/datastructures.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/exceptions.py` & `asyncz-0.6.0/asyncz/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/state.py` & `asyncz-0.6.0/asyncz/state.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/utils.py` & `asyncz-0.6.0/asyncz/utils.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/contrib/esmerald/decorator.py` & `asyncz-0.6.0/asyncz/contrib/esmerald/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,30 +10,30 @@
         self,
         *,
         name: Optional[str] = None,
         trigger: Optional[TriggerType] = None,
         id: Optional[str] = None,
         mistrigger_grace_time: Optional[int] = None,
         coalesce: Optional[bool] = None,
-        max_intances: Optional[int] = None,
+        max_instances: Optional[int] = None,
         next_run_time: Optional[datetime] = None,
         store: Optional[str] = "default",
         executor: Optional[str] = "default",
         replace_existing: bool = True,
         extra_args: Optional[Any] = None,
         extra_kwargs: Optional[Dict[str, Any]] = None,
         is_enabled: bool = True,
     ) -> None:
         super().__init__(
             name=name,
             trigger=trigger,
             id=id,
             mistrigger_grace_time=mistrigger_grace_time,
             coalesce=coalesce,
-            max_intances=max_intances,
+            max_instances=max_instances,
             next_run_time=next_run_time,
             store=store,
             executor=executor,
             replace_existing=replace_existing,
             args=extra_args,
             kwargs=extra_kwargs,
             is_enabled=is_enabled,
```

### Comparing `asyncz-0.5.0/asyncz/contrib/esmerald/scheduler.py` & `asyncz-0.6.0/asyncz/contrib/esmerald/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         self,
         *,
         name: Optional[str] = None,
         trigger: Optional[TriggerType] = None,
         id: Optional[str] = None,
         mistrigger_grace_time: Optional[int] = None,
         coalesce: Optional[bool] = None,
-        max_intances: Optional[int] = None,
+        max_instances: Optional[int] = None,
         next_run_time: Optional[datetime] = None,
         store: Optional[str] = "default",
         executor: Optional[str] = "default",
         replace_existing: bool = False,
         args: Optional[Any] = None,
         kwargs: Optional[Dict[str, Any]] = None,
         is_enabled: bool = True,
@@ -159,30 +159,30 @@
         Args:
             name: Textual description of the task.
             trigger: An instance of a trigger class.
             identifier: Explicit identifier for the task.
             mistrigger_grace_time: Seconds after the designated runtime that the task is still allowed to be run (or None to allow the task to run no
                 matter  how late it is).
             coalesce: Run once instead of many times if the scheduler determines that the task should be run more than once in succession.
-            max_intances: Maximum number of concurrently running instances allowed for this task.
+            max_instances: Maximum number of concurrently running instances allowed for this task.
             next_run_time: When to first run the task, regardless of the trigger (pass None to add the task as paused).
             store: Alias of the task store to store the task in.
             executor: Alias of the executor to run the task with.
             replace_existing: True to replace an existing task with the same id
                 (but retain the number of runs from the existing one).
             args: List of positional arguments to call func with.
             kwargs: Dict of keyword arguments to call func with.
             is_enabled: True if the the task to be added to the scheduler.
         """
         self.name = name
         self.trigger = trigger
         self.id = id
         self.mistrigger_grace_time = mistrigger_grace_time or undefined
         self.coalesce = coalesce or undefined
-        self.max_intances = max_intances or undefined
+        self.max_instances = max_instances or undefined
         self.next_run_time = next_run_time or undefined
         self.store = store
         self.executor = executor
         self.replace_existing = replace_existing
         self.args = args
         self.kwargs = kwargs
         self.is_enabled = is_enabled
@@ -195,15 +195,15 @@
                 trigger=self.trigger,
                 args=self.args,
                 kwargs=self.kwargs,
                 id=self.id,
                 name=self.name,
                 mistrigger_grace_time=self.mistrigger_grace_time,
                 coalesce=self.coalesce,
-                max_instances=self.max_intances,
+                max_instances=self.max_instances,
                 next_run_time=self.next_run_time,
                 store=self.store,
                 executor=self.executor,
                 replace_existing=self.replace_existing,
             )
         except Exception as e:
             raise ImproperlyConfigured(str(e)) from e
```

### Comparing `asyncz-0.5.0/asyncz/events/base.py` & `asyncz-0.6.0/asyncz/events/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/events/constants.py` & `asyncz-0.6.0/asyncz/events/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/executors/asyncio.py` & `asyncz-0.6.0/asyncz/executors/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/executors/base.py` & `asyncz-0.6.0/asyncz/executors/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/executors/debug.py` & `asyncz-0.6.0/asyncz/executors/debug.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/executors/pool.py` & `asyncz-0.6.0/asyncz/executors/pool.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/schedulers/asyncio.py` & `asyncz-0.6.0/asyncz/schedulers/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/schedulers/base.py` & `asyncz-0.6.0/asyncz/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/schedulers/datastructures.py` & `asyncz-0.6.0/asyncz/schedulers/datastructures.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/stores/base.py` & `asyncz-0.6.0/asyncz/stores/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/stores/memory.py` & `asyncz-0.6.0/asyncz/stores/memory.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/stores/mongo.py` & `asyncz-0.6.0/asyncz/stores/mongo.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/stores/redis.py` & `asyncz-0.6.0/asyncz/stores/redis.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/tasks/base.py` & `asyncz-0.6.0/asyncz/tasks/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/base.py` & `asyncz-0.6.0/asyncz/triggers/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/combination.py` & `asyncz-0.6.0/asyncz/triggers/combination.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/date.py` & `asyncz-0.6.0/asyncz/triggers/date.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/interval.py` & `asyncz-0.6.0/asyncz/triggers/interval.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/cron/constants.py` & `asyncz-0.6.0/asyncz/triggers/cron/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/cron/expressions.py` & `asyncz-0.6.0/asyncz/triggers/cron/expressions.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/asyncz/triggers/cron/fields.py` & `asyncz-0.6.0/asyncz/triggers/cron/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __init__(
         self,
         name: str,
         exprs: Any,
         is_default: Optional[bool] = False,
         compilers: Optional[List[Any]] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.name = name
         self.is_default = is_default
         self.exprs = exprs
         self.compilers = [AllExpression, RangeExpression]
```

### Comparing `asyncz-0.5.0/asyncz/triggers/cron/trigger.py` & `asyncz-0.6.0/asyncz/triggers/cron/trigger.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/LICENSE` & `asyncz-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/README.md` & `asyncz-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncz-0.5.0/pyproject.toml` & `asyncz-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "asyncio>=3.4.3,<4.0.0",
     "loguru>=0.7.0,<0.8.0",
-    "pydantic>=2.1.1,<3.0.0",
+    "pydantic>=2.5.3,<3.0.0",
     "pytz>=2022.6",
     "tzlocal>=4.2,<5.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
@@ -73,32 +73,33 @@
 Source = "https://github.com/tarsil/asyncz"
 
 [project.optional-dependencies]
 test = [
     # "esmerald==0.4.2",
     "mock>=4.0.3",
     "pymongo>=4.3.3,<5.0.0",
-    "pytest >=7.1.3,<8.0.0",
-    "pytest-cov >=2.12.0,<5.0.0",
+    "pytest>=7.1.3,<9.0.0",
+    "pytest-cov >=2.12.0,<6.0.0",
     "pytest-asyncio >=0.19.0,<1.0.0",
     "pytest-loguru>=0.2.0,<1",
-    "redis>=4.4.0,<5.0.0",
+    "redis>=4.4.0,<6.0.0",
     "requests >=2.27.0,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
 ]
 
 dev = [
-    "autoflake >=1.4.0,<3.0.0",
-    "black>=22.10.0,<23.0.0",
-    "flake8>=3.8.3,<7.0.0",
+    "autoflake>=1.4.0,<3.0.0",
+    "black==24.4.2",
+    "flake8>=3.8.3,<8.0.0",
     "ipdb>=0.13.13",
+    "pdbpp",
     "isort>=5.0.6,<6.0.0",
     "mypy>=0.982,<2.0.0",
     "pre-commit>=2.17.0,<3.0.0",
-    "watchfiles>=0.16.1,<0.20.0",
+    "watchfiles>=0.16.1,<0.22.0",
 ]
 
 doc = [
     "mkautodoc >=0.2.0,<0.3.0",
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=9.0.13,<10.0.0",
     "mdx-include >=1.4.2,<2.0.0",
@@ -126,27 +127,17 @@
 implicit_reexport = false
 show_error_codes = true
 disallow_incomplete_defs = true
 disable_error_code = "attr-defined"
 warn_unused_ignores = true
 warn_redundant_casts = true
 
-[tool.ruff]
-select = [
-    "E", # pycodestyle errors
-    "W", # pycodestyle warnings
-    "F", # pyflakes
-    "C", # flake8-comprehensions
-    "B", # flake8-bugbear
-]
-ignore = [
-    "E501", # line too long, handled by black
-    "B008", # do not perform function calls in argument defaults
-    "C901", # too complex
-]
+[tool.ruff.lint]
+select = ["E", "W", "F", "C", "B", "I"]
+ignore = ["E501", "B008", "C901", "B026"]
 
 exclude = ["docs_src/*"]
 
 [[tool.mypy.overrides]]
 module = "asyncz.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
```

### Comparing `asyncz-0.5.0/PKG-INFO` & `asyncz-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: asyncz
-Version: 0.5.0
+Version: 0.6.0
 Summary: The scheduler that nobody wants but every application needs.
 Project-URL: Homepage, https://github.com/tarsil/asyncz
 Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/asyncz
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -35,46 +35,47 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: asyncio<4.0.0,>=3.4.3
 Requires-Dist: loguru<0.8.0,>=0.7.0
-Requires-Dist: pydantic<3.0.0,>=2.1.1
+Requires-Dist: pydantic<3.0.0,>=2.5.3
 Requires-Dist: pytz>=2022.6
 Requires-Dist: tzlocal<5.0,>=4.2
 Provides-Extra: all
 Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all'
 Requires-Dist: pytz>=2022.6; extra == 'all'
 Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev'
-Requires-Dist: black<23.0.0,>=22.10.0; extra == 'dev'
-Requires-Dist: flake8<7.0.0,>=3.8.3; extra == 'dev'
+Requires-Dist: black==24.4.2; extra == 'dev'
+Requires-Dist: flake8<8.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: ipdb>=0.13.13; extra == 'dev'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev'
 Requires-Dist: mypy<2.0.0,>=0.982; extra == 'dev'
+Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
-Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
+Requires-Dist: watchfiles<0.22.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc'
 Requires-Dist: mkdocs-material<10.0.0,>=9.0.13; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: mock>=4.0.3; extra == 'test'
 Requires-Dist: pymongo<5.0.0,>=4.3.3; extra == 'test'
 Requires-Dist: pytest-asyncio<1.0.0,>=0.19.0; extra == 'test'
-Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
+Requires-Dist: pytest-cov<6.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest-loguru<1,>=0.2.0; extra == 'test'
-Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
-Requires-Dist: redis<5.0.0,>=4.4.0; extra == 'test'
+Requires-Dist: pytest<9.0.0,>=7.1.3; extra == 'test'
+Requires-Dist: redis<6.0.0,>=4.4.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.27.0; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Asyncz
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncz Version: 0.5.0 Summary: The scheduler that
+Metadata-Version: 2.3 Name: asyncz Version: 0.6.0 Summary: The scheduler that
 nobody wants but every application needs. Project-URL: Homepage, https://
 github.com/tarsil/asyncz Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/ Project-URL:
 Funding, https://github.com/sponsors/tarsil Project-URL: Source, https://
 github.com/tarsil/asyncz Author-email: Tiago Silva
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 api,apscheduler,asgi,asyncz,cron,fastapi,framework,http,machine
@@ -20,36 +20,37 @@
 Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
 Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Application Frameworks Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.8
 Requires-Dist: asyncio<4.0.0,>=3.4.3 Requires-Dist: loguru<0.8.0,>=0.7.0
-Requires-Dist: pydantic<3.0.0,>=2.1.1 Requires-Dist: pytz>=2022.6 Requires-
+Requires-Dist: pydantic<3.0.0,>=2.5.3 Requires-Dist: pytz>=2022.6 Requires-
 Dist: tzlocal<5.0,>=4.2 Provides-Extra: all Requires-Dist:
 asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist: pytz>=2022.6; extra ==
 'all' Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev' Requires-Dist:
-black<23.0.0,>=22.10.0; extra == 'dev' Requires-Dist: flake8<7.0.0,>=3.8.3;
-extra == 'dev' Requires-Dist: ipdb>=0.13.13; extra == 'dev' Requires-Dist:
+black==24.4.2; extra == 'dev' Requires-Dist: flake8<8.0.0,>=3.8.3; extra ==
+'dev' Requires-Dist: ipdb>=0.13.13; extra == 'dev' Requires-Dist:
 isort<6.0.0,>=5.0.6; extra == 'dev' Requires-Dist: mypy<2.0.0,>=0.982; extra ==
-'dev' Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist:
-watchfiles<0.20.0,>=0.16.1; extra == 'dev' Provides-Extra: doc Requires-Dist:
+'dev' Requires-Dist: pdbpp; extra == 'dev' Requires-Dist: pre-
+commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist:
+watchfiles<0.22.0,>=0.16.1; extra == 'dev' Provides-Extra: doc Requires-Dist:
 mdx-include<2.0.0,>=1.4.2; extra == 'doc' Requires-Dist:
 mkautodoc<0.3.0,>=0.2.0; extra == 'doc' Requires-Dist: mkdocs-
 markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc' Requires-Dist: mkdocs-
 material<10.0.0,>=9.0.13; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.1.2;
 extra == 'doc' Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc' Provides-Extra: test
 Requires-Dist: mock>=4.0.3; extra == 'test' Requires-Dist:
 pymongo<5.0.0,>=4.3.3; extra == 'test' Requires-Dist: pytest-
 asyncio<1.0.0,>=0.19.0; extra == 'test' Requires-Dist: pytest-
-cov<5.0.0,>=2.12.0; extra == 'test' Requires-Dist: pytest-loguru<1,>=0.2.0;
-extra == 'test' Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test' Requires-
-Dist: redis<5.0.0,>=4.4.0; extra == 'test' Requires-Dist:
+cov<6.0.0,>=2.12.0; extra == 'test' Requires-Dist: pytest-loguru<1,>=0.2.0;
+extra == 'test' Requires-Dist: pytest<9.0.0,>=7.1.3; extra == 'test' Requires-
+Dist: redis<6.0.0,>=4.4.0; extra == 'test' Requires-Dist:
 requests<3.0.0,>=2.27.0; extra == 'test' Requires-Dist: ruff<1.0.0,>=0.0.256;
 extra == 'test' Description-Content-Type: text/markdown # Asyncz
                                    _[_A_s_y_n_c_z_]
                   ?ð??? TThhee sscchheedduulleerr tthhaatt ssiimmppllyy wwoorrkkss.. ?ð???
            _[_T_e_s_t_ _S_u_i_t_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 --- **Documentation**: [https://asyncz.tarsild.io](https://asyncz.tarsild.io)
 ð **Source Code**: [https://github.com/tarsil/asyncz](https://github.com/
```

