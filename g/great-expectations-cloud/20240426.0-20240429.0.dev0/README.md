# Comparing `tmp/great_expectations_cloud-20240426.0.tar.gz` & `tmp/great_expectations_cloud-20240429.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240426.0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240429.0.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-20240426.0.tar` & `great_expectations_cloud-20240429.0.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-26 18:57:19.775872 great_expectations_cloud-20240426.0/LICENSE
--rw-r--r--   0        0        0     9269 2024-04-26 18:57:19.775872 great_expectations_cloud-20240426.0/README.md
--rw-r--r--   0        0        0      150 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    17084 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-26 18:57:19.811871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5918 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9457 2024-04-26 18:57:19.815871 great_expectations_cloud-20240426.0/pyproject.toml
--rw-r--r--   0        0        0    10598 1970-01-01 00:00:00.000000 great_expectations_cloud-20240426.0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-29 14:24:12.680714 great_expectations_cloud-20240429.0.dev0/LICENSE
+-rw-r--r--   0        0        0     9269 2024-04-29 14:24:12.680714 great_expectations_cloud-20240429.0.dev0/README.md
+-rw-r--r--   0        0        0      150 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    17128 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5918 2024-04-29 14:24:12.716714 great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9462 2024-04-29 14:24:12.720714 great_expectations_cloud-20240429.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    10603 1970-01-01 00:00:00.000000 great_expectations_cloud-20240429.0.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240426.0/LICENSE` & `great_expectations_cloud-20240429.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/README.md` & `great_expectations_cloud-20240429.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         self._correlation_ids: defaultdict[str, int] = defaultdict(lambda: 0)
 
     def run(self) -> None:
         """Open a connection to GX Cloud."""
 
         print("Opening connection to GX Cloud.")
         self._listen()
-        print("Connection to GX Cloud has been closed.")
+        print("The connection to GX Cloud has been closed.")
 
     # ZEL-505: A race condition can occur if two or more agents are started at the same time
     #          due to the generation of passwords for rabbitMQ queues. This can be mitigated
     #          by adding a delay and retrying the connection. Retrying with new credentials
     #          requires calling get_config again, which handles the password generation.
     @retry(
         retry=retry_if_exception_type((AuthenticationError, ProbableAuthenticationError)),
@@ -137,17 +137,17 @@
             print("The GX Agent is ready.")
             # Open a connection until encountering a shutdown event
             subscriber.consume(
                 queue=self._config.queue,
                 on_message=self._handle_event_as_thread_enter,
             )
         except KeyboardInterrupt:
-            print("Received request to shutdown.")
+            print("Received request to shut down.")
         except (SubscriberError, ClientError):
-            print("Connection to GX Cloud has encountered an error.")
+            print("The connection to GX Cloud has encountered an error.")
         except (AuthenticationError, ProbableAuthenticationError):
             # Retry with new credentials
             self._config = self._get_config()
             # Raise to use the retry decorator to handle the retry logic
             raise
         finally:
             if subscriber is not None:
@@ -231,15 +231,15 @@
         if error is None:
             result: ActionResult = future.result()
 
             if result.type == UnknownEvent().type:
                 status = JobCompleted(
                     success=False,
                     created_resources=[],
-                    error_stack_trace="The version of the GX Agent you are using does not support this functionality. Please upgrade to latest.",
+                    error_stack_trace="The version of the GX Agent you are using does not support this functionality. Please upgrade to the most recent image tagged with `stable`.",
                 )
                 LOGGER.error(
                     "Job completed with error. Ensure agent is up-to-date.",
                     extra={
                         "event_type": event_context.event.type,
                         "id": event_context.correlation_id,
                     },
@@ -270,15 +270,15 @@
         self._update_status(job_id=event_context.correlation_id, status=status)
 
         # ack message and cleanup resources
         event_context.processed_successfully()
         self._current_task = None
 
     def _can_accept_new_task(self) -> bool:
-        """Are we currently processing a task, or are we free to take a new one?"""
+        """Are we currently processing a task or are we free to take a new one?"""
         return self._current_task is None or self._current_task.done()
 
     def _reject_correlation_id(self, id: str) -> bool:
         """Has this correlation ID been seen too many times?"""
         MAX_REDELIVERY = 10
         MAX_KEYS = 100000
         self._correlation_ids[id] += 1
```

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240429.0.dev0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240426.0/pyproject.toml` & `great_expectations_cloud-20240429.0.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240426.0"
+version = "20240429.0.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240426.0/PKG-INFO` & `great_expectations_cloud-20240429.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240426.0
+Version: 20240429.0.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
```

