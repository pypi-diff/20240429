# Comparing `tmp/jb_manager_bot-0.1.4.tar.gz` & `tmp/jb_manager_bot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jb_manager_bot-0.1.4.tar", max compression
+gzip compressed data, was "jb_manager_bot-0.1.5.tar", max compression
```

## Comparing `jb_manager_bot-0.1.4.tar` & `jb_manager_bot-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       43 2024-03-06 06:29:11.977136 jb_manager_bot-0.1.4/README.md
--rw-r--r--   0        0        0      277 2024-02-28 11:22:08.027840 jb_manager_bot-0.1.4/jb_manager_bot/__init__.py
--rw-r--r--   0        0        0     7734 2024-02-28 11:22:08.027840 jb_manager_bot-0.1.4/jb_manager_bot/abstract_fsm.py
--rw-r--r--   0        0        0     1376 2024-02-28 11:22:08.027840 jb_manager_bot-0.1.4/jb_manager_bot/data_models.py
--rw-r--r--   0        0        0       89 2024-03-06 06:25:08.483538 jb_manager_bot-0.1.4/jb_manager_bot/parsers/__init__.py
--rw-r--r--   0        0        0     1641 2024-03-06 06:25:08.483538 jb_manager_bot-0.1.4/jb_manager_bot/parsers/option_parser/__init__.py
--rw-r--r--   0        0        0     1074 2024-03-06 06:25:08.483538 jb_manager_bot-0.1.4/jb_manager_bot/parsers/option_parser/prompt.txt
--rw-r--r--   0        0        0     3718 2024-03-06 06:25:08.483538 jb_manager_bot-0.1.4/jb_manager_bot/parsers/utils.py
--rw-r--r--   0        0        0      513 2024-03-06 06:25:08.483538 jb_manager_bot-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 jb_manager_bot-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/README.md
+-rw-r--r--   0        0        0      277 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/__init__.py
+-rw-r--r--   0        0        0     7734 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/abstract_fsm.py
+-rw-r--r--   0        0        0     1376 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/data_models.py
+-rw-r--r--   0        0        0       89 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/parsers/__init__.py
+-rw-r--r--   0        0        0     1641 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/__init__.py
+-rw-r--r--   0        0        0     1074 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/prompt.txt
+-rw-r--r--   0        0        0     4705 2024-04-15 13:11:47.196211 jb_manager_bot-0.1.5/jb_manager_bot/parsers/utils.py
+-rw-r--r--   0        0        0      513 2024-04-15 12:04:31.120779 jb_manager_bot-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 jb_manager_bot-0.1.5/PKG-INFO
```

### Comparing `jb_manager_bot-0.1.4/jb_manager_bot/abstract_fsm.py` & `jb_manager_bot-0.1.5/jb_manager_bot/abstract_fsm.py`

 * *Files identical despite different names*

### Comparing `jb_manager_bot-0.1.4/jb_manager_bot/data_models.py` & `jb_manager_bot-0.1.5/jb_manager_bot/data_models.py`

 * *Files identical despite different names*

### Comparing `jb_manager_bot-0.1.4/jb_manager_bot/parsers/option_parser/__init__.py` & `jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `jb_manager_bot-0.1.4/jb_manager_bot/parsers/option_parser/prompt.txt` & `jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/prompt.txt`

 * *Files identical despite different names*

### Comparing `jb_manager_bot-0.1.4/jb_manager_bot/parsers/utils.py` & `jb_manager_bot-0.1.5/jb_manager_bot/parsers/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from typing import List
 from openai import OpenAI, AzureOpenAI
 
 
 class LLMManager:
     """Language Model Manager for OpenAI's GPT."""
 
     client: OpenAI = None
@@ -115,7 +116,39 @@
                 "parameters": {
                     "type": "object",
                     "properties": params,
                     "required": required,
                 },
             },
         }
+
+    @classmethod
+    def generate_embeddings(
+        cls,
+        inputs: List[str],
+        model: str,
+        openai_api_key=None,
+        azure_openai_api_key=None,
+        azure_openai_api_version=None,
+        azure_endpoint=None,
+        **kwargs
+    ):
+        """Use the OpenAI Embeddings API to generate embeddings for the given inputs."""
+        client = cls.get_client(
+            openai_api_key=openai_api_key,
+            azure_openai_api_key=azure_openai_api_key,
+            azure_openai_api_version=azure_openai_api_version,
+            azure_endpoint=azure_endpoint,
+        )
+        args = {
+            k: v
+            for k, v in kwargs.items()
+            if k
+            in [
+                "encoding_format",
+                "dimensions",
+            ]
+        }
+        response = client.embeddings.create(model=model, input=inputs, **args)
+        embeddings = [emb.embedding for emb in response.data]
+
+        return embeddings
```

### Comparing `jb_manager_bot-0.1.4/pyproject.toml` & `jb_manager_bot-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "jb-manager-bot"
-version = "0.1.4"
+version = "0.1.5"
 description = "Bot for JugalBandi Manager"
-authors = ["Sameer Segal <sameersegal@gmail.com>", "Shrey Pandey <shreypandey1509@gmail.com>", "Atharv Kirtikar <atharv.kirtikar@gmail.com>"]
+authors = ["Shrey Pandey <shreypandey1509@gmail.com>", "Sameer Segal <sameersegal@gmail.com>", "Atharv Kirtikar <atharv.kirtikar@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.6.1"
 transitions = "^0.9.0"
 openai = "^1.12.0"
```

### Comparing `jb_manager_bot-0.1.4/PKG-INFO` & `jb_manager_bot-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: jb-manager-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Bot for JugalBandi Manager
-Author: Sameer Segal
-Author-email: sameersegal@gmail.com
+Author: Shrey Pandey
+Author-email: shreypandey1509@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: transitions (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-# JBManager Bot
+# JB Manager Bot
 
 Bot for JugalBandi Manager
```

