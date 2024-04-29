# Comparing `tmp/openai_responses-0.2.0.tar.gz` & `tmp/openai_responses-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.2.0.tar", max compression
+gzip compressed data, was "openai_responses-0.2.1.tar", max compression
```

## Comparing `openai_responses-0.2.0.tar` & `openai_responses-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.2.0/LICENSE
--rw-r--r--   0        0        0     2466 2024-04-25 00:49:10.288971 openai_responses-0.2.0/README.md
--rw-r--r--   0        0        0     1204 2024-04-24 20:15:43.213841 openai_responses-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      914 2024-03-21 19:31:44.143224 openai_responses-0.2.0/src/openai_responses/__init__.py
--rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.2.0/src/openai_responses/decorators.py
--rw-r--r--   0        0        0     3897 2024-04-08 18:59:21.709797 openai_responses-0.2.0/src/openai_responses/endpoints/_base.py
--rw-r--r--   0        0        0     3645 2024-04-24 19:35:49.112709 openai_responses-0.2.0/src/openai_responses/endpoints/_partial_schemas.py
--rw-r--r--   0        0        0     8027 2024-04-24 19:35:49.113131 openai_responses-0.2.0/src/openai_responses/endpoints/assistants.py
--rw-r--r--   0        0        0     5513 2024-04-24 20:15:43.214166 openai_responses-0.2.0/src/openai_responses/endpoints/chat.py
--rw-r--r--   0        0        0     1877 2024-03-21 18:18:07.877059 openai_responses-0.2.0/src/openai_responses/endpoints/embeddings.py
--rw-r--r--   0        0        0     4393 2024-03-21 18:18:14.915452 openai_responses-0.2.0/src/openai_responses/endpoints/files.py
--rw-r--r--   0        0        0    33237 2024-04-24 20:11:09.681468 openai_responses-0.2.0/src/openai_responses/endpoints/threads.py
--rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.2.0/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.2.0/src/openai_responses/py.typed
--rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.2.0/src/openai_responses/state.py
--rw-r--r--   0        0        0      154 2024-04-24 20:15:43.214354 openai_responses-0.2.0/src/openai_responses/tokens.py
--rw-r--r--   0        0        0      740 2024-04-24 14:35:49.271898 openai_responses-0.2.0/src/openai_responses/utils.py
--rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 openai_responses-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3182 2024-04-29 14:18:24.992114 openai_responses-0.2.1/README.md
+-rw-r--r--   0        0        0     1204 2024-04-29 17:51:43.342527 openai_responses-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1031 2024-04-26 21:00:00.629710 openai_responses-0.2.1/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.2.1/src/openai_responses/decorators.py
+-rw-r--r--   0        0        0     5182 2024-04-26 20:03:26.180623 openai_responses-0.2.1/src/openai_responses/endpoints/_base.py
+-rw-r--r--   0        0        0     3645 2024-04-24 19:35:49.112709 openai_responses-0.2.1/src/openai_responses/endpoints/_partial_schemas.py
+-rw-r--r--   0        0        0     8405 2024-04-26 20:03:26.181090 openai_responses-0.2.1/src/openai_responses/endpoints/assistants.py
+-rw-r--r--   0        0        0     5561 2024-04-26 20:03:26.181494 openai_responses-0.2.1/src/openai_responses/endpoints/chat.py
+-rw-r--r--   0        0        0     2126 2024-04-26 21:00:00.629975 openai_responses-0.2.1/src/openai_responses/endpoints/embeddings.py
+-rw-r--r--   0        0        0     4726 2024-04-26 20:03:26.182119 openai_responses-0.2.1/src/openai_responses/endpoints/files.py
+-rw-r--r--   0        0        0     8962 2024-04-26 21:00:00.630246 openai_responses-0.2.1/src/openai_responses/endpoints/messages.py
+-rw-r--r--   0        0        0     6622 2024-04-26 21:00:00.630518 openai_responses-0.2.1/src/openai_responses/endpoints/run_steps.py
+-rw-r--r--   0        0        0    15709 2024-04-26 21:00:00.630654 openai_responses-0.2.1/src/openai_responses/endpoints/runs.py
+-rw-r--r--   0        0        0     5261 2024-04-26 21:00:00.630964 openai_responses-0.2.1/src/openai_responses/endpoints/threads.py
+-rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.2.1/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.2.1/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.2.1/src/openai_responses/state.py
+-rw-r--r--   0        0        0      154 2024-04-26 20:23:05.154688 openai_responses-0.2.1/src/openai_responses/tokens.py
+-rw-r--r--   0        0        0      740 2024-04-24 14:35:49.271898 openai_responses-0.2.1/src/openai_responses/utils.py
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 openai_responses-0.2.1/PKG-INFO
```

### Comparing `openai_responses-0.2.0/LICENSE` & `openai_responses-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.2.0/README.md` & `openai_responses-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# openai-responses
+# 🧪🤖 openai-responses
 
