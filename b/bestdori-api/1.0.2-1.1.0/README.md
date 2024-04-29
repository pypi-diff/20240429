# Comparing `tmp/bestdori-api-1.0.2.tar.gz` & `tmp/bestdori-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori-api-1.0.2.tar", last modified: Fri Apr 26 16:48:20 2024, max compression
+gzip compressed data, was "bestdori-api-1.1.0.tar", last modified: Mon Apr 29 04:21:49 2024, max compression
```

## Comparing `bestdori-api-1.0.2.tar` & `bestdori-api-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.212263 bestdori-api-1.0.2/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.212263 bestdori-api-1.0.2/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/ayachan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/ayachan/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    20223 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/missions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/bestdori/models/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/models/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/models/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-26 16:48:19.000000 bestdori-api-1.0.2/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 16:48:20.000000 bestdori-api-1.0.2/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:48:19.000000 bestdori-api-1.0.2/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 16:48:19.000000 bestdori-api-1.0.2/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:48:20.216263 bestdori-api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-26 16:48:08.000000 bestdori-api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.050933 bestdori-api-1.1.0/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.050933 bestdori-api-1.1.0/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22526 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/festival.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/missions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/models/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-29 04:21:48.000000 bestdori-api-1.1.0/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-29 04:21:49.000000 bestdori-api-1.1.0/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:21:48.000000 bestdori-api-1.1.0/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 04:21:48.000000 bestdori-api-1.1.0/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/setup.py
```

### Comparing `bestdori-api-1.0.2/LICENSE` & `bestdori-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/PKG-INFO` & `bestdori-api-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -48,26 +48,26 @@
         
         ### 目前已有的 API 与功能
         
         |API 类别|是否完善|支持的内容|
         |:-------|:-----:|:------|
         |用户|👍👍|登录、查询、帖子获取、信息获取|
         |玩家|👍|信息获取|
-        |帖子|👍👍|搜索、获取、发表、评论、喜欢|
+        |帖子|👍👍👍|搜索、获取、发表、评论、喜欢|
         |谱面|👍👍👍|社区谱面获取、音源与封面获取、规整化、数据统计、格式互转|
         |故事|👍|社区故事获取|
-        |角色|👍|信息获取、资源获取|
-        |卡牌|👍|信息获取、资源获取|
-        |服装|👍|信息获取|
-        |活动|👍|信息获取、资源获取|
+        |角色|👍👍|信息获取、资源获取|
+        |卡牌|👍👍|信息获取、资源获取|
+        |服装|👍👍|信息获取、资源获取|
+        |活动|👍👍|信息获取、资源获取|
         |活动数据|👍|数据获取|
-        |招募|👍|数据获取、资源获取|
-        |歌曲|👍|信息获取、资源获取|
+        |招募|👍👍|数据获取、资源获取|
+        |歌曲|👍👍|信息获取、资源获取|
         |歌曲 Meta|👍|数据获取|
-        |登录奖励|👍|信息获取、资源获取|
+        |登录奖励|👍👍|信息获取、资源获取|
         |自选券|👍|信息获取|
         |漫画|👍👍|信息获取、图片获取|
         |任务|👍|信息获取|
         |ayachan|👍👍👍|谱面分析、测试服上传、难度分析|
         |其他资源|👍|部分独立资源的单独获取|
         
         ## 快速使用
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.2 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.0 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
@@ -16,23 +16,25 @@
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
 **è­¦åï¼æ­¤æ¨¡åç®åä»ç¶äºå¾å®åä¸æµè¯ï¼è¯·ä¸è¦å°å¶å½åä¸ä¸ªç¨³å®çåºä½¿ç¨ã**
 ### ç®åå·²æç API ä¸åè½ |API ç±»å«|æ¯å¦å®å|æ¯æçåå®¹| |:-
 ------|:-----:|:------
 | |ç¨æ·|ðð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
 |ç©å®¶|ð|ä¿¡æ¯è·å|
-|å¸å­|ðð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
+|å¸å­|ððð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
 |è°±é¢|ððð|ç¤¾åºè°±é¢è·åãé³æºä¸å°é¢è·åãè§æ´åãæ°æ®ç»è®¡ãæ ¼å¼äºè½¬|
