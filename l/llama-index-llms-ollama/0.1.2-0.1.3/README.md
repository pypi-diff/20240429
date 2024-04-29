# Comparing `tmp/llama_index_llms_ollama-0.1.2.tar.gz` & `tmp/llama_index_llms_ollama-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ollama-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_llms_ollama-0.1.3.tar", max compression
```

## Comparing `llama_index_llms_ollama-0.1.2.tar` & `llama_index_llms_ollama-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       38 2024-02-13 13:53:01.677850 llama_index_llms_ollama-0.1.2/README.md
--rw-r--r--   0        0        0       70 2024-02-13 13:53:01.678067 llama_index_llms_ollama-0.1.2/llama_index/llms/ollama/__init__.py
--rw-r--r--   0        0        0     7642 2024-02-13 13:53:01.678147 llama_index_llms_ollama-0.1.2/llama_index/llms/ollama/base.py
--rw-r--r--   0        0        0     1421 2024-02-21 17:54:19.416562 llama_index_llms_ollama-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 llama_index_llms_ollama-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/README.md
+-rw-r--r--   0        0        0       70 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/llama_index/llms/ollama/__init__.py
+-rw-r--r--   0        0        0    13809 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/llama_index/llms/ollama/base.py
+-rw-r--r--   0        0        0     1421 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 llama_index_llms_ollama-0.1.3/PKG-INFO
```

### Comparing `llama_index_llms_ollama-0.1.2/llama_index/llms/ollama/base.py` & `llama_index_llms_ollama-0.1.3/llama_index/llms/ollama/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,34 +3,57 @@
 
 import httpx
 from httpx import Timeout
 from llama_index.core.base.llms.types import (
     ChatMessage,
     ChatResponse,
     ChatResponseGen,
+    ChatResponseAsyncGen,
     CompletionResponse,
+    CompletionResponseAsyncGen,
     CompletionResponseGen,
     LLMMetadata,
     MessageRole,
 )
 from llama_index.core.bridge.pydantic import Field
 from llama_index.core.constants import DEFAULT_CONTEXT_WINDOW, DEFAULT_NUM_OUTPUTS
 from llama_index.core.llms.callbacks import llm_chat_callback, llm_completion_callback
 from llama_index.core.llms.custom import CustomLLM
 
 DEFAULT_REQUEST_TIMEOUT = 30.0
 
 
-def get_addtional_kwargs(
+def get_additional_kwargs(
     response: Dict[str, Any], exclude: Tuple[str, ...]
 ) -> Dict[str, Any]:
     return {k: v for k, v in response.items() if k not in exclude}
 
 
 class Ollama(CustomLLM):
+    """Ollama LLM.
+
+    Visit https://ollama.com/ to download and install Ollama.
+
+    Run `ollama serve` to start a server.
+
+    Run `ollama pull <name>` to download a model to run.
+
+    Examples:
+        `pip install llama-index-llms-ollama`
+
+        ```python
+        from llama_index.llms.ollama import Ollama
+
+        llm = Ollama(model="llama2", request_timeout=60.0)
+
+        response = llm.complete("What is the capital of France?")
+        print(response)
+        ```
+    """
+
     base_url: str = Field(
         default="http://localhost:11434",
         description="Base url the model is hosted under.",
     )
     model: str = Field(description="The Ollama model to use.")
     temperature: float = Field(
         default=0.75,
@@ -46,14 +69,18 @@
     request_timeout: float = Field(
         default=DEFAULT_REQUEST_TIMEOUT,
         description="The timeout for making http request to Ollama API server",
     )
     prompt_key: str = Field(
         default="prompt", description="The key to use for the prompt in API calls."
     )
+    json_mode: bool = Field(
+        default=False,
+        description="Whether to use JSON mode for the Ollama API.",
+    )
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict,
         description="Additional model parameters for the Ollama API.",
     )
 
     @classmethod
     def class_name(cls) -> str:
@@ -93,32 +120,77 @@
                 for message in messages
             ],
             "options": self._model_kwargs,
             "stream": False,
             **kwargs,
         }
 