-[![PyPI version](https://badge.fury.io/py/openai-responses.svg)](https://badge.fury.io/py/openai-responses)
-[![PyPI - License](https://img.shields.io/pypi/l/openai-responses)](https://opensource.org/blog/license/mit)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openai-responses.svg)](https://pypi.org/project/openai-responses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/openai-responses)](https://pypi.org/project/openai-responses/)
-[![Open Issues](https://img.shields.io/github/issues/mharrisb1/openai-responses-python)](https://github.com/mharrisb1/openai-responses-python/issues)
-[![Stargazers](https://img.shields.io/github/stars/mharrisb1/openai-responses-python?style)](https://pypistats.org/packages/openai-responses)
+Pytest plugin for automatically mocking OpenAI requests. Built on top of [RESPX](https://github.com/lundberg/respx).
 
+## Supported endpoints
 
-Pytest plugin for automatically mocking OpenAI requests. Simply decorate any test function that contains code that calls an OpenAI endpoint (either using the SDK or HTTPX).
+- `/v1/chat/completions`
+- `/v1/embeddings`
+- `/v1/files`
+- `/v1/assistants`
+- `/v1/threads` (+ messages, runs, and steps)
 
-> [!IMPORTANT]
-> This project does not try to generate fake responses from the models. Any part of a response that would be generated by a model will need to be defined by the user or will fallback to a default value.
+View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/endpoints/).
+
+## Usage
+
+Simply decorate any test function that contains code that makes a call to an OpenAI endpoint. See [docs](https://mharrisb1.github.io/openai-responses-python) for more.
 
 ```python
 import openai_responses
 from openai import OpenAI
 
 
 @openai_responses.mock.chat.completions(
@@ -34,30 +37,44 @@
             {"role": "user", "content": "Hello!"},
         ],
         n=3,
     )
     assert len(completion.choices) == 3
 ```
 
+> [!IMPORTANT]
+> This project does not try to generate fake responses from the models. Any part of a response that would be generated by a model will need to be defined by the user or will fallback to a default value.
+
 ## Installation
 
+[![PyPI version](https://badge.fury.io/py/openai-responses.svg)](https://badge.fury.io/py/openai-responses)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openai-responses.svg)](https://pypi.org/project/openai-responses/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/openai-responses)](https://pypi.org/project/openai-responses/)
+
 Available on [PyPi](https://pypi.org/project/openai-responses/)
 
 ```bash
 pip install openai-responses
 ```
 
-## Usage
+## Documentation
+
+[![Docs](https://github.com/mharrisb1/openai-responses-python/actions/workflows/docs.yml/badge.svg)](https://mharrisb1.github.io/openai-responses-python)
 
 See the [documentation site](https://mharrisb1.github.io/openai-responses-python) for more info.
 
 ## License
 
+[![PyPI - License](https://img.shields.io/pypi/l/openai-responses)](https://opensource.org/blog/license/mit)
+
 See [LICENSE](https://github.com/mharrisb1/openai-responses-python/blob/main/LICENSE) for more info.
 
 ## Contributing
 
-See [CONTRIBUTING.md](https://github.com/mharrisb1/openai-responses-python/blob/main/CONTRIBUTING.md) for more info.
+[![Open Issues](https://img.shields.io/github/issues/mharrisb1/openai-responses-python)](https://github.com/mharrisb1/openai-responses-python/issues)
+[![Stargazers](https://img.shields.io/github/stars/mharrisb1/openai-responses-python?style)](https://pypistats.org/packages/openai-responses)
+
+See [CONTRIBUTING.md](https://github.com/mharrisb1/openai-responses-python/blob/main/CONTRIBUTING.md) for info on PRs, issues, and feature requests.
 
 ## Changelog
 
-See [CHANGELOG.md](https://github.com/mharrisb1/openai-responses-python/blob/main/CHANGELOG.md) for more info.
+See [CHANGELOG.md](https://github.com/mharrisb1/openai-responses-python/blob/main/CHANGELOG.md) for summarized notes on changes or view [releases](https://github.com/mharrisb1/openai-responses-python/releases) for more details information on changes.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openai_responses-0.2.0/pyproject.toml` & `openai_responses-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.2.0"
+version = "0.2.1"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://github.com/mharrisb1/openai-responses-python"
 packages = [{ include = "openai_responses", from = "src" }]
```

### Comparing `openai_responses-0.2.0/src/openai_responses/__init__.py` & `openai_responses-0.2.1/src/openai_responses/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from openai_responses.endpoints.assistants import AssistantsMock
 from openai_responses.endpoints.chat import ChatMock, ChatCompletionMock
 from openai_responses.endpoints.embeddings import EmbeddingsMock
 from openai_responses.endpoints.files import FilesMock
-from openai_responses.endpoints.threads import (
-    ThreadsMock,
-    MessagesMock,
-    RunsMock,
-    RunStepsMock,
-)
+from openai_responses.endpoints.threads import ThreadsMock
+from openai_responses.endpoints.messages import MessagesMock
+from openai_responses.endpoints.runs import RunsMock
+from openai_responses.endpoints.run_steps import RunStepsMock
 
 __all__ = [
     # main API
     "mock",
     # mockers
     "AssistantsMock",
     "ChatCompletionMock",
```

### Comparing `openai_responses-0.2.0/src/openai_responses/decorators.py` & `openai_responses-0.2.1/src/openai_responses/decorators.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.2.0/src/openai_responses/endpoints/_partial_schemas.py` & `openai_responses-0.2.1/src/openai_responses/endpoints/_partial_schemas.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.2.0/src/openai_responses/endpoints/assistants.py` & `openai_responses-0.2.1/src/openai_responses/endpoints/assistants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from functools import partial
 from typing import Any, Iterable, List, Optional
 
 import httpx
 import respx
 
 from openai.pagination import SyncCursorPage
 from openai.types.beta.assistant import Assistant, ToolResources
@@ -27,56 +26,73 @@
 from ..decorators import side_effect
 from ..state import StateStore
 from ..utils import model_dict, model_parse, utcnow_unix_timestamp_s, remove_none
 
 
 class AssistantsMock(StatefulMock):
     def __init__(self) -> None:
-        super().__init__()
-        self.url = self.BASE_URL + "/assistants"
+        super().__init__(
+            name="assistants_mock",
+            endpoint="/v1/assistants",
+            route_registrations=[
+                {
+                    "name": "create",
+                    "method": respx.post,
+                    "pattern": None,
+                    "side_effect": self._create,
+                },
+                {
+                    "name": "list",
+                    "method": respx.get,
+                    "pattern": None,
+                    "side_effect": self._list,
+                },
+                {
+                    "name": "retrieve",
+                    "method": respx.get,
+                    "pattern": r"/(?P<id>\w+)",
+                    "side_effect": self._retrieve,
+                },
+                {
+                    "name": "update",
+                    "method": respx.post,
+                    "pattern": r"/(?P<id>\w+)",
+                    "side_effect": self._update,
+                },
+                {
+                    "name": "delete",
+                    "method": respx.delete,
+                    "pattern": r"/(?P<id>\w+)",
+                    "side_effect": self._delete,
+                },
+            ],
+        )
+
+        # NOTE: these are explicitly defined to help with autocomplete and type hints
         self.create = CallContainer()
         self.list = CallContainer()
         self.retrieve = CallContainer()
         self.update = CallContainer()
         self.delete = CallContainer()
 
-    def _register_routes(self, **common: Any) -> None:
-        self.create.route = respx.post(url__regex=self.url).mock(
-            side_effect=partial(self._create, **common)
-        )
-        self.list.route = respx.get(url__regex=self.url).mock(
-            side_effect=partial(self._list, **common)
-        )
-        self.retrieve.route = respx.get(url__regex=self.url + r"/(?P<id>\w+)").mock(
-            side_effect=partial(self._retrieve, **common)
-        )
-        self.update.route = respx.post(url__regex=self.url + r"/(?P<id>\w+)").mock(
-            side_effect=partial(self._update, **common)
-        )
-        self.delete.route = respx.delete(url__regex=self.url + r"/(?P<id>\w+)").mock(
-            side_effect=partial(self._delete, **common)
-        )
-
     def __call__(
         self,
         *,
         latency: Optional[float] = None,
         failures: Optional[int] = None,
         state_store: Optional[StateStore] = None,
     ):
         def getter(*args: Any, **kwargs: Any):
             return dict(
                 latency=latency or 0,
                 failures=failures or 0,
                 state_store=kwargs["used_state"],
             )
 
-        return self._make_decorator(
-            "assistants_mock", getter, state_store or StateStore()
-        )
+        return self._make_decorator(getter, state_store or StateStore())
 
     @side_effect
     def _create(
         self,
         request: httpx.Request,
         route: respx.Route,
         state_store: StateStore,
```

### Comparing `openai_responses-0.2.0/src/openai_responses/endpoints/chat.py` & `openai_responses-0.2.1/src/openai_responses/endpoints/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from functools import partial
 from typing import Any, List, Literal, Optional, TypedDict
 
 import httpx
 import respx
 
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.completion_usage import CompletionUsage
@@ -52,22 +51,27 @@
         "function_call",
     ]
     message: PartialMessage
 
 
 class ChatCompletionMock(StatelessMock):
     def __init__(self) -> None:
-        super().__init__()
-        self.url = self.BASE_URL + "/chat/completions"
-        self.create = CallContainer()
-
-    def _register_routes(self, **common: Any) -> None:
-        self.create.route = respx.post(url__regex=self.url).mock(
-            side_effect=partial(self._create, **common)
+        super().__init__(
+            name="chat_completion_mock",
+            endpoint="/v1/chat/completions",
+            route_registrations=[
+                {
+                    "name": "create",
+                    "method": respx.post,
+                    "pattern": None,
+                    "side_effect": self._create,
+                }
+            ],
         )
+        self.create = CallContainer()
 
     def __call__(
         self,
         *,
         choices: Optional[List[PartialChoice]] = None,
         latency: Optional[float] = None,
         failures: Optional[int] = None,
@@ -75,15 +79,15 @@
         def getter(*args: Any, **kwargs: Any):
             return dict(
                 choices=choices or [],
                 latency=latency or 0,
                 failures=failures or 0,
             )
 
-        return self._make_decorator("chat_completion_mock", getter)
+        return self._make_decorator(getter)
 
     @side_effect
     def _create(
         self,
         request: httpx.Request,
         route: respx.Route,
         choices: List[PartialChoice],
@@ -125,15 +129,14 @@
             prompt_tokens=prompt_tokens,
             total_tokens=total_tokens,
         )
 
         return httpx.Response(status_code=201, json=model_dict(completion))
 
     def _choice_partial_to_model(self, i: int, p: PartialChoice) -> Choice:
-
         def fn_call_partial_to_model(p: Optional[PartialFunctionCall]):
             if p is None:
                 return None
             else:
                 return FunctionCall(
                     arguments=p.get("arguments", ""),
                     name=p.get("name", ""),
```

### Comparing `openai_responses-0.2.0/src/openai_responses/endpoints/embeddings.py` & `openai_responses-0.2.1/src/openai_responses/endpoints/embeddings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import json
-from functools import partial
 from typing import Any, List, Optional
 
 import httpx
 import respx
 
 from openai.types.embedding import Embedding
 from openai.types.embedding_create_params import EmbeddingCreateParams
 from openai.types.create_embedding_response import CreateEmbeddingResponse, Usage
 
 from ._base import StatelessMock, CallContainer
 from ..decorators import side_effect
+from ..tokens import count_tokens
 from ..utils import model_dict
 
 
 class EmbeddingsMock(StatelessMock):
     def __init__(self) -> None:
-        super().__init__()
-        self.url = self.BASE_URL + "/embeddings"
-        self.create = CallContainer()
-
-    def _register_routes(self, **common: Any) -> None:
-        self.create.route = respx.post(url__regex=self.url).mock(
-            side_effect=partial(self._create, **common)
+        super().__init__(
+            name="embeddings_mock",
+            endpoint="/v1/embeddings",
+            route_registrations=[
+                {
+                    "name": "create",
+                    "method": respx.post,
+                    "pattern": None,
+                    "side_effect": self._create,
+                }
+            ],
         )
+        self.create = CallContainer()
 
     def __call__(
         self,
         *,
         embedding: Optional[List[float]] = None,
         latency: Optional[float] = None,
         failures: Optional[int] = None,
@@ -35,29 +40,33 @@
         def getter(*args: Any, **kwargs: Any):
             return dict(
                 embedding=embedding or [],
                 latency=latency or 0,
                 failures=failures or 0,
             )
 
-        return self._make_decorator("embeddings_mock", getter)
+        return self._make_decorator(getter)
 
     @side_effect
     def _create(
         self,
         request: httpx.Request,
         route: respx.Route,
         embedding: List[float],
         **kwargs: Any,
     ) -> httpx.Response:
         self.create.route = route
 
         content: EmbeddingCreateParams = json.loads(request.content)
 
+        token_count = 0
+        if isinstance(content["input"], str):
+            token_count = count_tokens(content["model"], content["input"])
+
         embeddings = CreateEmbeddingResponse(
             data=[Embedding(embedding=embedding, index=0, object="embedding")],
             model=content["model"],
             object="list",
-            usage=Usage(prompt_tokens=0, total_tokens=0),
+            usage=Usage(prompt_tokens=token_count, total_tokens=token_count),
         )
 
         return httpx.Response(status_code=201, json=model_dict(embeddings))
```

### Comparing `openai_responses-0.2.0/src/openai_responses/endpoints/files.py` & `openai_responses-0.2.1/src/openai_responses/endpoints/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from functools import partial
 from typing import Any, Optional
 
 import httpx
 import respx
 
 from openai.pagination import SyncPage
 from openai.types.file_object import FileObject
@@ -13,53 +12,66 @@
 from ..decorators import side_effect
 from ..state import StateStore
 from ..utils import model_dict, utcnow_unix_timestamp_s
 
 
 class FilesMock(StatefulMock):
     def __init__(self) -> None:
-        super().__init__()
-        self.url = self.BASE_URL + "/files"
+        super().__init__(
+            name="files_mock",
+            endpoint="/v1/files",
+            route_registrations=[
+                {
+                    "name": "create",
+                    "method": respx.post,
+                    "pattern": None,
+                    "side_effect": self._create,
+                },
+                {
+                    "name": "list",
+                    "method": respx.get,
+                    "pattern": None,
+                    "side_effect": self._list,
+                },
+                {
+                    "name": "retrieve",
+                    "method": respx.get,
+                    "pattern": r"/(?P<id>\w+)",
+                    "side_effect": self._retrieve,
+                },
+                {
+                    "name": "delete",
+                    "method": respx.delete,
+                    "pattern": r"/(?P<id>\w+)",
+                    "side_effect": self._delete,
+                },
+            ],
+        )
+
+        # NOTE: these are explicitly defined to help with autocomplete and type hints
         self.create = CallContainer()
         self.list = CallContainer()
         self.retrieve = CallContainer()
         self.delete = CallContainer()
 
-    def _register_routes(self, **common: Any) -> None:
-        self.create.route = respx.post(url__regex=self.url).mock(
-            side_effect=partial(self._create, **common)
-        )
-
-        self.list.route = respx.get(url__regex=self.url).mock(
-            side_effect=partial(self._list, **common)
-        )
-
-        self.retrieve.route = respx.get(url__regex=self.url + r"/(?P<id>\w+)").mock(
-            side_effect=partial(self._retrieve, **common)
-        )
-
-        self.delete.route = respx.delete(url__regex=self.url + r"/(?P<id>\w+)").mock(
-            side_effect=partial(self._delete, **common)
-        )
-
     def __call__(
         self,
         *,
         latency: Optional[float] = None,
         failures: Optional[int] = None,
         state_store: Optional[StateStore] = None,
     ):
         def getter(*args: Any, **kwargs: Any):
             return dict(
                 latency=latency or 0,
                 failures=failures or 0,
                 state_store=kwargs["used_state"],
             )
 
-        return self._make_decorator("files_mock", getter, state_store or StateStore())
+        return self._make_decorator(getter, state_store or StateStore())
 
     @side_effect
     def _create(
         self,
         request: httpx.Request,
         route: respx.Route,
         state_store: StateStore,
```

### Comparing `openai_responses-0.2.0/src/openai_responses/plugin.py` & `openai_responses-0.2.1/src/openai_responses/plugin.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.2.0/src/openai_responses/state.py` & `openai_responses-0.2.1/src/openai_responses/state.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.2.0/src/openai_responses/utils.py` & `openai_responses-0.2.1/src/openai_responses/utils.py`

 * *Files identical despite different names*

