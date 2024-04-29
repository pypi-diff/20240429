# Comparing `tmp/minimax_client-0.6.0.tar.gz` & `tmp/minimax_client-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimax_client-0.6.0.tar", last modified: Tue Apr 23 06:25:27 2024, max compression
+gzip compressed data, was "minimax_client-0.6.1.tar", last modified: Mon Apr 29 13:54:41 2024, max compression
```

## Comparing `minimax_client-0.6.0.tar` & `minimax_client-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.6.0/LICENSE.md
--rw-r--r--   0        0        0    13367 2024-04-23 06:23:06.665437 minimax_client-0.6.0/README.md
--rw-r--r--   0        0        0     2337 2024-04-23 06:25:27.923314 minimax_client-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.6.0/src/minimax_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-23 06:13:43.209671 minimax_client-0.6.0/src/minimax_client/__version__.py
--rw-r--r--   0        0        0     6268 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/client.py
--rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.6.0/src/minimax_client/entities/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.6.0/src/minimax_client/entities/assistant.py
--rw-r--r--   0        0        0     1743 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/entities/audio.py
--rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.6.0/src/minimax_client/entities/chat_completion.py
--rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.6.0/src/minimax_client/entities/common.py
--rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.6.0/src/minimax_client/entities/embedding.py
--rw-r--r--   0        0        0     1157 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/entities/file.py
--rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.6.0/src/minimax_client/entities/fine_tuning.py
--rw-r--r--   0        0        0       28 2024-04-18 09:58:33.261586 minimax_client-0.6.0/src/minimax_client/entities/retrieval.py
--rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.6.0/src/minimax_client/entities/thread.py
--rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.6.0/src/minimax_client/interfaces/__init__.py
--rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.6.0/src/minimax_client/interfaces/assistant.py
--rw-r--r--   0        0        0    31236 2024-04-23 06:13:30.322678 minimax_client-0.6.0/src/minimax_client/interfaces/audio.py
--rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.6.0/src/minimax_client/interfaces/base.py
--rw-r--r--   0        0        0     8842 2024-04-18 06:15:41.712616 minimax_client-0.6.0/src/minimax_client/interfaces/chat_completion.py
--rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.6.0/src/minimax_client/interfaces/embedding.py
--rw-r--r--   0        0        0     8150 2024-04-19 08:40:42.905673 minimax_client-0.6.0/src/minimax_client/interfaces/file.py
--rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.6.0/src/minimax_client/interfaces/fine_tuning.py
--rw-r--r--   0        0        0       28 2024-04-18 09:59:03.537448 minimax_client-0.6.0/src/minimax_client/interfaces/retrieval.py
--rw-r--r--   0        0        0    35341 2024-04-21 12:42:26.089567 minimax_client-0.6.0/src/minimax_client/interfaces/thread.py
--rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.6.0/tests/test_client.py
--rw-r--r--   0        0        0    14246 1970-01-01 00:00:00.000000 minimax_client-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.6.1/LICENSE.md
+-rw-r--r--   0        0        0    13367 2024-04-23 06:23:06.665437 minimax_client-0.6.1/README.md
+-rw-r--r--   0        0        0     2335 2024-04-29 13:54:41.248650 minimax_client-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.6.1/src/minimax_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-29 13:54:15.301452 minimax_client-0.6.1/src/minimax_client/__version__.py
+-rw-r--r--   0        0        0     6268 2024-04-21 12:42:26.089567 minimax_client-0.6.1/src/minimax_client/client.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.6.1/src/minimax_client/entities/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.6.1/src/minimax_client/entities/assistant.py
+-rw-r--r--   0        0        0     1743 2024-04-21 12:42:26.089567 minimax_client-0.6.1/src/minimax_client/entities/audio.py
+-rw-r--r--   0        0        0     1480 2024-04-29 13:54:15.302626 minimax_client-0.6.1/src/minimax_client/entities/chat_completion.py
+-rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.6.1/src/minimax_client/entities/common.py
+-rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.6.1/src/minimax_client/entities/embedding.py
+-rw-r--r--   0        0        0     1157 2024-04-21 12:42:26.089567 minimax_client-0.6.1/src/minimax_client/entities/file.py
+-rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.6.1/src/minimax_client/entities/fine_tuning.py
+-rw-r--r--   0        0        0       28 2024-04-18 09:58:33.261586 minimax_client-0.6.1/src/minimax_client/entities/retrieval.py
+-rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.6.1/src/minimax_client/entities/thread.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.6.1/src/minimax_client/interfaces/__init__.py
+-rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.6.1/src/minimax_client/interfaces/assistant.py
+-rw-r--r--   0        0        0    31236 2024-04-23 06:13:30.322678 minimax_client-0.6.1/src/minimax_client/interfaces/audio.py
+-rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.6.1/src/minimax_client/interfaces/base.py
+-rw-r--r--   0        0        0     9277 2024-04-29 13:54:15.303646 minimax_client-0.6.1/src/minimax_client/interfaces/chat_completion.py
+-rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.6.1/src/minimax_client/interfaces/embedding.py
+-rw-r--r--   0        0        0     8150 2024-04-19 08:40:42.905673 minimax_client-0.6.1/src/minimax_client/interfaces/file.py
+-rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.6.1/src/minimax_client/interfaces/fine_tuning.py
+-rw-r--r--   0        0        0       28 2024-04-18 09:59:03.537448 minimax_client-0.6.1/src/minimax_client/interfaces/retrieval.py
+-rw-r--r--   0        0        0    35341 2024-04-21 12:42:26.089567 minimax_client-0.6.1/src/minimax_client/interfaces/thread.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.6.1/tests/test_client.py
+-rw-r--r--   0        0        0    14244 1970-01-01 00:00:00.000000 minimax_client-0.6.1/PKG-INFO
```

### Comparing `minimax_client-0.6.0/LICENSE.md` & `minimax_client-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/README.md` & `minimax_client-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/pyproject.toml` & `minimax_client-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
-    "pytest>=8.1.1,<9",
+    "pytest>=8.2,<9",
 ]
 
 [project.urls]
 Homepage = "https://github.com/linzeyang/minimax-python-client"
 Repository = "https://github.com/linzeyang/minimax-python-client"
 
 [build-system]
