# Comparing `tmp/cntrlai-0.0.32.tar.gz` & `tmp/cntrlai-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cntrlai-0.0.32.tar", max compression
+gzip compressed data, was "cntrlai-0.0.33.tar", max compression
```

## Comparing `cntrlai-0.0.32.tar` & `cntrlai-0.0.33.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        6 2024-04-27 00:39:09.943029 cntrlai-0.0.32/README.md
--rw-r--r--   0        0        0      261 2024-04-27 05:08:57.442118 cntrlai-0.0.32/cntrlai/__init__.py
--rw-r--r--   0        0        0     7547 2024-04-27 05:08:50.953931 cntrlai-0.0.32/cntrlai/batch_evaluation.py
--rw-r--r--   0        0        0     3375 2024-04-27 05:22:11.564695 cntrlai-0.0.32/cntrlai/guardrails.py
--rw-r--r--   0        0        0    11019 2024-04-27 05:22:24.429837 cntrlai-0.0.32/cntrlai/langchain.py
--rw-r--r--   0        0        0     7824 2024-04-27 05:22:54.195820 cntrlai-0.0.32/cntrlai/logger.py
--rw-r--r--   0        0        0    18404 2024-04-27 05:23:13.506374 cntrlai-0.0.32/cntrlai/openai.py
--rw-r--r--   0        0        0     3566 2024-04-26 20:53:47.801336 cntrlai-0.0.32/cntrlai/types.py
--rw-r--r--   0        0        0     2698 2024-04-27 05:23:28.628931 cntrlai-0.0.32/cntrlai/utils.py
--rw-r--r--   0        0        0     1513 2024-04-27 05:29:22.636307 cntrlai-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 cntrlai-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0        6 2024-04-27 00:39:09.943029 cntrlai-0.0.33/README.md
+-rw-r--r--   0        0        0      284 2024-04-29 00:59:20.632041 cntrlai-0.0.33/cntrlai/__init__.py
+-rw-r--r--   0        0        0     7579 2024-04-29 00:59:54.678362 cntrlai-0.0.33/cntrlai/batch_evaluation.py
+-rw-r--r--   0        0        0     3401 2024-04-29 01:00:28.289059 cntrlai-0.0.33/cntrlai/guardrails.py
+-rw-r--r--   0        0        0    11044 2024-04-29 01:04:56.414065 cntrlai-0.0.33/cntrlai/langchain.py
+-rw-r--r--   0        0        0     8710 2024-04-29 05:35:40.848340 cntrlai-0.0.33/cntrlai/logger.py
+-rw-r--r--   0        0        0    20766 2024-04-29 05:35:35.729115 cntrlai-0.0.33/cntrlai/openai.py
+-rw-r--r--   0        0        0     3588 2024-04-29 01:05:54.216065 cntrlai-0.0.33/cntrlai/types.py
+-rw-r--r--   0        0        0     2720 2024-04-29 01:06:09.308725 cntrlai-0.0.33/cntrlai/utils.py
+-rw-r--r--   0        0        0     1477 2024-04-29 05:46:37.581213 cntrlai-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 cntrlai-0.0.33/PKG-INFO
```

### Comparing `cntrlai-0.0.32/cntrlai/batch_evaluation.py` & `cntrlai-0.0.33/cntrlai/batch_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+### cntrlai/batch_evaluation.py
 import asyncio
 from concurrent.futures import Future, ThreadPoolExecutor, as_completed
 from typing import (
     Any,
     Callable,
     Coroutine,
     List,
```

### Comparing `cntrlai-0.0.32/cntrlai/guardrails.py` & `cntrlai-0.0.33/cntrlai/guardrails.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+### cntrlai/guardrails.py
 from typing import List, Literal, Optional, Union, cast
 from warnings import warn
 
 import httpx
 from pydantic import BaseModel
 
 import cntrlai
```

### Comparing `cntrlai-0.0.32/cntrlai/langchain.py` & `cntrlai-0.0.33/cntrlai/langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+### cntrlai/langchain.py
 import json
 from typing import Any, Dict, List, Literal, Optional, Union, cast
 from langchain.schema import (
     LLMResult,
     AgentAction,
     AgentFinish,
     BaseMessage,
```

### Comparing `cntrlai-0.0.32/cntrlai/logger.py` & `cntrlai-0.0.33/cntrlai/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     autoconvert_typed_values,
     capture_exception,
     milliseconds_timestamp,
 )
 from retry import retry
 
 import cntrlai
+import logging
+
+logger = logging.getLogger("chainlit")
 
 T = TypeVar("T")
 
 _local_context = threading.local()
 
 
 class ContextSpan:
@@ -251,26 +254,45 @@
             ):
                 span["timestamps"]["finished_at"] = milliseconds_timestamp()
 
 
 @retry(tries=5, delay=0.5, backoff=3)
 def send_spans(data: CollectorRESTParams):
     if len(data["spans"]) == 0:
