# Comparing `tmp/tellibot-1.0.7.tar.gz` & `tmp/tellibot-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellibot-1.0.7.tar", last modified: Mon Apr 29 16:44:14 2024, max compression
+gzip compressed data, was "tellibot-1.0.8.tar", last modified: Mon Apr 29 16:49:10 2024, max compression
```

## Comparing `tellibot-1.0.7.tar` & `tellibot-1.0.8.tar`

### file list

```diff
@@ -1,152 +1,157 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.811294 tellibot-1.0.7/
--rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       96 2024-04-29 16:44:08.000000 tellibot-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      636 2024-04-29 16:44:14.794524 tellibot-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 16:44:14.811294 tellibot-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-04-29 16:42:44.000000 tellibot-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:11.977283 tellibot-1.0.7/tellibot/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:30:04.000000 tellibot-1.0.7/tellibot/__init__.py
--rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.7/tellibot/argparse.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:12.177545 tellibot-1.0.7/tellibot/interpreter/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:29:40.000000 tellibot-1.0.7/tellibot/interpreter/__init__.py
--rw-rw-rw-   0        0        0    21918 2024-04-29 16:37:44.000000 tellibot-1.0.7/tellibot/interpreter/interpreter.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:13.878268 tellibot-1.0.7/tellibot/interpreter/statements/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:29:52.000000 tellibot-1.0.7/tellibot/interpreter/statements/__init__.py
--rw-rw-rw-   0        0        0      259 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_admin_word.py
--rw-rw-rw-   0        0        0     1009 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_def_command.py
--rw-rw-rw-   0        0        0      656 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_handle_admin_message.py
--rw-rw-rw-   0        0        0      898 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_handle_message.py
--rw-rw-rw-   0        0        0      419 2024-04-23 22:38:43.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_send_response.py
--rw-rw-rw-   0        0        0      284 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_set_admin_username.py
--rw-rw-rw-   0        0        0      341 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_set_buttons.py
--rw-rw-rw-   0        0        0      254 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_set_token.py
--rw-rw-rw-   0        0        0      269 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_set_username.py
--rw-rw-rw-   0        0        0      337 2024-04-28 22:37:24.000000 tellibot-1.0.7/tellibot/interpreter/statements/bot_wait_for.py
--rw-rw-rw-   0        0        0      294 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/controls_flow_statements.py
--rw-rw-rw-   0        0        0      980 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/controls_for.py
--rw-rw-rw-   0        0        0     1046 2024-04-23 22:27:28.000000 tellibot-1.0.7/tellibot/interpreter/statements/controls_forEach.py
--rw-rw-rw-   0        0        0      800 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/controls_repeat_ext.py
--rw-rw-rw-   0        0        0     1030 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/controls_whileUntil.py
--rw-rw-rw-   0        0        0      956 2024-04-22 23:17:17.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_connect.py
--rw-rw-rw-   0        0        0      582 2024-04-22 22:31:21.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_create_table.py
--rw-rw-rw-   0        0        0      908 2024-04-23 21:20:25.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_delete_data.py
--rw-rw-rw-   0        0        0      309 2024-04-22 22:36:40.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_delete_table.py
--rw-rw-rw-   0        0        0      628 2024-04-23 21:22:03.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_insert.py
--rw-rw-rw-   0        0        0     1385 2024-04-23 20:58:58.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_read.py
--rw-rw-rw-   0        0        0      819 2024-04-23 21:20:00.000000 tellibot-1.0.7/tellibot/interpreter/statements/db_update.py
--rw-rw-rw-   0        0        0      604 2024-04-22 22:56:12.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_create_with.py
--rw-rw-rw-   0        0        0      287 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_get_all_keys.py
--rw-rw-rw-   0        0        0      397 2024-04-28 20:03:27.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_get_value.py
--rw-rw-rw-   0        0        0      367 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_key_exist.py
--rw-rw-rw-   0        0        0      379 2024-04-22 22:55:15.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_pair.py
--rw-rw-rw-   0        0        0      288 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_parse.py
--rw-rw-rw-   0        0        0      417 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/dict_set_value.py
--rw-rw-rw-   0        0        0     1177 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_callnoreturn.py
--rw-rw-rw-   0        0        0      171 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_callreturn.py
--rw-rw-rw-   0        0        0      608 2024-04-23 19:30:43.000000 tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_defnoreturn.py
--rw-rw-rw-   0        0        0      610 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_defreturn.py
--rw-rw-rw-   0        0        0      487 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_ifreturn.py
--rw-rw-rw-   0        0        0     1452 2024-04-23 22:27:33.000000 tellibot-1.0.7/tellibot/interpreter/statements/http_request.py
--rw-rw-rw-   0        0        0      760 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_chooser.py
--rw-rw-rw-   0        0        0      387 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_create_with.py
--rw-rw-rw-   0        0        0     1859 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_getIndex.py
--rw-rw-rw-   0        0        0     1396 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_getSublist.py
--rw-rw-rw-   0        0        0      651 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_indexOf.py
--rw-rw-rw-   0        0        0      309 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_isEmpty.py
--rw-rw-rw-   0        0        0      298 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_length.py
--rw-rw-rw-   0        0        0      569 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_regex.py
--rw-rw-rw-   0        0        0      381 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_repeat.py
--rw-rw-rw-   0        0        0     1796 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_setIndex.py
--rw-rw-rw-   0        0        0     1106 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_sort.py
--rw-rw-rw-   0        0        0      583 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/lists_split.py
--rw-rw-rw-   0        0        0      220 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_boolean.py
--rw-rw-rw-   0        0        0      782 2024-04-23 22:27:23.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_compare.py
--rw-rw-rw-   0        0        0      501 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_confirm.py
--rw-rw-rw-   0        0        0      692 2024-04-23 22:27:25.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_controls_if.py
--rw-rw-rw-   0        0        0      359 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_negate.py
--rw-rw-rw-   0        0        0      544 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_operation.py
--rw-rw-rw-   0        0        0      612 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/logic_ternary.py
--rw-rw-rw-   0        0        0     1714 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_arithmetic.py
--rw-rw-rw-   0        0        0      579 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_change.py
--rw-rw-rw-   0        0        0      715 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_constant.py
--rw-rw-rw-   0        0        0      685 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_constrain.py
--rw-rw-rw-   0        0        0      391 2024-04-23 20:08:59.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_convert_text_to_number.py
--rw-rw-rw-   0        0        0      491 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_modulo.py
--rw-rw-rw-   0        0        0      215 2024-04-22 22:16:40.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_number.py
--rw-rw-rw-   0        0        0     1243 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_number_property.py
--rw-rw-rw-   0        0        0     1508 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_on_list.py
--rw-rw-rw-   0        0        0      236 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_random_float.py
--rw-rw-rw-   0        0        0      434 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_random_int.py
--rw-rw-rw-   0        0        0      678 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_round.py
--rw-rw-rw-   0        0        0     1019 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_single.py
--rw-rw-rw-   0        0        0      924 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/math_trig.py
--rw-rw-rw-   0        0        0      886 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text.py
--rw-rw-rw-   0        0        0      497 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_append.py
--rw-rw-rw-   0        0        0      580 2024-04-22 21:24:06.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_changeCase.py
--rw-rw-rw-   0        0        0      764 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_charAt.py
--rw-rw-rw-   0        0        0      278 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_convert.py
--rw-rw-rw-   0        0        0     2393 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_getSubstring.py
--rw-rw-rw-   0        0        0      626 2024-04-23 22:28:36.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_indexOf.py
--rw-rw-rw-   0        0        0      317 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_isEmpty.py
--rw-rw-rw-   0        0        0      514 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_join.py
--rw-rw-rw-   0        0        0      298 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_length.py
--rw-rw-rw-   0        0        0      335 2024-04-29 14:59:51.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_print.py
--rw-rw-rw-   0        0        0      674 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_prompt.py
--rw-rw-rw-   0        0        0      556 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/text_trim.py
--rw-rw-rw-   0        0        0      472 2024-04-23 21:15:01.000000 tellibot-1.0.7/tellibot/interpreter/statements/util_try_catch.py
--rw-rw-rw-   0        0        0      337 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/variables_get.py
--rw-rw-rw-   0        0        0      357 2024-04-22 21:24:10.000000 tellibot-1.0.7/tellibot/interpreter/statements/variables_set.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:13.916056 tellibot-1.0.7/tellibot/interpreter/util/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:29:46.000000 tellibot-1.0.7/tellibot/interpreter/util/__init__.py
--rw-rw-rw-   0        0        0     2908 2024-04-20 20:54:51.000000 tellibot-1.0.7/tellibot/interpreter/util/color.py
--rw-rw-rw-   0        0        0      445 2024-04-29 16:37:57.000000 tellibot-1.0.7/tellibot/model.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:11.799905 tellibot-1.0.7/tellibot/static/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:13.928375 tellibot-1.0.7/tellibot/static/css/
--rw-rw-rw-   0        0        0     3014 2024-04-28 22:10:32.000000 tellibot-1.0.7/tellibot/static/css/editor.css
--rw-rw-rw-   0        0        0      622 2024-04-28 22:11:18.000000 tellibot-1.0.7/tellibot/static/css/main.css
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.028029 tellibot-1.0.7/tellibot/static/dist/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.178223 tellibot-1.0.7/tellibot/static/dist/.maps/
--rw-rw-rw-   0        0        0  1610684 2022-04-12 01:31:16.000000 tellibot-1.0.7/tellibot/static/dist/.maps/bundle.min.js.map
--rw-rw-rw-   0        0        0     5568 2022-04-12 01:16:44.000000 tellibot-1.0.7/tellibot/static/dist/.maps/compose.min.js.map
--rw-rw-rw-   0        0        0   144629 2024-04-23 00:02:37.000000 tellibot-1.0.7/tellibot/static/dist/.maps/editor.min.js.map
--rw-rw-rw-   0        0        0   788106 2024-04-22 18:42:54.000000 tellibot-1.0.7/tellibot/static/dist/bundle.min.js
--rw-rw-rw-   0        0        0    69133 2024-04-28 22:39:45.000000 tellibot-1.0.7/tellibot/static/dist/editor.min.js
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.214167 tellibot-1.0.7/tellibot/static/font/
--rw-rw-rw-   0        0        0   124372 2022-04-12 06:52:31.000000 tellibot-1.0.7/tellibot/static/font/icons.woff2
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.648653 tellibot-1.0.7/tellibot/static/media/
--rw-rw-rw-   0        0        0       43 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/1x1.gif
--rw-rw-rw-   0        0        0     2304 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/click.mp3
--rw-rw-rw-   0        0        0     4865 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/click.ogg
--rw-rw-rw-   0        0        0     3782 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/click.wav
--rw-rw-rw-   0        0        0     3123 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/delete.mp3
--rw-rw-rw-   0        0        0     5731 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/delete.ogg
--rw-rw-rw-   0        0        0     9164 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/delete.wav
--rw-rw-rw-   0        0        0     1586 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/disconnect.mp3
--rw-rw-rw-   0        0        0     4404 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/disconnect.ogg
--rw-rw-rw-   0        0        0     1492 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/disconnect.wav
--rw-rw-rw-   0        0        0      569 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/dropdown-arrow.svg
--rw-rw-rw-   0        0        0      326 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/handclosed.cur
--rw-rw-rw-   0        0        0      766 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/handdelete.cur
--rw-rw-rw-   0        0        0      198 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/handopen.cur
--rw-rw-rw-   0        0        0     1010 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/pilcrow.png
--rw-rw-rw-   0        0        0      771 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/quote0.png
--rw-rw-rw-   0        0        0      738 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/quote1.png
--rw-rw-rw-   0        0        0     2595 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/sprites.png
--rw-rw-rw-   0        0        0     1849 2020-06-15 14:02:44.000000 tellibot-1.0.7/tellibot/static/media/sprites.svg
--rw-rw-rw-   0        0        0     4489 2024-04-29 16:37:17.000000 tellibot-1.0.7/tellibot/tellibot.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.677852 tellibot-1.0.7/tellibot/templates/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.677852 tellibot-1.0.7/tellibot/templates/editor/
--rw-rw-rw-   0        0        0     6160 2024-04-28 22:19:00.000000 tellibot-1.0.7/tellibot/templates/editor/index.html
--rw-rw-rw-   0        0        0     3372 2024-04-28 22:21:10.000000 tellibot-1.0.7/tellibot/templates/index.html
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.761177 tellibot-1.0.7/tellibot/templates/scripts/
--rw-rw-rw-   0        0        0     2284 2024-04-28 22:04:58.000000 tellibot-1.0.7/tellibot/templates/scripts/009c829d-ba57-4ff4-83e3-1e85f79319fa.tel
--rw-rw-rw-   0        0        0   363436 2024-04-28 22:23:31.000000 tellibot-1.0.7/tellibot/templates/scripts/07a8c2fa-cd42-45d6-b488-460b18ce9dec.tel
--rw-rw-rw-   0        0        0   287360 2024-04-28 22:49:19.000000 tellibot-1.0.7/tellibot/templates/scripts/aae450d9-e709-4bbd-94ed-3290f084f9a9.tel
-drwxrwxrwx   0        0        0        0 2024-04-29 16:44:14.793449 tellibot-1.0.7/tellibot.egg-info/
--rw-rw-rw-   0        0        0      636 2024-04-29 16:44:11.000000 tellibot-1.0.7/tellibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5974 2024-04-29 16:44:11.000000 tellibot-1.0.7/tellibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:44:11.000000 tellibot-1.0.7/tellibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-29 16:44:11.000000 tellibot-1.0.7/tellibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-29 16:44:11.000000 tellibot-1.0.7/tellibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 16:44:11.000000 tellibot-1.0.7/tellibot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:10.007816 tellibot-1.0.8/
+-rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       96 2024-04-29 16:44:08.000000 tellibot-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:49:09.994818 tellibot-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:49:10.008817 tellibot-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      979 2024-04-29 16:49:00.000000 tellibot-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:07.612422 tellibot-1.0.8/tellibot/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:30:04.000000 tellibot-1.0.8/tellibot/__init__.py
+-rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.8/tellibot/argparse.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:07.790635 tellibot-1.0.8/tellibot/interpreter/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:29:40.000000 tellibot-1.0.8/tellibot/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    21918 2024-04-29 16:37:44.000000 tellibot-1.0.8/tellibot/interpreter/interpreter.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.260144 tellibot-1.0.8/tellibot/interpreter/statements/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:29:52.000000 tellibot-1.0.8/tellibot/interpreter/statements/__init__.py
+-rw-rw-rw-   0        0        0      259 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_admin_word.py
+-rw-rw-rw-   0        0        0     1009 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_def_command.py
+-rw-rw-rw-   0        0        0      656 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_handle_admin_message.py
+-rw-rw-rw-   0        0        0      898 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_handle_message.py
+-rw-rw-rw-   0        0        0      419 2024-04-23 22:38:43.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_send_response.py
+-rw-rw-rw-   0        0        0      284 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_set_admin_username.py
+-rw-rw-rw-   0        0        0      341 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_set_buttons.py
+-rw-rw-rw-   0        0        0      254 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_set_token.py
+-rw-rw-rw-   0        0        0      269 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_set_username.py
+-rw-rw-rw-   0        0        0      337 2024-04-28 22:37:24.000000 tellibot-1.0.8/tellibot/interpreter/statements/bot_wait_for.py
+-rw-rw-rw-   0        0        0      294 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/controls_flow_statements.py
+-rw-rw-rw-   0        0        0      980 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/controls_for.py
+-rw-rw-rw-   0        0        0     1046 2024-04-23 22:27:28.000000 tellibot-1.0.8/tellibot/interpreter/statements/controls_forEach.py
+-rw-rw-rw-   0        0        0      800 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/controls_repeat_ext.py
+-rw-rw-rw-   0        0        0     1030 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/controls_whileUntil.py
+-rw-rw-rw-   0        0        0      956 2024-04-22 23:17:17.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_connect.py
+-rw-rw-rw-   0        0        0      582 2024-04-22 22:31:21.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_create_table.py
+-rw-rw-rw-   0        0        0      908 2024-04-23 21:20:25.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_delete_data.py
+-rw-rw-rw-   0        0        0      309 2024-04-22 22:36:40.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_delete_table.py
+-rw-rw-rw-   0        0        0      628 2024-04-23 21:22:03.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_insert.py
+-rw-rw-rw-   0        0        0     1385 2024-04-23 20:58:58.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_read.py
+-rw-rw-rw-   0        0        0      819 2024-04-23 21:20:00.000000 tellibot-1.0.8/tellibot/interpreter/statements/db_update.py
+-rw-rw-rw-   0        0        0      604 2024-04-22 22:56:12.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_create_with.py
+-rw-rw-rw-   0        0        0      287 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_get_all_keys.py
+-rw-rw-rw-   0        0        0      397 2024-04-28 20:03:27.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_get_value.py
+-rw-rw-rw-   0        0        0      367 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_key_exist.py
+-rw-rw-rw-   0        0        0      379 2024-04-22 22:55:15.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_pair.py
+-rw-rw-rw-   0        0        0      288 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_parse.py
+-rw-rw-rw-   0        0        0      417 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/dict_set_value.py
+-rw-rw-rw-   0        0        0     1177 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_callnoreturn.py
+-rw-rw-rw-   0        0        0      171 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_callreturn.py
+-rw-rw-rw-   0        0        0      608 2024-04-23 19:30:43.000000 tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_defnoreturn.py
+-rw-rw-rw-   0        0        0      610 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_defreturn.py
+-rw-rw-rw-   0        0        0      487 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_ifreturn.py
+-rw-rw-rw-   0        0        0     1452 2024-04-23 22:27:33.000000 tellibot-1.0.8/tellibot/interpreter/statements/http_request.py
+-rw-rw-rw-   0        0        0      760 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_chooser.py
+-rw-rw-rw-   0        0        0      387 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_create_with.py
+-rw-rw-rw-   0        0        0     1859 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_getIndex.py
+-rw-rw-rw-   0        0        0     1396 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_getSublist.py
+-rw-rw-rw-   0        0        0      651 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_indexOf.py
+-rw-rw-rw-   0        0        0      309 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_isEmpty.py
+-rw-rw-rw-   0        0        0      298 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_length.py
+-rw-rw-rw-   0        0        0      569 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_regex.py
+-rw-rw-rw-   0        0        0      381 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_repeat.py
+-rw-rw-rw-   0        0        0     1796 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_setIndex.py
+-rw-rw-rw-   0        0        0     1106 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_sort.py
+-rw-rw-rw-   0        0        0      583 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/lists_split.py
+-rw-rw-rw-   0        0        0      220 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_boolean.py
+-rw-rw-rw-   0        0        0      782 2024-04-23 22:27:23.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_compare.py
+-rw-rw-rw-   0        0        0      501 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_confirm.py
+-rw-rw-rw-   0        0        0      692 2024-04-23 22:27:25.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_controls_if.py
+-rw-rw-rw-   0        0        0      359 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_negate.py
+-rw-rw-rw-   0        0        0      544 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_operation.py
+-rw-rw-rw-   0        0        0      612 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/logic_ternary.py
+-rw-rw-rw-   0        0        0     1714 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_arithmetic.py
+-rw-rw-rw-   0        0        0      579 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_change.py
+-rw-rw-rw-   0        0        0      715 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_constant.py
+-rw-rw-rw-   0        0        0      685 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_constrain.py
+-rw-rw-rw-   0        0        0      391 2024-04-23 20:08:59.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_convert_text_to_number.py
+-rw-rw-rw-   0        0        0      491 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_modulo.py
+-rw-rw-rw-   0        0        0      215 2024-04-22 22:16:40.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_number.py
+-rw-rw-rw-   0        0        0     1243 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_number_property.py
+-rw-rw-rw-   0        0        0     1508 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_on_list.py
+-rw-rw-rw-   0        0        0      236 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_random_float.py
+-rw-rw-rw-   0        0        0      434 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_random_int.py
+-rw-rw-rw-   0        0        0      678 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_round.py
+-rw-rw-rw-   0        0        0     1019 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_single.py
+-rw-rw-rw-   0        0        0      924 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/math_trig.py
+-rw-rw-rw-   0        0        0      886 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text.py
+-rw-rw-rw-   0        0        0      497 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_append.py
+-rw-rw-rw-   0        0        0      580 2024-04-22 21:24:06.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_changeCase.py
+-rw-rw-rw-   0        0        0      764 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_charAt.py
+-rw-rw-rw-   0        0        0      278 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_convert.py
+-rw-rw-rw-   0        0        0     2393 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_getSubstring.py
+-rw-rw-rw-   0        0        0      626 2024-04-23 22:28:36.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_indexOf.py
+-rw-rw-rw-   0        0        0      317 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_isEmpty.py
+-rw-rw-rw-   0        0        0      514 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_join.py
+-rw-rw-rw-   0        0        0      298 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_length.py
+-rw-rw-rw-   0        0        0      335 2024-04-29 14:59:51.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_print.py
+-rw-rw-rw-   0        0        0      674 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_prompt.py
+-rw-rw-rw-   0        0        0      556 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/text_trim.py
+-rw-rw-rw-   0        0        0      472 2024-04-23 21:15:01.000000 tellibot-1.0.8/tellibot/interpreter/statements/util_try_catch.py
+-rw-rw-rw-   0        0        0      337 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/variables_get.py
+-rw-rw-rw-   0        0        0      357 2024-04-22 21:24:10.000000 tellibot-1.0.8/tellibot/interpreter/statements/variables_set.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.289027 tellibot-1.0.8/tellibot/interpreter/util/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:29:46.000000 tellibot-1.0.8/tellibot/interpreter/util/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-04-20 20:54:51.000000 tellibot-1.0.8/tellibot/interpreter/util/color.py
+-rw-rw-rw-   0        0        0      445 2024-04-29 16:37:57.000000 tellibot-1.0.8/tellibot/model.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:07.361621 tellibot-1.0.8/tellibot/static/
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.310183 tellibot-1.0.8/tellibot/static/css/
+-rw-rw-rw-   0        0        0     3014 2024-04-28 22:10:32.000000 tellibot-1.0.8/tellibot/static/css/editor.css
+-rw-rw-rw-   0        0        0      622 2024-04-28 22:11:18.000000 tellibot-1.0.8/tellibot/static/css/main.css
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.361554 tellibot-1.0.8/tellibot/static/dist/
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.460146 tellibot-1.0.8/tellibot/static/dist/.maps/
+-rw-rw-rw-   0        0        0  1610684 2022-04-12 01:31:16.000000 tellibot-1.0.8/tellibot/static/dist/.maps/bundle.min.js.map
+-rw-rw-rw-   0        0        0     5568 2022-04-12 01:16:44.000000 tellibot-1.0.8/tellibot/static/dist/.maps/compose.min.js.map
+-rw-rw-rw-   0        0        0   144629 2024-04-23 00:02:37.000000 tellibot-1.0.8/tellibot/static/dist/.maps/editor.min.js.map
+-rw-rw-rw-   0        0        0   788106 2024-04-22 18:42:54.000000 tellibot-1.0.8/tellibot/static/dist/bundle.min.js
+-rw-rw-rw-   0        0        0    69133 2024-04-28 22:39:45.000000 tellibot-1.0.8/tellibot/static/dist/editor.min.js
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.501743 tellibot-1.0.8/tellibot/static/font/
+-rw-rw-rw-   0        0        0   124372 2022-04-12 06:52:31.000000 tellibot-1.0.8/tellibot/static/font/icons.woff2
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.787680 tellibot-1.0.8/tellibot/static/media/
+-rw-rw-rw-   0        0        0       43 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/1x1.gif
+-rw-rw-rw-   0        0        0     2304 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/click.mp3
+-rw-rw-rw-   0        0        0     4865 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/click.ogg
+-rw-rw-rw-   0        0        0     3782 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/click.wav
+-rw-rw-rw-   0        0        0     3123 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/delete.mp3
+-rw-rw-rw-   0        0        0     5731 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/delete.ogg
+-rw-rw-rw-   0        0        0     9164 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/delete.wav
+-rw-rw-rw-   0        0        0     1586 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/disconnect.mp3
+-rw-rw-rw-   0        0        0     4404 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/disconnect.ogg
+-rw-rw-rw-   0        0        0     1492 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/disconnect.wav
+-rw-rw-rw-   0        0        0      569 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/dropdown-arrow.svg
+-rw-rw-rw-   0        0        0      326 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/handclosed.cur
+-rw-rw-rw-   0        0        0      766 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/handdelete.cur
+-rw-rw-rw-   0        0        0      198 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/handopen.cur
+-rw-rw-rw-   0        0        0     1010 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/pilcrow.png
+-rw-rw-rw-   0        0        0      771 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/quote0.png
+-rw-rw-rw-   0        0        0      738 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/quote1.png
+-rw-rw-rw-   0        0        0     2595 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/sprites.png
+-rw-rw-rw-   0        0        0     1849 2020-06-15 14:02:44.000000 tellibot-1.0.8/tellibot/static/media/sprites.svg
+-rw-rw-rw-   0        0        0     4489 2024-04-29 16:37:17.000000 tellibot-1.0.8/tellibot/tellibot.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.800056 tellibot-1.0.8/tellibot/templates/
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.810264 tellibot-1.0.8/tellibot/templates/editor/
+-rw-rw-rw-   0        0        0     6160 2024-04-28 22:19:00.000000 tellibot-1.0.8/tellibot/templates/editor/index.html
+-rw-rw-rw-   0        0        0     3372 2024-04-28 22:21:10.000000 tellibot-1.0.8/tellibot/templates/index.html
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.885061 tellibot-1.0.8/tellibot/templates/scripts/
+-rw-rw-rw-   0        0        0     2284 2024-04-28 22:04:58.000000 tellibot-1.0.8/tellibot/templates/scripts/009c829d-ba57-4ff4-83e3-1e85f79319fa.tel
+-rw-rw-rw-   0        0        0   363436 2024-04-28 22:23:31.000000 tellibot-1.0.8/tellibot/templates/scripts/07a8c2fa-cd42-45d6-b488-460b18ce9dec.tel
+-rw-rw-rw-   0        0        0   287360 2024-04-28 22:49:19.000000 tellibot-1.0.8/tellibot/templates/scripts/aae450d9-e709-4bbd-94ed-3290f084f9a9.tel
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.956861 tellibot-1.0.8/tellibot/util/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:48:45.000000 tellibot-1.0.8/tellibot/util/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-04-29 15:41:51.000000 tellibot-1.0.8/tellibot/util/colorify.py
+-rw-rw-rw-   0        0        0      461 2024-04-18 22:36:27.000000 tellibot-1.0.8/tellibot/util/formatter.py
+-rw-rw-rw-   0        0        0      526 2024-04-29 15:36:19.000000 tellibot-1.0.8/tellibot/util/log.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:49:09.982124 tellibot-1.0.8/tellibot.egg-info/
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:49:07.000000 tellibot-1.0.8/tellibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6074 2024-04-29 16:49:07.000000 tellibot-1.0.8/tellibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:49:07.000000 tellibot-1.0.8/tellibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-29 16:49:07.000000 tellibot-1.0.8/tellibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-29 16:49:07.000000 tellibot-1.0.8/tellibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 16:49:07.000000 tellibot-1.0.8/tellibot.egg-info/top_level.txt
```

### Comparing `tellibot-1.0.7/LICENSE.txt` & `tellibot-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/PKG-INFO` & `tellibot-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.7
+Version: 1.0.8
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tellibot-1.0.7/setup.py` & `tellibot-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="tellibot",
-    version="1.0.7",
+    version="1.0.8",
     description="A drag and drop programming to create telegram bot",
     url="https://github.com/whoisjeeva/tellibot",
     author="Jeeva",
     author_email="support@gumify.me",
     license="MIT",
     packages=find_packages(),
     package_data={'tellibot': ["tellibot/templates", "tellibot/static"]},
