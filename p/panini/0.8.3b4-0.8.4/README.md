# Comparing `tmp/panini-0.8.3b4.tar.gz` & `tmp/panini-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panini-0.8.3b4.tar", last modified: Wed Nov 29 19:10:12 2023, max compression
+gzip compressed data, was "panini-0.8.4.tar", last modified: Mon Apr 29 15:09:30 2024, max compression
```

## Comparing `panini-0.8.3b4.tar` & `panini-0.8.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.334041 panini-0.8.3b4/
--rw-r--r--   0 artas      (502) staff       (20)     4249 2023-11-29 17:39:53.000000 panini-0.8.3b4/CHANGELOG.md
--rw-r--r--   0 artas      (502) staff       (20)     1223 2023-11-29 17:39:53.000000 panini-0.8.3b4/CONTRIBUTING.md
--rw-r--r--   0 artas      (502) staff       (20)     1091 2023-11-29 17:39:53.000000 panini-0.8.3b4/LICENSE.md
--rw-r--r--   0 artas      (502) staff       (20)      105 2023-11-29 17:39:53.000000 panini-0.8.3b4/MANIFEST.in
--rw-r--r--   0 artas      (502) staff       (20)     2273 2023-11-29 19:10:12.330823 panini-0.8.3b4/PKG-INFO
--rw-r--r--   0 artas      (502) staff       (20)    11821 2023-11-29 17:39:53.000000 panini-0.8.3b4/README.md
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.013543 panini-0.8.3b4/panini/
--rw-r--r--   0 artas      (502) staff       (20)        0 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)    15017 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/app.py
--rw-r--r--   0 artas      (502) staff       (20)    13391 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/async_test_client.py
--rw-r--r--   0 artas      (502) staff       (20)     5449 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/emulator_client.py
--rw-r--r--   0 artas      (502) staff       (20)     2209 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/exceptions.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.037843 panini-0.8.3b4/panini/http_server/
--rw-r--r--   0 artas      (502) staff       (20)        0 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/http_server/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     1163 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/http_server/http_server_app.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.063141 panini-0.8.3b4/panini/managers/
--rw-r--r--   0 artas      (502) staff       (20)        0 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/managers/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     2826 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/managers/event_manager.py
--rw-r--r--   0 artas      (502) staff       (20)     6385 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/managers/middleware_manager.py
--rw-r--r--   0 artas      (502) staff       (20)    18198 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/managers/nats_client.py
--rw-r--r--   0 artas      (502) staff       (20)     3709 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/managers/schema_manager.py
--rw-r--r--   0 artas      (502) staff       (20)     2251 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/managers/task_manager.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.126520 panini-0.8.3b4/panini/middleware/
--rw-r--r--   0 artas      (502) staff       (20)     1563 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     1383 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/debug_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)     1355 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/error.py
--rw-r--r--   0 artas      (502) staff       (20)     1200 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/nats_timeout.py
--rw-r--r--   0 artas      (502) staff       (20)     3281 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/prometheus_monitoring.py
--rw-r--r--   0 artas      (502) staff       (20)     1716 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/reader_emulator_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)    15057 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/tracing_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)     3810 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/middleware/writer_emulator_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)    11241 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/test_client.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.138541 panini-0.8.3b4/panini/utils/
--rw-r--r--   0 artas      (502) staff       (20)        0 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/utils/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     3133 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/utils/helper.py
--rw-r--r--   0 artas      (502) staff       (20)     9207 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/utils/logger.py
--rw-r--r--   0 artas      (502) staff       (20)      185 2023-11-29 17:39:53.000000 panini-0.8.3b4/panini/utils/singleton.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.033801 panini-0.8.3b4/panini.egg-info/
--rw-r--r--   0 artas      (502) staff       (20)     2273 2023-11-29 19:10:11.000000 panini-0.8.3b4/panini.egg-info/PKG-INFO
--rw-r--r--   0 artas      (502) staff       (20)     1868 2023-11-29 19:10:11.000000 panini-0.8.3b4/panini.egg-info/SOURCES.txt
--rw-r--r--   0 artas      (502) staff       (20)        1 2023-11-29 19:10:11.000000 panini-0.8.3b4/panini.egg-info/dependency_links.txt
--rw-r--r--   0 artas      (502) staff       (20)        1 2023-11-29 17:42:42.000000 panini-0.8.3b4/panini.egg-info/not-zip-safe
--rw-r--r--   0 artas      (502) staff       (20)      359 2023-11-29 19:10:11.000000 panini-0.8.3b4/panini.egg-info/requires.txt
--rw-r--r--   0 artas      (502) staff       (20)        7 2023-11-29 19:10:11.000000 panini-0.8.3b4/panini.egg-info/top_level.txt
--rw-r--r--   0 artas      (502) staff       (20)      180 2023-11-29 17:39:53.000000 panini-0.8.3b4/pyproject.toml
--rw-r--r--   0 artas      (502) staff       (20)      262 2023-11-29 19:10:12.339345 panini-0.8.3b4/setup.cfg
--rw-r--r--   0 artas      (502) staff       (20)     2699 2023-11-29 17:46:52.000000 panini-0.8.3b4/setup.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-11-29 19:10:12.301381 panini-0.8.3b4/tests/
--rwxr-xr-x   0 artas      (502) staff       (20)      469 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_client_listen.py
--rwxr-xr-x   0 artas      (502) staff       (20)      433 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_client_listen_response.py
--rw-r--r--   0 artas      (502) staff       (20)     4785 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_diff_datatypes.py
--rwxr-xr-x   0 artas      (502) staff       (20)     2138 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_encoding.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1200 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_listen.py
--rw-r--r--   0 artas      (502) staff       (20)     2039 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_logs.py
--rw-r--r--   0 artas      (502) staff       (20)     2675 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_logs_in_separate_process.py
--rw-r--r--   0 artas      (502) staff       (20)      827 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_long_requests.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1537 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_long_tasks.py
--rw-r--r--   0 artas      (502) staff       (20)     3822 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)    11061 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_middleware_manager.py
--rwxr-xr-x   0 artas      (502) staff       (20)      785 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_on_start.py
--rw-r--r--   0 artas      (502) staff       (20)     1265 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_parameter_listen_subject_only_if_exclude.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1269 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_parameter_listen_subject_only_if_include.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1207 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_publish.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1195 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_reply_to.py
--rwxr-xr-x   0 artas      (502) staff       (20)      857 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_request.py
--rw-r--r--   0 artas      (502) staff       (20)      981 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_request_listen_response.py
--rw-r--r--   0 artas      (502) staff       (20)     2510 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_serializer_callable.py
--rw-r--r--   0 artas      (502) staff       (20)     2188 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_serializer_dacite.py
--rwxr-xr-x   0 artas      (502) staff       (20)      880 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_task.py
--rwxr-xr-x   0 artas      (502) staff       (20)      809 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_timeout.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1088 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_timer_task.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1082 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_timer_task_new_interface.py
--rwxr-xr-x   0 artas      (502) staff       (20)     1496 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_web_server.py
--rwxr-xr-x   0 artas      (502) staff       (20)     2269 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_web_server_separately.py
--rw-r--r--   0 artas      (502) staff       (20)     2827 2023-11-29 17:39:53.000000 panini-0.8.3b4/tests/test_wss.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.686217 panini-0.8.4/
+-rw-r--r--   0 artas      (502) staff       (20)     4249 2024-04-29 15:00:52.000000 panini-0.8.4/CHANGELOG.md
+-rw-r--r--   0 artas      (502) staff       (20)     1223 2024-04-29 15:00:52.000000 panini-0.8.4/CONTRIBUTING.md
+-rw-r--r--   0 artas      (502) staff       (20)     1091 2024-04-29 15:00:52.000000 panini-0.8.4/LICENSE.md
+-rw-r--r--   0 artas      (502) staff       (20)      105 2024-04-29 15:00:52.000000 panini-0.8.4/MANIFEST.in
+-rw-r--r--   0 artas      (502) staff       (20)     2271 2024-04-29 15:09:30.685870 panini-0.8.4/PKG-INFO
+-rw-r--r--   0 artas      (502) staff       (20)    11821 2024-04-29 15:00:52.000000 panini-0.8.4/README.md
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.622208 panini-0.8.4/panini/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2024-04-29 15:00:52.000000 panini-0.8.4/panini/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)    15017 2024-04-29 15:00:52.000000 panini-0.8.4/panini/app.py
+-rw-r--r--   0 artas      (502) staff       (20)    13391 2024-04-29 15:00:52.000000 panini-0.8.4/panini/async_test_client.py
+-rw-r--r--   0 artas      (502) staff       (20)     5449 2024-04-29 15:00:52.000000 panini-0.8.4/panini/emulator_client.py
+-rw-r--r--   0 artas      (502) staff       (20)     2209 2024-04-29 15:00:52.000000 panini-0.8.4/panini/exceptions.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.626366 panini-0.8.4/panini/http_server/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2024-04-29 15:00:52.000000 panini-0.8.4/panini/http_server/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     1163 2024-04-29 15:00:52.000000 panini-0.8.4/panini/http_server/http_server_app.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.631014 panini-0.8.4/panini/managers/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2024-04-29 15:00:52.000000 panini-0.8.4/panini/managers/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     2826 2024-04-29 15:00:52.000000 panini-0.8.4/panini/managers/event_manager.py
+-rw-r--r--   0 artas      (502) staff       (20)     6385 2024-04-29 15:00:52.000000 panini-0.8.4/panini/managers/middleware_manager.py
+-rw-r--r--   0 artas      (502) staff       (20)    17275 2024-04-29 15:06:50.000000 panini-0.8.4/panini/managers/nats_client.py
+-rw-r--r--   0 artas      (502) staff       (20)     3709 2024-04-29 15:00:52.000000 panini-0.8.4/panini/managers/schema_manager.py
+-rw-r--r--   0 artas      (502) staff       (20)     2251 2024-04-29 15:00:52.000000 panini-0.8.4/panini/managers/task_manager.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.637887 panini-0.8.4/panini/middleware/
+-rw-r--r--   0 artas      (502) staff       (20)     1563 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     1383 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/debug_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)     1355 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/error.py
+-rw-r--r--   0 artas      (502) staff       (20)     1200 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/nats_timeout.py
+-rw-r--r--   0 artas      (502) staff       (20)     3281 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/prometheus_monitoring.py
+-rw-r--r--   0 artas      (502) staff       (20)     1716 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/reader_emulator_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)    15628 2024-04-29 15:06:50.000000 panini-0.8.4/panini/middleware/tracing_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)     3810 2024-04-29 15:00:52.000000 panini-0.8.4/panini/middleware/writer_emulator_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)    11241 2024-04-29 15:00:52.000000 panini-0.8.4/panini/test_client.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.641699 panini-0.8.4/panini/utils/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2024-04-29 15:00:52.000000 panini-0.8.4/panini/utils/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     3133 2024-04-29 15:00:52.000000 panini-0.8.4/panini/utils/helper.py
+-rw-r--r--   0 artas      (502) staff       (20)     9207 2024-04-29 15:00:52.000000 panini-0.8.4/panini/utils/logger.py
+-rw-r--r--   0 artas      (502) staff       (20)      185 2024-04-29 15:00:52.000000 panini-0.8.4/panini/utils/singleton.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.682362 panini-0.8.4/panini.egg-info/
+-rw-r--r--   0 artas      (502) staff       (20)     2271 2024-04-29 15:09:30.000000 panini-0.8.4/panini.egg-info/PKG-INFO
+-rw-r--r--   0 artas      (502) staff       (20)     1868 2024-04-29 15:09:30.000000 panini-0.8.4/panini.egg-info/SOURCES.txt
+-rw-r--r--   0 artas      (502) staff       (20)        1 2024-04-29 15:09:30.000000 panini-0.8.4/panini.egg-info/dependency_links.txt
+-rw-r--r--   0 artas      (502) staff       (20)        1 2024-04-29 15:01:24.000000 panini-0.8.4/panini.egg-info/not-zip-safe
+-rw-r--r--   0 artas      (502) staff       (20)      359 2024-04-29 15:09:30.000000 panini-0.8.4/panini.egg-info/requires.txt
+-rw-r--r--   0 artas      (502) staff       (20)        7 2024-04-29 15:09:30.000000 panini-0.8.4/panini.egg-info/top_level.txt
+-rw-r--r--   0 artas      (502) staff       (20)      180 2024-04-29 15:00:52.000000 panini-0.8.4/pyproject.toml
+-rw-r--r--   0 artas      (502) staff       (20)      262 2024-04-29 15:09:30.687267 panini-0.8.4/setup.cfg
+-rw-r--r--   0 artas      (502) staff       (20)     2697 2024-04-29 15:07:25.000000 panini-0.8.4/setup.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2024-04-29 15:09:30.679939 panini-0.8.4/tests/
+-rwxr-xr-x   0 artas      (502) staff       (20)      469 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_client_listen.py
+-rwxr-xr-x   0 artas      (502) staff       (20)      433 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_client_listen_response.py
+-rw-r--r--   0 artas      (502) staff       (20)     4785 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_diff_datatypes.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     2138 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_encoding.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1200 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_listen.py
+-rw-r--r--   0 artas      (502) staff       (20)     2039 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_logs.py
+-rw-r--r--   0 artas      (502) staff       (20)     2675 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_logs_in_separate_process.py
+-rw-r--r--   0 artas      (502) staff       (20)      827 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_long_requests.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1537 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_long_tasks.py
+-rw-r--r--   0 artas      (502) staff       (20)     3822 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)    11061 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_middleware_manager.py
+-rwxr-xr-x   0 artas      (502) staff       (20)      785 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_on_start.py
+-rw-r--r--   0 artas      (502) staff       (20)     1265 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_parameter_listen_subject_only_if_exclude.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1269 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_parameter_listen_subject_only_if_include.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1207 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_publish.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1195 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_reply_to.py
+-rwxr-xr-x   0 artas      (502) staff       (20)      857 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_request.py
+-rw-r--r--   0 artas      (502) staff       (20)      981 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_request_listen_response.py
+-rw-r--r--   0 artas      (502) staff       (20)     2510 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_serializer_callable.py
+-rw-r--r--   0 artas      (502) staff       (20)     2188 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_serializer_dacite.py
+-rwxr-xr-x   0 artas      (502) staff       (20)      880 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_task.py
+-rwxr-xr-x   0 artas      (502) staff       (20)      809 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_timeout.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1088 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_timer_task.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1082 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_timer_task_new_interface.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     1496 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_web_server.py
+-rwxr-xr-x   0 artas      (502) staff       (20)     2269 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_web_server_separately.py
+-rw-r--r--   0 artas      (502) staff       (20)     2827 2024-04-29 15:00:52.000000 panini-0.8.4/tests/test_wss.py
```

### Comparing `panini-0.8.3b4/CHANGELOG.md` & `panini-0.8.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/CONTRIBUTING.md` & `panini-0.8.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/LICENSE.md` & `panini-0.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/PKG-INFO` & `panini-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panini
-Version: 0.8.3b4
+Version: 0.8.4
 Summary: A python messaging framework for microservices based on NATS
 Home-page: https://github.com/lwinterface/panini
 Author: Op Return SA, developers: Andrii Volotskov, Danylo Tiutiushkin
 Author-email: example@example.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/lwinterface/panini/issues
 Project-URL: Source, https://github.com/lwinterface/panini/
