# Comparing `tmp/nonebot_adapter_qq-1.4.3.tar.gz` & `tmp/nonebot_adapter_qq-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_qq-1.4.3.tar", max compression
+gzip compressed data, was "nonebot_adapter_qq-1.4.4.tar", max compression
```

## Comparing `nonebot_adapter_qq-1.4.3.tar` & `nonebot_adapter_qq-1.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/LICENSE
--rw-r--r--   0        0        0     1609 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/README.md
--rw-r--r--   0        0        0      787 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/__init__.py
--rw-r--r--   0        0        0    14410 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/adapter.py
--rw-r--r--   0        0        0    60571 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/bot.py
--rw-r--r--   0        0        0      768 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/compat.py
--rw-r--r--   0        0        0     2148 2024-03-29 16:07:04.058552 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/config.py
--rw-r--r--   0        0        0    18754 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/event.py
--rw-r--r--   0        0        0     2701 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/exception.py
--rw-r--r--   0        0        0    11292 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/message.py
--rw-r--r--   0        0        0      537 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/__init__.py
--rw-r--r--   0        0        0     4046 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/common.py
--rw-r--r--   0        0        0    11973 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/guild.py
--rw-r--r--   0        0        0     2819 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/payload.py
--rw-r--r--   0        0        0     1859 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/qq.py
--rw-r--r--   0        0        0      988 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/permission.py
--rw-r--r--   0        0        0      874 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/store.py
--rw-r--r--   0        0        0     1568 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/utils.py
--rw-r--r--   0        0        0     1559 2024-03-29 16:07:04.062553 nonebot_adapter_qq-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 nonebot_adapter_qq-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-29 03:46:30.987344 nonebot_adapter_qq-1.4.4/LICENSE
+-rw-r--r--   0        0        0     1609 2024-04-29 03:46:30.987344 nonebot_adapter_qq-1.4.4/README.md
+-rw-r--r--   0        0        0      787 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/__init__.py
+-rw-r--r--   0        0        0    14464 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/adapter.py
+-rw-r--r--   0        0        0    60571 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/bot.py
+-rw-r--r--   0        0        0      768 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/compat.py
+-rw-r--r--   0        0        0     2148 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/config.py
+-rw-r--r--   0        0        0    18754 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/event.py
+-rw-r--r--   0        0        0     2701 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/exception.py
+-rw-r--r--   0        0        0    11292 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/message.py
+-rw-r--r--   0        0        0      537 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/__init__.py
+-rw-r--r--   0        0        0     4468 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/common.py
+-rw-r--r--   0        0        0    11692 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/guild.py
+-rw-r--r--   0        0        0     2819 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/payload.py
+-rw-r--r--   0        0        0     1859 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/qq.py
+-rw-r--r--   0        0        0      988 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/permission.py
+-rw-r--r--   0        0        0      874 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/store.py
+-rw-r--r--   0        0        0     1568 2024-04-29 03:46:30.991344 nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/utils.py
+-rw-r--r--   0        0        0     1559 2024-04-29 03:46:30.995344 nonebot_adapter_qq-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 nonebot_adapter_qq-1.4.4/PKG-INFO
```

### Comparing `nonebot_adapter_qq-1.4.3/LICENSE` & `nonebot_adapter_qq-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/README.md` & `nonebot_adapter_qq-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/__init__.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/adapter.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
-import json
 import asyncio
 from typing_extensions import override
 from typing import Any, List, Tuple, Literal, Optional
 
 from nonebot.utils import escape_tag
 from nonebot.exception import WebSocketClosed
-from nonebot.compat import PYDANTIC_V2, type_validate_python
+from nonebot.compat import PYDANTIC_V2, type_validate_json, type_validate_python
 from nonebot.drivers import (
     URL,
     Driver,
     Request,
     WebSocket,
     HTTPClientMixin,
     WebSocketClientMixin,
@@ -64,15 +63,15 @@
             )
         if not isinstance(self.driver, WebSocketClientMixin):
             raise RuntimeError(
                 f"Current driver {self.config.driver} does not support "
                 "websocket client! "
                 "QQ Adapter need a WebSocketClient Driver to work."
             )
