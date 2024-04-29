# Comparing `tmp/llmbot_plugin_bilisearch-0.1.5.tar.gz` & `tmp/llmbot_plugin_bilisearch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmbot_plugin_bilisearch-0.1.5.tar", max compression
+gzip compressed data, was "llmbot_plugin_bilisearch-0.2.0.tar", last modified: Mon Apr 29 13:57:02 2024, max compression
```

## Comparing `llmbot_plugin_bilisearch-0.1.5.tar` & `llmbot_plugin_bilisearch-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-11-14 14:49:15.051970 llmbot_plugin_bilisearch-0.1.5/LICENSE
--rw-r--r--   0        0        0      691 2023-11-14 14:49:15.051970 llmbot_plugin_bilisearch-0.1.5/README.md
--rw-r--r--   0        0        0     6040 2023-11-14 14:49:15.051970 llmbot_plugin_bilisearch-0.1.5/llmbot_plugin_bilisearch/__init__.py
--rw-r--r--   0        0        0      575 2023-11-14 14:49:15.051970 llmbot_plugin_bilisearch-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 llmbot_plugin_bilisearch-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2024-04-29 13:56:48.352428 llmbot_plugin_bilisearch-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0      645 2024-04-29 13:56:48.352428 llmbot_plugin_bilisearch-0.2.0/README.md
+-rwxr-xr-x   0        0        0     6089 2024-04-29 13:56:48.352428 llmbot_plugin_bilisearch-0.2.0/llmbot_plugin_bilisearch/__init__.py
+-rw-r--r--   0        0        0      565 2024-04-29 13:57:02.072682 llmbot_plugin_bilisearch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 llmbot_plugin_bilisearch-0.2.0/PKG-INFO
```

### Comparing `llmbot_plugin_bilisearch-0.1.5/LICENSE` & `llmbot_plugin_bilisearch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmbot_plugin_bilisearch-0.1.5/llmbot_plugin_bilisearch/__init__.py` & `llmbot_plugin_bilisearch-0.2.0/llmbot_plugin_bilisearch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 # -*- coding: utf-8 -*-
-__plugin_name__ = "search_in_bilibili"
-__openapi_version__ = "20231111"
-
-from typing import TYPE_CHECKING
-
-from llmkira.sdk import resign_plugin_executor
-from llmkira.sdk.func_calling import verify_openapi_version
-
-verify_openapi_version(__plugin_name__, __openapi_version__)
+from typing import Union, Type, List
 
 import inscriptis
-from llmkira.schema import RawMessage
-from llmkira.sdk.func_calling import BaseTool, PluginMetadata
-from llmkira.sdk.func_calling.schema import FuncPair
-from llmkira.sdk.schema import Function
-from llmkira.task import Task, TaskHeader
 from loguru import logger
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, Field
+from pydantic import ConfigDict
 
-if TYPE_CHECKING:
-    from llmkira.sdk.schema import TaskBatch
+__plugin_name__ = "search_in_bilibili"
+__openapi_version__ = "20240416"
 
+from llmkira.sdk.tools import verify_openapi_version  # noqa: E402
 