-|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ð|ä¿¡æ¯è·åãèµæºè·å|
-|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ð|ä¿¡æ¯è·å|
-|æ´»å¨|ð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
-|æå|ð|æ°æ®è·åãèµæºè·å|
-|æ­æ²|ð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
-|ç»å½å¥å±|ð|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð|ä¿¡æ¯è·å|
-|æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð|ä¿¡æ¯è·å|
+|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|å¡ç|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|æè£|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|æ´»å¨|ðð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
+|æå|ðð|æ°æ®è·åãèµæºè·å|
+|æ­æ²|ðð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
+|ç»å½å¥å±|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|èªéå¸|ð|ä¿¡æ¯è·å| |æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å|
+|ä»»å¡|ð|ä¿¡æ¯è·å|
 |ayachan|ððð|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
 |å¶ä»èµæº|ð|é¨åç¬ç«èµæºçåç¬è·å| ## å¿«éä½¿ç¨
 ä»¥ä¸å°ä»¥è·åç¤¾åºèªå¶è°±é¢ [[FULL] åã®ä¸­ã¸](https://
 bestdori.com/community/charts/111533/WindowsSov8-FULL) çä¿¡æ¯ä¸ºä¾ã
 é¦åï¼ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install bestdori-
 api ``` æ¥ä¸æ¥å¨ä¸ä¸ª Python
 èæ¬æä»¶ä¸­ï¼ä½¿ç¨å¦ä¸ä»£ç è·åæå®å¸å­çå¨é¨ä¿¡æ¯ï¼è¿éæä»¬å·²ç¥è¯¥å¸å­ç
```

### Comparing `bestdori-api-1.0.2/README.md` & `bestdori-api-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,26 @@
 
 ### 目前已有的 API 与功能
 
 |API 类别|是否完善|支持的内容|
 |:-------|:-----:|:------|
 |用户|👍👍|登录、查询、帖子获取、信息获取|
 |玩家|👍|信息获取|
-|帖子|👍👍|搜索、获取、发表、评论、喜欢|
+|帖子|👍👍👍|搜索、获取、发表、评论、喜欢|
 |谱面|👍👍👍|社区谱面获取、音源与封面获取、规整化、数据统计、格式互转|
 |故事|👍|社区故事获取|
-|角色|👍|信息获取、资源获取|
-|卡牌|👍|信息获取、资源获取|
-|服装|👍|信息获取|
-|活动|👍|信息获取、资源获取|
+|角色|👍👍|信息获取、资源获取|
+|卡牌|👍👍|信息获取、资源获取|
+|服装|👍👍|信息获取、资源获取|
+|活动|👍👍|信息获取、资源获取|
 |活动数据|👍|数据获取|
-|招募|👍|数据获取、资源获取|
-|歌曲|👍|信息获取、资源获取|
+|招募|👍👍|数据获取、资源获取|
+|歌曲|👍👍|信息获取、资源获取|
 |歌曲 Meta|👍|数据获取|
-|登录奖励|👍|信息获取、资源获取|
+|登录奖励|👍👍|信息获取、资源获取|
 |自选券|👍|信息获取|
 |漫画|👍👍|信息获取、图片获取|
 |任务|👍|信息获取|
 |ayachan|👍👍👍|谱面分析、测试服上传、难度分析|
 |其他资源|👍|部分独立资源的单独获取|
 
 ## 快速使用
```

#### html2text {}

```diff
@@ -12,23 +12,25 @@
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
 **è­¦åï¼æ­¤æ¨¡åç®åä»ç¶äºå¾å®åä¸æµè¯ï¼è¯·ä¸è¦å°å¶å½åä¸ä¸ªç¨³å®çåºä½¿ç¨ã**
 ### ç®åå·²æç API ä¸åè½ |API ç±»å«|æ¯å¦å®å|æ¯æçåå®¹| |:-
 ------|:-----:|:------
 | |ç¨æ·|ðð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
 |ç©å®¶|ð|ä¿¡æ¯è·å|
-|å¸å­|ðð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
+|å¸å­|ððð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
 |è°±é¢|ððð|ç¤¾åºè°±é¢è·åãé³æºä¸å°é¢è·åãè§æ´åãæ°æ®ç»è®¡ãæ ¼å¼äºè½¬|
