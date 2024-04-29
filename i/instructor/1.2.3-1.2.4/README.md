# Comparing `tmp/instructor-1.2.3.tar.gz` & `tmp/instructor-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.3.tar", max compression
+gzip compressed data, was "instructor-1.2.4.tar", max compression
```

## Comparing `instructor-1.2.3.tar` & `instructor-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-04-27 17:59:46.310827 instructor-1.2.3/LICENSE
--rw-r--r--   0        0        0     9716 2024-04-27 17:59:46.310827 instructor-1.2.3/README.md
--rw-r--r--   0        0        0     1445 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6476 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/cli/usage.py
--rw-r--r--   0        0        0     9747 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client.py
--rw-r--r--   0        0        0     2453 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2348 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_cohere.py
--rw-r--r--   0        0        0     1379 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_groq.py
--rw-r--r--   0        0        0     1709 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/client_mistral.py
--rw-r--r--   0        0        0     8968 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2580 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11052 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/exceptions.py
--rw-r--r--   0        0        0     8020 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-04-27 17:59:46.374827 instructor-1.2.3/instructor/mode.py
--rw-r--r--   0        0        0     4877 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/patch.py
--rw-r--r--   0        0        0    13509 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/py.typed
--rw-r--r--   0        0        0     9532 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/retry.py
--rw-r--r--   0        0        0     5505 2024-04-27 17:59:46.378827 instructor-1.2.3/instructor/utils.py
--rw-r--r--   0        0        0     2364 2024-04-27 17:59:46.378827 instructor-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    11658 1970-01-01 00:00:00.000000 instructor-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-29 18:30:51.796761 instructor-1.2.4/LICENSE
+-rw-r--r--   0        0        0     9716 2024-04-29 18:30:51.796761 instructor-1.2.4/README.md
+-rw-r--r--   0        0        0     1445 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6476 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/usage.py
+-rw-r--r--   0        0        0    10324 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client.py
+-rw-r--r--   0        0        0     2453 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2348 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_cohere.py
+-rw-r--r--   0        0        0     1379 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_groq.py
+-rw-r--r--   0        0        0     1709 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_mistral.py
+-rw-r--r--   0        0        0     8968 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2580 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11052 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/exceptions.py
+-rw-r--r--   0        0        0     8020 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/function_calls.py
+-rw-r--r--   0        0        0      852 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/mode.py
+-rw-r--r--   0        0        0     4989 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/patch.py
+-rw-r--r--   0        0        0    13509 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/py.typed
+-rw-r--r--   0        0        0     9532 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/retry.py
+-rw-r--r--   0        0        0     5505 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/utils.py
+-rw-r--r--   0        0        0     2364 2024-04-29 18:30:51.868761 instructor-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    11658 1970-01-01 00:00:00.000000 instructor-1.2.4/PKG-INFO
```

### Comparing `instructor-1.2.3/LICENSE` & `instructor-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/README.md` & `instructor-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/__init__.py` & `instructor-1.2.4/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/_types/_alias.py` & `instructor-1.2.4/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/cli/cli.py` & `instructor-1.2.4/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/cli/files.py` & `instructor-1.2.4/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/cli/hub.py` & `instructor-1.2.4/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/cli/jobs.py` & `instructor-1.2.4/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/cli/usage.py` & `instructor-1.2.4/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/client.py` & `instructor-1.2.4/instructor/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,85 +63,93 @@
     # TODO: we should overload a case where response_model is None
     def create(
         self,
         response_model: Type[T],
         messages: List[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict | None = None,
+        strict: bool = True,
         **kwargs,
     ) -> T:
         kwargs = self.handle_kwargs(kwargs)
 
         return self.create_fn(
             response_model=response_model,
             messages=messages,
             max_retries=max_retries,
             validation_context=validation_context,
+            strict=strict,
             **kwargs,
         )
 
     def create_partial(
         self,
         response_model: Type[T],
         messages: List[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict | None = None,
+        strict: bool = True,
         **kwargs,
     ) -> Generator[T, None, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support partial"
 
         kwargs["stream"] = True
 
         kwargs = self.handle_kwargs(kwargs)
 
         response_model = instructor.Partial[response_model]  # type: ignore
         return self.create_fn(
             messages=messages,
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
+            strict=strict,
             **kwargs,
         )
 
     def create_iterable(
         self,
         messages: List[ChatCompletionMessageParam],
         response_model: Type[T],
         max_retries: int = 3,
         validation_context: dict | None = None,
+        strict: bool = True,
         **kwargs,
     ) -> Iterable[T]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support iterable"
 
         kwargs["stream"] = True
         kwargs = self.handle_kwargs(kwargs)
 
         response_model = Iterable[response_model]  # type: ignore
         return self.create_fn(
             messages=messages,
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
+            strict=strict,
             **kwargs,
         )
 
     def create_with_completion(
         self,
         messages: List[ChatCompletionMessageParam],
         response_model: Type[T],
         max_retries: int = 3,
         validation_context: dict | None = None,
+        strict: bool = True,
         **kwargs,
     ) -> Tuple[T, ChatCompletion | Any]:
         kwargs = self.handle_kwargs(kwargs)
         model = self.create_fn(
             messages=messages,
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
+            strict=strict,
             **kwargs,
         )
         return model, model._raw_response
 
     def handle_kwargs(self, kwargs: dict):
         for key, value in self.kwargs.items():
             if key not in kwargs:
@@ -172,81 +180,89 @@
 
     async def create(
         self,
         messages: List[ChatCompletionMessageParam],
         response_model: Type[T],
         validation_context: dict | None = None,
         max_retries: int = 3,
+        strict: bool = True,
         **kwargs,
     ) -> T:
         kwargs = self.handle_kwargs(kwargs)
         return await self.create_fn(
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
+            strict=strict,
             **kwargs,
         )
 
     async def create_partial(
         self,
         response_model: Type[T],
         messages: List[ChatCompletionMessageParam],
         validation_context: dict | None = None,
         max_retries: int = 3,
+        strict: bool = True,
         **kwargs,
     ) -> AsyncGenerator[T, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support partial"
 
         kwargs = self.handle_kwargs(kwargs)
         kwargs["stream"] = True
         async for item in await self.create_fn(
             response_model=instructor.Partial[response_model],  # type: ignore
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
+            strict=strict,
             **kwargs,
         ):
             yield item
 
     async def create_iterable(
         self,
         response_model: Type[T],
         messages: List[ChatCompletionMessageParam],
         validation_context: dict | None = None,
         max_retries: int = 3,
+        strict: bool = True,
         **kwargs,
     ) -> AsyncGenerator[T, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support iterable"
 
         kwargs = self.handle_kwargs(kwargs)
         kwargs["stream"] = True
         async for item in await self.create_fn(
             response_model=Iterable[response_model],
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
+            strict=strict,
             **kwargs,
         ):
             yield item
 
     async def create_with_completion(
         self,
         response_model: Type[T],
         messages: List[ChatCompletionMessageParam],
         validation_context: dict | None = None,
         max_retries: int = 3,
+        strict: bool = True,
         **kwargs,
     ) -> Tuple[T, dict]:
         kwargs = self.handle_kwargs(kwargs)
         response = await self.create_fn(
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
+            strict=strict,
             **kwargs,
         )
         return response, response._raw_response
 
 
 @overload
 def from_openai(
@@ -270,17 +286,21 @@
     **kwargs,
 ) -> Instructor | AsyncInstructor:
     if hasattr(client, "base_url"):
         provider = get_provider(str(client.base_url))
     else:
         provider = Provider.OPENAI
 
-    assert isinstance(
-        client, (openai.OpenAI, openai.AsyncOpenAI)
-    ), "Client must be an instance of openai.OpenAI or openai.AsyncOpenAI"
+    if not isinstance(client, (openai.OpenAI, openai.AsyncOpenAI)):
+        import warnings
+
+        warnings.warn(
+            "Client should be an instance of openai.OpenAI or openai.AsyncOpenAI. "
+            "Unexpected behavior may occur with other client types."
+        )
 
     if provider in {Provider.ANYSCALE, Provider.TOGETHER}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.JSON_SCHEMA,
             instructor.Mode.MD_JSON,
```

### Comparing `instructor-1.2.3/instructor/client_anthropic.py` & `instructor-1.2.4/instructor/client_anthropic.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/client_cohere.py` & `instructor-1.2.4/instructor/client_cohere.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/client_groq.py` & `instructor-1.2.4/instructor/client_groq.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/client_mistral.py` & `instructor-1.2.4/instructor/client_mistral.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/distil.py` & `instructor-1.2.4/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/citation.py` & `instructor-1.2.4/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/iterable.py` & `instructor-1.2.4/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/maybe.py` & `instructor-1.2.4/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/parallel.py` & `instructor-1.2.4/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/partial.py` & `instructor-1.2.4/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/simple_type.py` & `instructor-1.2.4/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/dsl/validators.py` & `instructor-1.2.4/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/function_calls.py` & `instructor-1.2.4/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/mode.py` & `instructor-1.2.4/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/patch.py` & `instructor-1.2.4/instructor/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,48 +112,52 @@
     func_is_async = is_async(func)
 
     @wraps(func)
     async def new_create_async(
         response_model: Type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
+        strict: bool = True,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
     ) -> T_Model:
         response_model, new_kwargs = handle_response_model(
             response_model=response_model, mode=mode, **kwargs
         )
         response = await retry_async(
             func=func,
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             args=args,
             kwargs=new_kwargs,
+            strict=strict,
             mode=mode,
         )  # type: ignore
         return response
 
     @wraps(func)
     def new_create_sync(
         response_model: Type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
+        strict: bool = True,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
     ) -> T_Model:
         response_model, new_kwargs = handle_response_model(
             response_model=response_model, mode=mode, **kwargs
         )
         response = retry_sync(
             func=func,
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             args=args,
+            strict=strict,
             kwargs=new_kwargs,
             mode=mode,
         )
         return response
 
     new_create = new_create_async if func_is_async else new_create_sync
```

### Comparing `instructor-1.2.3/instructor/process_response.py` & `instructor-1.2.4/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/retry.py` & `instructor-1.2.4/instructor/retry.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/instructor/utils.py` & `instructor-1.2.4/instructor/utils.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.3/pyproject.toml` & `instructor-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.3"
+version = "1.2.4"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
```

### Comparing `instructor-1.2.3/PKG-INFO` & `instructor-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.3
+Version: 1.2.4
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

