# Comparing `tmp/scrapegraphai-0.4.0b3.tar.gz` & `tmp/scrapegraphai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.4.0b3.tar", max compression
+gzip compressed data, was "scrapegraphai-0.4.1.tar", max compression
```

## Comparing `scrapegraphai-0.4.0b3.tar` & `scrapegraphai-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1065 2024-04-27 19:26:02.905712 scrapegraphai-0.4.0b3/LICENSE
--rw-r--r--   0        0        0     7907 2024-04-27 19:26:02.905712 scrapegraphai-0.4.0b3/README.md
--rw-r--r--   0        0        0     1646 2024-04-27 19:26:21.481839 scrapegraphai-0.4.0b3/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3817 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     4868 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2493 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2192 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2378 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      829 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3647 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6860 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5165 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6555 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6118 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1635 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0     1504 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      731 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1070 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-27 19:26:02.941712 scrapegraphai-0.4.0b3/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 scrapegraphai-0.4.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-28 18:30:16.316592 scrapegraphai-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7907 2024-04-28 18:30:16.316592 scrapegraphai-0.4.1/README.md
+-rw-r--r--   0        0        0     1660 2024-04-28 18:30:35.296634 scrapegraphai-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3817 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5128 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2493 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2192 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2378 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3647 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5136 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6555 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6118 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      513 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9619 1970-01-01 00:00:00.000000 scrapegraphai-0.4.1/PKG-INFO
```

### Comparing `scrapegraphai-0.4.0b3/LICENSE` & `scrapegraphai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/README.md` & `scrapegraphai-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/pyproject.toml` & `scrapegraphai-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.4.0b3"
+version = "0.4.1"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
@@ -17,28 +17,29 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = ">3.9,<4.0"
+python = "^3.9"
 langchain = "0.1.14"
 langchain-openai = "0.1.1"
 langchain-google-genai = "1.0.1"
 html2text = "2020.1.16"
 faiss-cpu = "1.8.0"
 beautifulsoup4 = "4.12.3"
 pandas = "2.0.3"
 python-dotenv = "1.0.1"
 tiktoken = {version = ">=0.5.2,<0.6.0"}
 tqdm = "4.66.1"
 graphviz = "0.20.1"
 google = "3.0.0"
 minify-html = "0.15.0"
+free-proxy = "1.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "8.0.0"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.4.1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.4.1/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.4.1/scrapegraphai/graphs/base_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,33 +52,32 @@
             dict: A dictionary of edges with the from-node as keys and to-node as values.
         """
         edge_dict = {}
         for from_node, to_node in edges:
             edge_dict[from_node.node_name] = to_node.node_name
         return edge_dict
 
-    def execute(self, initial_state: dict) -> dict:
+    def execute(self, initial_state: dict) -> (dict, list):
         """
         Executes the graph by traversing nodes starting from the entry point. The execution
         follows the edges based on the result of each node's execution and continues until
         it reaches a node with no outgoing edges.
 
         Args:
             initial_state (dict): The initial state to pass to the entry point node.
 
         Returns:
             dict: The state after execution has completed, which may have been altered by the nodes.
         """
-        print(self.nodes)
         current_node_name = self.nodes[0]
         state = initial_state
 
         # variables for tracking execution info
         total_exec_time = 0.0
-        exec_info = {}
+        exec_info = []
         cb_total = {
             "total_tokens": 0,
             "prompt_tokens": 0,
             "completion_tokens": 0,
             "successful_requests": 0,
             "total_cost_USD": 0.0,
         }
@@ -90,39 +89,44 @@
 
             with get_openai_callback() as cb:
                 result = current_node.execute(state)
                 node_exec_time = time.time() - curr_time
                 total_exec_time += node_exec_time
 
                 cb = {
+                    "node_name": index.node_name,
                     "total_tokens": cb.total_tokens,
                     "prompt_tokens": cb.prompt_tokens,
                     "completion_tokens": cb.completion_tokens,
                     "successful_requests": cb.successful_requests,
                     "total_cost_USD": cb.total_cost,
-                }
-
-                exec_info[current_node_name] = {
                     "exec_time": node_exec_time,
-                    "model_info": cb
                 }
 
+                exec_info.append(
+                    cb
+                )
+
                 cb_total["total_tokens"] += cb["total_tokens"]
                 cb_total["prompt_tokens"] += cb["prompt_tokens"]
                 cb_total["completion_tokens"] += cb["completion_tokens"]
                 cb_total["successful_requests"] += cb["successful_requests"]
                 cb_total["total_cost_USD"] += cb["total_cost_USD"]
 
             if current_node.node_type == "conditional_node":
                 current_node_name = result
             elif current_node_name in self.edges:
                 current_node_name = self.edges[current_node_name]
             else:
                 current_node_name = None
 
-        execution_info = {
-            "total_exec_time": total_exec_time,
-            "total_model_info": cb_total,
-            "nodes_info": exec_info
-        }
+        exec_info.append({
+            "node_name": "TOTAL RESULT",
+            "total_tokens":  cb_total["total_tokens"],
+            "prompt_tokens":  cb_total["prompt_tokens"],
+            "completion_tokens": cb_total["completion_tokens"],
+            "successful_requests": cb_total["successful_requests"],
+            "total_cost_USD":   cb_total["total_cost_USD"],
+            "exec_time": total_exec_time,
+        })
 
-        return state, execution_info
+        return state, exec_info
```

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.4.1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.4.1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.4.1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.4.1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.4.1/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.4.1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.4.1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.4.1/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/gemini.py` & `scrapegraphai-0.4.1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.4.1/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/ollama.py` & `scrapegraphai-0.4.1/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/openai.py` & `scrapegraphai-0.4.1/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.4.1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.4.1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/rag_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,13 @@
         )
 
         # relevant filter compressor only
         # compression_retriever = ContextualCompressionRetriever(
         #     base_compressor=relevant_filter, base_retriever=retriever
         # )
 
-        compressed_docs = compression_retriever.get_relevant_documents(
-            user_prompt)
+        compressed_docs = compression_retriever.invoke(user_prompt)
 
         print("--- (tokens compressed and vector stored) ---")
 
         state.update({self.output[0]: compressed_docs})
         return state
```

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.4.1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/remover.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.4.1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.0b3/PKG-INFO` & `scrapegraphai-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.4.0b3
+Version: 0.4.1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
-Requires-Python: >3.9,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (==4.12.3)
 Requires-Dist: faiss-cpu (==1.8.0)
+Requires-Dist: free-proxy (==1.1.1)
 Requires-Dist: google (==3.0.0)
 Requires-Dist: graphviz (==0.20.1)
 Requires-Dist: html2text (==2020.1.16)
 Requires-Dist: langchain (==0.1.14)
 Requires-Dist: langchain-google-genai (==1.0.1)
 Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: minify-html (==0.15.0)
```

