# Comparing `tmp/mllm-0.1.3.tar.gz` & `tmp/mllm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllm-0.1.3.tar", max compression
+gzip compressed data, was "mllm-0.1.4.tar", max compression
```

## Comparing `mllm-0.1.3.tar` & `mllm-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.3/LICENSE
--rw-r--r--   0        0        0     2229 2024-04-27 17:12:21.883444 mllm-0.1.3/README.md
--rw-r--r--   0        0        0      154 2024-04-27 16:19:02.141169 mllm-0.1.3/mllm/__init__.py
--rw-r--r--   0        0        0     1983 2024-04-27 16:19:02.141340 mllm-0.1.3/mllm/db/conn.py
--rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.3/mllm/db/models.py
--rw-r--r--   0        0        0      852 2024-04-27 16:19:02.141546 mllm-0.1.3/mllm/models.py
--rw-r--r--   0        0        0     5661 2024-04-27 16:19:02.141676 mllm-0.1.3/mllm/prompt.py
--rw-r--r--   0        0        0     8212 2024-04-27 17:00:35.726193 mllm-0.1.3/mllm/router.py
--rw-r--r--   0        0        0      793 2024-04-27 16:19:02.141946 mllm-0.1.3/mllm/util.py
--rw-r--r--   0        0        0      390 2024-04-27 17:17:56.319107 mllm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 mllm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.4/README.md
+-rw-r--r--   0        0        0      154 2024-04-27 21:30:57.109430 mllm-0.1.4/mllm/__init__.py
+-rw-r--r--   0        0        0     1981 2024-04-27 22:13:37.479726 mllm-0.1.4/mllm/db/conn.py
+-rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.4/mllm/db/models.py
+-rw-r--r--   0        0        0      866 2024-04-27 21:28:03.888370 mllm-0.1.4/mllm/models.py
+-rw-r--r--   0        0        0     5625 2024-04-27 21:29:28.486764 mllm-0.1.4/mllm/prompt.py
+-rw-r--r--   0        0        0     8327 2024-04-27 21:28:31.215289 mllm-0.1.4/mllm/router.py
+-rw-r--r--   0        0        0      793 2024-04-27 21:31:01.883780 mllm-0.1.4/mllm/util.py
+-rw-r--r--   0        0        0      390 2024-04-29 21:12:15.343851 mllm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.4/PKG-INFO
```

### Comparing `mllm-0.1.3/LICENSE` & `mllm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mllm-0.1.3/README.md` & `mllm-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 ## Usage
 
 Create an MLLM router with a list of preferred models
 
 ```python
 import os
-from mllm import MLLMRouter
+from mllm import Router
 
 os.environ["OPENAI_API_KEY"] = "..."
 os.environ["ANTHROPIC_API_KEY"] = "..."
 os.environ["GEMINI_API_KEY"] = "..."
 
-router = MLLMRouter(
+router = Router(
     preference=["gpt-4-turbo", "anthropic/claude-3-opus-20240229", "gemini/gemini-pro-vision"]
 )
 ```
 
 Create a new role based chat thread
 
 ```python
```

### Comparing `mllm-0.1.3/mllm/db/conn.py` & `mllm-0.1.4/mllm/db/conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 DB_TYPE = os.environ.get("DB_TYPE", "sqlite")
 
 
 def get_pg_conn() -> Engine:
     # Helper function to get environment variable with fallback
     def get_env_var(key: str) -> str:
-        task_key = f"PROMPT_{key}"
+        task_key = f"MLLM_{key}"
         value = os.environ.get(task_key)
         if value is None:
             value = os.environ.get(key)
             if value is None:
                 raise ValueError(f"${key} must be set")
         return value
```

### Comparing `mllm-0.1.3/mllm/db/models.py` & `mllm-0.1.4/mllm/db/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.3/mllm/models.py` & `mllm-0.1.4/mllm/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import Optional, Dict, Any, List
 
 from pydantic import BaseModel
 from threadmem.server.models import RoleThreadModel, RoleMessageModel
 
 
