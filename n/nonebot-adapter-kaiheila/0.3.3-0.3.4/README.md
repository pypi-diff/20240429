# Comparing `tmp/nonebot_adapter_kaiheila-0.3.3.tar.gz` & `tmp/nonebot_adapter_kaiheila-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_kaiheila-0.3.3.tar", max compression
+gzip compressed data, was "nonebot_adapter_kaiheila-0.3.4.tar", max compression
```

## Comparing `nonebot_adapter_kaiheila-0.3.3.tar` & `nonebot_adapter_kaiheila-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2024-03-12 14:37:58.649452 nonebot_adapter_kaiheila-0.3.3/LICENSE
--rw-r--r--   0        0        0      296 2024-03-12 14:37:58.649452 nonebot_adapter_kaiheila-0.3.3/README.md
--rw-r--r--   0        0        0      358 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/__init__.py
--rw-r--r--   0        0        0    18261 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/adapter.py
--rw-r--r--   0        0        0       66 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/__init__.py
--rw-r--r--   0        0        0       27 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/client.py
--rw-r--r--   0        0        0     9726 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/client.pyi
--rw-r--r--   0        0        0     4663 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/handle.py
--rw-r--r--   0        0        0    15134 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/model.py
--rw-r--r--   0        0        0    12163 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/bot.py
--rw-r--r--   0        0        0      525 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/compat.py
--rw-r--r--   0        0        0     1358 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/config.py
--rw-r--r--   0        0        0    27338 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/event.py
--rw-r--r--   0        0        0     3425 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/exception.py
--rw-r--r--   0        0        0    28933 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/message.py
--rw-r--r--   0        0        0      488 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/permission.py
--rw-r--r--   0        0        0     2560 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/utils.py
--rw-r--r--   0        0        0     1347 2024-03-12 14:37:58.653452 nonebot_adapter_kaiheila-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/LICENSE
+-rw-r--r--   0        0        0      296 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/README.md
+-rw-r--r--   0        0        0      358 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/__init__.py
+-rw-r--r--   0        0        0    18261 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/adapter.py
+-rw-r--r--   0        0        0       66 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/client.py
+-rw-r--r--   0        0        0     9726 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/client.pyi
+-rw-r--r--   0        0        0     4663 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/handle.py
+-rw-r--r--   0        0        0    15165 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/model.py
+-rw-r--r--   0        0        0    12163 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/bot.py
+-rw-r--r--   0        0        0      525 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/compat.py
+-rw-r--r--   0        0        0     1358 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/config.py
+-rw-r--r--   0        0        0    27338 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/event.py
+-rw-r--r--   0        0        0     3425 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/exception.py
+-rw-r--r--   0        0        0    28933 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/message.py
+-rw-r--r--   0        0        0      488 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/permission.py
+-rw-r--r--   0        0        0     2560 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/utils.py
+-rw-r--r--   0        0        0     1347 2024-04-29 12:26:47.557890 nonebot_adapter_kaiheila-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.3.4/PKG-INFO
```

### Comparing `nonebot_adapter_kaiheila-0.3.3/LICENSE` & `nonebot_adapter_kaiheila-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/adapter.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/client.pyi` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/handle.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/api/model.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,27 +298,27 @@
     """消息 ID"""
     type: Optional[int] = None
     """消息类型"""
     content: Optional[str] = None
     """消息内容"""
     embeds: Optional[List[dict]] = None
     """超链接解析数据"""
-    attachments: Optional[Union[bool, Attachments]] = None
+    attachments: Optional[Union[bool, Attachments, List[Attachments]]] = None
     """附加的多媒体数据"""
     create_at: Optional[int] = None
     """创建时间"""
     updated_at: Optional[int] = None
     """更新时间"""
     reactions: Optional[List[Reaction]] = None
     """回应数据"""
     image_name: Optional[str] = None
     """"""
     read_status: Optional[bool] = None
     """是否已读"""
-    quote: Optional[Quote] = None
+    quote: Optional[Union[str, Quote]] = None
     """引用数据"""
     mention_info: Optional[MentionInfo] = None
     """引用特定用户或特定角色的信息"""
 
 
 class ChannelMessage(BaseMessage):
     """频道消息"""
```

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/bot.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/compat.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/config.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/event.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 class Extra(BaseModel):
     type_: Union[int, str] = Field(None, alias="type")
     guild_id: Optional[str] = Field(None)
     channel_name: Optional[str] = Field(None)
     mention: Optional[List[str]] = Field(None)
     mention_all: Optional[bool] = Field(None)
-    mention_roles: Optional[List[str]] = Field(None)
+    mention_roles: Optional[List[int]] = Field(None)
     mention_here: Optional[bool] = Field(None)
     author: Optional[User] = Field(None)
     body: Optional[AttrDict] = Field(None)
     attachments: Optional[Attachment] = Field(None)
     code: Optional[str] = Field(None)
 
     @validator("body", pre=True)
```

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/exception.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/message.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/nonebot/adapters/kaiheila/utils.py` & `nonebot_adapter_kaiheila-0.3.4/nonebot/adapters/kaiheila/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.3.3/pyproject.toml` & `nonebot_adapter_kaiheila-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-kaiheila"
-version = "0.3.3"
+version = "0.3.4"
 description = "kaiheila adapter for nonebot2"
 authors = ["Tian-que <1605206150@qq.com>", "ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tian-que/nonebot-adapter-kaiheila"
 keywords = ["bot", "khl", "kaiheila", "khlbot"]
```

### Comparing `nonebot_adapter_kaiheila-0.3.3/PKG-INFO` & `nonebot_adapter_kaiheila-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-kaiheila
-Version: 0.3.3
+Version: 0.3.4
 Summary: kaiheila adapter for nonebot2
 Home-page: https://github.com/Tian-que/nonebot-adapter-kaiheila
 License: MIT
 Keywords: bot,khl,kaiheila,khlbot
 Author: Tian-que
 Author-email: 1605206150@qq.com
 Requires-Python: >=3.8,<4.0
```

