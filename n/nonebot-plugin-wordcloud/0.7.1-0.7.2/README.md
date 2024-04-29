# Comparing `tmp/nonebot_plugin_wordcloud-0.7.1.tar.gz` & `tmp/nonebot_plugin_wordcloud-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wordcloud-0.7.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_wordcloud-0.7.2.tar", max compression
```

## Comparing `nonebot_plugin_wordcloud-0.7.1.tar` & `nonebot_plugin_wordcloud-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1067 2024-03-24 07:19:09.343802 nonebot_plugin_wordcloud-0.7.1/LICENSE
--rw-r--r--   0        0        0    13342 2024-03-24 07:19:09.347802 nonebot_plugin_wordcloud-0.7.1/README.md
--rw-r--r--   0        0        0  8331636 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/SourceHanSans.otf
--rw-r--r--   0        0        0    12932 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/__init__.py
--rw-r--r--   0        0        0      509 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/compat.py
--rw-r--r--   0        0        0     2351 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/config.py
--rw-r--r--   0        0        0     3944 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/data_source.py
--rw-r--r--   0        0        0     1294 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/migrations/557fef3a156f_init_db.py
--rw-r--r--   0        0        0        0 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/migrations/__init__.py
--rw-r--r--   0        0        0     3259 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/migrations/ade8cdca5470_migrate_datastore_data.py
--rw-r--r--   0        0        0      622 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/model.py
--rw-r--r--   0        0        0     6715 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/schedule.py
--rw-r--r--   0        0        0     3179 2024-03-24 07:19:09.399802 nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/utils.py
--rw-r--r--   0        0        0     2626 2024-03-24 07:19:09.403802 nonebot_plugin_wordcloud-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 nonebot_plugin_wordcloud-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-29 14:20:05.582695 nonebot_plugin_wordcloud-0.7.2/LICENSE
+-rw-r--r--   0        0        0    13342 2024-04-29 14:20:05.586695 nonebot_plugin_wordcloud-0.7.2/README.md
+-rw-r--r--   0        0        0  8331636 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/SourceHanSans.otf
+-rw-r--r--   0        0        0    12932 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/compat.py
+-rw-r--r--   0        0        0     2334 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/config.py
+-rw-r--r--   0        0        0     3932 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/data_source.py
+-rw-r--r--   0        0        0     1294 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/migrations/557fef3a156f_init_db.py
+-rw-r--r--   0        0        0        0 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/migrations/__init__.py
+-rw-r--r--   0        0        0     3259 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/migrations/ade8cdca5470_migrate_datastore_data.py
+-rw-r--r--   0        0        0      622 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/model.py
+-rw-r--r--   0        0        0     6832 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/schedule.py
+-rw-r--r--   0        0        0     3179 2024-04-29 14:20:05.638695 nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/utils.py
+-rw-r--r--   0        0        0     2618 2024-04-29 14:20:05.642695 nonebot_plugin_wordcloud-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 nonebot_plugin_wordcloud-0.7.2/PKG-INFO
```

### Comparing `nonebot_plugin_wordcloud-0.7.1/LICENSE` & `nonebot_plugin_wordcloud-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/README.md` & `nonebot_plugin_wordcloud-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/SourceHanSans.otf` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/SourceHanSans.otf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/__init__.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/config.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime, time
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Union
+from typing import Any, Optional, Union
 from zoneinfo import ZoneInfo
 
 from nonebot import get_driver, get_plugin_config
 from nonebot_plugin_localstore import get_data_dir
 from pydantic import BaseModel
 
 from .compat import model_validator
@@ -12,26 +12,26 @@
 DATA_DIR = get_data_dir("nonebot_plugin_wordcloud")
 
 
 class Config(BaseModel):
     wordcloud_width: int = 1920
     wordcloud_height: int = 1200
     wordcloud_background_color: str = "black"
-    wordcloud_colormap: Union[str, List[str]] = "viridis"
+    wordcloud_colormap: Union[str, list[str]] = "viridis"
     wordcloud_font_path: str
     wordcloud_stopwords_path: Optional[Path] = None
     wordcloud_userdict_path: Optional[Path] = None
     wordcloud_timezone: Optional[str] = None
     wordcloud_default_schedule_time: time
     """ 默认定时发送时间
 
     如果群内不单独设置则使用这个值，默认为晚上 10 点，时区为设定的时区
     """
-    wordcloud_options: Dict[str, Any] = {}
-    wordcloud_exclude_user_ids: Set[str] = set()
+    wordcloud_options: dict[str, Any] = {}
+    wordcloud_exclude_user_ids: set[str] = set()
     """排除的用户 ID 列表（全局，不区分平台）"""
 
     @model_validator(mode="before")
     def set_default_values(cls, values):
         if not values.get("wordcloud_font_path"):
             values["wordcloud_font_path"] = str(
                 Path(__file__).parent / "SourceHanSans.otf"
```

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/data_source.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import concurrent.futures
 import contextlib
 import re
 from functools import partial
 from io import BytesIO
 from random import choice
