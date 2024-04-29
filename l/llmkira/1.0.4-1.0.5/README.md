# Comparing `tmp/llmkira-1.0.4.tar.gz` & `tmp/llmkira-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmkira-1.0.4.tar", last modified: Mon Apr 22 09:03:29 2024, max compression
+gzip compressed data, was "llmkira-1.0.5.tar", last modified: Mon Apr 29 08:53:56 2024, max compression
```

## Comparing `llmkira-1.0.4.tar` & `llmkira-1.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-04-22 09:03:15.794260 llmkira-1.0.4/LICENSE
--rw-r--r--   0        0        0     1030 2024-04-22 09:03:15.794260 llmkira-1.0.4/NOTICE.MD
--rw-r--r--   0        0        0     8725 2024-04-22 09:03:15.794260 llmkira-1.0.4/README.md
--rw-r--r--   0        0        0      730 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/__init__.py
--rw-r--r--   0        0        0      209 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/_exception.py
--rw-r--r--   0        0        0     5346 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/elara_runtime.py
--rw-r--r--   0        0        0     2299 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/lmdb_runtime.py
--rw-r--r--   0        0        0     1451 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/redis_runtime.py
--rw-r--r--   0        0        0     1159 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/runtime_schema.py
--rw-r--r--   0        0        0     4711 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/doc_manager/__init__.py
--rw-r--r--   0        0        0      127 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/alarm/__init__.py
--rw-r--r--   0        0        0     8269 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/search/__init__.py
--rw-r--r--   0        0        0     2537 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/search/engine.py
--rw-r--r--   0        0        0     5372 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/voice/__init__.py
--rw-r--r--   0        0        0     3247 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/voice_hook.py
--rw-r--r--   0        0        0        0 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/__init__.py
--rw-r--r--   0        0        0      626 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/_base.py
--rw-r--r--   0        0        0     2323 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/env.py
--rw-r--r--   0        0        0     4419 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/file.py
--rw-r--r--   0        0        0     1025 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/instruction.py
--rw-r--r--   0        0        0     1512 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/time.py
--rw-r--r--   0        0        0     1158 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/tool_call.py
--rw-r--r--   0        0        0     4284 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/logic/__init__.py
--rw-r--r--   0        0        0      637 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/__init__.py
--rw-r--r--   0        0        0      733 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/_base.py
--rw-r--r--   0        0        0     2381 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/local_storage.py
--rw-r--r--   0        0        0     1070 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/redis_storage/LICENSE
--rw-r--r--   0        0        0     2819 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/redis_storage/__init__.py
--rw-r--r--   0        0        0     6192 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/redis_storage/utils.py
--rw-r--r--   0        0        0      522 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/__init__.py
--rw-r--r--   0        0        0     3431 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/_excption.py
--rw-r--r--   0        0        0    10731 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/cell.py
--rw-r--r--   0        0        0     8866 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/request.py
--rw-r--r--   0        0        0     1968 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/utils.py
--rw-r--r--   0        0        0      130 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/__init__.py
--rw-r--r--   0        0        0     2729 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/fuse/__init__.py
--rw-r--r--   0        0        0     1610 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/hook/__init__.py
--rw-r--r--   0        0        0     2143 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/trigger/__init__.py
--rw-r--r--   0        0        0      419 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/trigger/default_trigger.py
--rw-r--r--   0        0        0      321 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/sdk/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/LICENSE
--rw-r--r--   0        0        0     4501 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/__init__.py
--rw-r--r--   0        0        0      496 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/error.py
--rw-r--r--   0        0        0     3373 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/loader.py
--rw-r--r--   0        0        0     9551 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/model.py
--rw-r--r--   0        0        0     3286 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/register.py
--rw-r--r--   0        0        0    10609 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/schema.py
--rw-r--r--   0        0        0     4238 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/utils.py
--rw-r--r--   0        0        0     4848 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/__init__.py
--rw-r--r--   0        0        0    16694 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/schema.py
--rw-r--r--   0        0        0      219 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/snapshot/__init__.py
--rw-r--r--   0        0        0      422 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/snapshot/_base.py
--rw-r--r--   0        0        0     1237 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/snapshot/local.py
--rw-r--r--   0        0        0     2907 2024-04-22 09:03:29.578371 llmkira-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1485 2024-04-22 09:03:15.822260 llmkira-1.0.4/tests/pydantic_error.py
--rw-r--r--   0        0        0    12056 1970-01-01 00:00:00.000000 llmkira-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 08:53:43.421362 llmkira-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1030 2024-04-29 08:53:43.421362 llmkira-1.0.5/NOTICE.MD
+-rw-r--r--   0        0        0     8725 2024-04-29 08:53:43.421362 llmkira-1.0.5/README.md
+-rw-r--r--   0        0        0      730 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/_exception.py
+-rw-r--r--   0        0        0     5346 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/cache/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/cache/elara_runtime.py
+-rw-r--r--   0        0        0     2299 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/cache/lmdb_runtime.py
+-rw-r--r--   0        0        0     1451 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/cache/redis_runtime.py
+-rw-r--r--   0        0        0     1159 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/cache/runtime_schema.py
+-rw-r--r--   0        0        0     4711 2024-04-29 08:53:43.441362 llmkira-1.0.5/llmkira/doc_manager/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/plugins/__init__.py
+-rw-r--r--   0        0        0     6886 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/plugins/alarm/__init__.py
+-rw-r--r--   0        0        0     8269 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/plugins/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/plugins/search/__init__.py
+-rw-r--r--   0        0        0     2537 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/plugins/search/engine.py
+-rw-r--r--   0        0        0     5372 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/voice/__init__.py
+-rw-r--r--   0        0        0     3247 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/extra/voice_hook.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/_base.py
+-rw-r--r--   0        0        0     2323 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/env.py
+-rw-r--r--   0        0        0     4419 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/file.py
+-rw-r--r--   0        0        0     1194 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/instruction.py
+-rw-r--r--   0        0        0     1512 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/time.py
+-rw-r--r--   0        0        0     1158 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/kv_manager/tool_call.py
+-rw-r--r--   0        0        0     4284 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/logic/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/memory/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/memory/_base.py
+-rw-r--r--   0        0        0     2381 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/memory/local_storage.py
+-rw-r--r--   0        0        0     1070 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/memory/redis_storage/LICENSE
+-rw-r--r--   0        0        0     2819 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/memory/redis_storage/__init__.py
+-rw-r--r--   0        0        0     6192 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/memory/redis_storage/utils.py
+-rw-r--r--   0        0        0      522 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openai/__init__.py
+-rw-r--r--   0        0        0     3431 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openai/_excption.py
+-rw-r--r--   0        0        0    10731 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openai/cell.py
+-rw-r--r--   0        0        0     8866 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openai/request.py
+-rw-r--r--   0        0        0     1968 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openai/utils.py
+-rw-r--r--   0        0        0      130 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openapi/__init__.py
+-rw-r--r--   0        0        0     2729 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openapi/fuse/__init__.py
+-rw-r--r--   0        0        0     1610 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openapi/hook/__init__.py
+-rw-r--r--   0        0        0     2155 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openapi/trigger/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/openapi/trigger/default_trigger.py
+-rw-r--r--   0        0        0      321 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/LICENSE
+-rw-r--r--   0        0        0     4501 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/error.py
+-rw-r--r--   0        0        0     3373 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/loader.py
+-rw-r--r--   0        0        0     9551 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/model.py
+-rw-r--r--   0        0        0     3286 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/register.py
+-rw-r--r--   0        0        0    10609 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/tools/schema.py
+-rw-r--r--   0        0        0     4238 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/sdk/utils.py
+-rw-r--r--   0        0        0     4848 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/task/__init__.py
+-rw-r--r--   0        0        0    16694 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/task/schema.py
+-rw-r--r--   0        0        0      219 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/task/snapshot/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/task/snapshot/_base.py
+-rw-r--r--   0        0        0     1237 2024-04-29 08:53:43.445362 llmkira-1.0.5/llmkira/task/snapshot/local.py
+-rw-r--r--   0        0        0     2907 2024-04-29 08:53:56.973250 llmkira-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1485 2024-04-29 08:53:43.445362 llmkira-1.0.5/tests/pydantic_error.py
+-rw-r--r--   0        0        0    12056 1970-01-01 00:00:00.000000 llmkira-1.0.5/PKG-INFO
```

### Comparing `llmkira-1.0.4/LICENSE` & `llmkira-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/NOTICE.MD` & `llmkira-1.0.5/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/README.md` & `llmkira-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/__init__.py` & `llmkira-1.0.5/llmkira/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/cache/__init__.py` & `llmkira-1.0.5/llmkira/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/cache/elara_runtime.py` & `llmkira-1.0.5/llmkira/cache/elara_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/cache/lmdb_runtime.py` & `llmkira-1.0.5/llmkira/cache/lmdb_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/cache/redis_runtime.py` & `llmkira-1.0.5/llmkira/cache/redis_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/cache/runtime_schema.py` & `llmkira-1.0.5/llmkira/cache/runtime_schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/doc_manager/__init__.py` & `llmkira-1.0.5/llmkira/doc_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/extra/plugins/alarm/__init__.py` & `llmkira-1.0.5/llmkira/extra/plugins/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/extra/plugins/e2b_code_interpreter/__init__.py` & `llmkira-1.0.5/llmkira/extra/plugins/e2b_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/extra/plugins/search/__init__.py` & `llmkira-1.0.5/llmkira/extra/plugins/search/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/extra/plugins/search/engine.py` & `llmkira-1.0.5/llmkira/extra/plugins/search/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         )
     else:
         _build_result = []
         for result in search_result:
             _build_result.append(
                 SearchEngineResult(
                     title=result.get("title", "Undefined"),
-                    link=result.get("Href", "Undefined"),
+                    link=result.get("href", "Undefined"),
                     snippet=result.get("body", "Undefined"),
                 )
             )
         return _build_result
 
 
 def build_search_tips(search_items: List[SearchEngineResult], limit=5):