+        logger.info("No spans to send")
         return
+
     if not cntrlai.api_key:
         warn(
             "CONTROLAI_API_KEY is not set, LLMs traces will not be sent, go to https://app.controlai.org to set it up"
         )
+        logger.info("CONTROLAI_API_KEY is not set, traces will not be sent")
         return
-    response = requests.post(
-        cntrlai.endpoint + "/api/analytics",
-        json=data,
-        headers={"X-Auth-Token": str(cntrlai.api_key)},
-    )
-    if response.status_code == 429:
-        json = response.json()
-        if "message" in json and "ERR_PLAN_LIMIT" in json["message"]:
-            warn(json["message"])
+
+    logger.info(f"Sending spans data: {data}")
+
+    try:
+        # Log the API endpoint and API key
+        logger.info(f"Sending request to API endpoint: {cntrlai.endpoint + '/api/analytics'}")
+        logger.info(f"Using API key: {cntrlai.api_key}")
+
+        response = requests.post(
+            cntrlai.endpoint + "/api/analytics",
+            json=data,
+            headers={"x-api-key": str(cntrlai.api_key)},
+        )
+        logger.info(f"API response status code: {response.status_code}")
+        logger.info(f"API response content: {response.text}")
+
+        if response.status_code == 429:
+            json = response.json()
+            if "message" in json and "ERR_PLAN_LIMIT" in json["message"]:
+                warn(json["message"])
+                logger.info(f"Plan limit exceeded: {json['message']}")
+            else:
+                warn("Rate limit exceeded, dropping message from being sent to LangWatch")
+                logger.info("Rate limit exceeded, dropping message")
         else:
-            warn("Rate limit exceeded, dropping message from being sent to LangWatch")
-    else:
-        response.raise_for_status()
+            response.raise_for_status()
+    except requests.exceptions.RequestException as e:
+        logger.info("Error sending spans to the API", exc_info=e)
+        raise
```

### Comparing `cntrlai-0.0.32/cntrlai/openai.py` & `cntrlai-0.0.33/cntrlai/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # cntrlai/openai.py
 
+import logging
 from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Union, cast
 
 import nanoid
 from cntrlai.logger import BaseContextTracer
 
 from cntrlai.types import (
     ChatMessage,
@@ -33,14 +34,15 @@
     AzureOpenAI,
     AsyncAzureOpenAI,
 )
 
 from openai.types import Completion
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
+logger = logging.getLogger("chainlit")
 
 class OpenAITracer(BaseContextTracer):
     """
     Tracing for both Completion and ChatCompletion endpoints
     """
 
     def __init__(
@@ -61,19 +63,21 @@
             instance=instance, trace_id=trace_id, metadata=metadata
         )
 
     def __enter__(self):
         super().__enter__()
         self.completion_tracer.__enter__()
         self.chat_completion_tracer.__enter__()
+        logger.info("Entered OpenAITracer")
 
     def __exit__(self, _type, _value, _traceback):
         super().__exit__(_type, _value, _traceback)
         self.completion_tracer.__exit__(_type, _value, _traceback)
         self.chat_completion_tracer.__exit__(_type, _value, _traceback)
+        logger.info("Exited OpenAITracer")
 
 
 class AzureOpenAITracer(OpenAITracer):
     """
     Tracing for both Completion and ChatCompletion endpoints
     """
 
@@ -84,112 +88,124 @@
         metadata: Optional[TraceMetadata] = None,
     ):
         super().__init__(
             instance=instance,
             trace_id=trace_id,
             metadata=metadata,
         )
+        logger.info("Initialized AzureOpenAITracer")
 
 
 class OpenAICompletionTracer(BaseContextTracer):
     def __init__(
         self,
         instance: Union[OpenAI, AsyncOpenAI, AzureOpenAI, AsyncAzureOpenAI],
         trace_id: Optional[str] = None,
         metadata: Optional[TraceMetadata] = None,
     ):
         self.instance = instance
         super().__init__(
             trace_id=trace_id,
             metadata=metadata,
         )