```

### Comparing `tellibot-1.0.7/tellibot/argparse.py` & `tellibot-1.0.8/tellibot/argparse.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/interpreter.py` & `tellibot-1.0.8/tellibot/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/bot_def_command.py` & `tellibot-1.0.8/tellibot/interpreter/statements/bot_def_command.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/bot_handle_admin_message.py` & `tellibot-1.0.8/tellibot/interpreter/statements/bot_handle_admin_message.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/bot_handle_message.py` & `tellibot-1.0.8/tellibot/interpreter/statements/bot_handle_message.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/controls_for.py` & `tellibot-1.0.8/tellibot/interpreter/statements/controls_for.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/controls_forEach.py` & `tellibot-1.0.8/tellibot/interpreter/statements/controls_forEach.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/controls_repeat_ext.py` & `tellibot-1.0.8/tellibot/interpreter/statements/controls_repeat_ext.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/controls_whileUntil.py` & `tellibot-1.0.8/tellibot/interpreter/statements/controls_whileUntil.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/db_connect.py` & `tellibot-1.0.8/tellibot/interpreter/statements/db_connect.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/db_create_table.py` & `tellibot-1.0.8/tellibot/interpreter/statements/db_create_table.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/db_delete_data.py` & `tellibot-1.0.8/tellibot/interpreter/statements/db_delete_data.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/db_insert.py` & `tellibot-1.0.8/tellibot/interpreter/statements/db_insert.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/db_read.py` & `tellibot-1.0.8/tellibot/interpreter/statements/db_read.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/db_update.py` & `tellibot-1.0.8/tellibot/interpreter/statements/db_update.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/dict_create_with.py` & `tellibot-1.0.8/tellibot/interpreter/statements/dict_create_with.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_callnoreturn.py` & `tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_callnoreturn.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_defnoreturn.py` & `tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_defnoreturn.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/function_procedures_defreturn.py` & `tellibot-1.0.8/tellibot/interpreter/statements/function_procedures_defreturn.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/http_request.py` & `tellibot-1.0.8/tellibot/interpreter/statements/http_request.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_chooser.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_chooser.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_getIndex.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_getIndex.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_getSublist.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_getSublist.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_indexOf.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_indexOf.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_regex.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_regex.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_setIndex.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_setIndex.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_sort.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_sort.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/lists_split.py` & `tellibot-1.0.8/tellibot/interpreter/statements/lists_split.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/logic_compare.py` & `tellibot-1.0.8/tellibot/interpreter/statements/logic_compare.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/logic_controls_if.py` & `tellibot-1.0.8/tellibot/interpreter/statements/logic_controls_if.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/logic_operation.py` & `tellibot-1.0.8/tellibot/interpreter/statements/logic_operation.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/logic_ternary.py` & `tellibot-1.0.8/tellibot/interpreter/statements/logic_ternary.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_arithmetic.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_arithmetic.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_change.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_change.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_constant.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_constant.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_constrain.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_constrain.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_number_property.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_number_property.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_on_list.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_on_list.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_round.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_round.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_single.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_single.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/math_trig.py` & `tellibot-1.0.8/tellibot/interpreter/statements/math_trig.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_changeCase.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_changeCase.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_charAt.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_charAt.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_getSubstring.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_getSubstring.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_indexOf.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_indexOf.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_join.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_join.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_prompt.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_prompt.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/statements/text_trim.py` & `tellibot-1.0.8/tellibot/interpreter/statements/text_trim.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/interpreter/util/color.py` & `tellibot-1.0.8/tellibot/interpreter/util/color.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/css/editor.css` & `tellibot-1.0.8/tellibot/static/css/editor.css`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/css/main.css` & `tellibot-1.0.8/tellibot/static/css/main.css`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/dist/.maps/bundle.min.js.map` & `tellibot-1.0.8/tellibot/static/dist/.maps/bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/dist/.maps/compose.min.js.map` & `tellibot-1.0.8/tellibot/static/dist/.maps/compose.min.js.map`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/dist/.maps/editor.min.js.map` & `tellibot-1.0.8/tellibot/static/dist/.maps/editor.min.js.map`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/dist/bundle.min.js` & `tellibot-1.0.8/tellibot/static/dist/bundle.min.js`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/dist/editor.min.js` & `tellibot-1.0.8/tellibot/static/dist/editor.min.js`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/font/icons.woff2` & `tellibot-1.0.8/tellibot/static/font/icons.woff2`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/click.mp3` & `tellibot-1.0.8/tellibot/static/media/click.mp3`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/click.ogg` & `tellibot-1.0.8/tellibot/static/media/click.ogg`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/click.wav` & `tellibot-1.0.8/tellibot/static/media/click.wav`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/delete.mp3` & `tellibot-1.0.8/tellibot/static/media/delete.mp3`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/delete.ogg` & `tellibot-1.0.8/tellibot/static/media/delete.ogg`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/delete.wav` & `tellibot-1.0.8/tellibot/static/media/delete.wav`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/disconnect.mp3` & `tellibot-1.0.8/tellibot/static/media/disconnect.mp3`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/disconnect.ogg` & `tellibot-1.0.8/tellibot/static/media/disconnect.ogg`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/disconnect.wav` & `tellibot-1.0.8/tellibot/static/media/disconnect.wav`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/dropdown-arrow.svg` & `tellibot-1.0.8/tellibot/static/media/dropdown-arrow.svg`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/handdelete.cur` & `tellibot-1.0.8/tellibot/static/media/handdelete.cur`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/pilcrow.png` & `tellibot-1.0.8/tellibot/static/media/pilcrow.png`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/quote0.png` & `tellibot-1.0.8/tellibot/static/media/quote0.png`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/quote1.png` & `tellibot-1.0.8/tellibot/static/media/quote1.png`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/sprites.png` & `tellibot-1.0.8/tellibot/static/media/sprites.png`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/static/media/sprites.svg` & `tellibot-1.0.8/tellibot/static/media/sprites.svg`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/tellibot.py` & `tellibot-1.0.8/tellibot/tellibot.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/templates/editor/index.html` & `tellibot-1.0.8/tellibot/templates/editor/index.html`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/templates/index.html` & `tellibot-1.0.8/tellibot/templates/index.html`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/templates/scripts/009c829d-ba57-4ff4-83e3-1e85f79319fa.tel` & `tellibot-1.0.8/tellibot/templates/scripts/009c829d-ba57-4ff4-83e3-1e85f79319fa.tel`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/templates/scripts/07a8c2fa-cd42-45d6-b488-460b18ce9dec.tel` & `tellibot-1.0.8/tellibot/templates/scripts/07a8c2fa-cd42-45d6-b488-460b18ce9dec.tel`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot/templates/scripts/aae450d9-e709-4bbd-94ed-3290f084f9a9.tel` & `tellibot-1.0.8/tellibot/templates/scripts/aae450d9-e709-4bbd-94ed-3290f084f9a9.tel`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.7/tellibot.egg-info/PKG-INFO` & `tellibot-1.0.8/tellibot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.7
+Version: 1.0.8
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tellibot-1.0.7/tellibot.egg-info/SOURCES.txt` & `tellibot-1.0.8/tellibot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -128,8 +128,12 @@
 tellibot/static/media/quote1.png
 tellibot/static/media/sprites.png
 tellibot/static/media/sprites.svg
 tellibot/templates/index.html
 tellibot/templates/editor/index.html
 tellibot/templates/scripts/009c829d-ba57-4ff4-83e3-1e85f79319fa.tel
 tellibot/templates/scripts/07a8c2fa-cd42-45d6-b488-460b18ce9dec.tel
-tellibot/templates/scripts/aae450d9-e709-4bbd-94ed-3290f084f9a9.tel
+tellibot/templates/scripts/aae450d9-e709-4bbd-94ed-3290f084f9a9.tel
+tellibot/util/__init__.py
+tellibot/util/colorify.py
+tellibot/util/formatter.py
+tellibot/util/log.py
```

