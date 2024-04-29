# Comparing `tmp/edgegap_scheduling-0.1.0.tar.gz` & `tmp/edgegap_scheduling-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-0.1.0.tar", max compression
+gzip compressed data, was "edgegap_scheduling-0.1.1.tar", max compression
```

## Comparing `edgegap_scheduling-0.1.0.tar` & `edgegap_scheduling-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.375580 edgegap_scheduling-0.1.0/LICENSE
--rw-r--r--   0        0        0     2164 2024-04-29 14:47:02.455878 edgegap_scheduling-0.1.0/README.md
--rw-r--r--   0        0        0      324 2024-04-27 03:28:03.421729 edgegap_scheduling-0.1.0/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-04-25 13:10:38.954379 edgegap_scheduling-0.1.0/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0      402 2024-04-25 13:10:38.954460 edgegap_scheduling-0.1.0/edgegap_scheduling/_format.py
--rw-r--r--   0        0        0     2789 2024-04-27 04:24:27.836458 edgegap_scheduling-0.1.0/edgegap_scheduling/_model.py
--rw-r--r--   0        0        0     3390 2024-04-27 03:28:03.422097 edgegap_scheduling-0.1.0/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     3867 2024-04-27 03:28:03.421972 edgegap_scheduling-0.1.0/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1025 2024-04-25 13:10:38.955042 edgegap_scheduling-0.1.0/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-04-25 13:10:38.955122 edgegap_scheduling-0.1.0/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1233 2024-04-25 13:10:38.955206 edgegap_scheduling-0.1.0/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      188 2024-04-25 13:10:38.955422 edgegap_scheduling-0.1.0/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0      132 2024-04-25 20:04:14.788186 edgegap_scheduling-0.1.0/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-04-25 20:04:14.717257 edgegap_scheduling-0.1.0/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      494 2024-04-29 14:49:23.434068 edgegap_scheduling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 edgegap_scheduling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.375580 edgegap_scheduling-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2164 2024-04-29 14:47:02.455878 edgegap_scheduling-0.1.1/README.md
+-rw-r--r--   0        0        0      280 2024-04-29 15:32:04.063791 edgegap_scheduling-0.1.1/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-04-25 13:10:38.954379 edgegap_scheduling-0.1.1/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     3389 2024-04-29 15:32:04.067876 edgegap_scheduling-0.1.1/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     3855 2024-04-29 15:32:04.060315 edgegap_scheduling-0.1.1/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1025 2024-04-25 13:10:38.955042 edgegap_scheduling-0.1.1/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-04-25 13:10:38.955122 edgegap_scheduling-0.1.1/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1233 2024-04-25 13:10:38.955206 edgegap_scheduling-0.1.1/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      188 2024-04-25 13:10:38.955422 edgegap_scheduling-0.1.1/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     2780 2024-04-29 15:32:04.056350 edgegap_scheduling-0.1.1/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0      132 2024-04-25 20:04:14.788186 edgegap_scheduling-0.1.1/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-25 20:04:14.717257 edgegap_scheduling-0.1.1/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      501 2024-04-29 15:32:27.445016 edgegap_scheduling-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 edgegap_scheduling-0.1.1/PKG-INFO
```

### Comparing `edgegap_scheduling-0.1.0/LICENSE` & `edgegap_scheduling-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.0/README.md` & `edgegap_scheduling-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.0/edgegap_scheduling/_model.py` & `edgegap_scheduling-0.1.1/edgegap_scheduling/_task.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime
 from typing import Callable
 
-from colorama import Fore
+from edgegap_logging import Format, Color
 from pydantic import BaseModel, Field, computed_field
 from pytimeparse import parse
 
-from ._format import Format
 from ._state import TaskState
 
 
 class Task(BaseModel):
     identifier: str = Field(default=None, description="The identifier of the Task")
     name: str = Field(..., description="The name of the Task")
     every: str | None = Field(default=None, description="The interval to run the Task")
@@ -23,17 +22,17 @@
     sleep_at: datetime | None = Field(default=None, description="The last time where the Task slept")
     stopped_at: datetime | None = Field(default=None, description="The Time the Task stopped")
     continue_on_exception: bool = Field(default=True, description="If the Task continue after an exception")
     manual_run_allowed: bool = Field(default=False, description="If the Task can be manually run")
 
     def __str__(self):
         return (
-            f"Task {Format.squared(self.name, Fore.GREEN)} - "
-            f"Every {Format.squared(self.every, Fore.GREEN)} - "
-            f"Delay {Format.squared(self.delay, Fore.GREEN)} - "
+            f"Task {Format.squared(self.name, Color.GREEN)} - "
+            f"Every {Format.squared(self.every, Color.GREEN)} - "
+            f"Delay {Format.squared(self.delay, Color.GREEN)} - "
             f"{self.state}"
         )
 
     @property
     def every_in_seconds(self) -> int | None:
         return parse(self.every) if isinstance(self.every, str) else None
```

### Comparing `edgegap_scheduling-0.1.0/edgegap_scheduling/_runner.py` & `edgegap_scheduling-0.1.1/edgegap_scheduling/_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from datetime import datetime, timezone
 from typing import Callable
 
-from ._model import Task
 from ._signature import TaskSignature
 from ._state import TaskState
+from ._task import Task
 
 logger = logging.getLogger("scheduling.Runner")
 
 
 class TaskRunner:
     def __init__(self, task: Task, sleep: Callable):
         super().__init__()
```

### Comparing `edgegap_scheduling-0.1.0/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-0.1.1/edgegap_scheduling/_scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 import logging
 
-from colorama import Fore
+from edgegap_logging import Format, Color
 
-from ._format import Format
-from ._model import Task
 from ._runner import TaskRunner
 from ._sleep import AsyncSleep
+from ._task import Task
 from .errors import ManualRunNotAllowedError
 
 
 class Scheduler:
 
     def __init__(self, timeout: int = 10):
         self.timeout = timeout
@@ -43,15 +42,15 @@
             )
             self.__register(task.identifier, runner)
 
         return decorator
 
     def __register(self, identifier: str, runner: TaskRunner) -> None:
         if identifier in self.__runners.keys():
-            raise Exception(f"Task {Format.squared(identifier, Fore.RED)} already exists")
+            raise Exception(f"Task {Format.squared(identifier, Color.RED)} already exists")
 
         self.__runners[identifier] = runner
 
     def __get_or_raise(self, identifier: str) -> TaskRunner:
         runner = self.__runners.get(identifier)
 
         if runner is None:
```

### Comparing `edgegap_scheduling-0.1.0/edgegap_scheduling/_signature.py` & `edgegap_scheduling-0.1.1/edgegap_scheduling/_signature.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.0/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-0.1.1/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.0/PKG-INFO` & `edgegap_scheduling-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Edgegap Scheduling library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: edgegap-logging (>=0.1.2,<0.2.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Scheduling Library
 
 This is the README for the Edgegap Scheduling Helper, which is part of the Edgegap suite of helpers.
```