-class Bili(BaseModel):
-    """
-    Search videos on bilibili.com(哔哩哔哩)
-    """
-    keywords: str = Field(..., description="Keywords entered in the search box")
-    model_config = ConfigDict(extra="allow")
+verify_openapi_version(__plugin_name__, __openapi_version__)  # noqa: E402
+from llmkira.openai.cell import Tool, ToolCall, class_tool  # noqa: E402
+from llmkira.openapi.fuse import resign_plugin_executor  # noqa: E402
+from llmkira.sdk.tools import PluginMetadata  # noqa: E402
+from llmkira.sdk.tools.schema import FuncPair, BaseTool  # noqa: E402
+from llmkira.task import Task, TaskHeader  # noqa: E402
+from llmkira.task.schema import Location, ToolResponse, EventMessage  # noqa: E402
 
 
-bilibili = Function.parse_from_pydantic(schema_model=Bili, plugin_name=__plugin_name__)
+class BiliBiliSearch(BaseModel):
+    keywords: str = Field(description="question entered in the search website")
+    model_config = ConfigDict(extra="allow")
 
 
-@resign_plugin_executor(function=bilibili, handle_exceptions=(Exception,))
+@resign_plugin_executor(tool=BiliBiliSearch, handle_exceptions=(Exception,))
 async def search_on_bilibili(keywords):
     from bilibili_api import search
     logger.debug(f"Plugin:search_on_bilibili {keywords}")
     _result = await search.search_by_type(
         keyword=keywords,
         search_type=search.SearchObjectType.VIDEO,
         order_type=search.OrderVideo.TOTALRANK,
@@ -60,25 +52,34 @@
 
 
 class BiliBiliSearch(BaseTool):
     """
     搜索工具
     """
     silent: bool = True
-    function: Function = bilibili
+    function: Union[Tool, Type[BaseModel]] = BiliBiliSearch
     keywords: list = ["哔哩哔哩", "b站", "B站", "视频", '搜索', '新闻', 'bilibili']
-    require_auth: bool = False
 
-    def pre_check(self):
-        try:
-            import bilibili_api
-            return True
-        except ImportError as e:
-            logger.error(f"Plugin:bilibili:package <bilibili_api> not installed:{e}")
-            return False
+    def require_auth(self, env_map: dict) -> bool:
+        """
+        Auth or not
+        :param env_map: virtual env
+        :return:
+        """
+        return False
+
+    @classmethod
+    def env_help_docs(cls, empty_env: List[str]) -> str:
+        """
+        Provide help message for environment variables
+        :param empty_env: The environment variable list that not configured
+        :return: The help message
+        """
+        message = ""
+        return message
 
     def func_message(self, message_text, **kwargs):
         """
         如果合格则返回message，否则返回None，表示不处理
         """
         for i in self.keywords:
             if i in message_text:
@@ -86,95 +87,103 @@
         # 正则匹配
         if self.pattern:
             match = self.pattern.match(message_text)
             if match:
                 return self.function
         return None
 
-    async def failed(self,
-                     task: "TaskHeader", receiver: "TaskHeader.Location",
-                     exception,
-                     env: dict,
-                     arg: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                     **kwargs
-                     ):
-        _meta = task.task_meta.reply_notify(
+    async def failed(
+            self,
+            task: "TaskHeader",
+            receiver: "Location",
+            exception,
+            env: dict,
+            arg: dict,
+            pending_task: "ToolCall",
+            refer_llm_result: dict = None,
+            **kwargs,
+    ):
+        meta = task.task_sign.reply(
             plugin_name=__plugin_name__,
-            callback=[TaskHeader.Meta.Callback.create(
-                name=__plugin_name__,
-                function_response=f"Run Failed --{exception}",
-                tool_call_id=pending_task.get_batch_id()
-            )
+            tool_response=[
+                ToolResponse(
+                    name=__plugin_name__,
+                    function_response=f"Run Failed {exception}",
+                    tool_call_id=pending_task.id,
+                    tool_call=pending_task,
+                )
             ],
-            write_back=True,
-            release_chain=True
         )
-        logger.error(f"Plugin:{__plugin_name__} Run Failed:{exception}")
         await Task.create_and_send(
             queue_name=receiver.platform,
             task=TaskHeader(
                 sender=task.sender,
                 receiver=receiver,
-                task_meta=_meta,
+                task_sign=meta,
                 message=[
-                    RawMessage(
+                    EventMessage(
                         user_id=receiver.user_id,
                         chat_id=receiver.chat_id,
-                        text="Can't speak Chinese"
+                        text=f"🍖{__plugin_name__} Run Failed：{exception},report it to user.",
                     )
-                ]
-            )
+                ],
+            ),
         )
 
-    async def callback(self,
-                       task: "TaskHeader", receiver: "TaskHeader.Location",
-                       env: dict,
-                       arg: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                       **kwargs
-                       ):
-        return None
-
-    async def run(self,
-                  task: "TaskHeader", receiver: "TaskHeader.Location",
-                  arg: dict, env: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                  ):
+    async def callback(
+            self,
+            task: "TaskHeader",
+            receiver: "Location",
+            env: dict,
+            arg: dict,
+            pending_task: "ToolCall",
+            refer_llm_result: dict = None,
+            **kwargs,
+    ):
+        return True
+
+    async def run(
+            self,
+            task: "TaskHeader",
+            receiver: "Location",
+            arg: dict,
+            env: dict,
+            pending_task: "ToolCall",
+            refer_llm_result: dict = None,
+    ):
         """
         处理message，返回message
         """
 
-        _set = Bili.model_validate(arg)
+        _set = BiliBiliSearch.model_validate(arg)
         _search_result = await search_on_bilibili(_set.keywords)
-        _meta = task.task_meta.reply_raw(
+        _meta = task.task_sign.reprocess(
             plugin_name=__plugin_name__,
-            callback=[
-                TaskHeader.Meta.Callback.create(
+            tool_response=[
+                ToolResponse(
                     name=__plugin_name__,
-                    function_response=f"Run Success",
-                    tool_call_id=pending_task.get_batch_id()
+                    function_response=f"SearchData: {_search_result},Please give reference link when use it.",
+                    tool_call_id=pending_task.id,
+                    tool_call=pending_task,
                 )
             ]
         )
-        await Task(queue=receiver.platform).send_task(
+        await Task.create_and_send(
+            queue_name=receiver.platform,
             task=TaskHeader(
                 sender=task.sender,  # 继承发送者
                 receiver=receiver,  # 因为可能有转发，所以可以单配
-                task_meta=_meta,
-                message=[
-                    RawMessage(
-                        user_id=receiver.user_id,
-                        chat_id=receiver.chat_id,
-                        text=_search_result
-                    )
-                ]
-            )
+                task_sign=_meta,
+                message=[],
+            ),
         )
 
 
 __plugin_meta__ = PluginMetadata(
     name=__plugin_name__,
     description="Search videos on bilibili.com(哔哩哔哩)",
     usage="bilibili search <keywords>",
     openapi_version=__openapi_version__,
     function={
-        FuncPair(function=bilibili, tool=BiliBiliSearch)
+        FuncPair(function=class_tool(BiliBiliSearch), tool=BiliBiliSearch)
     }
 )
```