```

### Comparing `llmkira-1.0.4/llmkira/extra/voice/__init__.py` & `llmkira-1.0.5/llmkira/extra/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/extra/voice_hook.py` & `llmkira-1.0.5/llmkira/extra/voice_hook.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/kv_manager/_base.py` & `llmkira-1.0.5/llmkira/kv_manager/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/kv_manager/env.py` & `llmkira-1.0.5/llmkira/kv_manager/env.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/kv_manager/file.py` & `llmkira-1.0.5/llmkira/kv_manager/file.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/kv_manager/instruction.py` & `llmkira-1.0.5/llmkira/kv_manager/instruction.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,17 +19,20 @@
     def __init__(self, user_id: str):
         self.user_id = str(user_id)
 
     def prefix(self, key: str) -> str:
         return f"instruction:{key}"
 
     async def read_instruction(self) -> str:
+        """
+        读取指令，如果没有指令则返回默认指令，指令长度大于5，否则返回默认指令
+        """
         result = await self.read_data(self.user_id)
-        if not result:
-            return f"Now={time_now()}\n{DEFAULT_INSTRUCTION}"
-        return f"Now={time_now()}\n{result}"
+        if isinstance(result, str) and len(result) > 5:
+            return f"Now={time_now()}\n{result}"
+        return f"Now={time_now()}\n{DEFAULT_INSTRUCTION}"
 
     async def set_instruction(self, instruction: str) -> str:
         if not isinstance(instruction, str):
             raise ValueError("Instruction should be str")
         await self.save_data(self.user_id, instruction)
         return instruction