-|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ð|ä¿¡æ¯è·åãèµæºè·å|
-|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ð|ä¿¡æ¯è·å|
-|æ´»å¨|ð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
-|æå|ð|æ°æ®è·åãèµæºè·å|
-|æ­æ²|ð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
-|ç»å½å¥å±|ð|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð|ä¿¡æ¯è·å|
-|æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð|ä¿¡æ¯è·å|
+|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|å¡ç|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|æè£|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|æ´»å¨|ðð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
+|æå|ðð|æ°æ®è·åãèµæºè·å|
+|æ­æ²|ðð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
+|ç»å½å¥å±|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|èªéå¸|ð|ä¿¡æ¯è·å| |æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å|
+|ä»»å¡|ð|ä¿¡æ¯è·å|
 |ayachan|ððð|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
 |å¶ä»èµæº|ð|é¨åç¬ç«èµæºçåç¬è·å| ## å¿«éä½¿ç¨
 ä»¥ä¸å°ä»¥è·åç¤¾åºèªå¶è°±é¢ [[FULL] åã®ä¸­ã¸](https://
 bestdori.com/community/charts/111533/WindowsSov8-FULL) çä¿¡æ¯ä¸ºä¾ã
 é¦åï¼ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install bestdori-
 api ``` æ¥ä¸æ¥å¨ä¸ä¸ª Python
 èæ¬æä»¶ä¸­ï¼ä½¿ç¨å¦ä¸ä»£ç è·åæå®å¸å­çå¨é¨ä¿¡æ¯ï¼è¿éæä»¬å·²ç¥è¯¥å¸å­ç
```

### Comparing `bestdori-api-1.0.2/bestdori/__init__.py` & `bestdori-api-1.1.0/bestdori/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/ayachan/__init__.py` & `bestdori-api-1.1.0/bestdori/ayachan/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/ayachan/exceptions.py` & `bestdori-api-1.1.0/bestdori/ayachan/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/ayachan/utils/network.py` & `bestdori-api-1.1.0/bestdori/ayachan/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/ayachan/utils/utils.py` & `bestdori-api-1.1.0/bestdori/ayachan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/cards.py` & `bestdori-api-1.1.0/bestdori/cards.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/characters.py` & `bestdori-api-1.1.0/bestdori/characters.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/charts.py` & `bestdori-api-1.1.0/bestdori/charts.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/comics.py` & `bestdori-api-1.1.0/bestdori/comics.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/costumes.py` & `bestdori-api-1.1.0/bestdori/costumes.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/eventarchives.py` & `bestdori-api-1.1.0/bestdori/eventarchives.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/events.py` & `bestdori-api-1.1.0/bestdori/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .eventarchives import EventArchive
 from .post import get_list, get_list_async
+from .festival import (
+    Stage,
+    RotationMusic,
+    get_stages,
+    get_stages_async,
+    get_rotation_musics,
+    get_rotation_musics_async
+)
 from .exceptions import (
     NoDataException,
     EventNotExistError,
     AssetsNotExistError,
     EventHasNoStampError,
     ServerNotAvailableError
 )
@@ -552,7 +560,55 @@
             if self.server == 'jp': server = 0
             elif self.server == 'en': server = 1
             elif self.server == 'tw': server = 2
             elif self.server == 'cn': server = 3
             elif self.server == 'kr': server = 4
             else: raise NoDataException('活动服务器')
         return await self.archive.get_top_async(server, mid, latest)
