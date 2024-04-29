# Comparing `tmp/pytgpt_bot-0.1.3.tar.gz` & `tmp/pytgpt_bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.1.3.tar", last modified: Sun Apr 28 15:22:37 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.4.tar", last modified: Sun Apr 28 21:36:03 2024, max compression
```

## Comparing `pytgpt_bot-0.1.3.tar` & `pytgpt_bot-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:22:37.189545 pytgpt_bot-0.1.3/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    25018 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 21:36:03.000000 pytgpt_bot-0.1.4/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:36:03.301828 pytgpt_bot-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-28 21:35:45.000000 pytgpt_bot-0.1.4/setup.py
```

### Comparing `pytgpt_bot-0.1.3/LICENSE` & `pytgpt_bot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.3/PKG-INFO` & `pytgpt_bot-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -139,18 +139,14 @@
 - `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 > [!TIP]
 > For a better understanding of these commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/pytgpt_bot). This can give you a practical idea of how the bot works and how to use it effectively.
 
 ### Administrative Commands
 
-To make the administrative commands more understandable, let's simplify the descriptions and provide a bit more context for each command. This should help administrators manage the bot more effectively.
-
-### Simplified Administrative Commands
-
 - **/clear**: Use this command to remove all chat data from the bot's database. It's a powerful tool, so use it carefully to avoid losing important data.
 
 - **/total**: This command shows you the total number of chats the bot has handled. It's a quick way to see how much interaction the bot has had.
 
 - **/drop**: If you need to completely wipe out all chat data and logs, use this command. It's more extreme than `/clear` and should be used with caution to avoid losing all data.
 
 - **/sql**: Want to directly interact with the bot's database? This command lets you run SQL queries. It's a powerful feature for managing and analyzing data, but be cautious to avoid mistakes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.3 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.4 Summary: Telegram bot for
 chatting, text-to-image and text-to-speech conversions Home-page: https://
 github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -62,37 +62,34 @@
 Delete everything from the chat table and bot logs. This is more extreme than
 `/clear`. - **/sql**: Run SQL queries on the bot's database. Use this with
 caution! - **/logs**: Check the bot's logs for activity, errors, and user
 interactions. - `any other text`: An alias for `/chat`, allowing users to
 continue with chatting. > [!TIP] > For a better understanding of these
 commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/
 pytgpt_bot). This can give you a practical idea of how the bot works and how to
-use it effectively. ### Administrative Commands To make the administrative
-commands more understandable, let's simplify the descriptions and provide a bit
-more context for each command. This should help administrators manage the bot
-more effectively. ### Simplified Administrative Commands - **/clear**: Use this
-command to remove all chat data from the bot's database. It's a powerful tool,
-so use it carefully to avoid losing important data. - **/total**: This command
-shows you the total number of chats the bot has handled. It's a quick way to
-see how much interaction the bot has had. - **/drop**: If you need to
-completely wipe out all chat data and logs, use this command. It's more extreme
-than `/clear` and should be used with caution to avoid losing all data. - **/
-sql**: Want to directly interact with the bot's database? This command lets you
-run SQL queries. It's a powerful feature for managing and analyzing data, but
-be cautious to avoid mistakes. - **/logs**: This command gives you access to
-the bot's logs. It's useful for monitoring the bot's activity, spotting errors,
-and understanding user interactions. > [!IMPORTANT] > Administrative commands
-are restricted to the users whose Telegram IDs are specified in the [.env]
-(https://github.com/Simatwa/pytgpt-bot/blob/
-308f6079d153a429c445649896840fdc7cbfac11/env#L12) file. ## Further Tips - The
-bot features inline query for text generation. The query must end with *three
-ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/
-pytgpt_bot). `/setinline` - You can as well add the bot to a Telegram channel.
-Grant it read and delete permissions. The access commands will still work out.
-`@bot_username ` will trigger **text generation**. - Channel Admin will control
-the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
-## Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+use it effectively. ### Administrative Commands - **/clear**: Use this command
+to remove all chat data from the bot's database. It's a powerful tool, so use
+it carefully to avoid losing important data. - **/total**: This command shows
+you the total number of chats the bot has handled. It's a quick way to see how
+much interaction the bot has had. - **/drop**: If you need to completely wipe
+out all chat data and logs, use this command. It's more extreme than `/clear`
+and should be used with caution to avoid losing all data. - **/sql**: Want to
+directly interact with the bot's database? This command lets you run SQL
+queries. It's a powerful feature for managing and analyzing data, but be
+cautious to avoid mistakes. - **/logs**: This command gives you access to the
+bot's logs. It's useful for monitoring the bot's activity, spotting errors, and
+understanding user interactions. > [!IMPORTANT] > Administrative commands are
+restricted to the users whose Telegram IDs are specified in the [.env](https://
+github.com/Simatwa/pytgpt-bot/blob/308f6079d153a429c445649896840fdc7cbfac11/
+env#L12) file. ## Further Tips - The bot features inline query for text
+generation. The query must end with *three ellipsis* `...`. Remember to enable
+the mode from [@BotFather](https://t.me/pytgpt_bot). `/setinline` - You can as
+well add the bot to a Telegram channel. Grant it read and delete permissions.
+The access commands will still work out. `@bot_username ` will trigger **text
+generation**. - Channel Admin will control the bot access using the `/suspend`
+and `/resume` commands. *(Experimental).* ## Support and Feedback If you have
+any questions, feedback, or suggestions for `pytgpt`, please feel free to reach
+out. Your input is valuable in helping us improve and expand the bot's
+capabilities. ## License `pytgpt-bot` is open-source and available under the
+[MIT License](LICENSE). Feel free to use, modify, and distribute the code as
+you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
+interactions!
```