```

### Comparing `panini-0.8.3b4/README.md` & `panini-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/app.py` & `panini-0.8.4/panini/app.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/async_test_client.py` & `panini-0.8.4/panini/async_test_client.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/emulator_client.py` & `panini-0.8.4/panini/emulator_client.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/exceptions.py` & `panini-0.8.4/panini/exceptions.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/http_server/http_server_app.py` & `panini-0.8.4/panini/http_server/http_server_app.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/managers/event_manager.py` & `panini-0.8.4/panini/managers/event_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/managers/middleware_manager.py` & `panini-0.8.4/panini/managers/middleware_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/managers/nats_client.py` & `panini-0.8.4/panini/managers/nats_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,49 +372,14 @@
 
     async def _publish_js(
             self,
             subject: str,
             message,
             timeout: float = None,
             stream: str = None,
-            headers: dict = None
-    ) :
-        payload: bytes = self.format_message_data_type(message, type(message))
-        return await self._js.publish(
-                subject=subject,
-                payload=payload,
-                timeout=timeout,
-                stream=stream,
-                headers=headers
-        )
-
-    async def publish_js(
-            self,
-            subject: str,
-            message,
-            timeout: float = None,
-            stream: str = None,
-            headers: dict = None,
-            *args,
-            **kwargs
-    ):
-        return await self._publish_js(
-            subject=subject,
-            message=message,
-            timeout=timeout,
-            stream=stream,
-            headers=headers,
-        )
-
-    async def _publish_js(
-            self,
-            subject: str,
-            message,
-            timeout: float = None,
-            stream: str = None,
             data_type: type = dict,
             headers: dict = None,
             *args,
             **kwargs
     ) :
         payload: bytes = self.format_message_data_type(message, data_type)
         return await self._js.publish(
```

### Comparing `panini-0.8.3b4/panini/managers/schema_manager.py` & `panini-0.8.4/panini/managers/schema_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/managers/task_manager.py` & `panini-0.8.4/panini/managers/task_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/__init__.py` & `panini-0.8.4/panini/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/debug_middleware.py` & `panini-0.8.4/panini/middleware/debug_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/error.py` & `panini-0.8.4/panini/middleware/error.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/nats_timeout.py` & `panini-0.8.4/panini/middleware/nats_timeout.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/prometheus_monitoring.py` & `panini-0.8.4/panini/middleware/prometheus_monitoring.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/reader_emulator_middleware.py` & `panini-0.8.4/panini/middleware/reader_emulator_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/middleware/tracing_middleware.py` & `panini-0.8.4/panini/middleware/tracing_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,14 +160,20 @@
         if otel_tracer:
             self._otel_tracer = otel_tracer
         else:
             self._otel_tracer = OTELTracer(tracing_config=tracing_config, **kwargs)
         self.tracer: Tracer = self._otel_tracer.tracer
         self.parent = TraceContextTextMapPropagator()
         self._service_name = tracing_config["service_name"]
+        self._ignored_subjects_listen = tracing_config.get("custom_config", {}).get(
+            "ignore_listen_subjects", []
+        )
+        self._ignored_subjects_send = tracing_config.get("custom_config", {}).get(
+            "ignore_send_subjects", []
+        )
         super().__init__()
 
     def _create_uuid(self) -> str:
         return uuid.uuid4().hex
 
     def _get_span_name(self, action: str, subject: str) -> str:
         return f"{action.upper()} {subject}"
@@ -195,35 +201,35 @@
             link = [trace.Link(ctx)]
         else:
             link = []
         if not isinstance(span_config, SpanConfig):
             span_config = SpanConfig(
                 span_name=self._get_span_name(action, subject), span_attributes={}
             )
-        if use_tracing is True:
+        if use_tracing is True and subject not in self._ignored_subjects_send:
             self.tracer.start_span(name=span_config.span_name)
             with self.tracer.start_as_current_span(
                 span_config.span_name, links=link, context=context, kind=SpanKind.SERVER
             ) as span:
                 for attr_key, attr_value in span_config.span_attributes.items():
                     span.set_attribute(attr_key, attr_value)
                 span.add_event(
                     action,
                     {
                         "nats.subject": subject,
-                        "nats.message": json.dumps(message) if verbose else json.dumps(message)[:300],
+                        "nats.message": json.dumps(message, default=str) if verbose else json.dumps(message, default=str)[:300],
                     },
                 )
                 for existing_event in existing_events:
                     span.add_event(existing_event.event_name, existing_event.event_data)
                 span.set_attribute("nats.subject", subject)
                 self.parent.inject(carrier=carrier)
                 headers = {
                     "tracing_span_name": span_config.span_name,
-                    "tracing_span_carrier": json.dumps(carrier),
+                    "tracing_span_carrier": json.dumps(carrier, default=str),
                 }
                 kwargs.update({"headers": headers})
                 try:
                     response = await send_func(subject, message, *args, **kwargs)
                     if response and verbose:
                         span.add_event("request_response", {"nats.message": response})
                     return response
@@ -275,14 +281,18 @@
 
         return None
 
     async def trace_listen_any(self, msg: Msg, callback, nats_action=None):
         context = {}
         app = get_app()
         assert app is not None
+        for subject in self._ignored_subjects_listen:
+            if self.wildcard_match(subject, msg.subject):
+                response = await callback(msg)
+                return response
         for subject in app._event_manager.subscriptions.keys():
             matched_subject = self.wildcard_match(subject, msg.subject)
             if not matched_subject:
                 continue
             listen_obj_list = app._event_manager.subscriptions[matched_subject]
             listen_object: Listen
             for listen_object in listen_obj_list:
@@ -315,15 +325,15 @@
                             ) in span_config.span_attributes.items():
                                 span.set_attribute(attr_key, attr_val)
                             span.set_attribute("nats.subject", subject)
                             span.add_event(
                                 nats_action,
                                 {
                                     "nats.subject": subject,
-                                    "nats.message": json.dumps(msg.data) if verbose else json.dumps(msg.data)[:300],
+                                    "nats.message": json.dumps(msg.data, default=str) if verbose else json.dumps(msg.data, default=str)[:300],
                                 },
                             )
                             try:
                                 response = await callback(msg)
                                 if response and "tracing_events" in response.keys():
                                     tracing_events: List[TracingEvent] = response.pop(
                                         "tracing_events", []
```

### Comparing `panini-0.8.3b4/panini/middleware/writer_emulator_middleware.py` & `panini-0.8.4/panini/middleware/writer_emulator_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/test_client.py` & `panini-0.8.4/panini/test_client.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/utils/helper.py` & `panini-0.8.4/panini/utils/helper.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini/utils/logger.py` & `panini-0.8.4/panini/utils/logger.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/panini.egg-info/PKG-INFO` & `panini-0.8.4/panini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panini
-Version: 0.8.3b4
+Version: 0.8.4
 Summary: A python messaging framework for microservices based on NATS
 Home-page: https://github.com/lwinterface/panini
 Author: Op Return SA, developers: Andrii Volotskov, Danylo Tiutiushkin
 Author-email: example@example.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/lwinterface/panini/issues
 Project-URL: Source, https://github.com/lwinterface/panini/
```

### Comparing `panini-0.8.3b4/panini.egg-info/SOURCES.txt` & `panini-0.8.4/panini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/setup.py` & `panini-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "opentelemetry-sdk==1.19.0",
     "opentelemetry-exporter-otlp-proto-grpc==1.19.0",
     "opentelemetry-exporter-prometheus==1.12.0rc1"
 ]
 
 setup(
     name="panini",
-    version="0.8.3b4",
+    version="0.8.4",
     description="A python messaging framework for microservices based on NATS",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/lwinterface/panini",
     author="Op Return SA, developers: Andrii Volotskov, Danylo Tiutiushkin",
     author_email="example@example.com",
     python_requires=">=3.8.3",
```

### Comparing `panini-0.8.3b4/tests/test_diff_datatypes.py` & `panini-0.8.4/tests/test_diff_datatypes.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_encoding.py` & `panini-0.8.4/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_listen.py` & `panini-0.8.4/tests/test_listen.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_logs.py` & `panini-0.8.4/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_logs_in_separate_process.py` & `panini-0.8.4/tests/test_logs_in_separate_process.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_long_requests.py` & `panini-0.8.4/tests/test_long_requests.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_long_tasks.py` & `panini-0.8.4/tests/test_long_tasks.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_middleware.py` & `panini-0.8.4/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_middleware_manager.py` & `panini-0.8.4/tests/test_middleware_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_on_start.py` & `panini-0.8.4/tests/test_on_start.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_parameter_listen_subject_only_if_exclude.py` & `panini-0.8.4/tests/test_parameter_listen_subject_only_if_exclude.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_parameter_listen_subject_only_if_include.py` & `panini-0.8.4/tests/test_parameter_listen_subject_only_if_include.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_publish.py` & `panini-0.8.4/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_reply_to.py` & `panini-0.8.4/tests/test_reply_to.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_request.py` & `panini-0.8.4/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_request_listen_response.py` & `panini-0.8.4/tests/test_request_listen_response.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_serializer_callable.py` & `panini-0.8.4/tests/test_serializer_callable.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_serializer_dacite.py` & `panini-0.8.4/tests/test_serializer_dacite.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_task.py` & `panini-0.8.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_timeout.py` & `panini-0.8.4/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_timer_task.py` & `panini-0.8.4/tests/test_timer_task.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_timer_task_new_interface.py` & `panini-0.8.4/tests/test_timer_task_new_interface.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_web_server.py` & `panini-0.8.4/tests/test_web_server.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_web_server_separately.py` & `panini-0.8.4/tests/test_web_server_separately.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.3b4/tests/test_wss.py` & `panini-0.8.4/tests/test_wss.py`

 * *Files identical despite different names*

