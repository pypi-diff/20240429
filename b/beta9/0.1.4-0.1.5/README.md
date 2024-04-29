# Comparing `tmp/beta9-0.1.4.tar.gz` & `tmp/beta9-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.4.tar", max compression
+gzip compressed data, was "beta9-0.1.5.tar", max compression
```

## Comparing `beta9-0.1.4.tar` & `beta9-0.1.5.tar`

### file list

```diff
@@ -1,82 +1,47 @@
--rw-r--r--   0        0        0     1127 2024-04-26 17:02:31.346466 beta9-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      586 2024-04-26 16:58:18.488727 beta9-0.1.4/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.4/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0      170 2024-01-27 18:19:06.888984 beta9-0.1.4/src/beta9/abstractions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5495 2024-04-21 16:47:13.563006 beta9-0.1.4/src/beta9/abstractions/__pycache__/container.cpython-311.pyc
--rw-r--r--   0        0        0     7714 2024-04-26 17:01:21.727355 beta9-0.1.4/src/beta9/abstractions/__pycache__/endpoint.cpython-311.pyc
--rw-r--r--   0        0        0    11097 2024-04-26 17:01:21.729113 beta9-0.1.4/src/beta9/abstractions/__pycache__/function.cpython-311.pyc
--rw-r--r--   0        0        0     6226 2024-04-24 22:32:45.911483 beta9-0.1.4/src/beta9/abstractions/__pycache__/image.cpython-311.pyc
--rw-r--r--   0        0        0     6188 2024-04-21 16:47:13.732114 beta9-0.1.4/src/beta9/abstractions/__pycache__/map.cpython-311.pyc
--rw-r--r--   0        0        0     5648 2024-04-21 16:47:13.734715 beta9-0.1.4/src/beta9/abstractions/__pycache__/queue.cpython-311.pyc
--rw-r--r--   0        0        0    12041 2024-04-26 17:01:21.735990 beta9-0.1.4/src/beta9/abstractions/__pycache__/taskqueue.cpython-311.pyc
--rw-r--r--   0        0        0     2647 2024-04-21 16:47:13.714395 beta9-0.1.4/src/beta9/abstractions/__pycache__/volume.cpython-311.pyc
--rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.4/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     1685 2024-01-27 18:19:06.984688 beta9-0.1.4/src/beta9/abstractions/base/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11772 2024-04-26 17:02:13.977328 beta9-0.1.4/src/beta9/abstractions/base/__pycache__/runner.cpython-311.pyc
--rw-r--r--   0        0        0     8955 2024-04-26 17:02:11.892971 beta9-0.1.4/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.4/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     4574 2024-04-26 16:58:18.489070 beta9-0.1.4/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     6565 2024-04-26 16:58:18.489246 beta9-0.1.4/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4264 2024-04-24 22:31:23.870406 beta9-0.1.4/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.4/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.4/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     8548 2024-04-26 16:58:18.489543 beta9-0.1.4/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.4/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.4/src/beta9/aio.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.4/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      161 2024-02-07 17:33:34.585819 beta9-0.1.4/src/beta9/cli/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1786 2024-04-22 03:01:00.641942 beta9-0.1.4/src/beta9/cli/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     1433 2024-04-01 17:03:29.905084 beta9-0.1.4/src/beta9/cli/__pycache__/configure.cpython-311.pyc
--rw-r--r--   0        0        0     2197 2024-04-22 03:01:00.644896 beta9-0.1.4/src/beta9/cli/__pycache__/contexts.cpython-311.pyc
--rw-r--r--   0        0        0     2486 2024-04-01 17:03:29.905700 beta9-0.1.4/src/beta9/cli/__pycache__/deploy.cpython-311.pyc
--rw-r--r--   0        0        0     4533 2024-04-22 03:01:00.644129 beta9-0.1.4/src/beta9/cli/__pycache__/deployment.cpython-311.pyc
--rw-r--r--   0        0        0     6533 2024-04-22 03:01:00.643173 beta9-0.1.4/src/beta9/cli/__pycache__/extraclick.cpython-311.pyc
--rw-r--r--   0        0        0     1531 2024-02-07 17:33:34.615345 beta9-0.1.4/src/beta9/cli/__pycache__/formatters.cpython-311.pyc
--rw-r--r--   0        0        0     2634 2024-04-22 03:01:00.635557 beta9-0.1.4/src/beta9/cli/__pycache__/main.cpython-311.pyc
--rw-r--r--   0        0        0     6911 2024-04-22 03:01:00.646800 beta9-0.1.4/src/beta9/cli/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     6901 2024-04-10 01:00:13.874183 beta9-0.1.4/src/beta9/cli/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0    15122 2024-04-22 03:01:00.648559 beta9-0.1.4/src/beta9/cli/__pycache__/volume.cpython-311.pyc
--rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.4/src/beta9/cli/config.py
--rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.4/src/beta9/cli/contexts.py
--rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.4/src/beta9/cli/deployment.py
--rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.4/src/beta9/cli/extraclick.py
--rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.4/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.4/src/beta9/cli/task.py
--rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.4/src/beta9/cli/volume.py
--rw-r--r--   0        0        0        0 2024-04-25 22:02:49.680323 beta9-0.1.4/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0      165 2024-04-25 22:07:33.794285 beta9-0.1.4/src/beta9/clients/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2980 2024-04-25 22:02:49.680448 beta9-0.1.4/src/beta9/clients/container/__init__.py
--rw-r--r--   0        0        0     5732 2024-04-25 22:07:33.847103 beta9-0.1.4/src/beta9/clients/container/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4275 2024-04-25 22:02:49.473122 beta9-0.1.4/src/beta9/clients/endpoint/__init__.py
--rw-r--r--   0        0        0     7204 2024-04-25 22:07:33.849454 beta9-0.1.4/src/beta9/clients/endpoint/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8023 2024-04-25 22:02:48.559816 beta9-0.1.4/src/beta9/clients/function/__init__.py
--rw-r--r--   0        0        0    13329 2024-04-25 22:07:33.853498 beta9-0.1.4/src/beta9/clients/function/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    21072 2024-04-26 16:58:18.489835 beta9-0.1.4/src/beta9/clients/gateway/__init__.py
--rw-r--r--   0        0        0    35251 2024-04-26 17:01:21.674321 beta9-0.1.4/src/beta9/clients/gateway/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4773 2024-04-25 22:02:48.104339 beta9-0.1.4/src/beta9/clients/image/__init__.py
--rw-r--r--   0        0        0     8254 2024-04-25 22:07:33.834827 beta9-0.1.4/src/beta9/clients/image/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8003 2024-04-25 22:02:48.322282 beta9-0.1.4/src/beta9/clients/map/__init__.py
--rw-r--r--   0        0        0    13990 2024-04-25 22:07:33.855581 beta9-0.1.4/src/beta9/clients/map/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8687 2024-04-25 22:02:48.786327 beta9-0.1.4/src/beta9/clients/simplequeue/__init__.py
--rw-r--r--   0        0        0    13538 2024-04-25 22:07:33.857419 beta9-0.1.4/src/beta9/clients/simplequeue/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13315 2024-04-25 22:02:49.277977 beta9-0.1.4/src/beta9/clients/taskqueue/__init__.py
--rw-r--r--   0        0        0    21218 2024-04-25 22:07:33.860493 beta9-0.1.4/src/beta9/clients/taskqueue/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9482 2024-04-25 22:02:49.031862 beta9-0.1.4/src/beta9/clients/volume/__init__.py
--rw-r--r--   0        0        0    16586 2024-04-25 22:07:33.836911 beta9-0.1.4/src/beta9/clients/volume/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.4/src/beta9/config.py
--rw-r--r--   0        0        0      492 2024-04-26 16:58:18.490032 beta9-0.1.4/src/beta9/env.py
--rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.4/src/beta9/exceptions.py
--rw-r--r--   0        0        0      883 2024-04-26 16:58:18.490335 beta9-0.1.4/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.4/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0      164 2024-04-26 05:59:09.072510 beta9-0.1.4/src/beta9/runner/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7724 2024-04-26 05:59:09.073289 beta9-0.1.4/src/beta9/runner/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0     4442 2024-04-26 16:58:18.490515 beta9-0.1.4/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.4/src/beta9/runner/container.py
--rw-r--r--   0        0        0     7465 2024-04-26 16:58:18.490672 beta9-0.1.4/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     6006 2024-04-26 16:58:18.490846 beta9-0.1.4/src/beta9/runner/function.py
--rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.4/src/beta9/runner/serve.py
--rw-r--r--   0        0        0    11017 2024-04-26 16:58:18.491042 beta9-0.1.4/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     5713 2024-04-26 16:58:18.491443 beta9-0.1.4/src/beta9/sync.py
--rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.4/src/beta9/terminal.py
--rw-r--r--   0        0        0     1460 2024-04-26 16:58:18.491680 beta9-0.1.4/src/beta9/type.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-04-29 01:18:24.481123 beta9-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      586 2024-04-26 16:58:18.488727 beta9-0.1.5/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.5/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.5/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     9102 2024-04-27 21:55:06.431092 beta9-0.1.5/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.5/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     4574 2024-04-27 22:12:45.987796 beta9-0.1.5/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     6646 2024-04-27 21:51:14.004880 beta9-0.1.5/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4264 2024-04-24 22:31:23.870406 beta9-0.1.5/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.5/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.5/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     8770 2024-04-28 15:07:42.087524 beta9-0.1.5/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.5/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.5/src/beta9/aio.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.5/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.5/src/beta9/cli/config.py
+-rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.5/src/beta9/cli/contexts.py
+-rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.5/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.5/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.5/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.5/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.5/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:49:44.298869 beta9-0.1.5/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-27 21:49:44.298980 beta9-0.1.5/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     4275 2024-04-27 21:49:44.117994 beta9-0.1.5/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     8023 2024-04-27 21:49:43.256507 beta9-0.1.5/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    22783 2024-04-27 21:49:42.650953 beta9-0.1.5/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0     4773 2024-04-27 21:49:42.845715 beta9-0.1.5/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8003 2024-04-27 21:49:43.051036 beta9-0.1.5/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-27 21:49:43.458692 beta9-0.1.5/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0    13315 2024-04-27 21:49:43.930351 beta9-0.1.5/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-27 21:49:43.680311 beta9-0.1.5/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.5/src/beta9/config.py
+-rw-r--r--   0        0        0      492 2024-04-26 16:58:18.490032 beta9-0.1.5/src/beta9/env.py
+-rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.5/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      883 2024-04-26 16:58:18.490335 beta9-0.1.5/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.5/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0     6376 2024-04-28 15:05:22.253663 beta9-0.1.5/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.5/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     7453 2024-04-27 23:00:49.696829 beta9-0.1.5/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     6889 2024-04-27 23:26:29.020035 beta9-0.1.5/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.5/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    12265 2024-04-28 14:38:37.123539 beta9-0.1.5/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5713 2024-04-26 16:58:18.491443 beta9-0.1.5/src/beta9/sync.py
+-rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.5/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1541 2024-04-28 14:38:45.304071 beta9-0.1.5/src/beta9/type.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.5/PKG-INFO
```

### Comparing `beta9-0.1.4/pyproject.toml` & `beta9-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
```

### Comparing `beta9-0.1.4/src/beta9/__init__.py` & `beta9-0.1.5/src/beta9/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/base/__init__.py` & `beta9-0.1.5/src/beta9/abstractions/base/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/base/runner.py` & `beta9-0.1.5/src/beta9/abstractions/base/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         max_containers: int = 1,
         keep_warm_seconds: float = 10.0,
         max_pending_tasks: int = 100,
         retries: int = 3,
         timeout: int = 3600,
         volumes: Optional[List[Volume]] = None,
         on_start: Optional[Callable] = None,
