# Comparing `tmp/beta9-0.1.5.tar.gz` & `tmp/beta9-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.5.tar", max compression
+gzip compressed data, was "beta9-0.1.6.tar", max compression
```

## Comparing `beta9-0.1.5.tar` & `beta9-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1127 2024-04-29 01:18:24.481123 beta9-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      586 2024-04-26 16:58:18.488727 beta9-0.1.5/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.5/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.5/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     9102 2024-04-27 21:55:06.431092 beta9-0.1.5/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.5/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     4574 2024-04-27 22:12:45.987796 beta9-0.1.5/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     6646 2024-04-27 21:51:14.004880 beta9-0.1.5/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4264 2024-04-24 22:31:23.870406 beta9-0.1.5/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.5/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.5/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     8770 2024-04-28 15:07:42.087524 beta9-0.1.5/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.5/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.5/src/beta9/aio.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.5/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.5/src/beta9/cli/config.py
--rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.5/src/beta9/cli/contexts.py
--rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.5/src/beta9/cli/deployment.py
--rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.5/src/beta9/cli/extraclick.py
--rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.5/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.5/src/beta9/cli/task.py
--rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.5/src/beta9/cli/volume.py
--rw-r--r--   0        0        0        0 2024-04-27 21:49:44.298869 beta9-0.1.5/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0     2980 2024-04-27 21:49:44.298980 beta9-0.1.5/src/beta9/clients/container/__init__.py
--rw-r--r--   0        0        0     4275 2024-04-27 21:49:44.117994 beta9-0.1.5/src/beta9/clients/endpoint/__init__.py
--rw-r--r--   0        0        0     8023 2024-04-27 21:49:43.256507 beta9-0.1.5/src/beta9/clients/function/__init__.py
--rw-r--r--   0        0        0    22783 2024-04-27 21:49:42.650953 beta9-0.1.5/src/beta9/clients/gateway/__init__.py
--rw-r--r--   0        0        0     4773 2024-04-27 21:49:42.845715 beta9-0.1.5/src/beta9/clients/image/__init__.py
--rw-r--r--   0        0        0     8003 2024-04-27 21:49:43.051036 beta9-0.1.5/src/beta9/clients/map/__init__.py
--rw-r--r--   0        0        0     8687 2024-04-27 21:49:43.458692 beta9-0.1.5/src/beta9/clients/simplequeue/__init__.py
--rw-r--r--   0        0        0    13315 2024-04-27 21:49:43.930351 beta9-0.1.5/src/beta9/clients/taskqueue/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-27 21:49:43.680311 beta9-0.1.5/src/beta9/clients/volume/__init__.py
--rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.5/src/beta9/config.py
--rw-r--r--   0        0        0      492 2024-04-26 16:58:18.490032 beta9-0.1.5/src/beta9/env.py
--rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.5/src/beta9/exceptions.py
--rw-r--r--   0        0        0      883 2024-04-26 16:58:18.490335 beta9-0.1.5/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.5/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0     6376 2024-04-28 15:05:22.253663 beta9-0.1.5/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.5/src/beta9/runner/container.py
--rw-r--r--   0        0        0     7453 2024-04-27 23:00:49.696829 beta9-0.1.5/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     6889 2024-04-27 23:26:29.020035 beta9-0.1.5/src/beta9/runner/function.py
--rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.5/src/beta9/runner/serve.py
--rw-r--r--   0        0        0    12265 2024-04-28 14:38:37.123539 beta9-0.1.5/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     5713 2024-04-26 16:58:18.491443 beta9-0.1.5/src/beta9/sync.py
--rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.5/src/beta9/terminal.py
--rw-r--r--   0        0        0     1541 2024-04-28 14:38:45.304071 beta9-0.1.5/src/beta9/type.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-04-29 20:32:04.904245 beta9-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      586 2024-04-26 16:58:18.488727 beta9-0.1.6/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.6/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.6/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     9102 2024-04-29 01:46:22.899381 beta9-0.1.6/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.6/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     4698 2024-04-29 20:30:30.521016 beta9-0.1.6/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     7229 2024-04-29 20:35:39.853896 beta9-0.1.6/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4264 2024-04-24 22:31:23.870406 beta9-0.1.6/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.6/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.6/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     9026 2024-04-29 20:33:22.790110 beta9-0.1.6/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.6/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.6/src/beta9/aio.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.6/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.6/src/beta9/cli/config.py
+-rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.6/src/beta9/cli/contexts.py
+-rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.6/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.6/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.6/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.6/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.6/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:49:44.298869 beta9-0.1.6/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-27 21:49:44.298980 beta9-0.1.6/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     4275 2024-04-27 21:49:44.117994 beta9-0.1.6/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     8023 2024-04-27 21:49:43.256507 beta9-0.1.6/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    22783 2024-04-29 01:46:22.900294 beta9-0.1.6/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0     4773 2024-04-27 21:49:42.845715 beta9-0.1.6/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8003 2024-04-27 21:49:43.051036 beta9-0.1.6/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-27 21:49:43.458692 beta9-0.1.6/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0    13315 2024-04-27 21:49:43.930351 beta9-0.1.6/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-27 21:49:43.680311 beta9-0.1.6/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.6/src/beta9/config.py
+-rw-r--r--   0        0        0      492 2024-04-26 16:58:18.490032 beta9-0.1.6/src/beta9/env.py
+-rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.6/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      883 2024-04-26 16:58:18.490335 beta9-0.1.6/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.6/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0     6376 2024-04-29 01:46:22.900678 beta9-0.1.6/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.6/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     7453 2024-04-29 01:46:22.901219 beta9-0.1.6/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     6889 2024-04-29 01:46:22.901734 beta9-0.1.6/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.6/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    12265 2024-04-29 01:46:22.902140 beta9-0.1.6/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5713 2024-04-26 16:58:18.491443 beta9-0.1.6/src/beta9/sync.py
+-rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.6/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1541 2024-04-29 01:46:22.902589 beta9-0.1.6/src/beta9/type.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.6/PKG-INFO
```

### Comparing `beta9-0.1.5/pyproject.toml` & `beta9-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
```

### Comparing `beta9-0.1.5/src/beta9/__init__.py` & `beta9-0.1.6/src/beta9/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/base/__init__.py` & `beta9-0.1.6/src/beta9/abstractions/base/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/base/runner.py` & `beta9-0.1.6/src/beta9/abstractions/base/runner.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/container.py` & `beta9-0.1.6/src/beta9/abstractions/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/endpoint.py` & `beta9-0.1.6/src/beta9/abstractions/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 
 from .. import terminal
 from ..abstractions.base.runner import (
     ENDPOINT_DEPLOYMENT_STUB_TYPE,
     ENDPOINT_SERVE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
+from ..abstractions.volume import Volume
 from ..clients.endpoint import (
     EndpointServiceStub,
     StartEndpointServeRequest,
     StopEndpointServeRequest,
 )
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..config import GatewayConfig, get_gateway_config
@@ -27,27 +28,29 @@
         image: Image = Image(),
         timeout: int = 180,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 300,
         max_pending_tasks: int = 100,
         on_start: Optional[Callable] = None,
+        volumes: Optional[List[Volume]] = None,
     ):
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             concurrency=concurrency,
             max_containers=max_containers,
             timeout=timeout,
             retries=0,
             keep_warm_seconds=keep_warm_seconds,
             max_pending_tasks=max_pending_tasks,
             on_start=on_start,
