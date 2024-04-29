# Comparing `tmp/langchain_mistralai-0.1.4.tar.gz` & `tmp/langchain_mistralai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.4.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.5.tar", max compression
```

## Comparing `langchain_mistralai-0.1.4.tar` & `langchain_mistralai-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/LICENSE
--rw-r--r--   0        0        0     1336 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/README.md
--rw-r--r--   0        0        0      173 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    29480 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     7158 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2391 2024-04-26 17:15:19.603220 langchain_mistralai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1336 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/README.md
+-rw-r--r--   0        0        0      173 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    29632 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     7310 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2391 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.5/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.4/LICENSE` & `langchain_mistralai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.4/README.md` & `langchain_mistralai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.4/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.5/langchain_mistralai/chat_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,33 +404,35 @@
         values["mistral_api_key"] = convert_to_secret_str(
             get_from_dict_or_env(
                 values, "mistral_api_key", "MISTRAL_API_KEY", default=""
             )
         )
         api_key_str = values["mistral_api_key"].get_secret_value()
         # todo: handle retries
-        values["client"] = httpx.Client(
-            base_url=values["endpoint"],
-            headers={
-                "Content-Type": "application/json",
-                "Accept": "application/json",
-                "Authorization": f"Bearer {api_key_str}",
-            },
-            timeout=values["timeout"],
-        )
+        if not values.get("client"):
+            values["client"] = httpx.Client(
+                base_url=values["endpoint"],
+                headers={
+                    "Content-Type": "application/json",
+                    "Accept": "application/json",
+                    "Authorization": f"Bearer {api_key_str}",
+                },
+                timeout=values["timeout"],
+            )
         # todo: handle retries and max_concurrency
-        values["async_client"] = httpx.AsyncClient(
-            base_url=values["endpoint"],
-            headers={
-                "Content-Type": "application/json",
-                "Accept": "application/json",
-                "Authorization": f"Bearer {api_key_str}",
-            },
-            timeout=values["timeout"],
-        )
+        if not values.get("async_client"):
+            values["async_client"] = httpx.AsyncClient(
+                base_url=values["endpoint"],
+                headers={
+                    "Content-Type": "application/json",
+                    "Accept": "application/json",
+                    "Authorization": f"Bearer {api_key_str}",
+                },
+                timeout=values["timeout"],
+            )
 
         if values["temperature"] is not None and not 0 <= values["temperature"] <= 1:
             raise ValueError("temperature must be in the range [0.0, 1.0]")
 
         if values["top_p"] is not None and not 0 <= values["top_p"] <= 1:
             raise ValueError("top_p must be in the range [0.0, 1.0]")
```

### Comparing `langchain_mistralai-0.1.4/langchain_mistralai/embeddings.py` & `langchain_mistralai-0.1.5/langchain_mistralai/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,33 +71,35 @@
         values["mistral_api_key"] = convert_to_secret_str(
             get_from_dict_or_env(
                 values, "mistral_api_key", "MISTRAL_API_KEY", default=""
             )
         )
         api_key_str = values["mistral_api_key"].get_secret_value()
         # todo: handle retries
-        values["client"] = httpx.Client(
-            base_url=values["endpoint"],
-            headers={
-                "Content-Type": "application/json",
-                "Accept": "application/json",
-                "Authorization": f"Bearer {api_key_str}",
-            },
-            timeout=values["timeout"],
-        )
+        if not values.get("client"):
+            values["client"] = httpx.Client(
+                base_url=values["endpoint"],
+                headers={
+                    "Content-Type": "application/json",
+                    "Accept": "application/json",
+                    "Authorization": f"Bearer {api_key_str}",
+                },
+                timeout=values["timeout"],
+            )
         # todo: handle retries and max_concurrency
-        values["async_client"] = httpx.AsyncClient(
-            base_url=values["endpoint"],
-            headers={
-                "Content-Type": "application/json",
-                "Accept": "application/json",
-                "Authorization": f"Bearer {api_key_str}",
-            },
-            timeout=values["timeout"],
-        )
+        if not values.get("async_client"):
+            values["async_client"] = httpx.AsyncClient(
+                base_url=values["endpoint"],
+                headers={
+                    "Content-Type": "application/json",
+                    "Accept": "application/json",
+                    "Authorization": f"Bearer {api_key_str}",
+                },
+                timeout=values["timeout"],
+            )
         if values["tokenizer"] is None:
             try:
                 values["tokenizer"] = Tokenizer.from_pretrained(
                     "mistralai/Mixtral-8x7B-v0.1"
                 )
             except IOError:  # huggingface_hub GatedRepoError
                 warnings.warn(
```

### Comparing `langchain_mistralai-0.1.4/pyproject.toml` & `langchain_mistralai-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.4"
+version = "0.1.5"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_mistralai-0.1.4/PKG-INFO` & `langchain_mistralai-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.4
+Version: 0.1.5
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

