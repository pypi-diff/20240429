# Comparing `tmp/log10_io-0.8.3.tar.gz` & `tmp/log10_io-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.8.3.tar", max compression
+gzip compressed data, was "log10_io-0.8.4.tar", max compression
```

## Comparing `log10_io-0.8.3.tar` & `log10_io-0.8.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1083 2024-04-26 00:11:42.135162 log10_io-0.8.3/LICENSE
--rw-r--r--   0        0        0     9613 2024-04-26 00:11:42.135162 log10_io-0.8.3/README.md
--rw-r--r--   0        0        0        0 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/__main__.py
--rw-r--r--   0        0        0    11352 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/bigquery.py
--rw-r--r--   0        0        0      719 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/cli_utils.py
--rw-r--r--   0        0        0    22337 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/evals.py
--rw-r--r--   0        0        0     5459 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4487 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8357 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/feedback.py
--rw-r--r--   0        0        0     4880 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/langchain.py
--rw-r--r--   0        0        0     4432 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/litellm.py
--rw-r--r--   0        0        0     7967 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/llm.py
--rw-r--r--   0        0        0    39993 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/load.py
--rw-r--r--   0        0        0     2886 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/openai.py
--rw-r--r--   0        0        0     6915 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/together.py
--rw-r--r--   0        0        0     2101 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/tools.py
--rw-r--r--   0        0        0     1211 2024-04-26 00:11:42.139162 log10_io-0.8.3/log10/utils.py
--rw-r--r--   0        0        0     2242 2024-04-26 00:11:42.143162 log10_io-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 log10_io-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-29 19:07:55.897681 log10_io-0.8.4/LICENSE
+-rw-r--r--   0        0        0     9613 2024-04-29 19:07:55.897681 log10_io-0.8.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/__main__.py
+-rw-r--r--   0        0        0    11352 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6079 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/bigquery.py
+-rw-r--r--   0        0        0      719 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/cli_utils.py
+-rw-r--r--   0        0        0    22337 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/evals.py
+-rw-r--r--   0        0        0     5459 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4487 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     5206 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/langchain.py
+-rw-r--r--   0        0        0     4432 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/llm.py
+-rw-r--r--   0        0        0    39993 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/openai.py
+-rw-r--r--   0        0        0     6915 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/tools.py
+-rw-r--r--   0        0        0     1211 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/utils.py
+-rw-r--r--   0        0        0     2242 2024-04-29 19:07:55.901681 log10_io-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 log10_io-0.8.4/PKG-INFO
```

### Comparing `log10_io-0.8.3/LICENSE` & `log10_io-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/README.md` & `log10_io-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/__main__.py` & `log10_io-0.8.4/log10/__main__.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/_httpx_utils.py` & `log10_io-0.8.4/log10/_httpx_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/agents/camel.py` & `log10_io-0.8.4/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/agents/scrape_summarizer.py` & `log10_io-0.8.4/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/anthropic.py` & `log10_io-0.8.4/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/bigquery.py` & `log10_io-0.8.4/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/cli_utils.py` & `log10_io-0.8.4/log10/cli_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/completions/completions.py` & `log10_io-0.8.4/log10/completions/completions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/evals.py` & `log10_io-0.8.4/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.8.4/log10/feedback/_summary_feedback_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/feedback/autofeedback.py` & `log10_io-0.8.4/log10/feedback/autofeedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/feedback/feedback.py` & `log10_io-0.8.4/log10/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/feedback/feedback_task.py` & `log10_io-0.8.4/log10/feedback/feedback_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,18 +40,18 @@
             res.raise_for_status()
             return res
         except Exception as e:
             logger.error(e)
             logger.error(e.response.json()["error"])
             raise
 
-    def create(self, task_schema: dict, name: str = None, instruction: str = None) -> httpx.Response:
-        json_payload = {"json_schema": task_schema}
-        if name:
-            json_payload["name"] = name
+    def create(
+        self, task_schema: dict, name: str, completion_tags_selector: list[str] = None, instruction: str = None
+    ) -> httpx.Response:
+        json_payload = {"json_schema": task_schema, "name": name, "completion_tags_selector": completion_tags_selector}
         if instruction:
             json_payload["instruction"] = instruction
 
         res = self._post_request(self.feedback_task_create_url, json_payload)
         return res
 
     def list(self, limit: int = 10, offset: int = 0) -> httpx.Response:
@@ -77,18 +77,29 @@
 
 
 # create a cli interface for FeebackTask.create function
 @click.command()
 @click.option("--name", prompt="Enter feedback task name", help="Name of the task")
 @click.option("--task_schema", prompt="Enter feedback task schema", help="Task schema")
 @click.option("--instruction", help="Task instruction", default="")
-def create_feedback_task(name, task_schema, instruction):
+@click.option(
+    "--completion_tags_selector",
+    help="Completion tags selector",
+)
+def create_feedback_task(name, task_schema, instruction, completion_tags_selector=None):
     click.echo("Creating feedback task")
+    tags = []
+
+    if completion_tags_selector:
+        tags = completion_tags_selector.split(",")
+
     task_schema = json.loads(task_schema)
-    task = FeedbackTask().create(name=name, task_schema=task_schema, instruction=instruction)
+    task = FeedbackTask().create(
+        name=name, task_schema=task_schema, completion_tags_selector=tags, instruction=instruction
+    )
     click.echo(f"Use this task_id to add feedback: {task.json()['id']}")
 
 
 @click.command()
 @click.option("--limit", default=25, help="Number of feedback tasks to fetch")
 @click.option("--offset", default=0, help="Offset for the feedback tasks")
 def list_feedback_task(limit, offset):
```

### Comparing `log10_io-0.8.3/log10/langchain.py` & `log10_io-0.8.4/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/litellm.py` & `log10_io-0.8.4/log10/litellm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/llm.py` & `log10_io-0.8.4/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/load.py` & `log10_io-0.8.4/log10/load.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/mosaicml.py` & `log10_io-0.8.4/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/openai.py` & `log10_io-0.8.4/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/prompt_analyzer.py` & `log10_io-0.8.4/log10/prompt_analyzer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/schemas/bigquery.json` & `log10_io-0.8.4/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/together.py` & `log10_io-0.8.4/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/tools.py` & `log10_io-0.8.4/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/log10/utils.py` & `log10_io-0.8.4/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.3/pyproject.toml` & `log10_io-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.8.3"
+version = "0.8.4"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `log10_io-0.8.3/PKG-INFO` & `log10_io-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.8.3
+Version: 0.8.4
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