+            volumes=volumes,
         )
 
         self.endpoint_stub: EndpointServiceStub = EndpointServiceStub(self.channel)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
```

### Comparing `beta9-0.1.5/src/beta9/abstractions/function.py` & `beta9-0.1.6/src/beta9/abstractions/function.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,23 @@
             The amount of memory allocated to the container. It should be specified in
             megabytes (e.g., 128 for 128 megabytes). Default is 128.
         gpu (Union[GpuType, str]):
             The type or name of the GPU device to be used for GPU-accelerated tasks. If not
             applicable or no GPU required, leave it empty. Default is [GpuType.NoGPU](#gputype).
         image (Union[Image, dict]):
             The container image used for the task execution. Default is [Image](#image).
+        timeout (Optional[int]):
+            The maximum number of seconds a task can run before it times out.
+            Default is 3600. Set it to -1 to disable the timeout.
+        retries (Optional[int]):
+            The maximum number of times a task will be retried if the container crashes. Default is 3.
+        callback_url (Optional[str]):
+            An optional URL to send a callback to when a task is completed, timed out, or cancelled.
+        volumes (Optional[List[Volume]]):
+            A list of storage volumes to be associated with the function. Default is [].
     Example:
         ```python
         from beta9 import function, Image
 
         @function(cpu=1.0, memory=128, gpu="T4", image=Image(python_packages=["torch"]), keep_warm_seconds=1000)
         def transcribe(filename: str):
             print(filename)
@@ -59,29 +68,29 @@
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
+        image: Image = Image(),
         timeout: int = 3600,
         retries: int = 3,
-        image: Image = Image(),
-        volumes: Optional[List[Volume]] = None,
         callback_url: Optional[str] = "",
+        volumes: Optional[List[Volume]] = None,
     ) -> None:
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
-            volumes=volumes,
             timeout=timeout,
             retries=retries,
             callback_url=callback_url,
+            volumes=volumes,
         )
 
         self.function_stub: FunctionServiceStub = FunctionServiceStub(self.channel)
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
```

### Comparing `beta9-0.1.5/src/beta9/abstractions/image.py` & `beta9-0.1.6/src/beta9/abstractions/image.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/map.py` & `beta9-0.1.6/src/beta9/abstractions/map.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/queue.py` & `beta9-0.1.6/src/beta9/abstractions/queue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.6/src/beta9/abstractions/taskqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import os
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 
 from .. import terminal
 from ..abstractions.base.runner import (
     TASKQUEUE_DEPLOYMENT_STUB_TYPE,
     TASKQUEUE_SERVE_STUB_TYPE,
     TASKQUEUE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
+from ..abstractions.volume import Volume
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..clients.taskqueue import (
     StartTaskQueueServeRequest,
     StopTaskQueueServeRequest,
     TaskQueuePutRequest,
     TaskQueuePutResponse,
     TaskQueueServiceStub,
@@ -64,14 +65,16 @@
             pending tasks exceeds this value, the task queue will stop accepting new tasks.
             Default is 100.
         on_start (Optional[Callable]):
             An optional function to run once (per process) when the container starts. Can be used for downloading data,
             loading models, or anything else computationally expensive.
         callback_url (Optional[str]):
             An optional URL to send a callback to when a task is completed, timed out, or cancelled.
+        volumes (Optional[List[Volume]]):
+            A list of storage volumes to be associated with the taskqueue. Default is [].
     Example:
         ```python
         from beta9 import task_queue, Image
 
         @task_queue(cpu=1.0, memory=128, gpu="T4", image=Image(python_packages=["torch"]), keep_warm_seconds=1000)
         def transcribe(filename: str):
             print(filename)
@@ -92,28 +95,30 @@
         retries: int = 3,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 10,
         max_pending_tasks: int = 100,
         on_start: Optional[Callable] = None,
         callback_url: Optional[str] = None,
+        volumes: Optional[List[Volume]] = None,
     ) -> None:
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             concurrency=concurrency,
             max_containers=max_containers,
             timeout=timeout,
             retries=retries,
             keep_warm_seconds=keep_warm_seconds,
             max_pending_tasks=max_pending_tasks,
             on_start=on_start,
             callback_url=callback_url,
+            volumes=volumes,
         )
 
         self.taskqueue_stub: TaskQueueServiceStub = TaskQueueServiceStub(self.channel)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
```

### Comparing `beta9-0.1.5/src/beta9/abstractions/volume.py` & `beta9-0.1.6/src/beta9/abstractions/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/config.py` & `beta9-0.1.6/src/beta9/cli/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/contexts.py` & `beta9-0.1.6/src/beta9/cli/contexts.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/deployment.py` & `beta9-0.1.6/src/beta9/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/extraclick.py` & `beta9-0.1.6/src/beta9/cli/extraclick.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/main.py` & `beta9-0.1.6/src/beta9/cli/main.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/task.py` & `beta9-0.1.6/src/beta9/cli/task.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/cli/volume.py` & `beta9-0.1.6/src/beta9/cli/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/container/__init__.py` & `beta9-0.1.6/src/beta9/clients/container/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/endpoint/__init__.py` & `beta9-0.1.6/src/beta9/clients/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/function/__init__.py` & `beta9-0.1.6/src/beta9/clients/function/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/gateway/__init__.py` & `beta9-0.1.6/src/beta9/clients/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/image/__init__.py` & `beta9-0.1.6/src/beta9/clients/image/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/map/__init__.py` & `beta9-0.1.6/src/beta9/clients/map/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/simplequeue/__init__.py` & `beta9-0.1.6/src/beta9/clients/simplequeue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/taskqueue/__init__.py` & `beta9-0.1.6/src/beta9/clients/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/clients/volume/__init__.py` & `beta9-0.1.6/src/beta9/clients/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/config.py` & `beta9-0.1.6/src/beta9/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/logging.py` & `beta9-0.1.6/src/beta9/logging.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/runner/common.py` & `beta9-0.1.6/src/beta9/runner/common.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/runner/container.py` & `beta9-0.1.6/src/beta9/runner/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/runner/endpoint.py` & `beta9-0.1.6/src/beta9/runner/endpoint.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/runner/function.py` & `beta9-0.1.6/src/beta9/runner/function.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/runner/serve.py` & `beta9-0.1.6/src/beta9/runner/serve.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/runner/taskqueue.py` & `beta9-0.1.6/src/beta9/runner/taskqueue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/sync.py` & `beta9-0.1.6/src/beta9/sync.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/terminal.py` & `beta9-0.1.6/src/beta9/terminal.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/src/beta9/type.py` & `beta9-0.1.6/src/beta9/type.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.5/PKG-INFO` & `beta9-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