```

### Comparing `llmkira-1.0.4/llmkira/kv_manager/time.py` & `llmkira-1.0.5/llmkira/kv_manager/time.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/kv_manager/tool_call.py` & `llmkira-1.0.5/llmkira/kv_manager/tool_call.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/logic/__init__.py` & `llmkira-1.0.5/llmkira/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/memory/__init__.py` & `llmkira-1.0.5/llmkira/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/memory/_base.py` & `llmkira-1.0.5/llmkira/memory/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/memory/local_storage.py` & `llmkira-1.0.5/llmkira/memory/local_storage.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/memory/redis_storage/LICENSE` & `llmkira-1.0.5/llmkira/memory/redis_storage/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/memory/redis_storage/__init__.py` & `llmkira-1.0.5/llmkira/memory/redis_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/memory/redis_storage/utils.py` & `llmkira-1.0.5/llmkira/memory/redis_storage/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openai/__init__.py` & `llmkira-1.0.5/llmkira/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openai/_excption.py` & `llmkira-1.0.5/llmkira/openai/_excption.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openai/cell.py` & `llmkira-1.0.5/llmkira/openai/cell.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openai/request.py` & `llmkira-1.0.5/llmkira/openai/request.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openai/utils.py` & `llmkira-1.0.5/llmkira/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openapi/fuse/__init__.py` & `llmkira-1.0.5/llmkira/openapi/fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openapi/hook/__init__.py` & `llmkira-1.0.5/llmkira/openapi/hook/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/openapi/trigger/__init__.py` & `llmkira-1.0.5/llmkira/openapi/trigger/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 
 async def get_trigger_loop(platform_name: str, message: str, uid: str = None):
     """
     receiver builder
     message: Message Content
     :return 如果有触发，则返回触发的action，否则返回None 代表没有操作
     """