+        if self.json_mode:
+            payload["format"] = "json"
+
         with httpx.Client(timeout=Timeout(self.request_timeout)) as client:
             response = client.post(
                 url=f"{self.base_url}/api/chat",
                 json=payload,
             )
             response.raise_for_status()
             raw = response.json()
             message = raw["message"]
             return ChatResponse(
                 message=ChatMessage(
                     content=message.get("content"),
                     role=MessageRole(message.get("role")),
-                    additional_kwargs=get_addtional_kwargs(
+                    additional_kwargs=get_additional_kwargs(
+                        message, ("content", "role")
+                    ),
+                ),
+                raw=raw,
+                additional_kwargs=get_additional_kwargs(raw, ("message",)),
+            )
+
+    @llm_chat_callback()
+    async def achat(
+        self, messages: Sequence[ChatMessage], **kwargs: Any
+    ) -> ChatResponse:
+        payload = {
+            "model": self.model,
+            "messages": [
+                {
+                    "role": message.role.value,
+                    "content": message.content,
+                    **message.additional_kwargs,
+                }
+                for message in messages
+            ],
+            "options": self._model_kwargs,
+            "stream": False,
+            **kwargs,
+        }
+
+        if self.json_mode:
+            payload["format"] = "json"
+
+        async with httpx.AsyncClient(timeout=Timeout(self.request_timeout)) as client:
+            response = await client.post(
+                url=f"{self.base_url}/api/chat",
+                json=payload,
+            )
+            response.raise_for_status()
+            raw = response.json()
+            message = raw["message"]
+            return ChatResponse(
+                message=ChatMessage(
+                    content=message.get("content"),
+                    role=MessageRole(message.get("role")),
+                    additional_kwargs=get_additional_kwargs(
                         message, ("content", "role")
                     ),
                 ),
                 raw=raw,
-                additional_kwargs=get_addtional_kwargs(raw, ("message",)),
+                additional_kwargs=get_additional_kwargs(raw, ("message",)),
             )
 
     @llm_chat_callback()
     def stream_chat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponseGen:
         payload = {
@@ -132,14 +204,17 @@
                 for message in messages
             ],
             "options": self._model_kwargs,
             "stream": True,
             **kwargs,
         }
 
+        if self.json_mode:
+            payload["format"] = "json"
+
         with httpx.Client(timeout=Timeout(self.request_timeout)) as client:
             with client.stream(
                 method="POST",
                 url=f"{self.base_url}/api/chat",
                 json=payload,
             ) as response:
                 response.raise_for_status()