+        callback_url: Optional[str] = None,
     ) -> None:
         super().__init__()
 
         if image is None:
             image = Image()
 
         self.image: Image = image
@@ -58,14 +59,15 @@
         self.stub_created: bool = False
         self.runtime_ready: bool = False
         self.object_id: str = ""
         self.image_id: str = ""
         self.stub_id: str = ""
         self.handler: str = ""
         self.on_start: str = ""
+        self.callback_url = callback_url or ""
         self.cpu = cpu
         self.memory = memory
         self.gpu = gpu
         self.volumes = volumes or []
         self.concurrency = concurrency
         self.keep_warm_seconds = keep_warm_seconds
         self.max_pending_tasks = max_pending_tasks
@@ -227,14 +229,15 @@
                         name=stub_name,
                         python_version=self.image.python_version,
                         cpu=self.cpu,
                         memory=self.memory,
                         gpu=self.gpu,
                         handler=self.handler,
                         on_start=self.on_start,
+                        callback_url=self.callback_url,
                         retries=self.retries,
                         timeout=self.timeout,
                         keep_warm_seconds=self.keep_warm_seconds,
                         concurrency=self.concurrency,
                         max_containers=self.max_containers,
                         max_pending_tasks=self.max_pending_tasks,
                         volumes=[v.export() for v in self.volumes],