-from typing import Dict, List, Optional
+from typing import Optional
 
 import jieba
 import jieba.analyse
 import numpy as np
 from emoji import replace_emoji
 from PIL import Image
 from wordcloud import WordCloud
@@ -33,15 +33,15 @@
     # 去除 emoji
     # https://github.com/carpedm20/emoji
     msg = replace_emoji(msg)
 
     return msg
 
 
-def analyse_message(msg: str) -> Dict[str, float]:
+def analyse_message(msg: str) -> dict[str, float]:
     """分析消息
 
     分词，并统计词频
     """
     # 设置停用词表
     if plugin_config.wordcloud_stopwords_path:
         jieba.analyse.set_stop_words(plugin_config.wordcloud_stopwords_path)
@@ -61,15 +61,15 @@
         return np.array(Image.open(mask_path))
     # 如果指定 mask 文件不存在，则尝试默认 mask
     default_mask_path = plugin_config.get_mask_path()
     if default_mask_path.exists():
         return np.array(Image.open(default_mask_path))
 
 
-def _get_wordcloud(messages: List[str], mask_key: str) -> Optional[bytes]:
+def _get_wordcloud(messages: list[str], mask_key: str) -> Optional[bytes]:
     # 过滤掉命令
     command_start = tuple(i for i in global_config.command_start if i)
     message = " ".join(m for m in messages if not m.startswith(command_start))
     # 预处理
     message = pre_precess(message)
     # 分析消息。分词，并统计词频
     frequency = analyse_message(message)
@@ -94,14 +94,14 @@
         wordcloud = WordCloud(**wordcloud_options)
         image = wordcloud.generate_from_frequencies(frequency).to_image()
         image_bytes = BytesIO()
         image.save(image_bytes, format="PNG")
         return image_bytes.getvalue()
 
 
-async def get_wordcloud(messages: List[str], mask_key: str) -> Optional[bytes]:
+async def get_wordcloud(messages: list[str], mask_key: str) -> Optional[bytes]:
     loop = asyncio.get_running_loop()
     pfunc = partial(_get_wordcloud, messages, mask_key)
     # 虽然不知道具体是哪里泄漏了，但是通过每次关闭线程池可以避免这个问题
     # https://github.com/he0119/nonebot-plugin-wordcloud/issues/99
     with concurrent.futures.ThreadPoolExecutor() as pool:
         return await loop.run_in_executor(pool, pfunc)
```

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/migrations/557fef3a156f_init_db.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/migrations/557fef3a156f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/migrations/ade8cdca5470_migrate_datastore_data.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/migrations/ade8cdca5470_migrate_datastore_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/model.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/schedule.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import time
-from typing import Dict, Optional, Tuple
+from typing import Optional
 
 import nonebot_plugin_saa as saa
 from apscheduler.job import Job
 from nonebot.compat import model_dump
 from nonebot.log import logger
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_cesaa import get_messages_plain_text
@@ -25,15 +25,15 @@
 saa.enable_auto_select_bot()
 
 
 class Scheduler:
     def __init__(self):
         # 默认定时任务的 key 为 default
         # 其他则为 ISO 8601 格式的时间字符串
-        self.schedules: Dict[str, Job] = {}
+        self.schedules: dict[str, Job] = {}
 
         # 转换到 APScheduler 的时区
         scheduler_time = get_time_with_scheduler_timezone(
             plugin_config.wordcloud_default_schedule_time
         )
         # 添加默认定时任务
         self.schedules["default"] = scheduler.add_job(
@@ -97,19 +97,24 @@
                     target=target,
                     types=["message"],
                     time_start=start,
                     time_stop=stop,
                     exclude_id1s=plugin_config.wordcloud_exclude_user_ids,
                 )
                 mask_key = get_mask_key(target)
-                if not (image := await get_wordcloud(messages, mask_key)):
-                    await saa.Text("今天没有足够的数据生成词云").send_to(target)
-                    continue
 
-                await saa.Image(image).send_to(target)
+                if image := await get_wordcloud(messages, mask_key):
+                    msg = saa.Image(image)
+                else:
+                    msg = saa.Text("今天没有足够的数据生成词云")
+
+                try:
+                    await msg.send_to(target)
+                except Exception:
+                    logger.exception(f"{target} 发送词云失败")
 
     async def get_schedule(self, target: saa.PlatformTarget) -> Optional[time]:
         """获取定时任务时间"""
         async with get_session() as session:
             statement = self.select_target_statement(target, session)
             results = await session.scalars(statement)
             if schedule := results.one_or_none():
@@ -151,15 +156,15 @@
             if schedule := results.one_or_none():
                 await session.delete(schedule)
                 await session.commit()
 
     @staticmethod
     def select_target_statement(
         target: saa.PlatformTarget, session: AsyncSession
-    ) -> Select[Tuple[Schedule]]:
+    ) -> Select[tuple[Schedule]]:
         """获取查询目标的语句
 
         MySQL 需要手动将 JSON 类型的字段转换为 JSON 类型
         """
         engine = session.get_bind()
         if engine.dialect.name == "mysql":
             return select(Schedule).where(
```

