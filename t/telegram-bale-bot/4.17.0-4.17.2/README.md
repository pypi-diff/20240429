# Comparing `tmp/telegram-bale-bot-4.17.0.tar.gz` & `tmp/telegram-bale-bot-4.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-bale-bot-4.17.0.tar", last modified: Mon Apr 29 15:06:19 2024, max compression
+gzip compressed data, was "telegram-bale-bot-4.17.2.tar", last modified: Mon Apr 29 15:19:06 2024, max compression
```

## Comparing `telegram-bale-bot-4.17.0.tar` & `telegram-bale-bot-4.17.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.047820 telegram-bale-bot-4.17.0/
--rw-rw-r--   0 ali       (1001) ali       (1001)    18047 2024-04-29 14:53:45.000000 telegram-bale-bot-4.17.0/LICENSE
--rw-r--r--   0 ali       (1001) ali       (1001)    48462 2024-04-29 15:06:19.047820 telegram-bale-bot-4.17.0/PKG-INFO
--rw-rw-r--   0 ali       (1001) ali       (1001)    46533 2024-04-29 15:04:15.000000 telegram-bale-bot-4.17.0/README.md
--rw-rw-r--   0 ali       (1001) ali       (1001)     1520 2024-04-29 15:06:14.000000 telegram-bale-bot-4.17.0/pyproject.toml
--rw-rw-r--   0 ali       (1001) ali       (1001)       38 2024-04-29 15:06:19.047820 telegram-bale-bot-4.17.0/setup.cfg
--rw-rw-r--   0 ali       (1001) ali       (1001)      947 2024-04-29 15:05:46.000000 telegram-bale-bot-4.17.0/setup.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.039820 telegram-bale-bot-4.17.0/telebot/
--rw-rw-r--   0 ali       (1001) ali       (1001)   407042 2024-04-29 15:00:12.000000 telegram-bale-bot-4.17.0/telebot/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    90266 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.0/telebot/apihelper.py
--rw-rw-r--   0 ali       (1001) ali       (1001)   379777 2024-04-29 14:58:29.000000 telegram-bale-bot-4.17.0/telebot/async_telebot.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    13230 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.0/telebot/asyncio_filters.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     3793 2024-04-29 14:57:57.000000 telegram-bale-bot-4.17.0/telebot/asyncio_handler_backends.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    91482 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.0/telebot/asyncio_helper.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.039820 telegram-bale-bot-4.17.0/telebot/asyncio_storage/
--rw-rw-r--   0 ali       (1001) ali       (1001)      424 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/asyncio_storage/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     1710 2024-04-29 14:58:00.000000 telegram-bale-bot-4.17.0/telebot/asyncio_storage/base_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     2309 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/asyncio_storage/memory_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     3792 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/asyncio_storage/pickle_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     6025 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/asyncio_storage/redis_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     5263 2024-04-29 14:58:01.000000 telegram-bale-bot-4.17.0/telebot/callback_data.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    13362 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/custom_filters.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.039820 telegram-bale-bot-4.17.0/telebot/ext/
--rw-rw-r--   0 ali       (1001) ali       (1001)       63 2024-04-29 14:53:45.000000 telegram-bale-bot-4.17.0/telebot/ext/__init__.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.039820 telegram-bale-bot-4.17.0/telebot/ext/aio/
--rw-rw-r--   0 ali       (1001) ali       (1001)      128 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/ext/aio/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     3742 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/ext/aio/webhooks.py
--rw-rw-r--   0 ali       (1001) ali       (1001)      766 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/ext/reloader.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.039820 telegram-bale-bot-4.17.0/telebot/ext/sync/
--rw-rw-r--   0 ali       (1001) ali       (1001)      125 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/ext/sync/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     3445 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/ext/sync/webhooks.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    15113 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.0/telebot/formatting.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     9085 2024-04-29 14:58:02.000000 telegram-bale-bot-4.17.0/telebot/handler_backends.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     1972 2024-04-29 14:58:02.000000 telegram-bale-bot-4.17.0/telebot/service_utils.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.043820 telegram-bale-bot-4.17.0/telebot/storage/
--rw-rw-r--   0 ali       (1001) ali       (1001)      392 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/storage/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     1699 2024-04-29 14:58:02.000000 telegram-bale-bot-4.17.0/telebot/storage/base_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     2287 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/storage/memory_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     3954 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/storage/pickle_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     5693 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/storage/redis_storage.py
--rw-rw-r--   0 ali       (1001) ali       (1001)   413414 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/telebot/types.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    21298 2024-04-29 14:58:25.000000 telegram-bale-bot-4.17.0/telebot/util.py
--rw-rw-r--   0 ali       (1001) ali       (1001)       96 2024-04-29 14:58:04.000000 telegram-bale-bot-4.17.0/telebot/version.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.043820 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/
--rw-r--r--   0 ali       (1001) ali       (1001)    48462 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1001) ali       (1001)     1233 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/not-zip-safe
--rw-rw-r--   0 ali       (1001) ali       (1001)      202 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/requires.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)       14 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/top_level.txt
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:06:19.043820 telegram-bale-bot-4.17.0/tests/
--rw-rw-r--   0 ali       (1001) ali       (1001)        0 2024-04-29 14:53:45.000000 telegram-bale-bot-4.17.0/tests/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    10848 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/tests/test_handler_backends.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    27963 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.0/tests/test_telebot.py
--rw-rw-r--   0 ali       (1001) ali       (1001)    22202 2024-04-29 14:58:07.000000 telegram-bale-bot-4.17.0/tests/test_types.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.950963 telegram-bale-bot-4.17.2/
+-rw-rw-r--   0 ali       (1001) ali       (1001)    18047 2024-04-29 14:53:45.000000 telegram-bale-bot-4.17.2/LICENSE
+-rw-r--r--   0 ali       (1001) ali       (1001)    48558 2024-04-29 15:19:06.950963 telegram-bale-bot-4.17.2/PKG-INFO
+-rw-rw-r--   0 ali       (1001) ali       (1001)    46629 2024-04-29 15:12:55.000000 telegram-bale-bot-4.17.2/README.md
+-rw-rw-r--   0 ali       (1001) ali       (1001)     1520 2024-04-29 15:16:46.000000 telegram-bale-bot-4.17.2/pyproject.toml
+-rw-rw-r--   0 ali       (1001) ali       (1001)       38 2024-04-29 15:19:06.950963 telegram-bale-bot-4.17.2/setup.cfg
+-rw-rw-r--   0 ali       (1001) ali       (1001)      947 2024-04-29 15:13:59.000000 telegram-bale-bot-4.17.2/setup.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.942962 telegram-bale-bot-4.17.2/telebot/
+-rw-rw-r--   0 ali       (1001) ali       (1001)   407044 2024-04-29 15:17:45.000000 telegram-bale-bot-4.17.2/telebot/__init__.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    90266 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.2/telebot/apihelper.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)   379777 2024-04-29 14:58:29.000000 telegram-bale-bot-4.17.2/telebot/async_telebot.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    13230 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.2/telebot/asyncio_filters.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     3793 2024-04-29 14:57:57.000000 telegram-bale-bot-4.17.2/telebot/asyncio_handler_backends.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    91482 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.2/telebot/asyncio_helper.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.942962 telegram-bale-bot-4.17.2/telebot/asyncio_storage/
+-rw-rw-r--   0 ali       (1001) ali       (1001)      424 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/asyncio_storage/__init__.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     1710 2024-04-29 14:58:00.000000 telegram-bale-bot-4.17.2/telebot/asyncio_storage/base_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     2309 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/asyncio_storage/memory_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     3792 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/asyncio_storage/pickle_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     6025 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/asyncio_storage/redis_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     5263 2024-04-29 14:58:01.000000 telegram-bale-bot-4.17.2/telebot/callback_data.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    13362 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/custom_filters.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.942962 telegram-bale-bot-4.17.2/telebot/ext/
+-rw-rw-r--   0 ali       (1001) ali       (1001)       63 2024-04-29 14:53:45.000000 telegram-bale-bot-4.17.2/telebot/ext/__init__.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.942962 telegram-bale-bot-4.17.2/telebot/ext/aio/
+-rw-rw-r--   0 ali       (1001) ali       (1001)      128 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/ext/aio/__init__.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     3742 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/ext/aio/webhooks.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)      766 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/ext/reloader.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.942962 telegram-bale-bot-4.17.2/telebot/ext/sync/
+-rw-rw-r--   0 ali       (1001) ali       (1001)      125 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/ext/sync/__init__.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     3445 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/ext/sync/webhooks.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    15113 2024-04-29 14:58:18.000000 telegram-bale-bot-4.17.2/telebot/formatting.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     9085 2024-04-29 14:58:02.000000 telegram-bale-bot-4.17.2/telebot/handler_backends.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     1972 2024-04-29 14:58:02.000000 telegram-bale-bot-4.17.2/telebot/service_utils.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.946962 telegram-bale-bot-4.17.2/telebot/storage/
+-rw-rw-r--   0 ali       (1001) ali       (1001)      392 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/storage/__init__.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     1699 2024-04-29 14:58:02.000000 telegram-bale-bot-4.17.2/telebot/storage/base_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     2287 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/storage/memory_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     3954 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/storage/pickle_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)     5693 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/storage/redis_storage.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)   413414 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/telebot/types.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    21298 2024-04-29 14:58:25.000000 telegram-bale-bot-4.17.2/telebot/util.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)       96 2024-04-29 14:58:04.000000 telegram-bale-bot-4.17.2/telebot/version.py
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.946962 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/
+-rw-r--r--   0 ali       (1001) ali       (1001)    48558 2024-04-29 15:19:06.000000 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1001) ali       (1001)     1233 2024-04-29 15:19:06.000000 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-29 15:19:06.000000 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-29 15:06:18.000000 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/not-zip-safe
+-rw-rw-r--   0 ali       (1001) ali       (1001)      202 2024-04-29 15:19:06.000000 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1001) ali       (1001)       14 2024-04-29 15:19:06.000000 telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/top_level.txt
+drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-29 15:19:06.946962 telegram-bale-bot-4.17.2/tests/
+-rw-rw-r--   0 ali       (1001) ali       (1001)        0 2024-04-29 14:53:45.000000 telegram-bale-bot-4.17.2/tests/__init__.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    10848 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/tests/test_handler_backends.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    27963 2024-04-29 14:58:19.000000 telegram-bale-bot-4.17.2/tests/test_telebot.py
+-rw-rw-r--   0 ali       (1001) ali       (1001)    22202 2024-04-29 14:58:07.000000 telegram-bale-bot-4.17.2/tests/test_types.py
```

### Comparing `telegram-bale-bot-4.17.0/LICENSE` & `telegram-bale-bot-4.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/PKG-INFO` & `telegram-bale-bot-4.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-bale-bot
-Version: 4.17.0
+Version: 4.17.2
 Summary: A simple and easy-to-use library for creating Telegram bots and Bale messenger bots.
 Home-page: https://github.com/mahdikiani/telegram-bale-bot
 Author: Mahdi Kiani
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: GPL2
 Project-URL: Homepage, https://github.com/mahdikiani/telegram-bale-bot
 Project-URL: OriginalPackage, https://github.com/eternnoir/pyTelegramBotAPI