### Comparing `pytgpt_bot-0.1.3/README.md` & `pytgpt_bot-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -100,18 +100,14 @@
 - `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 > [!TIP]
 > For a better understanding of these commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/pytgpt_bot). This can give you a practical idea of how the bot works and how to use it effectively.
 
 ### Administrative Commands
 
-To make the administrative commands more understandable, let's simplify the descriptions and provide a bit more context for each command. This should help administrators manage the bot more effectively.
-
-### Simplified Administrative Commands
-
 - **/clear**: Use this command to remove all chat data from the bot's database. It's a powerful tool, so use it carefully to avoid losing important data.
 
 - **/total**: This command shows you the total number of chats the bot has handled. It's a quick way to see how much interaction the bot has had.
 
 - **/drop**: If you need to completely wipe out all chat data and logs, use this command. It's more extreme than `/clear` and should be used with caution to avoid losing all data.
 
 - **/sql**: Want to directly interact with the bot's database? This command lets you run SQL queries. It's a powerful feature for managing and analyzing data, but be cautious to avoid mistakes.
```

#### html2text {}

```diff
@@ -37,37 +37,34 @@
 Delete everything from the chat table and bot logs. This is more extreme than
 `/clear`. - **/sql**: Run SQL queries on the bot's database. Use this with
 caution! - **/logs**: Check the bot's logs for activity, errors, and user
 interactions. - `any other text`: An alias for `/chat`, allowing users to
 continue with chatting. > [!TIP] > For a better understanding of these
 commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/
 pytgpt_bot). This can give you a practical idea of how the bot works and how to
-use it effectively. ### Administrative Commands To make the administrative
-commands more understandable, let's simplify the descriptions and provide a bit
-more context for each command. This should help administrators manage the bot
-more effectively. ### Simplified Administrative Commands - **/clear**: Use this
-command to remove all chat data from the bot's database. It's a powerful tool,
-so use it carefully to avoid losing important data. - **/total**: This command
-shows you the total number of chats the bot has handled. It's a quick way to
-see how much interaction the bot has had. - **/drop**: If you need to
-completely wipe out all chat data and logs, use this command. It's more extreme
-than `/clear` and should be used with caution to avoid losing all data. - **/
-sql**: Want to directly interact with the bot's database? This command lets you
-run SQL queries. It's a powerful feature for managing and analyzing data, but
-be cautious to avoid mistakes. - **/logs**: This command gives you access to
-the bot's logs. It's useful for monitoring the bot's activity, spotting errors,
-and understanding user interactions. > [!IMPORTANT] > Administrative commands
-are restricted to the users whose Telegram IDs are specified in the [.env]
-(https://github.com/Simatwa/pytgpt-bot/blob/
-308f6079d153a429c445649896840fdc7cbfac11/env#L12) file. ## Further Tips - The
-bot features inline query for text generation. The query must end with *three
-ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/
-pytgpt_bot). `/setinline` - You can as well add the bot to a Telegram channel.
-Grant it read and delete permissions. The access commands will still work out.
-`@bot_username ` will trigger **text generation**. - Channel Admin will control
-the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
-## Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+use it effectively. ### Administrative Commands - **/clear**: Use this command
+to remove all chat data from the bot's database. It's a powerful tool, so use
+it carefully to avoid losing important data. - **/total**: This command shows
+you the total number of chats the bot has handled. It's a quick way to see how
+much interaction the bot has had. - **/drop**: If you need to completely wipe
+out all chat data and logs, use this command. It's more extreme than `/clear`
+and should be used with caution to avoid losing all data. - **/sql**: Want to
+directly interact with the bot's database? This command lets you run SQL
+queries. It's a powerful feature for managing and analyzing data, but be
+cautious to avoid mistakes. - **/logs**: This command gives you access to the
+bot's logs. It's useful for monitoring the bot's activity, spotting errors, and
+understanding user interactions. > [!IMPORTANT] > Administrative commands are
+restricted to the users whose Telegram IDs are specified in the [.env](https://
+github.com/Simatwa/pytgpt-bot/blob/308f6079d153a429c445649896840fdc7cbfac11/
+env#L12) file. ## Further Tips - The bot features inline query for text
+generation. The query must end with *three ellipsis* `...`. Remember to enable
+the mode from [@BotFather](https://t.me/pytgpt_bot). `/setinline` - You can as
+well add the bot to a Telegram channel. Grant it read and delete permissions.
+The access commands will still work out. `@bot_username ` will trigger **text
+generation**. - Channel Admin will control the bot access using the `/suspend`
+and `/resume` commands. *(Experimental).* ## Support and Feedback If you have
+any questions, feedback, or suggestions for `pytgpt`, please feel free to reach
+out. Your input is valuable in helping us improve and expand the bot's
+capabilities. ## License `pytgpt-bot` is open-source and available under the
+[MIT License](LICENSE). Feel free to use, modify, and distribute the code as
+you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
+interactions!
```

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.4/pytgpt_bot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 @click.group()
 @click.version_option(
     __version__, "-v", "--version", package_name="pytgpt-bot", prog_name="pytgpt-bot"
 )
 @click.help_option("-h", "--help")
 def bot():