+
+    # 获取团队 LIVE 佳节活动歌曲循环数据
+    def get_rotation_musics(self) -> list[RotationMusic]:
+        '''获取团队 LIVE 佳节活动歌曲循环数据
+
+        返回:
+            list[dict[str, Any]]: 团队 LIVE 佳节活动歌曲循环数据
+        '''
+        info = self.__get_info_cache()
+        if (_event_type := info.get('eventTyppe', '')) != 'festival':
+            raise ValueError(f'Rotation musics are only available for festival events, not {_event_type}.')
+        return get_rotation_musics(self.id)
+    
+    # 异步获取团队 LIVE 佳节活动歌曲循环数据
+    async def get_rotation_musics_async(self) -> list[RotationMusic]:
+        '''获取团队 LIVE 佳节活动歌曲循环数据
+
+        返回:
+            list[dict[str, Any]]: 团队 LIVE 佳节活动歌曲循环数据
+        '''
+        info = await self.__get_info_cache_async()
+        if (_event_type := info.get('eventTyppe', '')) != 'festival':
+            raise ValueError(f'Rotation musics are only available for festival events, not {_event_type}.')
+        return await get_rotation_musics_async(self.id)
+    
+    # 获取团队 LIVE 佳节活动舞台数据
+    def get_stages(self) -> list[Stage]:
+        '''获取团队 LIVE 佳节活动舞台数据
+
+        返回:
+            list[dict[str, Any]]: 团队 LIVE 佳节活动舞台数据
+        '''
+        info = self.__get_info_cache()
+        if (_event_type := info.get('eventTyppe', '')) != 'festival':
+            raise ValueError(f'Stages are only available for festival events, not {_event_type}.')
+        return get_stages(self.id)
+    
+    # 异步获取团队 LIVE 佳节活动舞台数据
+    async def get_stages_async(self) -> list[Stage]:
+        '''获取团队 LIVE 佳节活动舞台数据
+
+        返回:
+            list[dict[str, Any]]: 团队 LIVE 佳节活动舞台数据
+        '''
+        info = await self.__get_info_cache_async()
+        if (_event_type := info.get('eventTyppe', '')) != 'festival':
+            raise ValueError(f'Stages are only available for festival events, not {_event_type}.')
+        return await get_stages_async(self.id)
```

### Comparing `bestdori-api-1.0.2/bestdori/exceptions.py` & `bestdori-api-1.1.0/bestdori/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/gacha.py` & `bestdori-api-1.1.0/bestdori/gacha.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/logincampaigns.py` & `bestdori-api-1.1.0/bestdori/logincampaigns.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/miracleticket.py` & `bestdori-api-1.1.0/bestdori/miracleticket.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/missions.py` & `bestdori-api-1.1.0/bestdori/missions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/models/__init__.py` & `bestdori-api-1.1.0/bestdori/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/models/content.py` & `bestdori-api-1.1.0/bestdori/models/content.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/models/note.py` & `bestdori-api-1.1.0/bestdori/models/note.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/player.py` & `bestdori-api-1.1.0/bestdori/player.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/post.py` & `bestdori-api-1.1.0/bestdori/post.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/settings.py` & `bestdori-api-1.1.0/bestdori/settings.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/songmeta.py` & `bestdori-api-1.1.0/bestdori/songmeta.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/songs.py` & `bestdori-api-1.1.0/bestdori/songs.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/upload.py` & `bestdori-api-1.1.0/bestdori/upload.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/user.py` & `bestdori-api-1.1.0/bestdori/user.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/utils/__init__.py` & `bestdori-api-1.1.0/bestdori/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/utils/network.py` & `bestdori-api-1.1.0/bestdori/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.0.2/bestdori/utils/utils.py` & `bestdori-api-1.1.0/bestdori/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         'all': 'costumes/all.{index}.json'
     },
     'events': {
         'info': 'events/{id}.json',
         'all': 'events/all.{index}.json',
         'top': 'eventtop/data'
     },