### Comparing `nonebot_plugin_wordcloud-0.7.1/nonebot_plugin_wordcloud/utils.py` & `nonebot_plugin_wordcloud-0.7.2/nonebot_plugin_wordcloud/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordcloud-0.7.1/pyproject.toml` & `nonebot_plugin_wordcloud-0.7.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-wordcloud"
-version = "0.7.1"
+version = "0.7.2"
 description = "适用于 NoneBot2 的词云插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-wordcloud"
 repository = "https://github.com/he0119/nonebot-plugin-wordcloud"
 documentation = "https://github.com/he0119/nonebot-plugin-wordcloud#readme"
@@ -22,53 +22,53 @@
 tzdata = "*"
 emoji = ">=1.6.3,<3.0.0"
 
 nonebot-plugin-datastore = { version = ">=1.2.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.4.0"
-nonebug = "^0.3.1"
-nonebug-saa = "^0.4.0"
+nonebug = "^0.3.7"
+nonebug-saa = "^0.4.1"
 nonebot-adapter-onebot = "^2.2.4"
 nonebot-plugin-orm = { extras = ["default"], version = ">=0.7.0" }
 nonebot-plugin-datastore = "^1.2.0"
-pytest-cov = "^4.0.0"
-pytest-xdist = "^3.1.0"
-pytest-mock = "^3.7.0"
-pytest-asyncio = "^0.21.0"
 asyncpg = "*"
 aiomysql = "*"
-respx = "^0.20.2"
-httpx = ">=0.24.1,<0.26.0"
-gevent = "^23.7.0"
+pytest-cov = ">=4,<6"
+pytest-xdist = "^3.1.0"
+pytest-mock = "^3.7.0"
+pytest-asyncio = ">=0.21,<0.24"
+respx = ">=0.20.2,<0.22.0"
+httpx = ">=0.24.1,<0.28.0"
+gevent = ">=23.7,<25.0"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_wordcloud"]
 adapters = [
   { name = "OneBot V12", module_name = "nonebot.adapters.onebot.v12", project_link = "nonebot-adapter-onebot", desc = "OneBot V12 协议" },
   { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11", project_link = "nonebot-adapter-onebot", desc = "OneBot V11 协议" },
 ]
 
-[tool.black]
-line-length = 88
-
-[tool.isort]
-profile = "black"
-line_length = 88
-skip_gitignore = true
-
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.pyright]
 pythonVersion = "3.9"
 pythonPlatform = "All"
-typeCheckingMode = "basic"
+typeCheckingMode = "standard"
 defineConstant = { PYDANTIC_V2 = true }
 
+[tool.ruff]
+line-length = 88
+target-version = "py39"
+
 [tool.ruff.lint]
 select = [
   "W",   # pycodestyle warnings
   "E",   # pycodestyle errors
   "F",   # Pyflakes
   "UP",  # pyupgrade
   "C4",  # flake8-comprehensions
@@ -84,12 +84,8 @@
 ]
 
 [tool.coverage.run]
 # https://github.com/nedbat/coveragepy/issues/1082
 concurrency = ["thread", "gevent"]
 
 [tool.coverage.report]
-omit = ["*/compat.py"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+omit = ["*/compat.py", "*/migrations/*"]
```

### Comparing `nonebot_plugin_wordcloud-0.7.1/PKG-INFO` & `nonebot_plugin_wordcloud-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-wordcloud
-Version: 0.7.1
+Version: 0.7.2
 Summary: 适用于 NoneBot2 的词云插件
 Home-page: https://github.com/he0119/nonebot-plugin-wordcloud
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-wordcloud Version: 0.7.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-wordcloud Version: 0.7.2 Summary:
 éç¨äº NoneBot2 çè¯äºæä»¶ Home-page: https://github.com/he0119/
 nonebot-plugin-wordcloud License: MIT Author: hemengyang Author-email:
 hmy0119@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: emoji
```

