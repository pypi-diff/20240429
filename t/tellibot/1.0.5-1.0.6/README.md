# Comparing `tmp/tellibot-1.0.5.tar.gz` & `tmp/tellibot-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellibot-1.0.5.tar", last modified: Mon Apr 29 16:30:18 2024, max compression
+gzip compressed data, was "tellibot-1.0.6.tar", last modified: Mon Apr 29 16:34:38 2024, max compression
```

## Comparing `tellibot-1.0.5.tar` & `tellibot-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:30:18.993071 tellibot-1.0.5/
--rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      636 2024-04-29 16:30:18.990079 tellibot-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 16:30:18.993071 tellibot-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      852 2024-04-29 16:30:07.000000 tellibot-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:30:18.862782 tellibot-1.0.5/tellibot/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:30:04.000000 tellibot-1.0.5/tellibot/__init__.py
--rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.5/tellibot/argparse.py
--rw-rw-rw-   0        0        0      445 2024-04-28 21:17:41.000000 tellibot-1.0.5/tellibot/model.py
--rw-rw-rw-   0        0        0     4486 2024-04-29 16:25:12.000000 tellibot-1.0.5/tellibot/tellibot.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:30:18.985076 tellibot-1.0.5/tellibot.egg-info/
--rw-rw-rw-   0        0        0      636 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 16:34:38.288406 tellibot-1.0.6/
+-rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:34:38.265482 tellibot-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:34:38.288406 tellibot-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      870 2024-04-29 16:34:31.000000 tellibot-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:34:36.521318 tellibot-1.0.6/tellibot/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:30:04.000000 tellibot-1.0.6/tellibot/__init__.py
+-rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.6/tellibot/argparse.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:34:36.647849 tellibot-1.0.6/tellibot/interpreter/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:29:40.000000 tellibot-1.0.6/tellibot/interpreter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:34:38.232924 tellibot-1.0.6/tellibot/interpreter/statements/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:29:52.000000 tellibot-1.0.6/tellibot/interpreter/statements/__init__.py
+-rw-rw-rw-   0        0        0      259 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_admin_word.py
+-rw-rw-rw-   0        0        0     1009 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_def_command.py
+-rw-rw-rw-   0        0        0      656 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_handle_admin_message.py
+-rw-rw-rw-   0        0        0      898 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_handle_message.py
+-rw-rw-rw-   0        0        0      419 2024-04-23 22:38:43.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_send_response.py
+-rw-rw-rw-   0        0        0      284 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_set_admin_username.py
+-rw-rw-rw-   0        0        0      341 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_set_buttons.py
+-rw-rw-rw-   0        0        0      254 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_set_token.py
+-rw-rw-rw-   0        0        0      269 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_set_username.py
+-rw-rw-rw-   0        0        0      337 2024-04-28 22:37:24.000000 tellibot-1.0.6/tellibot/interpreter/statements/bot_wait_for.py
+-rw-rw-rw-   0        0        0      294 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/controls_flow_statements.py
+-rw-rw-rw-   0        0        0      980 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/controls_for.py
+-rw-rw-rw-   0        0        0     1046 2024-04-23 22:27:28.000000 tellibot-1.0.6/tellibot/interpreter/statements/controls_forEach.py
+-rw-rw-rw-   0        0        0      800 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/controls_repeat_ext.py
+-rw-rw-rw-   0        0        0     1030 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/controls_whileUntil.py
+-rw-rw-rw-   0        0        0      956 2024-04-22 23:17:17.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_connect.py
+-rw-rw-rw-   0        0        0      582 2024-04-22 22:31:21.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_create_table.py
+-rw-rw-rw-   0        0        0      908 2024-04-23 21:20:25.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_delete_data.py
+-rw-rw-rw-   0        0        0      309 2024-04-22 22:36:40.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_delete_table.py
+-rw-rw-rw-   0        0        0      628 2024-04-23 21:22:03.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_insert.py
+-rw-rw-rw-   0        0        0     1385 2024-04-23 20:58:58.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_read.py
+-rw-rw-rw-   0        0        0      819 2024-04-23 21:20:00.000000 tellibot-1.0.6/tellibot/interpreter/statements/db_update.py
+-rw-rw-rw-   0        0        0      604 2024-04-22 22:56:12.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_create_with.py
+-rw-rw-rw-   0        0        0      287 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_get_all_keys.py
+-rw-rw-rw-   0        0        0      397 2024-04-28 20:03:27.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_get_value.py
+-rw-rw-rw-   0        0        0      367 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_key_exist.py
+-rw-rw-rw-   0        0        0      379 2024-04-22 22:55:15.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_pair.py
+-rw-rw-rw-   0        0        0      288 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_parse.py
+-rw-rw-rw-   0        0        0      417 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/dict_set_value.py
+-rw-rw-rw-   0        0        0     1177 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/function_procedures_callnoreturn.py
+-rw-rw-rw-   0        0        0      171 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/function_procedures_callreturn.py
+-rw-rw-rw-   0        0        0      608 2024-04-23 19:30:43.000000 tellibot-1.0.6/tellibot/interpreter/statements/function_procedures_defnoreturn.py
+-rw-rw-rw-   0        0        0      610 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/function_procedures_defreturn.py
+-rw-rw-rw-   0        0        0      487 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/function_procedures_ifreturn.py
+-rw-rw-rw-   0        0        0     1452 2024-04-23 22:27:33.000000 tellibot-1.0.6/tellibot/interpreter/statements/http_request.py
+-rw-rw-rw-   0        0        0      760 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_chooser.py
+-rw-rw-rw-   0        0        0      387 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_create_with.py
+-rw-rw-rw-   0        0        0     1859 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_getIndex.py
+-rw-rw-rw-   0        0        0     1396 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_getSublist.py
+-rw-rw-rw-   0        0        0      651 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_indexOf.py
+-rw-rw-rw-   0        0        0      309 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_isEmpty.py
+-rw-rw-rw-   0        0        0      298 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_length.py
+-rw-rw-rw-   0        0        0      569 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_regex.py
+-rw-rw-rw-   0        0        0      381 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_repeat.py
+-rw-rw-rw-   0        0        0     1796 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_setIndex.py
+-rw-rw-rw-   0        0        0     1106 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_sort.py
+-rw-rw-rw-   0        0        0      583 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/lists_split.py
+-rw-rw-rw-   0        0        0      220 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_boolean.py
+-rw-rw-rw-   0        0        0      782 2024-04-23 22:27:23.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_compare.py
+-rw-rw-rw-   0        0        0      501 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_confirm.py
+-rw-rw-rw-   0        0        0      692 2024-04-23 22:27:25.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_controls_if.py
+-rw-rw-rw-   0        0        0      359 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_negate.py
+-rw-rw-rw-   0        0        0      544 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_operation.py
+-rw-rw-rw-   0        0        0      612 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/logic_ternary.py
+-rw-rw-rw-   0        0        0     1714 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_arithmetic.py
+-rw-rw-rw-   0        0        0      579 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_change.py
+-rw-rw-rw-   0        0        0      715 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_constant.py
+-rw-rw-rw-   0        0        0      685 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_constrain.py
+-rw-rw-rw-   0        0        0      391 2024-04-23 20:08:59.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_convert_text_to_number.py
+-rw-rw-rw-   0        0        0      491 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_modulo.py
+-rw-rw-rw-   0        0        0      215 2024-04-22 22:16:40.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_number.py
+-rw-rw-rw-   0        0        0     1243 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_number_property.py
+-rw-rw-rw-   0        0        0     1508 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_on_list.py
+-rw-rw-rw-   0        0        0      236 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_random_float.py
+-rw-rw-rw-   0        0        0      434 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_random_int.py
+-rw-rw-rw-   0        0        0      678 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_round.py
+-rw-rw-rw-   0        0        0     1019 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_single.py
+-rw-rw-rw-   0        0        0      924 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/math_trig.py
+-rw-rw-rw-   0        0        0      886 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text.py
+-rw-rw-rw-   0        0        0      497 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_append.py
+-rw-rw-rw-   0        0        0      580 2024-04-22 21:24:06.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_changeCase.py
+-rw-rw-rw-   0        0        0      764 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_charAt.py
+-rw-rw-rw-   0        0        0      278 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_convert.py
+-rw-rw-rw-   0        0        0     2393 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_getSubstring.py
+-rw-rw-rw-   0        0        0      626 2024-04-23 22:28:36.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_indexOf.py
+-rw-rw-rw-   0        0        0      317 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_isEmpty.py
+-rw-rw-rw-   0        0        0      514 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_join.py
+-rw-rw-rw-   0        0        0      298 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_length.py
+-rw-rw-rw-   0        0        0      335 2024-04-29 14:59:51.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_print.py
+-rw-rw-rw-   0        0        0      674 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_prompt.py
+-rw-rw-rw-   0        0        0      556 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/text_trim.py
+-rw-rw-rw-   0        0        0      472 2024-04-23 21:15:01.000000 tellibot-1.0.6/tellibot/interpreter/statements/util_try_catch.py
+-rw-rw-rw-   0        0        0      337 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/variables_get.py
+-rw-rw-rw-   0        0        0      357 2024-04-22 21:24:10.000000 tellibot-1.0.6/tellibot/interpreter/statements/variables_set.py
+-rw-rw-rw-   0        0        0    22938 2024-04-29 16:10:10.000000 tellibot-1.0.6/tellibot/interpreter/tellibot.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:34:38.248314 tellibot-1.0.6/tellibot/interpreter/util/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:29:46.000000 tellibot-1.0.6/tellibot/interpreter/util/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-04-20 20:54:51.000000 tellibot-1.0.6/tellibot/interpreter/util/color.py
+-rw-rw-rw-   0        0        0      445 2024-04-28 21:17:41.000000 tellibot-1.0.6/tellibot/model.py
+-rw-rw-rw-   0        0        0     4486 2024-04-29 16:25:12.000000 tellibot-1.0.6/tellibot/tellibot.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:34:38.265482 tellibot-1.0.6/tellibot.egg-info/
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:34:36.000000 tellibot-1.0.6/tellibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4735 2024-04-29 16:34:36.000000 tellibot-1.0.6/tellibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:34:36.000000 tellibot-1.0.6/tellibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-29 16:34:36.000000 tellibot-1.0.6/tellibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-29 16:34:36.000000 tellibot-1.0.6/tellibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 16:34:36.000000 tellibot-1.0.6/tellibot.egg-info/top_level.txt
```

### Comparing `tellibot-1.0.5/LICENSE.txt` & `tellibot-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.5/PKG-INFO` & `tellibot-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.5
+Version: 1.0.6
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tellibot-1.0.5/setup.py` & `tellibot-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="tellibot",
-    version="1.0.5",
+    version="1.0.6",
     description="A drag and drop programming to create telegram bot",
     url="https://github.com/whoisjeeva/tellibot",
     author="Jeeva",
     author_email="support@gumify.me",
     license="MIT",
-    packages=["tellibot"],
+    packages=find_packages(),
     install_requires=[
         "Flask==3.0.3",
         "peewee==3.17.3",
         "requests==2.31.0",
         "python-telegram-bot==21.1.1",
         "PyMySQL==1.1.0",
         "Flask-SocketIO==5.3.6",
```

### Comparing `tellibot-1.0.5/tellibot/argparse.py` & `tellibot-1.0.6/tellibot/argparse.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.5/tellibot/tellibot.py` & `tellibot-1.0.6/tellibot/tellibot.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.5/tellibot.egg-info/PKG-INFO` & `tellibot-1.0.6/tellibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.5
+Version: 1.0.6
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