+        logger.info("Initialized OpenAICompletionTracer")
 
     def __enter__(self):
         super().__enter__()
         self.instance.completions._original_create = self.instance.completions.create  # type: ignore
         if isinstance(self.instance, AsyncOpenAI):
             self.instance.completions.create = self.patched_completion_acreate  # type: ignore
         else:
             self.instance.completions.create = self.patched_completion_create  # type: ignore
+        logger.info("Entered OpenAICompletionTracer")
 
     def __exit__(self, _type, _value, _traceback):
         super().__exit__(_type, _value, _traceback)
         self.instance.completions.create = self.instance.completions._original_create  # type: ignore
+        logger.info("Exited OpenAICompletionTracer")
 
     def patched_completion_create(self, *args, **kwargs):
         started_at = milliseconds_timestamp()
+        logger.info(f"Patched completion create started at: {started_at}")
         try:
             response: Union[Completion, Stream[Completion]] = cast(
                 Any, self.instance.completions
             )._original_create(*args, **kwargs)
 
             if isinstance(response, Stream):
+                logger.info("Response is a Stream")
                 return capture_chunks_with_timings_and_reyield(
                     cast(Generator[Completion, Any, Any], response),
                     lambda chunks, first_token_at, finished_at: self.handle_deltas(
                         chunks,
                         SpanTimestamps(
                             started_at=started_at,
                             first_token_at=first_token_at,
                             finished_at=finished_at,
                         ),
                         **kwargs,
                     ),
                 )
             else:
                 finished_at = milliseconds_timestamp()
+                logger.info(f"Completion finished at: {finished_at}")
                 self.handle_completion(
                     response,
                     SpanTimestamps(started_at=started_at, finished_at=finished_at),
                     **kwargs,
                 )
                 return response
         except Exception as err:
             finished_at = milliseconds_timestamp()
+            logger.exception(f"Exception occurred at: {finished_at}", exc_info=err)
             self.handle_exception(
                 err,
                 SpanTimestamps(started_at=started_at, finished_at=finished_at),
                 **kwargs,
             )
             raise err
 
     async def patched_completion_acreate(self, *args, **kwargs):
         started_at = milliseconds_timestamp()
+        logger.info(f"Patched async completion create started at: {started_at}")
         response: Union[Completion, AsyncStream[Completion]] = await cast(
             Any, self.instance.completions
         )._original_create(*args, **kwargs)
 
         if isinstance(response, AsyncStream):
+            logger.info("Response is an AsyncStream")
             return capture_async_chunks_with_timings_and_reyield(
                 cast(AsyncGenerator[Completion, Any], response),
                 lambda chunks, first_token_at, finished_at: self.handle_deltas(
                     chunks,
                     SpanTimestamps(
                         started_at=started_at,
                         first_token_at=first_token_at,
                         finished_at=finished_at,
                     ),
                     **kwargs,
                 ),
             )
         else:
             finished_at = milliseconds_timestamp()
+            logger.info(f"Async completion finished at: {finished_at}")
             self.handle_completion(
                 response,
                 SpanTimestamps(started_at=started_at, finished_at=finished_at),
                 **kwargs,
             )
             return response
 
     def handle_deltas(
         self,
         deltas: List[Completion],
         timestamps: SpanTimestamps,
         **kwargs,
     ):
+        logger.info(f"Handling deltas: {deltas}")
         text_outputs: Dict[int, str] = {}
         for delta in deltas:
             for choice in delta.choices:
                 index = choice.index or 0
                 text_outputs[index] = text_outputs.get(index, "") + (choice.text or "")
 
         self.append_span(
@@ -200,21 +216,23 @@
                 ],
                 metrics=SpanMetrics(),
                 timestamps=timestamps,
                 error=None,
                 **kwargs,
             )
         )
+        logger.info("Deltas handled successfully")
 
     def handle_completion(
         self,
         response: Completion,
         timestamps: SpanTimestamps,
         **kwargs,
     ):
+        logger.info(f"Handling completion: {response}")
         self.append_span(
             self.build_trace(
                 outputs=[
                     TypedValueText(type="text", value=output.text)
                     for output in response.choices
                 ],
                 metrics=SpanMetrics(
@@ -222,39 +240,43 @@
                     completion_tokens=safe_get(response, "usage", "completion_tokens"),
                 ),
                 timestamps=timestamps,
                 error=None,
                 **kwargs,
             )
         )