-class PromptModel(BaseModel):
+class V1PromptModel(BaseModel):
     """An LLM prompt model"""
 
     id: Optional[str] = None
     thread: RoleThreadModel
     response: RoleMessageModel
     namespace: str = "default"
     metadata: Dict[str, Any] = {}
     created: Optional[float] = None
     approved: bool = False
     flagged: bool = False
 
 
-class EnvVarOptModel(BaseModel):
+class V1EnvVarOptModel(BaseModel):
     name: str
     description: Optional[str] = None
     required: bool = False
     default: Optional[str] = None
     secret: bool = False
     options: List[str] = []
 
 
-class MLLMProviders(BaseModel):
+class V1MLLMProviders(BaseModel):
     preference: List[str] = []
 
 
-class MLLMOption(BaseModel):
+class V1MLLMOption(BaseModel):
     model: str
-    env_var: EnvVarOptModel
+    env_var: V1EnvVarOptModel
 
 
-class MLLMModel(BaseModel):
-    options: List[MLLMOption]
+class V1MLLMModel(BaseModel):
+    options: List[V1MLLMOption]
```

### Comparing `mllm-0.1.3/mllm/prompt.py` & `mllm-0.1.4/mllm/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, Any, List, Optional
 
 from threadmem import RoleThread, RoleMessage
 from threadmem.server.models import RoleMessageModel, RoleThreadModel
 
 from .db.models import PromptRecord
 from .db.conn import WithDB
-from .models import PromptModel
+from .models import V1PromptModel
 
 logger = logging.getLogger(__name__)
 
 
 class Prompt(WithDB):
     """An LLM prompt"""
 
@@ -140,38 +140,38 @@
         obj._metadata = metadata
         obj._created = record.created
         obj._approved = record.approved
         obj._flagged = record.flagged
 
         return obj
 