-        self.driver.on_startup(self.startup)
+        self.on_ready(self.startup)
         self.driver.on_shutdown(self.shutdown)
 
     async def startup(self) -> None:
         log(
             "DEBUG",
             ("QQ run in sandbox mode: " f"<y>{self.qq_config.qq_is_sandbox}</y>"),
         )
@@ -237,37 +236,39 @@
             )
 
     async def _authenticate(
         self, bot: Bot, ws: WebSocket, shard: Tuple[int, int]
     ) -> Optional[Literal[True]]:
         """鉴权连接"""
         if not bot.ready:
-            payload = Identify.parse_obj(
+            payload = type_validate_python(
+                Identify,
                 {
                     "data": {
                         "token": await bot._get_authorization_header(),
                         "intents": bot.bot_info.intent.to_int(),
                         "shard": shard,
                         "properties": {
                             "$os": sys.platform,
                             "$language": f"python {sys.version}",
                             "$sdk": "NoneBot2",
                         },
-                    },
-                }
+                    }
+                },
             )
         else:
-            payload = Resume.parse_obj(
+            payload = type_validate_python(
+                Resume,
                 {
                     "data": {
                         "token": await bot._get_authorization_header(),
                         "session_id": bot.session_id,
                         "seq": bot.sequence,
                     }
-                }
+                },
             )
 
         try:
             await ws.send(self.payload_to_json(payload))
         except Exception as e:
             log(
                 "ERROR",
@@ -322,15 +323,15 @@
         return True
 
     async def _heartbeat(self, bot: Bot, ws: WebSocket, heartbeat_interval: int):
         """心跳"""
         while True:
             if bot.ready:
                 log("TRACE", f"Heartbeat {bot.sequence}")
-                payload = Heartbeat.parse_obj({"data": bot.sequence})
+                payload = type_validate_python(Heartbeat, {"data": bot.sequence})
                 try:
                     await ws.send(self.payload_to_json(payload))
                 except Exception as e:
                     log("WARNING", "Error while sending heartbeat, Ignored!", e)
             await asyncio.sleep(heartbeat_interval / 1000)
 
     async def _loop(self, bot: Bot, ws: WebSocket):
@@ -383,15 +384,15 @@
         if self.qq_config.qq_is_sandbox:
             return URL(str(self.qq_config.qq_sandbox_api_base))
         else:
             return URL(str(self.qq_config.qq_api_base))
 
     @staticmethod
     async def receive_payload(bot: Bot, ws: WebSocket) -> Payload:
-        payload = type_validate_python(PayloadType, json.loads(await ws.receive()))
+        payload = type_validate_json(PayloadType, await ws.receive())
         if isinstance(payload, Dispatch):
             bot.on_dispatch(payload)
         return payload
 
     @staticmethod
     def payload_to_json(payload: Payload) -> str:
         if PYDANTIC_V2:
```

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/bot.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/compat.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/config.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/event.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/exception.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/message.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/__init__.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/common.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from urllib.parse import urlparse
 from typing import List, Literal, Optional
 
 from pydantic import BaseModel
 
 from nonebot.adapters.qq.compat import field_validator
 
@@ -115,14 +116,27 @@
 
 
 class MessageKeyboard(BaseModel):
     id: Optional[str] = None
     content: Optional[InlineKeyboard] = None
 
 
+# Message Audit Event
+class MessageAudited(BaseModel):
+    audit_id: str
+    message_id: Optional[str] = None
+    user_openid: Optional[str] = None
+    group_openid: Optional[str] = None
+    guild_id: Optional[str] = None
+    channel_id: Optional[str] = None
+    audit_time: datetime
+    create_time: Optional[datetime] = None
+    seq_in_channel: Optional[str] = None
+
+
 # Interaction Event
 class ButtonInteractionContent(BaseModel):
     user_id: Optional[str] = None
     message_id: Optional[str] = None
     feature_id: Optional[str] = None
     button_id: Optional[str] = None
     button_data: Optional[str] = None
@@ -163,11 +177,12 @@
     "Permission",
     "Action",
     "RenderData",
     "Button",
     "InlineKeyboardRow",
     "InlineKeyboard",
     "MessageKeyboard",
+    "MessageAudited",
     "ButtonInteractionContent",
     "ButtonInteractionData",
     "ButtonInteraction",
 ]
```

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/guild.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/guild.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,25 +158,14 @@
 
 # Message Delete Event
 class MessageDelete(BaseModel):
     message: Message
     op_user: User
 
 
-# Message Audit Event
-class MessageAudited(BaseModel):
-    audit_id: str
-    message_id: Optional[str] = None
-    guild_id: str
-    channel_id: str
-    audit_time: datetime
-    create_time: Optional[datetime] = None
-    seq_in_channel: Optional[str] = None
-
-
 # Message Setting
 class MessageSetting(BaseModel):
     disable_create_dm: bool
     disable_push_msg: bool
     channel_ids: List[str]
     channel_push_max_num: int
 
@@ -521,15 +510,14 @@
     "Role",
     "GetGuildRolesReturn",
     "PostGuildRoleReturn",
     "PatchGuildRoleReturn",
     "ChannelPermissions",
     "Message",
     "MessageDelete",
-    "MessageAudited",
     "MessageSetting",
     "DMS",
     "RecommendChannel",
     "Announces",
     "PinsMessage",
     "RemindType",
     "Schedule",
```

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/payload.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/models/qq.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/models/qq.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/permission.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/store.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/nonebot/adapters/qq/utils.py` & `nonebot_adapter_qq-1.4.4/nonebot/adapters/qq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qq-1.4.3/pyproject.toml` & `nonebot_adapter_qq-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-qq"
-version = "1.4.3"
+version = "1.4.4"
 description = "QQ adapter for nonebot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/adapter-qq"
 repository = "https://github.com/nonebot/adapter-qq"
 documentation = "https://github.com/nonebot/adapter-qq#readme"
@@ -17,20 +17,20 @@
   "Programming Language :: Python :: 3",
 ]
 packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 yarl = "^1.9.0"
-nonebot2 = "^2.2.0"
+nonebot2 = "^2.2.1"
 typing-extensions = ">=4.4.0, <5.0.0"
 pydantic = ">=1.10.0,<3.0.0,!=2.5.0,!=2.5.1"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 isort = "^5.10.1"
 black = "^24.0.0"
 nonemoji = "^0.1.3"
 pre-commit = "^3.3.0"
 
 [tool.black]
 line-length = 88
```

### Comparing `nonebot_adapter_qq-1.4.3/PKG-INFO` & `nonebot_adapter_qq-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-qq
-Version: 1.4.3
+Version: 1.4.4
 Summary: QQ adapter for nonebot2
 Home-page: https://github.com/nonebot/adapter-qq
 License: MIT
 Keywords: bot,qq,qqbot,qqguild
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
+Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic (>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: yarl (>=1.9.0,<2.0.0)
 Project-URL: Documentation, https://github.com/nonebot/adapter-qq#readme
 Project-URL: Repository, https://github.com/nonebot/adapter-qq
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-qq Version: 1.4.3 Summary: QQ
+Metadata-Version: 2.1 Name: nonebot-adapter-qq Version: 1.4.4 Summary: QQ
 adapter for nonebot2 Home-page: https://github.com/nonebot/adapter-qq License:
 MIT Keywords: bot,qq,qqbot,qqguild Author: yanyongyu Author-email:
 yyy@nonebot.dev Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: nonebot2 (>=2.2.0,<3.0.0) Requires-Dist: pydantic
+Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: pydantic
 (>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1) Requires-Dist: typing-extensions
 (>=4.4.0,<5.0.0) Requires-Dist: yarl (>=1.9.0,<2.0.0) Project-URL:
 Documentation, https://github.com/nonebot/adapter-qq#readme Project-URL:
 Repository, https://github.com/nonebot/adapter-qq Description-Content-Type:
 text/markdown
                              _[_n_o_n_e_b_o_t_-_a_d_a_p_t_e_r_-_q_q_]
                 # NoneBot-Adapter-QQ _â¨ QQ åè®®éé â¨_
```