```

### Comparing `beta9-0.1.4/src/beta9/abstractions/container.py` & `beta9-0.1.5/src/beta9/abstractions/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/endpoint.py` & `beta9-0.1.5/src/beta9/abstractions/endpoint.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/function.py` & `beta9-0.1.5/src/beta9/abstractions/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,23 +63,25 @@
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
         timeout: int = 3600,
         retries: int = 3,
         image: Image = Image(),
         volumes: Optional[List[Volume]] = None,
+        callback_url: Optional[str] = "",
     ) -> None:
         super().__init__(
             cpu=cpu,
             memory=memory,
             gpu=gpu,
             image=image,
             volumes=volumes,
             timeout=timeout,
             retries=retries,
+            callback_url=callback_url,
         )
 
         self.function_stub: FunctionServiceStub = FunctionServiceStub(self.channel)
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
```

### Comparing `beta9-0.1.4/src/beta9/abstractions/image.py` & `beta9-0.1.5/src/beta9/abstractions/image.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/map.py` & `beta9-0.1.5/src/beta9/abstractions/map.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/queue.py` & `beta9-0.1.5/src/beta9/abstractions/queue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.5/src/beta9/abstractions/taskqueue.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         max_pending_tasks (int):
             The maximum number of tasks that can be pending in the queue. If the number of
             pending tasks exceeds this value, the task queue will stop accepting new tasks.
             Default is 100.
         on_start (Optional[Callable]):
             An optional function to run once (per process) when the container starts. Can be used for downloading data,
             loading models, or anything else computationally expensive.