-    """Telegram bot for text generation, text-to-image and text-to-audio conversions."""
+    """Telegram bot for text generation, text-to-image and text-to-speech conversions."""
     pass
 
 
 @click.command(context_settings=context_settings)
 @click.argument("token", required=True)
 @click.option(
     "-m",
@@ -39,15 +39,15 @@
     default=30,
 )
 @click.option(
     "-v",
     "--voice",
     type=click.Choice(Audio.all_voices),
     metavar="|".join(Audio.all_voices[:10]),
-    help="The voice to use for speech synthesis",
+    help="The default voice for speech synthesis",
     default="Brian",
 )
 @click.option(
     "-l",
     "--loglevel",
     type=click.Choice(["10", "20", "30", "40", "50", "51"]),
     default="20",
@@ -85,15 +85,19 @@
     for key, value in kwargs.items():
         modded_kwargs[key.replace("_", "-")] = str(value) if value else ""
 
     environ.update(modded_kwargs)
     try:
         from pytgpt_bot.main import bot
 
-        bot.infinity_polling(timeout=kwargs.get("timeout"), skip_pending=True)
+        bot.infinity_polling(
+            timeout=kwargs.get("timeout"),
+            skip_pending=True,
+            long_polling_timeout=kwargs.get("timeout"),
+        )
     except Exception as e:
         logging.error(e.args[1] if e.args and len(e.args) > 1 else str(e))
         click.secho("[^] Quitting", fg="yellow")
 
 
 @click.command()
 @click.option("-y", "--yes", is_flag=True, help="Okay to confirmations")
```

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot/config.py` & `pytgpt_bot-0.1.4/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot/db.py` & `pytgpt_bot-0.1.4/pytgpt_bot/db.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot/filters.py` & `pytgpt_bot-0.1.4/pytgpt_bot/filters.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot/main.py` & `pytgpt_bot-0.1.4/pytgpt_bot/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import telebot.util as telebot_util
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 from functools import wraps
 from sqlalchemy import text
+from uuid import uuid4
 
 from pytgpt_bot import __version__, __repo__
 
 from pytgpt_bot.config import (
     bot_token,
     max_tokens,
     timeout,
@@ -22,17 +23,16 @@
 )
 from pytgpt_bot.db import User
 from pytgpt_bot.utils import (
     provider_keys,
     get_random_emoji,
     provider_map,
     make_delete_markup,
-    make_regenerate_and_delete_markup,
 )
-from pytgpt_bot.models import session, Chat, create_all, drop_all
+from pytgpt_bot.models import session, Chat, Temp, create_all, drop_all
 from pytgpt_bot.filters import (
     IsActiveFilter,
     IsBotOwnerFilter,
     IsAdminFilter,
     IsBotTaggedFilter,
     IsChatCommandFilter,
 )
@@ -87,19 +87,19 @@
     "\t\t\t/prodia Clear cool shore view\n"
     "\t\t\t/speak I am better than you.\n\n"
     f"[🌟 Star me on Github]({__repo__}) pytgpt-bot v{__version__}"
 )
 
 admin_commands = (
     "\n\nAdmin Commands\n"
-    "/clear : Clear all chats 🧹\n"
+    "/clear : Clear all tables 🧹\n"
     "/total : Total chats available 📊\n"
-    "/drop : Clear entire chat table and bot logs 🗑️\n"
+    "/drop : Delete all tables and bot logs 🗑️\n"
     "/sql : Run sql statements against database ⏳\n"
-    "/logs : View bot logs 📜"
+    "/logs : View bot's log 📜"
 )
 
 
 def handler_formatter(text: bool = False, preserve: bool = False):
     """Handles common message handler verification and execptions
 
     Args:
@@ -200,14 +200,46 @@
         for part in parts:
             if as_reply:
                 bot.reply_to(message, part, parse_mode=parse_mode)
             else:
                 bot.send_message(message.chat.id, part, parse_mode=parse_mode)
 
 
+def make_regenerate_and_delete_markup(
+    message: telebot.types.Message, provider: str, prompt: str
+) -> telebot.types.InlineKeyboardMarkup:
+    """Makes a markup for deleting and regenerating images and speeches (media).
+
+    Args:
+        message (telebot.types.Message): Message object.
+        provider (str): Image provider. default/prodia.
+        prompt (str): text
+
+    Returns:
+        telebot.types.InlineKeyboardMarkup: Markup
+    """
+    markup = telebot.types.InlineKeyboardMarkup(row_width=2)
+    uuid = uuid4().__str__()
+    session.add(
+        Temp(
+            uuid=uuid,
+            provider=provider,
+            prompt=prompt,
+        )
+    )
+    regenerate_button = telebot.types.InlineKeyboardButton(
+        text="♻️", callback_data=f"media:{message.from_user.id}:{uuid}"
+    )
+    delete_button = telebot.types.InlineKeyboardButton(
+        text="🗑️", callback_data=f"delete:{message.chat.id}:{message.id}"
+    )
+    markup.add(regenerate_button, delete_button)
+    return markup
+
+
 @bot.message_handler(commands=["help", "start"], is_chat_active=True)
 @bot.channel_post_handler(commands=["help", "start"], is_chat_active=True)
 @handler_formatter()
 def home(message: telebot.types.Message):
     """Show help"""
     # print(message)
     return bot.send_message(
@@ -503,25 +535,26 @@
     chat = User(message).chat
     chat.is_active = True
     return bot.reply_to(
         message, text=f"Service Resumed 🚀.", reply_markup=make_delete_markup(message)
     )
 
 
-@bot.message_handler(commands=["clear", "clear_chats"], is_bot_owner=True)
+@bot.message_handler(commands=["clear", "clear_tables"], is_bot_owner=True)
 @handler_formatter()
 def clear_chats(message: telebot.types.Message):
-    """Delete all chat entries"""
+    """Delete all Tables"""
     session.query(Chat).delete()
+    session.query(Temp).delete()
     logging.warning(
         f"Clearing Chats - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     return bot.reply_to(
         message,
-        f"{get_random_emoji('love')} Chats cleared successfully.",
+        f"{get_random_emoji('love')} Tables cleared successfully.",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["total", "total_chats"], is_bot_owner=True)
 @handler_formatter()
 def total_chats_query(message: telebot.types.Message):
@@ -533,31 +566,32 @@
     return bot.reply_to(
         message,
         f"Total Chats {total_chats}",
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["drop", "drop_chats"], is_bot_owner=True)
+@bot.message_handler(commands=["drop", "drop_tables"], is_bot_owner=True)
 @handler_formatter()
 def total_chats_table_and_logs(message: telebot.types.Message):
-    """Drop chat table and create new"""
+    """Drop all tables and create new"""
     if logfile:
         with open(logfile, "w") as fh:
-            fh.write(
-                f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
-            )
+            pass
+        logging.info(
+            f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
+        )
     logging.warning(
-        f"Dropping Chat table and reinitialize - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
+        f"Dropping all tables and recreate - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     drop_all()
     create_all()
     return bot.reply_to(
         message,
-        f"{get_random_emoji('love')} Chat table and bot logs dropped and new one created.",
+        f"{get_random_emoji('love')} All tables dropped and logs cleared. New one created.",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["sql"], is_bot_owner=True)
 @handler_formatter(text=True)
 def run_sql_statement(message: telebot.types.Message):
@@ -608,15 +642,14 @@
 
 @bot.message_handler(content_types=["text"], is_chat_active=True, is_chat_command=True)
 @bot.channel_post_handler(
     content_types=["text"],
     is_chat_active=True,
     commands=["chat"],
 )
-@handler_formatter()
 def text_chat(message: telebot.types.Message):
     """Text generation"""
     user = User(message)
     conversation = Conversation(max_tokens=max_tokens)
     conversation.chat_history = user.chat.history
     user_provider = provider_map.get(user.chat.provider)
     conversation_prompt = conversation.gen_complete_prompt(
@@ -629,28 +662,40 @@
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.chat.history = conversation.chat_history
     send_long_text(message, ai_response, as_reply=False if message.from_user else True)
 
 
-@bot.callback_query_handler(func=lambda call: call.data.startswith("media::"))
+@bot.callback_query_handler(func=lambda call: call.data.startswith("media:"))
 def media_regeneration_callback_handler(
     call: telebot.types.CallbackQuery,
 ):
     """Media regeneration callback handler"""
-    action, provider, prompt = call.data.split("::")
+    action, user_id, uuid = call.data.split(":")
     message = call.message
-    message.text = prompt
-    if provider == "prodia":
-        return text_to_image_prodia(message)
-    elif provider == "default":
-        return text_to_image_default(message)
-    elif provider == "speech":
-        return text_to_speech(message)
+    message.from_user.id = int(user_id)
+    temp = session.query(Temp).filter_by(uuid=uuid).first()
+
+    if temp:
+        message.text = temp.prompt
+        if temp.provider == "prodia":
+            return text_to_image_prodia(message)
+
+        elif temp.provider == "default":
+            return text_to_image_default(message)
+
+        elif temp.provider == "speech":
+            return text_to_speech(message)
+    else:
+        send_and_add_delete_button(
+            message,
+            f"{get_random_emoji('angry')} Cache containing that prompt was cleared!",
+            as_reply=True,
+        )
 
 
 @bot.inline_handler(lambda query: query.query.endswith("..."))
 def handle_inline_query(inline_query: telebot.types.InlineQuery):
     """Process the inline query and return AI response"""
     try:
         logging.info("Serving INLINE-QUERY - [{inline_query.from_user.id}].")
@@ -691,20 +736,20 @@
         message,
         usage_info,
         reply_markup=make_delete_markup(message),
         parse_mode="Markdown",
     )
 
 
-@bot.callback_query_handler(func=lambda call: call.data.startswith("delete::"))
+@bot.callback_query_handler(func=lambda call: call.data.startswith("delete:"))
 def delete_callback_handler(
     call: telebot.types.CallbackQuery,
 ):
     """Delete callback handler"""
-    action, trigger_chat_id, trigger_message_id = call.data.split("::")
+    action, trigger_chat_id, trigger_message_id = call.data.split(":")
     try:
         bot.delete_message(trigger_chat_id, trigger_message_id)
     except:
         pass
     try:
         bot.delete_message(call.message.chat.id, call.message.id)
     except:
```

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot/models.py` & `pytgpt_bot-0.1.4/pytgpt_bot/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.orm import declarative_base
+from sqlalchemy.orm import relationship
 from sqlalchemy import Column, Integer, Text, String, Boolean
 from pytgpt.utils import Conversation
 from pytgpt_bot.config import database as database_str
 from pytgpt_bot.config import provider as default_provider
 from pytgpt_bot.config import voice
 
 if not database_str:
@@ -29,14 +30,21 @@
     intro = Column(Text, default=Conversation.intro, nullable=False)
     provider = Column(String(20), default=default_provider, nullable=False)
     history = Column(Text, default="")
     voice = Column(String(30), default=voice, nullable=False)
     is_active = Column(Boolean, default=True, nullable=False)
 
 
+class Temp(Base):
+    __tablename__ = "temps"
+    uuid = Column(String(48), primary_key=True)
+    prompt = Column(Text)
+    provider = Column(String(20))
+
+
 def create_all():
     """Create tables from models"""
     Base.metadata.create_all(engine)
 
 
 def drop_all():
     """Drop all tables created"""
```

### Comparing `pytgpt_bot-0.1.3/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.4/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -139,18 +139,14 @@
 - `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 > [!TIP]
 > For a better understanding of these commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/pytgpt_bot). This can give you a practical idea of how the bot works and how to use it effectively.
 
 ### Administrative Commands
 
-To make the administrative commands more understandable, let's simplify the descriptions and provide a bit more context for each command. This should help administrators manage the bot more effectively.
-
-### Simplified Administrative Commands
-
 - **/clear**: Use this command to remove all chat data from the bot's database. It's a powerful tool, so use it carefully to avoid losing important data.
 
 - **/total**: This command shows you the total number of chats the bot has handled. It's a quick way to see how much interaction the bot has had.
 
 - **/drop**: If you need to completely wipe out all chat data and logs, use this command. It's more extreme than `/clear` and should be used with caution to avoid losing all data.
 
 - **/sql**: Want to directly interact with the bot's database? This command lets you run SQL queries. It's a powerful feature for managing and analyzing data, but be cautious to avoid mistakes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.3 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.4 Summary: Telegram bot for
 chatting, text-to-image and text-to-speech conversions Home-page: https://
 github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -62,37 +62,34 @@
 Delete everything from the chat table and bot logs. This is more extreme than
 `/clear`. - **/sql**: Run SQL queries on the bot's database. Use this with
 caution! - **/logs**: Check the bot's logs for activity, errors, and user
 interactions. - `any other text`: An alias for `/chat`, allowing users to
 continue with chatting. > [!TIP] > For a better understanding of these
 commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/
 pytgpt_bot). This can give you a practical idea of how the bot works and how to
-use it effectively. ### Administrative Commands To make the administrative
-commands more understandable, let's simplify the descriptions and provide a bit
-more context for each command. This should help administrators manage the bot
-more effectively. ### Simplified Administrative Commands - **/clear**: Use this
-command to remove all chat data from the bot's database. It's a powerful tool,
-so use it carefully to avoid losing important data. - **/total**: This command
-shows you the total number of chats the bot has handled. It's a quick way to
-see how much interaction the bot has had. - **/drop**: If you need to
-completely wipe out all chat data and logs, use this command. It's more extreme
-than `/clear` and should be used with caution to avoid losing all data. - **/
-sql**: Want to directly interact with the bot's database? This command lets you
-run SQL queries. It's a powerful feature for managing and analyzing data, but
-be cautious to avoid mistakes. - **/logs**: This command gives you access to
-the bot's logs. It's useful for monitoring the bot's activity, spotting errors,
-and understanding user interactions. > [!IMPORTANT] > Administrative commands
-are restricted to the users whose Telegram IDs are specified in the [.env]
-(https://github.com/Simatwa/pytgpt-bot/blob/
-308f6079d153a429c445649896840fdc7cbfac11/env#L12) file. ## Further Tips - The
-bot features inline query for text generation. The query must end with *three
-ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/
-pytgpt_bot). `/setinline` - You can as well add the bot to a Telegram channel.
-Grant it read and delete permissions. The access commands will still work out.
-`@bot_username ` will trigger **text generation**. - Channel Admin will control
-the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
-## Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+use it effectively. ### Administrative Commands - **/clear**: Use this command
+to remove all chat data from the bot's database. It's a powerful tool, so use
+it carefully to avoid losing important data. - **/total**: This command shows
+you the total number of chats the bot has handled. It's a quick way to see how
+much interaction the bot has had. - **/drop**: If you need to completely wipe
+out all chat data and logs, use this command. It's more extreme than `/clear`
+and should be used with caution to avoid losing all data. - **/sql**: Want to
+directly interact with the bot's database? This command lets you run SQL
+queries. It's a powerful feature for managing and analyzing data, but be
+cautious to avoid mistakes. - **/logs**: This command gives you access to the
+bot's logs. It's useful for monitoring the bot's activity, spotting errors, and
+understanding user interactions. > [!IMPORTANT] > Administrative commands are
+restricted to the users whose Telegram IDs are specified in the [.env](https://
+github.com/Simatwa/pytgpt-bot/blob/308f6079d153a429c445649896840fdc7cbfac11/
+env#L12) file. ## Further Tips - The bot features inline query for text
+generation. The query must end with *three ellipsis* `...`. Remember to enable
+the mode from [@BotFather](https://t.me/pytgpt_bot). `/setinline` - You can as
+well add the bot to a Telegram channel. Grant it read and delete permissions.
+The access commands will still work out. `@bot_username ` will trigger **text
+generation**. - Channel Admin will control the bot access using the `/suspend`
+and `/resume` commands. *(Experimental).* ## Support and Feedback If you have
+any questions, feedback, or suggestions for `pytgpt`, please feel free to reach
+out. Your input is valuable in helping us improve and expand the bot's
+capabilities. ## License `pytgpt-bot` is open-source and available under the
+[MIT License](LICENSE). Feel free to use, modify, and distribute the code as
+you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
+interactions!
```

### Comparing `pytgpt_bot-0.1.3/setup.py` & `pytgpt_bot-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.1.3",
+    version="0.1.4",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for chatting, text-to-image and text-to-speech conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
```