+        logger.info("Completion handled successfully")
 
     def handle_exception(
         self,
         err: Exception,
         timestamps: SpanTimestamps,
         **kwargs,
     ):
+        logger.exception("Handling exception", exc_info=err)
         self.append_span(
             self.build_trace(
                 outputs=[],
                 metrics=SpanMetrics(),
                 timestamps=timestamps,
                 error=capture_exception(err),
                 **kwargs,
             )
         )
+        logger.info("Exception handled")
 
     def build_trace(
         self,
         outputs: List[SpanInputOutput],
         metrics: SpanMetrics,
         timestamps: SpanTimestamps,
         error: Optional[ErrorCapture],
         **kwargs,
     ) -> LLMSpan:
+        logger.info("Building trace")
         return LLMSpan(
             type="llm",
             span_id=f"span_{nanoid.generate()}",
             parent_id=self.get_parent_id(),
             trace_id=self.trace_id,
             vendor="openai",
             model=kwargs.get("model", "unknown"),
@@ -278,98 +300,109 @@
         metadata: Optional[TraceMetadata] = None,
     ):
         self.instance = instance
         super().__init__(
             trace_id=trace_id,
             metadata=metadata,
         )
+        logger.info("Initialized OpenAIChatCompletionTracer")
 
     def __enter__(self):
         super().__enter__()
         self.instance.chat.completions._original_create = self.instance.chat.completions.create  # type: ignore
         if isinstance(self.instance, AsyncOpenAI):
             self.instance.chat.completions.create = self.patched_completion_acreate  # type: ignore
         else:
             self.instance.chat.completions.create = self.patched_completion_create  # type: ignore
+        logger.info("Entered OpenAIChatCompletionTracer")
 
     def __exit__(self, _type, _value, _traceback):
         super().__exit__(_type, _value, _traceback)
         self.instance.chat.completions.create = self.instance.chat.completions._original_create  # type: ignore
+        logger.info("Exited OpenAIChatCompletionTracer")
 
     def patched_completion_create(self, *args, **kwargs):
         started_at = milliseconds_timestamp()
+        logger.info(f"Patched chat completion create started at: {started_at}")
         try:
             response: Union[ChatCompletion, Stream[ChatCompletionChunk]] = cast(
                 Any, self.instance.chat.completions
             )._original_create(*args, **kwargs)
 
             if isinstance(response, Stream):
+                logger.info("Response is a Stream")
                 return capture_chunks_with_timings_and_reyield(
                     cast(Generator[ChatCompletionChunk, Any, Any], response),
                     lambda chunks, first_token_at, finished_at: self.handle_deltas(
                         chunks,
                         SpanTimestamps(
                             started_at=started_at,
                             first_token_at=first_token_at,
                             finished_at=finished_at,
                         ),
                         **kwargs,
                     ),
                 )
             else:
                 finished_at = milliseconds_timestamp()
+                logger.info(f"Chat completion finished at: {finished_at}")
                 self.handle_completion(
                     response,
                     SpanTimestamps(started_at=started_at, finished_at=finished_at),
                     **kwargs,
                 )
                 return response
         except Exception as err:
             finished_at = milliseconds_timestamp()
+            logger.exception(f"Exception occurred at: {finished_at}", exc_info=err)
             self.handle_exception(
                 err,
                 SpanTimestamps(started_at=started_at, finished_at=finished_at),
                 **kwargs,
             )
             raise err
 
     async def patched_completion_acreate(self, *args, **kwargs):
         started_at = milliseconds_timestamp()
+        logger.info(f"Patched async chat completion create started at: {started_at}")
         response: Union[ChatCompletion, AsyncStream[ChatCompletionChunk]] = await cast(
             Any, self.instance.chat.completions
         )._original_create(*args, **kwargs)
 
         if isinstance(response, AsyncStream):
+            logger.info("Response is an AsyncStream")
             return capture_async_chunks_with_timings_and_reyield(
                 cast(AsyncGenerator[ChatCompletionChunk, Any], response),
                 lambda chunks, first_token_at, finished_at: self.handle_deltas(
                     chunks,
                     SpanTimestamps(
                         started_at=started_at,
                         first_token_at=first_token_at,
                         finished_at=finished_at,
                     ),
                     **kwargs,
                 ),
             )
         else:
             finished_at = milliseconds_timestamp()