@@ -152,61 +227,140 @@
                         message = chunk["message"]
                         delta = message.get("content")
                         text += delta
                         yield ChatResponse(
                             message=ChatMessage(
                                 content=text,
                                 role=MessageRole(message.get("role")),
-                                additional_kwargs=get_addtional_kwargs(
+                                additional_kwargs=get_additional_kwargs(
                                     message, ("content", "role")
                                 ),
                             ),
                             delta=delta,
                             raw=chunk,
-                            additional_kwargs=get_addtional_kwargs(chunk, ("message",)),
+                            additional_kwargs=get_additional_kwargs(
+                                chunk, ("message",)
+                            ),
                         )
 
+    @llm_chat_callback()
+    async def achat(
+        self, messages: Sequence[ChatMessage], **kwargs: Any
+    ) -> ChatResponseAsyncGen:
+        payload = {
+            "model": self.model,
+            "messages": [
+                {
+                    "role": message.role.value,
+                    "content": message.content,
+                    **message.additional_kwargs,
+                }
+                for message in messages
+            ],
+            "options": self._model_kwargs,
+            "stream": False,
+            **kwargs,
+        }
+
+        if self.json_mode:
+            payload["format"] = "json"
+
+        async with httpx.AsyncClient(timeout=Timeout(self.request_timeout)) as client:
+            response = await client.post(
+                url=f"{self.base_url}/api/chat",
+                json=payload,
+            )
+            response.raise_for_status()
+            raw = response.json()
+            message = raw["message"]
+            return ChatResponse(
+                message=ChatMessage(
+                    content=message.get("content"),
+                    role=MessageRole(message.get("role")),
+                    additional_kwargs=get_additional_kwargs(
+                        message, ("content", "role")
+                    ),
+                ),
+                raw=raw,
+                additional_kwargs=get_additional_kwargs(raw, ("message",)),
+            )
+
     @llm_completion_callback()
     def complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponse:
         payload = {
             self.prompt_key: prompt,
             "model": self.model,
             "options": self._model_kwargs,
             "stream": False,
             **kwargs,
         }
 
+        if self.json_mode:
+            payload["format"] = "json"
+
         with httpx.Client(timeout=Timeout(self.request_timeout)) as client:
             response = client.post(
                 url=f"{self.base_url}/api/generate",
                 json=payload,
             )
             response.raise_for_status()
             raw = response.json()
             text = raw.get("response")
             return CompletionResponse(
                 text=text,
                 raw=raw,
-                additional_kwargs=get_addtional_kwargs(raw, ("response",)),
+                additional_kwargs=get_additional_kwargs(raw, ("response",)),
+            )
+
+    @llm_completion_callback()
+    async def acomplete(
+        self, prompt: str, formatted: bool = False, **kwargs: Any
+    ) -> CompletionResponse:
+        payload = {
+            self.prompt_key: prompt,
+            "model": self.model,
+            "options": self._model_kwargs,
+            "stream": False,
+            **kwargs,
+        }
+
+        if self.json_mode:
+            payload["format"] = "json"
+
+        async with httpx.AsyncClient(timeout=Timeout(self.request_timeout)) as client:
+            response = await client.post(
+                url=f"{self.base_url}/api/generate",
+                json=payload,
+            )
+            response.raise_for_status()
+            raw = response.json()
+            text = raw.get("response")
+            return CompletionResponse(
+                text=text,
+                raw=raw,
+                additional_kwargs=get_additional_kwargs(raw, ("response",)),
             )
 
     @llm_completion_callback()
     def stream_complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponseGen:
         payload = {
             self.prompt_key: prompt,
             "model": self.model,
             "options": self._model_kwargs,
             "stream": True,
             **kwargs,
         }
 
+        if self.json_mode:
+            payload["format"] = "json"
+
         with httpx.Client(timeout=Timeout(self.request_timeout)) as client:
             with client.stream(
                 method="POST",
                 url=f"{self.base_url}/api/generate",
                 json=payload,
             ) as response:
                 response.raise_for_status()
@@ -216,11 +370,50 @@
                         chunk = json.loads(line)
                         delta = chunk.get("response")
                         text += delta
                         yield CompletionResponse(
                             delta=delta,
                             text=text,
                             raw=chunk,
-                            additional_kwargs=get_addtional_kwargs(
+                            additional_kwargs=get_additional_kwargs(
                                 chunk, ("response",)
                             ),
                         )
+
+    @llm_completion_callback()
+    async def astream_complete(
+        self, prompt: str, formatted: bool = False, **kwargs: Any
+    ) -> CompletionResponseAsyncGen:
+        payload = {
+            self.prompt_key: prompt,
+            "model": self.model,
+            "options": self._model_kwargs,
+            "stream": True,
+            **kwargs,
+        }
+
+        if self.json_mode:
+            payload["format"] = "json"
+
+        async def gen() -> CompletionResponseAsyncGen:
+            async with httpx.AsyncClient(
+                timeout=Timeout(self.request_timeout)
+            ) as client:
+                async with client.stream(
+                    method="POST",
+                    url=f"{self.base_url}/api/generate",
+                    json=payload,
+                ) as response:
+                    async for line in response.aiter_text():
+                        if line:
+                            chunk = json.loads(line)
+                            delta = chunk.get("response")
+                            yield CompletionResponse(
+                                delta=delta,
+                                text=delta,
+                                raw=chunk,
+                                additional_kwargs=get_additional_kwargs(
+                                    chunk, ("response",)
+                                ),
+                            )
+
+        return gen()
```

### Comparing `llama_index_llms_ollama-0.1.2/pyproject.toml` & `llama_index_llms_ollama-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ollama integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-ollama"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