@@ -120,35 +120,37 @@
 
 This API is tested with Python 3.8-3.12 and Pypy 3.
 There are two ways to install the library:
 
 * Installation using pip (a Python package manager):
 
 ```
-$ pip install pyTelegramBotAPI
+$ pip install telegram-bale-bot
 ```
 * Installation from source (requires git):
 
 ```
-$ pip install git+https://github.com/eternnoir/pyTelegramBotAPI.git
+$ pip install git+https://github.com/mahdikiani/telegram-bale-bot.git
 ```
 
 It is generally recommended to use the first option.
 
 *While the API is production-ready, it is still under development and it has regular updates, do not forget to update it regularly by calling*
 ```
-pip install pytelegrambotapi --upgrade
+pip install telegram-bale-bot --upgrade
 ```
 
 ## Writing your first bot
 
 ### Prerequisites
 
 It is presumed that you [have obtained an API token with @BotFather](https://core.telegram.org/bots#botfather). We will call this token `TOKEN`.
 Furthermore, you have basic knowledge of the Python programming language and more importantly [the Telegram Bot API](https://core.telegram.org/bots/api).
+- [Telegram botfather](https://t.me/botfather)
+- [Bale botfather](https://ble.ir/botfather)
 
 ### A simple echo bot
 
 The TeleBot class (defined in \__init__.py) encapsulates all API calls in a single class. It provides functions such as `send_xyz` (`send_message`, `send_document` etc.) and several ways to listen for incoming messages.
 
 Create a file called `echo_bot.py`.
 Then, open the file and create an instance of the TeleBot class.
```

### Comparing `telegram-bale-bot-4.17.0/README.md` & `telegram-bale-bot-4.17.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,35 +72,37 @@
 
 This API is tested with Python 3.8-3.12 and Pypy 3.
 There are two ways to install the library:
 
 * Installation using pip (a Python package manager):
 
 ```
-$ pip install pyTelegramBotAPI
+$ pip install telegram-bale-bot
 ```
 * Installation from source (requires git):
 
 ```
-$ pip install git+https://github.com/eternnoir/pyTelegramBotAPI.git
+$ pip install git+https://github.com/mahdikiani/telegram-bale-bot.git
 ```
 
 It is generally recommended to use the first option.
 
 *While the API is production-ready, it is still under development and it has regular updates, do not forget to update it regularly by calling*
 ```
-pip install pytelegrambotapi --upgrade
+pip install telegram-bale-bot --upgrade
 ```
 
 ## Writing your first bot
 
 ### Prerequisites
 
 It is presumed that you [have obtained an API token with @BotFather](https://core.telegram.org/bots#botfather). We will call this token `TOKEN`.
 Furthermore, you have basic knowledge of the Python programming language and more importantly [the Telegram Bot API](https://core.telegram.org/bots/api).
+- [Telegram botfather](https://t.me/botfather)
+- [Bale botfather](https://ble.ir/botfather)
 
 ### A simple echo bot
 
 The TeleBot class (defined in \__init__.py) encapsulates all API calls in a single class. It provides functions such as `send_xyz` (`send_message`, `send_document` etc.) and several ways to listen for incoming messages.
 
 Create a file called `echo_bot.py`.
 Then, open the file and create an instance of the TeleBot class.
```

### Comparing `telegram-bale-bot-4.17.0/pyproject.toml` & `telegram-bale-bot-4.17.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "telegram-bale-bot"
-version = "4.17.0"
+version = "4.17.2"
 description = "A simple and easy-to-use library for creating Telegram bots and Bale messenger bots."
 authors = [{name = "Mahdi Kiani", email = "mahdikiany@gmail.com"}]
 license = {text = "GPL2"}
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["telegram", "bot", "api", "tools"]
 classifiers = [
```

### Comparing `telegram-bale-bot-4.17.0/setup.py` & `telegram-bale-bot-4.17.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     with open("README.md", encoding="utf8") as f:
         return f.read()
 
 
 setup(
     name="telegram-bale-bot",
-    version="4.17.0",
+    version="4.17.2",
     python_requires=">=3.8",
     url="https://github.com/mahdikiani/telegram-bale-bot",
     license="GPL2",
     description="A simple and easy-to-use library for creating Telegram bots and Bale messenger bots.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Mahdi Kiani",
```

### Comparing `telegram-bale-bot-4.17.0/telebot/__init__.py` & `telegram-bale-bot-4.17.2/telebot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3999,15 +3999,15 @@
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         reply_markup: Optional[types.InlineKeyboardMarkup] = None,
         timeout: Optional[int] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
-    ) -> types.Message | bool:
+    ) -> types.Message or bool:
         """
         Use this method to edit live location messages. A location can be edited until its live_period expires or editing is explicitly
             disabled by a call to stopMessageLiveLocation. On success, if the edited message is not an inline message, the edited Message
             is returned, otherwise True is returned.
 
         Telegram documentation: https://core.telegram.org/bots/api#editmessagelivelocation
 
@@ -4064,15 +4064,15 @@
     def stop_message_live_location(
         self,
         chat_id: Optional[Union[int, str]] = None,
         message_id: Optional[int] = None,
         inline_message_id: Optional[str] = None,
         reply_markup: Optional[types.InlineKeyboardMarkup] = None,
         timeout: Optional[int] = None,
-    ) -> types.Message | bool:
+    ) -> types.Message or bool:
         """
         Use this method to stop updating a live location message before live_period expires.
         On success, if the message is not an inline message, the edited Message is returned, otherwise True is returned.
 
         Telegram documentation: https://core.telegram.org/bots/api#stopmessagelivelocation
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format @channelusername)
```

### Comparing `telegram-bale-bot-4.17.0/telebot/apihelper.py` & `telegram-bale-bot-4.17.2/telebot/apihelper.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/async_telebot.py` & `telegram-bale-bot-4.17.2/telebot/async_telebot.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_filters.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_filters.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_handler_backends.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_handler_backends.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_helper.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_helper.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_storage/base_storage.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_storage/memory_storage.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_storage/pickle_storage.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_storage/pickle_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/asyncio_storage/redis_storage.py` & `telegram-bale-bot-4.17.2/telebot/asyncio_storage/redis_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/callback_data.py` & `telegram-bale-bot-4.17.2/telebot/callback_data.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/custom_filters.py` & `telegram-bale-bot-4.17.2/telebot/custom_filters.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/ext/aio/webhooks.py` & `telegram-bale-bot-4.17.2/telebot/ext/aio/webhooks.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/ext/reloader.py` & `telegram-bale-bot-4.17.2/telebot/ext/reloader.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/ext/sync/webhooks.py` & `telegram-bale-bot-4.17.2/telebot/ext/sync/webhooks.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/formatting.py` & `telegram-bale-bot-4.17.2/telebot/formatting.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/handler_backends.py` & `telegram-bale-bot-4.17.2/telebot/handler_backends.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/service_utils.py` & `telegram-bale-bot-4.17.2/telebot/service_utils.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/storage/base_storage.py` & `telegram-bale-bot-4.17.2/telebot/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/storage/memory_storage.py` & `telegram-bale-bot-4.17.2/telebot/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/storage/pickle_storage.py` & `telegram-bale-bot-4.17.2/telebot/storage/pickle_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/storage/redis_storage.py` & `telegram-bale-bot-4.17.2/telebot/storage/redis_storage.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/types.py` & `telegram-bale-bot-4.17.2/telebot/types.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telebot/util.py` & `telegram-bale-bot-4.17.2/telebot/util.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/PKG-INFO` & `telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-bale-bot
-Version: 4.17.0
+Version: 4.17.2
 Summary: A simple and easy-to-use library for creating Telegram bots and Bale messenger bots.
 Home-page: https://github.com/mahdikiani/telegram-bale-bot
 Author: Mahdi Kiani
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: GPL2
 Project-URL: Homepage, https://github.com/mahdikiani/telegram-bale-bot
 Project-URL: OriginalPackage, https://github.com/eternnoir/pyTelegramBotAPI
@@ -120,35 +120,37 @@
 
 This API is tested with Python 3.8-3.12 and Pypy 3.
 There are two ways to install the library:
 
 * Installation using pip (a Python package manager):
 
 ```
-$ pip install pyTelegramBotAPI
+$ pip install telegram-bale-bot
 ```
 * Installation from source (requires git):
 
 ```
-$ pip install git+https://github.com/eternnoir/pyTelegramBotAPI.git
+$ pip install git+https://github.com/mahdikiani/telegram-bale-bot.git
 ```
 
 It is generally recommended to use the first option.
 
 *While the API is production-ready, it is still under development and it has regular updates, do not forget to update it regularly by calling*
 ```
-pip install pytelegrambotapi --upgrade
+pip install telegram-bale-bot --upgrade
 ```
 
 ## Writing your first bot
 
 ### Prerequisites
 
 It is presumed that you [have obtained an API token with @BotFather](https://core.telegram.org/bots#botfather). We will call this token `TOKEN`.
 Furthermore, you have basic knowledge of the Python programming language and more importantly [the Telegram Bot API](https://core.telegram.org/bots/api).
+- [Telegram botfather](https://t.me/botfather)
+- [Bale botfather](https://ble.ir/botfather)
 
 ### A simple echo bot
 
 The TeleBot class (defined in \__init__.py) encapsulates all API calls in a single class. It provides functions such as `send_xyz` (`send_message`, `send_document` etc.) and several ways to listen for incoming messages.
 
 Create a file called `echo_bot.py`.
 Then, open the file and create an instance of the TeleBot class.
```

### Comparing `telegram-bale-bot-4.17.0/telegram_bale_bot.egg-info/SOURCES.txt` & `telegram-bale-bot-4.17.2/telegram_bale_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/tests/test_handler_backends.py` & `telegram-bale-bot-4.17.2/tests/test_handler_backends.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/tests/test_telebot.py` & `telegram-bale-bot-4.17.2/tests/test_telebot.py`

 * *Files identical despite different names*

### Comparing `telegram-bale-bot-4.17.0/tests/test_types.py` & `telegram-bale-bot-4.17.2/tests/test_types.py`

 * *Files identical despite different names*