+        callback_url (Optional[str]):
+            An optional URL to send a callback to when a task is completed, timed out, or cancelled.
     Example:
         ```python
         from beta9 import task_queue, Image
 
         @task_queue(cpu=1.0, memory=128, gpu="T4", image=Image(python_packages=["torch"]), keep_warm_seconds=1000)
         def transcribe(filename: str):
             print(filename)
@@ -89,27 +91,29 @@
         timeout: int = 3600,
         retries: int = 3,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 10,
         max_pending_tasks: int = 100,
         on_start: Optional[Callable] = None,
+        callback_url: Optional[str] = None,
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
+            callback_url=callback_url,
         )
 
         self.taskqueue_stub: TaskQueueServiceStub = TaskQueueServiceStub(self.channel)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
```

### Comparing `beta9-0.1.4/src/beta9/abstractions/volume.py` & `beta9-0.1.5/src/beta9/abstractions/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/config.py` & `beta9-0.1.5/src/beta9/cli/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/contexts.py` & `beta9-0.1.5/src/beta9/cli/contexts.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/deployment.py` & `beta9-0.1.5/src/beta9/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/extraclick.py` & `beta9-0.1.5/src/beta9/cli/extraclick.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/main.py` & `beta9-0.1.5/src/beta9/cli/main.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/task.py` & `beta9-0.1.5/src/beta9/cli/task.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/cli/volume.py` & `beta9-0.1.5/src/beta9/cli/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/container/__init__.py` & `beta9-0.1.5/src/beta9/clients/container/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/endpoint/__init__.py` & `beta9-0.1.5/src/beta9/clients/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/function/__init__.py` & `beta9-0.1.5/src/beta9/clients/function/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/gateway/__init__.py` & `beta9-0.1.5/src/beta9/clients/gateway/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,27 @@
     ok: bool = betterproto.bool_field(1)
     workspace_id: str = betterproto.string_field(2)
     new_token: str = betterproto.string_field(3)
     error_msg: str = betterproto.string_field(4)
 
 
 @dataclass(eq=False, repr=False)
