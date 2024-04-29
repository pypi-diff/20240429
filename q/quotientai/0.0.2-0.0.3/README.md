# Comparing `tmp/quotientai-0.0.2.tar.gz` & `tmp/quotientai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quotientai-0.0.2.tar", max compression
+gzip compressed data, was "quotientai-0.0.3.tar", max compression
```

## Comparing `quotientai-0.0.2.tar` & `quotientai-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11345 2024-04-11 06:20:12.620846 quotientai-0.0.2/LICENSE
--rw-r--r--   0        0        0      390 2024-04-11 06:20:12.620846 quotientai-0.0.2/README.md
--rw-r--r--   0        0        0     1011 2024-04-11 06:20:12.620846 quotientai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      288 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/__init__.py
--rw-r--r--   0        0        0       47 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/cli/__init__.py
--rw-r--r--   0        0        0    19112 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/cli/entrypoint.py
--rw-r--r--   0        0        0     9663 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/cli/format.py
--rw-r--r--   0        0        0    41502 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/client.py
--rw-r--r--   0        0        0      181 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/exceptions.py
--rw-r--r--   0        0        0     3118 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/utils.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 quotientai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-29 14:35:38.397110 quotientai-0.0.3/LICENSE
+-rw-r--r--   0        0        0      390 2024-04-29 14:35:38.397110 quotientai-0.0.3/README.md
+-rw-r--r--   0        0        0     1011 2024-04-29 14:35:38.397110 quotientai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/cli/__init__.py
+-rw-r--r--   0        0        0    18956 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/cli/entrypoint.py
+-rw-r--r--   0        0        0     7961 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/cli/format.py
+-rw-r--r--   0        0        0    41452 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/client.py
+-rw-r--r--   0        0        0      181 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/exceptions.py
+-rw-r--r--   0        0        0     4280 2024-04-29 14:35:38.397110 quotientai-0.0.3/quotientai/utils.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 quotientai-0.0.3/PKG-INFO
```

### Comparing `quotientai-0.0.2/LICENSE` & `quotientai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quotientai-0.0.2/pyproject.toml` & `quotientai-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quotientai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     "Vic Weiss <vic@quotientai.co>",
     "Freddie Vargus <freddie@quotientai.co>",
     "Allison Kunz <allison@quotient.co>",
 ]
 description = "CLI for evaluating large language models with Quotient"
 readme = "README.md"
```

### Comparing `quotientai-0.0.2/quotientai/cli/entrypoint.py` & `quotientai-0.0.3/quotientai/cli/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,18 @@
     format_models_table,
     format_prompt_template_table,
     format_recipes_table,
     format_results_summary_table,
     format_results_table,
     format_system_prompt_table,
     format_tasks_table,
-    save_eval_metadata_to_file,
-    save_metrics_to_file,
-    save_results_to_file,
 )
 from quotientai.client import QuotientClient
 from quotientai.exceptions import QuotientAIException
-from quotientai.utils import show_job_progress
+from quotientai.utils import results_to_csv, show_job_progress
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -544,17 +541,15 @@
 @save.command(name="results")
 @click.option("--job-id", required=True, type=int, help="Job ID to pull results for.")
 def save_results(job_id):
     """Command to save results for a job."""
     try:
         client = QuotientClient()
         results = client.get_eval_results(job_id)
-        save_results_to_file(results)
-        save_metrics_to_file(results)
-        save_eval_metadata_to_file(results)
+        results_to_csv(results)
 
     except QuotientAIException as e:
         click.echo(str(e))
 
 
 @create.command(name="job")
 @click.option("--task-id", required=True, type=int, help="Task ID for the job.")
```

### Comparing `quotientai-0.0.2/quotientai/cli/format.py` & `quotientai-0.0.3/quotientai/cli/format.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import json
-import os
 import textwrap
 
-import pandas as pd
 from prettytable import PrettyTable
 
 
 def format_api_keys_table(data):
     table = PrettyTable()
     table.field_names = ["Name", "Revoked", "Created At", "Expires At"]
     for item in data:
@@ -305,56 +302,7 @@
             [
                 metric_data["id"],
                 metric_data["name"],
                 owner_id,
             ]
         )
     return table
-
-
-def save_results_to_file(data):
-    data_to_frame = []
-    for item in data["results"]:
-        content = item["content"]
-        row = {
-            "id": content["id"],
-            "input_text": content["input_text"],
-            "answer": content["answer"],
-            "completion": content["completion"],
-            "context": content["context"],
-            "formatted_content": content["formatted_content"],
-        }
-        data_to_frame.append(row)
-
-    df = pd.DataFrame(data_to_frame)
-    file_name = f"quotient-results-{data['id']}.csv"
-    df.to_csv(file_name, index=False)
-    full_path = os.path.abspath(file_name)
-    print(f"Results saved to {full_path}")
-
-
-def save_metrics_to_file(data):
-    df = pd.json_normalize(data, "results")
-    df = df[df.columns[df.columns.str.contains("metric")]]
-    df.columns = df.columns.str.replace("metric.", "")
-    description = df.describe()
-    file_name = f"quotient-metrics-{data['id']}.csv"
-    description.to_csv(file_name, index=False)
-    full_path = os.path.abspath(file_name)
-    print(f"Metrics saved to {full_path}")
-
-
-def save_eval_metadata_to_file(data):
-    selected_info = {
-        "model_name": data.get("model_name"),
-        "task_name": data.get("task_name"),
-        "completed_at": data.get("completed_at"),
-        "id": data.get("id"),
-        "task_type": data.get("task_type"),
-        "seed": data.get("seed"),
-    }
-
-    file_name = f"quotient-eval-metadata-{data['id']}.json"
-    with open(file_name, "w") as json_file:
-        json.dump(selected_info, json_file, indent=4)
-    full_path = os.path.abspath(file_name)
-    print(f"Evaluation metadata saved to {full_path}")
```

### Comparing `quotientai-0.0.2/quotientai/client.py` & `quotientai-0.0.3/quotientai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1070,17 +1070,15 @@
         --------
         dict
             The metric record from the API.
         """
         try:
             # check for valid template
             if "{input_text}" not in rubric_template:
-                raise QuotientAIInvalidInputException(
-                    "Rubric template must include `{input_text}`"
-                )
+                raise QuotientAIException("Rubric template must include `{input_text}`")
 
             byo_metric_data = {
                 "name": name,
                 "rubric_template": rubric_template,
                 "model_id": model_id,
                 "created_at": datetime.utcnow().isoformat(),
             }
```

### Comparing `quotientai-0.0.2/PKG-INFO` & `quotientai-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quotientai
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI for evaluating large language models with Quotient
 License: Apache-2.0
 Keywords: quotient,evaluation,llms,machine learning,ai
 Author: Vic Weiss
 Author-email: vic@quotientai.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