```

### Comparing `minimax_client-0.6.0/src/minimax_client/client.py` & `minimax_client-0.6.1/src/minimax_client/client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/assistant.py` & `minimax_client-0.6.1/src/minimax_client/entities/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/audio.py` & `minimax_client-0.6.1/src/minimax_client/entities/audio.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/chat_completion.py` & `minimax_client-0.6.1/src/minimax_client/entities/chat_completion.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,10 +47,12 @@
 
 class ChatCompletionResponse(BareResponse):
     """Chat Completion Response"""
 
     id: str
     choices: List[Choice]
     created: int
-    model: Literal["abab5.5s-chat", "abab5.5-chat", "abab6-chat"]
+    model: Literal[
+        "abab5.5s-chat", "abab5.5-chat", "abab6-chat", "abab6.5s-chat", "abab6.5-chat"
+    ]
     object: Literal["chat.completion", "chat.completion.chunk"]
     usage: Optional[Usage] = None
```

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/common.py` & `minimax_client-0.6.1/src/minimax_client/entities/common.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/file.py` & `minimax_client-0.6.1/src/minimax_client/entities/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/fine_tuning.py` & `minimax_client-0.6.1/src/minimax_client/entities/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/entities/thread.py` & `minimax_client-0.6.1/src/minimax_client/entities/thread.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/assistant.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/audio.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/audio.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/base.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/chat_completion.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/chat_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """chat_completion.py"""
 
 import json
 from http import HTTPStatus
-from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Union
+from typing import Any, AsyncGenerator, Dict, Generator, List, Literal, Optional, Union
 
 import httpx
 
 from minimax_client.entities.chat_completion import ChatCompletionResponse
 from minimax_client.interfaces.base import BaseAsyncInterface, BaseSyncInterface
 
 
@@ -15,44 +15,51 @@
 
     url_path: str = "text/chatcompletion_v2"
 
     def create(
         self,
         *,
         messages: List[Dict[str, Union[str, List[Dict[str, Any]]]]],
-        model: str = "abab5.5s-chat",
+        model: Literal[
+            "abab5.5s-chat",
+            "abab5.5-chat",
+            "abab6-chat",
+            "abab6.5s-chat",
+            "abab6.5-chat",
+        ] = "abab5.5s-chat",
         max_tokens: int = 256,
         temperature: float = 0.9,
         top_p: float = 0.95,
         stream: bool = False,
-        tool_choice: str = "auto",
+        tool_choice: Literal["none", "auto"] = "auto",
         tools: Optional[List[Dict[str, Union[str, Dict[str, str]]]]] = None,
     ) -> Union[ChatCompletionResponse, Generator[ChatCompletionResponse, None, None]]:
         """
         Create a new chat completion request.
 
         Requests can be sent in or not in stream by setting the "stream" parameter.
         Streaming requests return a generator that yields ResponseEntities,
         while non-streaming requests return a single ResponseEntity.
 
         Args:
             messages (list[dict[str, Union[str, list[dict[str, Any]]]]]):
                 The messages to generate responses to
             model (str, optional):
-                The chatbot model to use. Defaults to "abab5.5s-chat".
+                The language model to use. Defaults to "abab5.5s-chat".
             max_tokens (int, optional):
                 The maximum number of tokens to generate. Defaults to 256.
             temperature (float, optional):
-                The temperature of the chatbot's responses. Defaults to 0.9.
+                The temperature of the responses. Defaults to 0.9.
             top_p (float, optional):
-                The top_p of the chatbot's responses. Defaults to 0.95.
+                The top_p of the responses. Defaults to 0.95.
             stream (bool, optional):
                 Whether to stream the responses or not. Defaults to False.
             tool_choice (str, optional):
-                The tool choice mode. Defaults to "auto".
+                The tool choice mode. Could be either "none" or "auto".
+                Defaults to "auto".
             tools (Optional[list[dict[str, Union[str, dict[str, str]]]]], optional):
                 The tools to use. Defaults to None.
 
         Returns:
             ChatCompletionResponse | Generator[ChatCompletionResponse, None, None]:
                 The response from the API or a generator of responses
         """
@@ -127,40 +134,47 @@
 class AsyncChatCompletions(BaseAsyncInterface, ChatCompletions):
     """Asynchronous Chat Completions interface"""
 
     async def create(
         self,
         *,
         messages: List[Dict[str, Union[str, List[Dict[str, Any]]]]],
-        model: str = "abab5.5s-chat",
+        model: Literal[
+            "abab5.5s-chat",
+            "abab5.5-chat",
+            "abab6-chat",
+            "abab6.5s-chat",
+            "abab6.5-chat",
+        ] = "abab5.5s-chat",
         max_tokens: int = 256,
         temperature: float = 0.9,
         top_p: float = 0.95,
         stream: bool = False,
-        tool_choice: str = "auto",
+        tool_choice: Literal["none", "auto"] = "auto",
         tools: Optional[List[Dict[str, Union[str, Dict[str, str]]]]] = None,
     ) -> Union[ChatCompletionResponse, AsyncGenerator[ChatCompletionResponse, None]]:
         """
         Create a new chat completion for the given messages.
 
         Args:
             messages (list[dict[str, Union[str, list[dict[str, Any]]]]]):
                 The messages to generate responses to
             model (str, optional):
-                The chatbot model to use. Defaults to "abab5.5s-chat".
+                The language model to use. Defaults to "abab5.5s-chat".
             max_tokens (int, optional):
                 The maximum number of tokens to generate. Defaults to 256.
             temperature (float, optional):
-                The temperature of the chatbot's responses. Defaults to 0.9.
+                The temperature of the responses. Defaults to 0.9.
             top_p (float, optional):
-                The top_p of the chatbot's responses. Defaults to 0.95.
+                The top_p of the responses. Defaults to 0.95.
             stream (bool, optional):
                 Whether to stream the responses or not. Defaults to False.
             tool_choice (str, optional):
-                The tool choice mode. Defaults to "auto".
+                The tool choice mode. Could be either "none" or "auto".
+                Defaults to "auto".
             tools (Optional[list[dict[str, Union[str, dict[str, str]]]]], optional):
                 The tools to use. Defaults to None.
 
         Returns:
             ChatCompletionResponse | AsyncGenerator[ChatCompletionResponse, None]:
                 The response from the API or a generator of responses
         """
```

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/embedding.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/embedding.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/file.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/fine_tuning.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/src/minimax_client/interfaces/thread.py` & `minimax_client-0.6.1/src/minimax_client/interfaces/thread.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/tests/test_client.py` & `minimax_client-0.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.6.0/PKG-INFO` & `minimax_client-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimax-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: An (unofficial) python native client for easy interaction with MiniMax Open Platform
 Keywords: web,api,llm
 Author-Email: Zeyang Lin <4020306+linzeyang@users.noreply.github.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://github.com/linzeyang/minimax-python-client
 Project-URL: Repository, https://github.com/linzeyang/minimax-python-client
 Requires-Python: >=3.8
 Requires-Dist: httpx<1
 Requires-Dist: python-dotenv<2
 Requires-Dist: pydantic<3
-Requires-Dist: pytest<9,>=8.1.1; extra == "dev"
+Requires-Dist: pytest<9,>=8.2; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # MiniMax Python Client
 
 [![PyPI version](https://img.shields.io/pypi/v/minimax-client.svg)](https://pypi.org/project/minimax-client/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
```