+class SignPayloadRequest(betterproto.Message):
+    payload: bytes = betterproto.bytes_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class SignPayloadResponse(betterproto.Message):
+    ok: bool = betterproto.bool_field(1)
+    signature: str = betterproto.string_field(2)
+    timestamp: int = betterproto.int64_field(3)
+    error_msg: str = betterproto.string_field(4)
+
+
+@dataclass(eq=False, repr=False)
 class ObjectMetadata(betterproto.Message):
     name: str = betterproto.string_field(1)
     size: int = betterproto.int64_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class HeadObjectRequest(betterproto.Message):
@@ -190,14 +203,15 @@
     keep_warm_seconds: float = betterproto.float_field(12)
     concurrency: int = betterproto.uint32_field(13)
     max_containers: int = betterproto.uint32_field(14)
     max_pending_tasks: int = betterproto.uint32_field(15)
     volumes: List["Volume"] = betterproto.message_field(16)
     force_create: bool = betterproto.bool_field(17)
     on_start: str = betterproto.string_field(18)
+    callback_url: str = betterproto.string_field(19)
 
 
 @dataclass(eq=False, repr=False)
 class GetOrCreateStubResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
     stub_id: str = betterproto.string_field(2)
 
@@ -229,14 +243,31 @@
             authorize_request,
             AuthorizeResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