+    'festival':{
+        'stages': 'festival/stages/{id}.json',
+        'rotation_musics': 'festival/rotationMusics/{id}.json',
+    },
     'gacha': {
         'info': 'gacha/{id}.json',
         'all': 'gacha/all.{index}.json'
     },
     'songs': {
         'info': 'songs/{id}.json',
         'all': 'songs/all.{index}.json'
```

### Comparing `bestdori-api-1.0.2/bestdori_api.egg-info/PKG-INFO` & `bestdori-api-1.1.0/bestdori_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -48,26 +48,26 @@
         
         ### 目前已有的 API 与功能
         
         |API 类别|是否完善|支持的内容|
         |:-------|:-----:|:------|
         |用户|👍👍|登录、查询、帖子获取、信息获取|
         |玩家|👍|信息获取|
-        |帖子|👍👍|搜索、获取、发表、评论、喜欢|
+        |帖子|👍👍👍|搜索、获取、发表、评论、喜欢|
         |谱面|👍👍👍|社区谱面获取、音源与封面获取、规整化、数据统计、格式互转|
         |故事|👍|社区故事获取|
-        |角色|👍|信息获取、资源获取|
-        |卡牌|👍|信息获取、资源获取|
-        |服装|👍|信息获取|
-        |活动|👍|信息获取、资源获取|
+        |角色|👍👍|信息获取、资源获取|
+        |卡牌|👍👍|信息获取、资源获取|
+        |服装|👍👍|信息获取、资源获取|
+        |活动|👍👍|信息获取、资源获取|
         |活动数据|👍|数据获取|
-        |招募|👍|数据获取、资源获取|
-        |歌曲|👍|信息获取、资源获取|
+        |招募|👍👍|数据获取、资源获取|
+        |歌曲|👍👍|信息获取、资源获取|
         |歌曲 Meta|👍|数据获取|
-        |登录奖励|👍|信息获取、资源获取|
+        |登录奖励|👍👍|信息获取、资源获取|
         |自选券|👍|信息获取|
         |漫画|👍👍|信息获取、图片获取|
         |任务|👍|信息获取|
         |ayachan|👍👍👍|谱面分析、测试服上传、难度分析|
         |其他资源|👍|部分独立资源的单独获取|
         
         ## 快速使用
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.0.2 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.0 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
@@ -16,23 +16,25 @@
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
 **è­¦åï¼æ­¤æ¨¡åç®åä»ç¶äºå¾å®åä¸æµè¯ï¼è¯·ä¸è¦å°å¶å½åä¸ä¸ªç¨³å®çåºä½¿ç¨ã**
 ### ç®åå·²æç API ä¸åè½ |API ç±»å«|æ¯å¦å®å|æ¯æçåå®¹| |:-
 ------|:-----:|:------
 | |ç¨æ·|ðð|ç»å½ãæ¥è¯¢ãå¸å­è·åãä¿¡æ¯è·å|
 |ç©å®¶|ð|ä¿¡æ¯è·å|
-|å¸å­|ðð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
+|å¸å­|ððð|æç´¢ãè·åãåè¡¨ãè¯è®ºãåæ¬¢|
 |è°±é¢|ððð|ç¤¾åºè°±é¢è·åãé³æºä¸å°é¢è·åãè§æ´åãæ°æ®ç»è®¡ãæ ¼å¼äºè½¬|
-|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ð|ä¿¡æ¯è·åãèµæºè·å|
-|å¡ç|ð|ä¿¡æ¯è·åãèµæºè·å| |æè£|ð|ä¿¡æ¯è·å|
-|æ´»å¨|ð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
-|æå|ð|æ°æ®è·åãèµæºè·å|
-|æ­æ²|ð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
-|ç»å½å¥å±|ð|ä¿¡æ¯è·åãèµæºè·å| |èªéå¸|ð|ä¿¡æ¯è·å|
-|æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å| |ä»»å¡|ð|ä¿¡æ¯è·å|
+|æäº|ð|ç¤¾åºæäºè·å| |è§è²|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|å¡ç|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|æè£|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|æ´»å¨|ðð|ä¿¡æ¯è·åãèµæºè·å| |æ´»å¨æ°æ®|ð|æ°æ®è·å|
+|æå|ðð|æ°æ®è·åãèµæºè·å|
+|æ­æ²|ðð|ä¿¡æ¯è·åãèµæºè·å| |æ­æ² Meta|ð|æ°æ®è·å|
+|ç»å½å¥å±|ðð|ä¿¡æ¯è·åãèµæºè·å|
+|èªéå¸|ð|ä¿¡æ¯è·å| |æ¼«ç»|ðð|ä¿¡æ¯è·åãå¾çè·å|
+|ä»»å¡|ð|ä¿¡æ¯è·å|
 |ayachan|ððð|è°±é¢åæãæµè¯æä¸ä¼ ãé¾åº¦åæ|
 |å¶ä»èµæº|ð|é¨åç¬ç«èµæºçåç¬è·å| ## å¿«éä½¿ç¨
 ä»¥ä¸å°ä»¥è·åç¤¾åºèªå¶è°±é¢ [[FULL] åã®ä¸­ã¸](https://
 bestdori.com/community/charts/111533/WindowsSov8-FULL) çä¿¡æ¯ä¸ºä¾ã
 é¦åï¼ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install bestdori-
 api ``` æ¥ä¸æ¥å¨ä¸ä¸ª Python
 èæ¬æä»¶ä¸­ï¼ä½¿ç¨å¦ä¸ä»£ç è·åæå®å¸å­çå¨é¨ä¿¡æ¯ï¼è¿éæä»¬å·²ç¥è¯¥å¸å­ç
```

### Comparing `bestdori-api-1.0.2/bestdori_api.egg-info/SOURCES.txt` & `bestdori-api-1.1.0/bestdori_api.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 bestdori/characters.py
 bestdori/charts.py
 bestdori/comics.py
 bestdori/costumes.py
 bestdori/eventarchives.py
 bestdori/events.py
 bestdori/exceptions.py
+bestdori/festival.py
 bestdori/gacha.py
 bestdori/logincampaigns.py
 bestdori/miracleticket.py
 bestdori/missions.py
 bestdori/player.py
 bestdori/post.py
 bestdori/settings.py
```

### Comparing `bestdori-api-1.0.2/setup.py` & `bestdori-api-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='bestdori-api',
-    version='1.0.2',
+    version='1.1.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/bestdori-api',
     include_package_data=False,
```

