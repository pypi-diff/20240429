# Comparing `tmp/pytgpt_bot-0.1.4.tar.gz` & `tmp/pytgpt_bot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.1.4.tar", last modified: Sun Apr 28 21:36:03 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.5.tar", last modified: Mon Apr 29 01:20:26 2024, max compression
```

## Comparing `pytgpt_bot-0.1.4.tar` & `pytgpt_bot-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:20:26.851401 pytgpt_bot-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-29 01:20:26.851401 pytgpt_bot-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:20:26.851401 pytgpt_bot-0.1.5/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26385 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:20:26.851401 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-29 01:20:26.000000 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-29 01:20:26.000000 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:20:26.000000 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 01:20:26.000000 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 01:20:26.000000 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 01:20:26.000000 pytgpt_bot-0.1.5/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:20:26.851401 pytgpt_bot-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-29 01:20:09.000000 pytgpt_bot-0.1.5/setup.py
```

### Comparing `pytgpt_bot-0.1.4/LICENSE` & `pytgpt_bot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/PKG-INFO` & `pytgpt_bot-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.4
-Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
+Version: 0.1.5
+Summary: AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.4 Summary: Telegram bot for
-chatting, text-to-image and text-to-speech conversions Home-page: https://
-github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.5 Summary: AI powered
+Telegram bot for chatting, text-to-image and text-to-speech conversions Home-
+page: https://github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
 pytgpt-bot/blob/main/README.md Keywords:
```

### Comparing `pytgpt_bot-0.1.4/README.md` & `pytgpt_bot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.5/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/config.py` & `pytgpt_bot-0.1.5/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/db.py` & `pytgpt_bot-0.1.5/pytgpt_bot/db.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/filters.py` & `pytgpt_bot-0.1.5/pytgpt_bot/filters.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/main.py` & `pytgpt_bot-0.1.5/pytgpt_bot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
         )
 
 
 @bot.inline_handler(lambda query: query.query.endswith("..."))
 def handle_inline_query(inline_query: telebot.types.InlineQuery):
     """Process the inline query and return AI response"""
     try:
-        logging.info("Serving INLINE-QUERY - [{inline_query.from_user.id}].")
+        logging.info(f"Serving INLINE-QUERY - [{inline_query.from_user.id}].")
         prompt = inline_query.query[:-3]
         user = User(user_id=inline_query.from_user.id)
         conversation = Conversation(max_tokens=max_tokens)
         user_provider = provider_map.get(user.chat.provider)
         conversation_prompt = conversation.gen_complete_prompt(
             prompt, intro=user.chat.intro
         )
```

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/models.py` & `pytgpt_bot-0.1.5/pytgpt_bot/models.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot/utils.py` & `pytgpt_bot-0.1.5/pytgpt_bot/utils.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.4/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.5/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.4
-Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
+Version: 0.1.5
+Summary: AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.4 Summary: Telegram bot for
-chatting, text-to-image and text-to-speech conversions Home-page: https://
-github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.5 Summary: AI powered
+Telegram bot for chatting, text-to-image and text-to-speech conversions Home-
+page: https://github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
 pytgpt-bot/blob/main/README.md Keywords:
```

### Comparing `pytgpt_bot-0.1.4/setup.py` & `pytgpt_bot-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.1.4",
+    version="0.1.5",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
-    description="Telegram bot for chatting, text-to-image and text-to-speech conversions",
+    description="AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
         "Bug Report": "https://github.com/Simatwa/pytgpt-bot/issues/new",
         "Homepage": "https://github.com/Simatwa/pytgpt-bot",
         "Source Code": "https://github.com/Simatwa/pytgpt-bot",
         "Issue Tracker": "https://github.com/Simatwa/pytgpt-bot/issues",
         "Download": "https://github.com/Simatwa/pytgpt-bot/releases",
```