+    async def sign_payload(
+        self,
+        sign_payload_request: "SignPayloadRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "SignPayloadResponse":
+        return await self._unary_unary(
+            "/gateway.GatewayService/SignPayload",
+            sign_payload_request,
+            SignPayloadResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
     async def head_object(
         self,
         head_object_request: "HeadObjectRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
@@ -414,14 +445,19 @@
 class GatewayServiceBase(ServiceBase):
 
     async def authorize(
         self, authorize_request: "AuthorizeRequest"
     ) -> "AuthorizeResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
+    async def sign_payload(
+        self, sign_payload_request: "SignPayloadRequest"
+    ) -> "SignPayloadResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
     async def head_object(
         self, head_object_request: "HeadObjectRequest"
     ) -> "HeadObjectResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def put_object(
         self, put_object_request: "PutObjectRequest"
@@ -472,14 +508,21 @@
     async def __rpc_authorize(
         self, stream: "grpclib.server.Stream[AuthorizeRequest, AuthorizeResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.authorize(request)
         await stream.send_message(response)
 
+    async def __rpc_sign_payload(
+        self, stream: "grpclib.server.Stream[SignPayloadRequest, SignPayloadResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.sign_payload(request)
+        await stream.send_message(response)
+
     async def __rpc_head_object(
         self, stream: "grpclib.server.Stream[HeadObjectRequest, HeadObjectResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.head_object(request)
         await stream.send_message(response)
 
@@ -552,14 +595,20 @@
         return {
             "/gateway.GatewayService/Authorize": grpclib.const.Handler(
                 self.__rpc_authorize,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 AuthorizeRequest,
                 AuthorizeResponse,
             ),
+            "/gateway.GatewayService/SignPayload": grpclib.const.Handler(
+                self.__rpc_sign_payload,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                SignPayloadRequest,
+                SignPayloadResponse,
+            ),
             "/gateway.GatewayService/HeadObject": grpclib.const.Handler(
                 self.__rpc_head_object,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 HeadObjectRequest,
                 HeadObjectResponse,
             ),
             "/gateway.GatewayService/PutObject": grpclib.const.Handler(
```

### Comparing `beta9-0.1.4/src/beta9/clients/image/__init__.py` & `beta9-0.1.5/src/beta9/clients/image/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/map/__init__.py` & `beta9-0.1.5/src/beta9/clients/map/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/simplequeue/__init__.py` & `beta9-0.1.5/src/beta9/clients/simplequeue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/taskqueue/__init__.py` & `beta9-0.1.5/src/beta9/clients/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/clients/volume/__init__.py` & `beta9-0.1.5/src/beta9/clients/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/config.py` & `beta9-0.1.5/src/beta9/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/logging.py` & `beta9-0.1.5/src/beta9/logging.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/runner/container.py` & `beta9-0.1.5/src/beta9/runner/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/runner/endpoint.py` & `beta9-0.1.5/src/beta9/runner/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,27 +188,29 @@
             args = []
 
         kwargs = payload.get("kwargs", {})
         if kwargs is None:
             kwargs = {}
 
         context = FunctionContext.new(
-            config=cfg, task_id=task_id, on_start_value=self.on_start_value
+            config=cfg,
+            task_id=task_id,
+            on_start_value=self.on_start_value,
         )
 
         try:
             response_body = self.handler(
                 context,
                 *args,
                 **kwargs,
             )
         except BaseException:
-            self.logger.exception("Unhandled exception")
-            error = traceback.format_exc()
-            response_body = {"error": traceback.format_exc()}
+            exception = traceback.format_exc()
+            print(exception)
+            response_body = {"error": exception}
 
         return response_body, error
 
     def shutdown(self, signum=None, frame=None):
         os._exit(self.exit_code)
```

### Comparing `beta9-0.1.4/src/beta9/runner/function.py` & `beta9-0.1.5/src/beta9/runner/function.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     GatewayServiceStub,
     StartTaskRequest,
     StartTaskResponse,
 )
 from ..config import with_runner_context
 from ..exceptions import InvalidFunctionArgumentsException, RunnerException
 from ..logging import StdoutJsonInterceptor
-from ..runner.common import FunctionContext, FunctionHandler, config
+from ..runner.common import FunctionContext, FunctionHandler, config, send_callback
 from ..type import TaskExitCode, TaskStatus
 
 
 def _load_args(args: bytes) -> dict:
     try:
         return cloudpickle.loads(args)
     except BaseException:
@@ -42,18 +42,20 @@
             return json.loads(args.decode("utf-8"))
         except json.JSONDecodeError:
             raise InvalidFunctionArgumentsException
 
 
 async def _monitor_task(
     *,
+    context: FunctionContext,
     stub_id: str,
     task_id: str,
     container_id: str,
     function_stub: FunctionServiceStub,
+    gateway_stub: GatewayServiceStub,
 ) -> None:
     initial_backoff = 5
     max_retries = 5
     backoff = initial_backoff
     retry = 0
 
     while retry <= max_retries:
@@ -64,21 +66,35 @@
                     stub_id=stub_id,
                     container_id=container_id,
                 )
             ):
                 response: FunctionMonitorResponse
                 if response.cancelled:
                     print(f"Task cancelled: {task_id}")
+
+                    await send_callback(
+                        gateway_stub=gateway_stub,
+                        context=context,
+                        payload={},
+                        task_status=TaskStatus.Cancelled,
+                    )
                     os._exit(TaskExitCode.Cancelled)
 
                 if response.complete:
                     return
 
                 if response.timed_out:
                     print(f"Task timed out: {task_id}")
+
+                    await send_callback(
+                        gateway_stub=gateway_stub,
+                        context=context,
+                        payload={},
+                        task_status=TaskStatus.Timeout,
+                    )
                     os._exit(TaskExitCode.Timeout)
 
                 retry = 0
                 backoff = initial_backoff
 
             # If successful, it means the stream is finished.
             # Break out of the retry loop
@@ -124,20 +140,23 @@
         start_task_response: StartTaskResponse = run_sync(
             gateway_stub.start_task(StartTaskRequest(task_id=task_id, container_id=container_id))
         )
         if not start_task_response.ok:
             raise RunnerException("Unable to start task")
 
         # Kick off monitoring task
+        context = FunctionContext.new(config=config, task_id=task_id)
         monitor_task = loop.create_task(
             _monitor_task(
+                context=context,
                 stub_id=config.stub_id,
                 task_id=task_id,
                 container_id=config.container_id,
                 function_stub=function_stub,
+                gateway_stub=gateway_stub,
             ),
         )
 
         task_status = TaskStatus.Complete
         error = None
 
         # Invoke function
@@ -145,29 +164,27 @@
             get_args_resp: FunctionGetArgsResponse = run_sync(
                 function_stub.function_get_args(FunctionGetArgsRequest(task_id=task_id)),
             )
             if not get_args_resp.ok:
                 raise InvalidFunctionArgumentsException
 
             handler = FunctionHandler()
-            context = FunctionContext.new(config=config, task_id=task_id)
-
             payload: dict = _load_args(get_args_resp.args)
             args = payload.get("args") or []
             kwargs = payload.get("kwargs") or {}
 
             result = handler(context, *args, **kwargs)
         except BaseException as exc:
             result = error = exc
             task_status = TaskStatus.Error
         finally:
-            result = cloudpickle.dumps(result)
+            pickled_result = cloudpickle.dumps(result)
             set_result_resp: FunctionSetResultResponse = run_sync(
                 function_stub.function_set_result(
-                    FunctionSetResultRequest(task_id=task_id, result=result)
+                    FunctionSetResultRequest(task_id=task_id, result=pickled_result)
                 ),
             )
             if not set_result_resp.ok:
                 raise RunnerException("Unable to set function result")
 
         task_duration = time.time() - start_time
 
@@ -185,13 +202,19 @@
             )
         )
         if not end_task_response.ok:
             raise RunnerException("Unable to end task")
 
         monitor_task.cancel()
 
+        run_sync(
+            send_callback(
+                gateway_stub=gateway_stub, context=context, payload=result, task_status=task_status
+            )
+        )  # Send callback to callback_url, if defined
+
         if task_status == TaskStatus.Error:
             raise error.with_traceback(error.__traceback__)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `beta9-0.1.4/src/beta9/runner/serve.py` & `beta9-0.1.5/src/beta9/runner/serve.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/runner/taskqueue.py` & `beta9-0.1.5/src/beta9/runner/taskqueue.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,34 +6,40 @@
 import threading
 import time
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from multiprocessing import Event, Process, set_start_method
 from typing import Any, List, NamedTuple, Union
 
-import cloudpickle
 import grpc
 import grpclib
 from grpclib.client import Channel
 from grpclib.exceptions import StreamTerminatedError
 
 from ..aio import run_sync
+from ..clients.gateway import GatewayServiceStub
 from ..clients.taskqueue import (
     TaskQueueCompleteRequest,
     TaskQueueCompleteResponse,
     TaskQueueMonitorRequest,
     TaskQueueMonitorResponse,
     TaskQueuePopRequest,
     TaskQueuePopResponse,
     TaskQueueServiceStub,
 )
 from ..config import with_runner_context
 from ..exceptions import RunnerException
 from ..logging import StdoutJsonInterceptor
-from ..runner.common import FunctionContext, FunctionHandler, config, execute_lifecycle_method
+from ..runner.common import (
+    FunctionContext,
+    FunctionHandler,
+    config,
+    execute_lifecycle_method,
+    send_callback,
+)
 from ..type import LifeCycleMethod, TaskExitCode, TaskStatus
 
 TASK_PROCESS_WATCHDOG_INTERVAL = 0.01
 TASK_POLLING_INTERVAL = 0.01
 TASK_MANAGER_INTERVAL = 0.1
 
 
@@ -170,20 +176,31 @@
                     TaskQueuePopRequest(stub_id=stub_id, container_id=container_id)
                 )
             )
             if not r.ok or not r.task_msg:
                 return None
 
             task = json.loads(r.task_msg)
-            return Task(id=task["task_id"], args=task["args"], kwargs=task["kwargs"])
+            return Task(
+                id=task["task_id"],
+                args=task["args"],
+                kwargs=task["kwargs"],
+            )
         except (grpclib.exceptions.StreamTerminatedError, OSError):
             return None
 
     async def _monitor_task(
-        self, stub_id: str, container_id: str, taskqueue_stub: TaskQueueServiceStub, task: Task
+        self,
+        *,
+        context: FunctionContext,
+        stub_id: str,
+        container_id: str,
+        task: Task,
+        taskqueue_stub: TaskQueueServiceStub,
+        gateway_stub: GatewayServiceStub,
     ) -> None:
         initial_backoff = 5
         max_retries = 5
         backoff = initial_backoff
         retry = 0
 
         while retry <= max_retries:
@@ -194,21 +211,35 @@
                         stub_id=stub_id,
                         container_id=container_id,
                     )
                 ):
                     response: TaskQueueMonitorResponse
                     if response.cancelled:
                         print(f"Task cancelled: {task.id}")
+
+                        await send_callback(
+                            gateway_stub=gateway_stub,
+                            context=context,
+                            payload={},
+                            task_status=TaskStatus.Cancelled,
+                        )
                         os._exit(TaskExitCode.Cancelled)
 
                     if response.complete:
                         return
 
                     if response.timed_out:
                         print(f"Task timed out: {task.id}")
+
+                        await send_callback(
+                            gateway_stub=gateway_stub,
+                            context=context,
+                            payload={},
+                            task_status=TaskStatus.Timeout,
+                        )
                         os._exit(TaskExitCode.Timeout)
 
                     retry = 0
                     backoff = initial_backoff
 
                 # If successful, it means the stream is finished.
                 # Break out of the retry loop
@@ -237,14 +268,15 @@
 
     @with_runner_context
     def process_tasks(self, channel: Channel) -> None:
         self.worker_startup_event.set()
         loop = asyncio.get_event_loop()
         executor = ThreadPoolExecutor()
         taskqueue_stub = TaskQueueServiceStub(channel)
+        gateway_stub = GatewayServiceStub(channel)
 
         # Load handler and execute on_start method
         handler = FunctionHandler()
         on_start_value = execute_lifecycle_method(name=LifeCycleMethod.OnStart)
 
         print(f"Worker[{self.worker_index}] ready")
         while True:
@@ -253,39 +285,42 @@
                 time.sleep(TASK_POLLING_INTERVAL)
                 continue
 
             async def _run_task():
                 with StdoutJsonInterceptor(task_id=task.id):
                     print(f"Running task <{task.id}>")
 
+                    context = FunctionContext.new(
+                        config=config,
+                        task_id=task.id,
+                        on_start_value=on_start_value,
+                    )
+
                     monitor_task = loop.create_task(
                         self._monitor_task(
-                            config.stub_id, config.container_id, taskqueue_stub, task
+                            context=context,
+                            stub_id=config.stub_id,
+                            container_id=config.container_id,
+                            task=task,
+                            taskqueue_stub=taskqueue_stub,
+                            gateway_stub=gateway_stub,
                         ),
                     )
 
                     start_time = time.time()
                     task_status = TaskStatus.Complete
                     try:
                         args = task.args or []
                         kwargs = task.kwargs or {}
 
-                        context = FunctionContext.new(
-                            config=config,
-                            task_id=task.id,
-                            on_start_value=on_start_value,
-                        )
-
                         result = await loop.run_in_executor(
                             executor, lambda: handler(context, *args, **kwargs)
                         )
-                        result = cloudpickle.dumps(result)
-                    except BaseException as exc:
+                    except BaseException:
                         print(traceback.format_exc())
-                        result = cloudpickle.dumps(exc)
                         task_status = TaskStatus.Error
                     finally:
                         complete_task_response: TaskQueueCompleteResponse = (
                             await taskqueue_stub.task_queue_complete(
                                 TaskQueueCompleteRequest(
                                     task_id=task.id,
                                     stub_id=config.stub_id,
@@ -297,16 +332,23 @@
                                 )
                             )
                         )
 
                         if not complete_task_response.ok:
                             raise RunnerException("Unable to end task")
 
-                        print(f"Task completed <{task.id}>")
                         monitor_task.cancel()
+                        print(f"Task completed <{task.id}>")
+
+                        await send_callback(
+                            gateway_stub=gateway_stub,
+                            context=context,
+                            payload=result,
+                            task_status=task_status,
+                        )  # Send callback to callback_url, if defined
 
             loop.run_until_complete(_run_task())
 
 
 if __name__ == "__main__":
     tq = TaskQueueManager()
     tq.run()
```

### Comparing `beta9-0.1.4/src/beta9/sync.py` & `beta9-0.1.5/src/beta9/sync.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/terminal.py` & `beta9-0.1.5/src/beta9/terminal.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.4/src/beta9/type.py` & `beta9-0.1.5/src/beta9/type.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 class TaskStatus(str, Enum):
     Complete = "COMPLETE"
     Error = "ERROR"
     Pending = "PENDING"
     Running = "RUNNING"
     Cancelled = "CANCELLED"
     Retry = "RETRY"
+    Timeout = "TIMEOUT"
+
+    def __str__(self) -> str:
+        return self.value
 
 
 class TaskExitCode:
     SigTerm = -15
     SigKill = -9
     Success = 0
     Error = 1
```

### Comparing `beta9-0.1.4/PKG-INFO` & `beta9-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

