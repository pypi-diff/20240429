# Comparing `tmp/nonebot_plugin_bilichat-5.7.0.tar.gz` & `tmp/nonebot_plugin_bilichat-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.7.0.tar", last modified: Thu Apr 25 13:14:17 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.7.1.tar", last modified: Mon Apr 29 14:03:53 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.7.0.tar` & `nonebot_plugin_bilichat-5.7.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    34523 2024-04-25 13:14:11.917305 nonebot_plugin_bilichat-5.7.0/LICENSE
--rw-r--r--   0        0        0    17907 2024-04-25 13:14:11.917305 nonebot_plugin_bilichat-5.7.0/README.md
--rw-r--r--   0        0        0     2718 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2176 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1622 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2655 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7996 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      942 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3848 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5196 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9227 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3130 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4227 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3958 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      494 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6142 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2346 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      366 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1136 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7275 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3187 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3091 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1701 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1739 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     3988 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      552 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      809 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      532 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2988 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1016 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      596 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/const.py
--rw-r--r--   0        0        0     1163 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      291 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     3111 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7187 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    15592 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4894 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2243 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1578 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1755 2024-04-25 13:14:17.689287 nonebot_plugin_bilichat-5.7.0/pyproject.toml
--rw-r--r--   0        0        0    19603 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-29 14:03:46.593820 nonebot_plugin_bilichat-5.7.1/LICENSE
+-rw-r--r--   0        0        0    17907 2024-04-29 14:03:46.593820 nonebot_plugin_bilichat-5.7.1/README.md
+-rw-r--r--   0        0        0     2718 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2176 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1622 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2655 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7996 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      942 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3848 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5196 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9227 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3130 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4227 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3958 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      494 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6142 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2346 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3379 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1136 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7275 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3187 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3091 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1701 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1739 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     3988 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      552 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      809 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      532 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3030 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1016 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      596 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/const.py
+-rw-r--r--   0        0        0     1163 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      291 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     3111 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7187 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    15592 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4894 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2243 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1578 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1755 2024-04-29 14:03:53.033960 nonebot_plugin_bilichat-5.7.1/pyproject.toml
+-rw-r--r--   0        0        0    19603 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.7.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.7.0/LICENSE` & `nonebot_plugin_bilichat-5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/README.md` & `nonebot_plugin_bilichat-5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
             await page.set_viewport_size({"width": 1080, "height": int(clip["height"] + 720)})
             await asyncio.sleep(1)
             await page.wait_for_load_state(state="networkidle")
             if picture := await page.screenshot(
                 clip=clip, full_page=True, type="jpeg", quality=plugin_config.bilichat_browser_shot_quality
             ):
                 return picture
+            else:
+                logger.warning(f"专栏 cv{cvid} 截图失败, 可能是专栏过长无法截图")
         except CaptchaAbortError:
             raise
         except TimeoutError:
             if retry:
                 logger.error(f"专栏 cv{cvid} 截图超时, 重试...")
                 return await screenshot(cvid, retry=False)
             raise AbortError(f"cv{cvid} 专栏截图超时")
```

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/arguments.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/arguments.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 
 class ASRDataSeg(BaseModel):
     "文字识别-断句"
 
     class ASRDataWords(BaseModel):
         "文字识别-逐字"
-        label: str
-        start_time: int
-        end_time: int
-        confidence: int
+        label: str | None
+        start_time: int | None
+        end_time: int | None
+        confidence: int | None
 
     start_time: int
     end_time: int
     transcript: str
-    words: list[ASRDataWords]
-    confidence: int
+    words: list[ASRDataWords] | None
+    confidence: int | None
 
     def to_srt_ts(self) -> str:
         "转换为srt时间戳"
 
         def _conv(ms: int) -> tuple[int, int, int, int]:
             return ms // 3600000, ms // 60000 % 60, ms // 1000 % 60, ms % 1000
```

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/const.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.0/pyproject.toml` & `nonebot_plugin_bilichat-5.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.7.0"
+version = "5.7.1"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
```

### Comparing `nonebot_plugin_bilichat-5.7.0/PKG-INFO` & `nonebot_plugin_bilichat-5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.7.0
+Version: 5.7.1
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.10
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.7.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.7.1 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.10 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
```