-    sorted(__trigger_phrases__, key=lambda x: x.priority)
+    trigger_sorted = sorted(__trigger_phrases__, key=lambda x: x.priority)
     if not message:
         message = ""
-    for trigger in __trigger_phrases__:
+    for trigger in trigger_sorted:
         if trigger.on_platform == platform_name:
             try:
                 if await trigger.on_func(message, uid):
                     return trigger
             except Exception as e:
                 logger.error(f"📦 Plugin:trigger error: {e}")
                 pass
```

### Comparing `llmkira-1.0.4/llmkira/sdk/tools/LICENSE` & `llmkira-1.0.5/llmkira/sdk/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/sdk/tools/__init__.py` & `llmkira-1.0.5/llmkira/sdk/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/sdk/tools/loader.py` & `llmkira-1.0.5/llmkira/sdk/tools/loader.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/sdk/tools/model.py` & `llmkira-1.0.5/llmkira/sdk/tools/model.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/sdk/tools/register.py` & `llmkira-1.0.5/llmkira/sdk/tools/register.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/sdk/tools/schema.py` & `llmkira-1.0.5/llmkira/sdk/tools/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/sdk/utils.py` & `llmkira-1.0.5/llmkira/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/task/__init__.py` & `llmkira-1.0.5/llmkira/task/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/task/schema.py` & `llmkira-1.0.5/llmkira/task/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/llmkira/task/snapshot/local.py` & `llmkira-1.0.5/llmkira/task/snapshot/local.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/pyproject.toml` & `llmkira-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmkira"
-version = "1.0.4"
+version = "1.0.5"
 description = "A chain message bot based on OpenAI"
 authors = [
     { name = "sudoskys", email = "me@dianas.cyou" },
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = [
     "pathlib>=1.0.1",
```

### Comparing `llmkira-1.0.4/tests/pydantic_error.py` & `llmkira-1.0.5/tests/pydantic_error.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.4/PKG-INFO` & `llmkira-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmkira
-Version: 1.0.4
+Version: 1.0.5
 Summary: A chain message bot based on OpenAI
 Keywords: llmbot,llmkira,openai,chatgpt,llm
 Home-page: https://llmkira.github.io/Docs/
 Author-Email: sudoskys <me@dianas.cyou>, llmkira <me@dianas.cyou>
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: llmkira Version: 1.0.4 Summary: A chain message bot
+Metadata-Version: 2.1 Name: llmkira Version: 1.0.5 Summary: A chain message bot
 based on OpenAI Keywords: llmbot,llmkira,openai,chatgpt,llm Home-page: https://
 llmkira.github.io/Docs/ Author-Email: sudoskys
 dianas.cyou>, llmkira
 dianas.cyou> License: Apache-2.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage,
 https://llmkira.github.io/Docs/ Project-URL: Repository, https://github.com/
 LlmKira/Openaibot Requires-Python: <3.12,>=3.9 Requires-Dist: pathlib>=1.0.1
```