-    def to_schema(self) -> PromptModel:
-        return PromptModel(
+    def to_v1(self) -> V1PromptModel:
+        return V1PromptModel(
             id=self._id,
             namespace=self._namespace,
             thread=self._thread.to_schema(),
             response=self._response.to_schema(),
             metadata=self._metadata,
             created=self._created,
             approved=self._approved,
             flagged=self._flagged,
         )
 
     @classmethod
-    def from_schema(cls, schema: PromptModel) -> "Prompt":
+    def from_v1(cls, v1: V1PromptModel) -> "Prompt":
         obj = cls.__new__(cls)
 
-        obj._id = schema.id
-        obj._namespace = schema.namespace
-        obj._thread = RoleThread.from_schema(schema.thread)
-        obj._response = RoleMessage.from_schema(schema.response)
-        obj._metadata = schema.metadata
-        obj._created = schema.created
-        obj._approved = schema.approved
-        obj._flagged = schema.flagged
+        obj._id = v1.id
+        obj._namespace = v1.namespace
+        obj._thread = RoleThread.from_schema(v1.thread)
+        obj._response = RoleMessage.from_schema(v1.response)
+        obj._metadata = v1.metadata
+        obj._created = v1.created
+        obj._approved = v1.approved
+        obj._flagged = v1.flagged
 
         return obj
 
     @classmethod
     def find(cls, **kwargs) -> List["Prompt"]:
         for db in cls.get_db():
             records = (
```

### Comparing `mllm-0.1.3/mllm/router.py` & `mllm-0.1.4/mllm/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import logging
 from typing import Optional, List, Dict, TypeVar, Type, Generic
 import time
 
-from litellm import Router, ModelResponse
+from litellm import Router as LLMRouter, ModelResponse
 from threadmem import RoleThread, RoleMessage
 from litellm._logging import handler
 from pydantic import BaseModel
 from tenacity import retry, stop_after_attempt
 
-from .models import EnvVarOptModel, MLLMModel, MLLMOption
+from .models import V1EnvVarOptModel, V1MLLMModel, V1MLLMOption
 from .util import extract_parse_json
 from .prompt import Prompt
 
 
 T = TypeVar("T", bound=BaseModel)
 
 
@@ -23,38 +23,41 @@
     parsed: Optional[T] = None
     time_elapsed: float
     tokens_request: int
     tokens_response: int
     prompt_id: str
 
 
-class MLLMRouter:
+class Router:
     """
     A multimodal chat provider
     """
 
     provider_api_keys: Dict[str, str] = {
         "gpt-4-turbo": "OPENAI_API_KEY",
         "anthropic/claude-3-opus-20240229": "ANTHROPIC_API_KEY",
         "gemini/gemini-pro-vision": "GEMINI_API_KEY",
     }
 
     def __init__(
         self,
-        preference: List[str],
+        preference: List[str] | str,
         timeout: int = 30,
         allow_fails: int = 1,
         num_retries: int = 3,
     ) -> None:
         self.model_list = []
         fallbacks = []
 
         if len(preference) == 0:
             raise Exception("No chat providers specified.")
 
+        if isinstance(preference, str):
+            preference = [preference]
+
         self.model = preference[0]
 
         # Construct the model list based on provided preferences and available API keys
         for provider in preference:
             api_key_env = self.provider_api_keys.get(provider)
             if api_key_env:
                 api_key = os.getenv(api_key_env)
@@ -80,15 +83,15 @@
                     {
                         model["model_name"]: [
                             fallback["model_name"] for fallback in fallback_models
                         ]
                     }
                 )
 
-        self.router = Router(
+        self.router = LLMRouter(
             model_list=self.model_list,
             timeout=timeout,
             allowed_fails=allow_fails,
             num_retries=num_retries,
             set_verbose=False,
             debug_level="INFO",
             fallbacks=fallbacks,
@@ -97,21 +100,21 @@
         verbose_router_logger = logging.getLogger("LiteLLM Router")
         verbose_router_logger.setLevel(logging.ERROR)
         verbose_logger = logging.getLogger("LiteLLM")
         verbose_logger.setLevel(logging.ERROR)
         handler.setLevel(logging.ERROR)
 
     @classmethod
-    def all_opts(cls) -> List[MLLMOption]:
+    def all_opts(cls) -> List[V1MLLMOption]:
         out = []
         for model, key in cls.provider_api_keys.items():
             out.append(
-                MLLMOption(
+                V1MLLMOption(
                     model=model,
-                    env_var=EnvVarOptModel(
+                    env_var=V1EnvVarOptModel(
                         name=key,
                         description=f"{model} API key",
                         required=True,
                         secret=True,
                     ),
                 )
             )
@@ -195,24 +198,24 @@
         thread = RoleThread()
         thread.post(
             "user", "Just checking if you are working... please return 'yes' if you are"
         )
         response = self.chat(thread)
         print("response from checking oai functionality: ", response)
 
-    def options(self) -> List[MLLMOption]:
+    def options(self) -> List[V1MLLMOption]:
         """Dynamically generates options based on the configured providers."""
         options = []
         for model_info in self.model_list:
             model_name = model_info["model_name"]
             api_key_env = self.provider_api_keys.get(model_name)
             if api_key_env:
-                option = MLLMOption(
+                option = V1MLLMOption(
                     model=model_name,
-                    env_var=EnvVarOptModel(
+                    env_var=V1EnvVarOptModel(
                         name=api_key_env,
                         description=f"{model_name} API key",
                         required=True,
                         secret=True,
                     ),
                 )
                 options.append(option)
```

### Comparing `mllm-0.1.3/mllm/util.py` & `mllm-0.1.4/mllm/util.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.3/PKG-INFO` & `mllm-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Multimodal Large Language Models
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -27,21 +27,21 @@
 
 ## Usage
 
 Create an MLLM router with a list of preferred models
 
 ```python
 import os
-from mllm import MLLMRouter
+from mllm import Router
 
 os.environ["OPENAI_API_KEY"] = "..."
 os.environ["ANTHROPIC_API_KEY"] = "..."
 os.environ["GEMINI_API_KEY"] = "..."
 
-router = MLLMRouter(
+router = Router(
     preference=["gpt-4-turbo", "anthropic/claude-3-opus-20240229", "gemini/gemini-pro-vision"]
 )
 ```
 
 Create a new role based chat thread
 
 ```python
```