+            logger.info(f"Async chat completion finished at: {finished_at}")
             self.handle_completion(
                 response,
                 SpanTimestamps(started_at=started_at, finished_at=finished_at),
                 **kwargs,
             )
             return response
 
     def handle_deltas(
         self,
         deltas: List[ChatCompletionChunk],
         timestamps: SpanTimestamps,
         **kwargs,
     ):
+        logger.info(f"Handling chat completion deltas: {deltas}")
         # Accumulate deltas
         chat_outputs: Dict[int, List[ChatMessage]] = {}
         for delta in deltas:
             for choice in delta.choices:
                 index = choice.index
                 delta = choice.delta
                 if delta.role:
@@ -435,21 +468,23 @@
                 ],
                 metrics=SpanMetrics(),
                 timestamps=timestamps,
                 error=None,
                 **kwargs,
             )
         )
+        logger.info("Chat completion deltas handled successfully")
 
     def handle_completion(
         self,
         response: ChatCompletion,
         timestamps: SpanTimestamps,
         **kwargs,
     ):
+        logger.info(f"Handling chat completion: {response}")
         self.append_span(
             self.build_trace(
                 outputs=[
                     TypedValueChatMessages(
                         type="chat_messages",
                         value=[cast(ChatMessage, output.message.model_dump())],
                     )
@@ -460,39 +495,43 @@
                     completion_tokens=safe_get(response, "usage", "completion_tokens"),
                 ),
                 timestamps=timestamps,
                 error=None,
                 **kwargs,
             )
         )
+        logger.info("Chat completion handled successfully")
 
     def handle_exception(
         self,
         err: Exception,
         timestamps: SpanTimestamps,
         **kwargs,
     ):
+        logger.exception("Handling exception in chat completion", exc_info=err)
         self.append_span(
             self.build_trace(
                 outputs=[],
                 metrics=SpanMetrics(),
                 timestamps=timestamps,
                 error=capture_exception(err),
                 **kwargs,
             )
         )
+        logger.info("Chat completion exception handled")
 
     def build_trace(
         self,
         outputs: List[SpanInputOutput],
         metrics: SpanMetrics,
         timestamps: SpanTimestamps,
         error: Optional[ErrorCapture],
         **kwargs,
     ) -> LLMSpan:
+        logger.info("Building chat completion trace")
         params = SpanParams(
             temperature=kwargs.get("temperature", 1.0),
             stream=kwargs.get("stream", False),
         )
         functions = kwargs.get("functions", None)
         if functions:
             params["functions"] = functions
@@ -518,8 +557,9 @@
                 type="chat_messages", value=kwargs.get("messages", []).copy()
             ),
             outputs=outputs,
             error=error,
             params=params,
             metrics=metrics,
             timestamps=timestamps,
-        )
+        )
+
```

### Comparing `cntrlai-0.0.32/cntrlai/types.py` & `cntrlai-0.0.33/cntrlai/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+### cntrlai/types.py
+
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 from pydantic import BaseModel, Field
 
 
 ChatRole = Literal[
     "system", "user", "assistant", "function", "tool", "guardrail", "unknown"
```

### Comparing `cntrlai-0.0.32/cntrlai/utils.py` & `cntrlai-0.0.33/cntrlai/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+### cntrlai/utils.py
+
 import json
 import time
 import traceback
 from typing import (
     Any,
     AsyncGenerator,
     Callable,
```

### Comparing `cntrlai-0.0.32/pyproject.toml` & `cntrlai-0.0.33/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cntrlai"
-version = "0.0.32"
+version = "0.0.33"
 description = "ControlAI's Client for Monitoring Your LLM performance"
 authors = ["Lukasz Bartoszcze <lbartoszcze@controlai.org>"]
 homepage = "https://controlai.org"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -25,16 +25,16 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 nanoid = "^2.0.0"
 requests = "^2.31.0"
 pydantic = ">=2.5.2"
 httpx = "^0.27.0"
 
-openai = { version = "^1.3.7", optional = true }
-langchain = { version = "^0.0.345", optional = true }
+openai = { version = "^1.3.7"}
+langchain = { version = "^0.0.345"}
 retry = "^0.9.2"
 tqdm = "^4.66.2"
 pandas = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 chainlit = "^0.7.501"
```

### Comparing `cntrlai-0.0.32/PKG-INFO` & `cntrlai-0.0.33/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cntrlai
-Version: 0.0.32
+Version: 0.0.33
 Summary: ControlAI's Client for Monitoring Your LLM performance
 Home-page: https://controlai.org
 License: MIT
 Author: Lukasz Bartoszcze
 Author-email: lbartoszcze@controlai.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

