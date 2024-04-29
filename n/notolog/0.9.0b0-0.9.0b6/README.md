# Comparing `tmp/notolog-0.9.0b0.tar.gz` & `tmp/notolog-0.9.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.0b0.tar", last modified: Sun Apr 28 22:53:55 2024, max compression
+gzip compressed data, was "notolog-0.9.0b6.tar", last modified: Mon Apr 29 00:19:06 2024, max compression
```

## Comparing `notolog-0.9.0b0.tar` & `notolog-0.9.0b6.tar`

### file list

```diff
@@ -1,75 +1,88 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.975938 notolog-0.9.0b0/
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b0/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-28 22:53:55.975139 notolog-0.9.0b0/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14412 2024-04-28 22:22:21.000000 notolog-0.9.0b0/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.902611 notolog-0.9.0b0/notolog/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b0/notolog/app_config.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b0/notolog/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.911361 notolog-0.9.0b0/notolog/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b0/notolog/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/encrypt/enc_password_reset_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/etree_extension.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.916162 notolog-0.9.0b0/notolog/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b0/notolog/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.925408 notolog-0.9.0b0/notolog/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b0/notolog/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)   176633 2024-04-28 22:15:02.000000 notolog-0.9.0b0/notolog/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.964706 notolog-0.9.0b0/notolog/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b0/notolog/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b0/notolog/view_widget.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.974318 notolog-0.9.0b0/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-28 22:53:55.000000 notolog-0.9.0b0/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)     1811 2024-04-28 22:53:55.000000 notolog-0.9.0b0/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-28 22:53:55.000000 notolog-0.9.0b0/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-28 22:53:55.000000 notolog-0.9.0b0/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-28 22:53:55.000000 notolog-0.9.0b0/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-04-28 22:53:55.000000 notolog-0.9.0b0/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-28 22:53:55.976077 notolog-0.9.0b0/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     1388 2024-04-28 22:15:02.000000 notolog-0.9.0b0/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 22:53:55.973426 notolog-0.9.0b0/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9205 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5661 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1158 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4073 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6186 2024-04-28 21:48:22.000000 notolog-0.9.0b0/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.111420 notolog-0.9.0b6/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b6/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-29 00:19:06.110397 notolog-0.9.0b6/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14412 2024-04-28 22:22:21.000000 notolog-0.9.0b6/README.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     2529 2024-04-28 22:15:02.000000 notolog-0.9.0b6/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.042338 notolog-0.9.0b6/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b6/notolog/app_config.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b6/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.054671 notolog-0.9.0b6/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b6/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.061322 notolog-0.9.0b6/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1335 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.062575 notolog-0.9.0b6/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.066923 notolog-0.9.0b6/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b6/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.071565 notolog-0.9.0b6/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b6/notolog/highlight/view_highlighter.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.073031 notolog-0.9.0b6/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/lexemes/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-04-28 21:48:23.000000 notolog-0.9.0b6/notolog/lexemes/lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   176633 2024-04-28 22:15:02.000000 notolog-0.9.0b6/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.096231 notolog-0.9.0b6/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b6/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b6/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.109037 notolog-0.9.0b6/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-29 00:19:05.000000 notolog-0.9.0b6/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)     2088 2024-04-29 00:19:05.000000 notolog-0.9.0b6/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-29 00:19:05.000000 notolog-0.9.0b6/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 00:19:05.000000 notolog-0.9.0b6/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-29 00:19:05.000000 notolog-0.9.0b6/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       19 2024-04-29 00:19:05.000000 notolog-0.9.0b6/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 00:19:06.111579 notolog-0.9.0b6/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1445 2024-04-29 00:18:58.000000 notolog-0.9.0b6/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:19:06.107889 notolog-0.9.0b6/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9205 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5661 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1158 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4073 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6186 2024-04-28 21:48:22.000000 notolog-0.9.0b6/tests/test_themes.py
```

### Comparing `notolog-0.9.0b0/LICENSE` & `notolog-0.9.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/PKG-INFO` & `notolog-0.9.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b0
+Version: 0.9.0b6
 Summary: Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `notolog-0.9.0b0/README.md` & `notolog-0.9.0b6/README.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/app_config.py` & `notolog-0.9.0b6/notolog/app_config.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/edit_widget.py` & `notolog-0.9.0b6/notolog/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/editor_state.py` & `notolog-0.9.0b6/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_helper.py` & `notolog-0.9.0b6/notolog/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_new_password_dialog.py` & `notolog-0.9.0b6/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_password.py` & `notolog-0.9.0b6/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_password_dialog.py` & `notolog-0.9.0b6/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.0b6/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/etree_extension.py` & `notolog-0.9.0b6/notolog/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/file_header.py` & `notolog-0.9.0b6/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/file_system_watcher.py` & `notolog-0.9.0b6/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/file_helper.py` & `notolog-0.9.0b6/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/theme_helper.py` & `notolog-0.9.0b6/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/tooltip_helper.py` & `notolog-0.9.0b6/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/update_helper.py` & `notolog-0.9.0b6/notolog/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/highlight/main_highlighter.py` & `notolog-0.9.0b6/notolog/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/highlight/md_highlighter.py` & `notolog-0.9.0b6/notolog/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/highlight/view_highlighter.py` & `notolog-0.9.0b6/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/notolog_editor.py` & `notolog-0.9.0b6/notolog/notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/settings.py` & `notolog-0.9.0b6/notolog/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/text_block_data.py` & `notolog-0.9.0b6/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/theme.py` & `notolog-0.9.0b6/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/about_popup.py` & `notolog-0.9.0b6/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/ai_assistant.py` & `notolog-0.9.0b6/notolog/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/color_picker_dialog.py` & `notolog-0.9.0b6/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/common_dialog.py` & `notolog-0.9.0b6/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/enum_combo_box.py` & `notolog-0.9.0b6/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/file_system_model.py` & `notolog-0.9.0b6/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/line_numbers.py` & `notolog-0.9.0b6/notolog/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/rename_file_dialog.py` & `notolog-0.9.0b6/notolog/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/rotating_label.py` & `notolog-0.9.0b6/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/settings_dialog.py` & `notolog-0.9.0b6/notolog/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/sort_filter_proxy_model.py` & `notolog-0.9.0b6/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/statusbar.py` & `notolog-0.9.0b6/notolog/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/toolbar.py` & `notolog-0.9.0b6/notolog/ui/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/view_decorator.py` & `notolog-0.9.0b6/notolog/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/view_processor.py` & `notolog-0.9.0b6/notolog/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/view_widget.py` & `notolog-0.9.0b6/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog.egg-info/PKG-INFO` & `notolog-0.9.0b6/notolog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b0
+Version: 0.9.0b6
 Summary: Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `notolog-0.9.0b0/notolog.egg-info/SOURCES.txt` & `notolog-0.9.0b6/notolog.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+main.py
 setup.py
 notolog/__init__.py
 notolog/app_config.py
 notolog/edit_widget.py
 notolog/editor_state.py
 notolog/etree_extension.py
 notolog/file_header.py
@@ -23,24 +24,33 @@
 notolog.egg-info/top_level.txt
 notolog/encrypt/__init__.py
 notolog/encrypt/enc_helper.py
 notolog/encrypt/enc_new_password_dialog.py
 notolog/encrypt/enc_password.py
 notolog/encrypt/enc_password_dialog.py
 notolog/encrypt/enc_password_reset_dialog.py
+notolog/enums/__init__.py
+notolog/enums/ai_model_names.py
+notolog/enums/colors.py
+notolog/enums/languages.py
+notolog/enums/themes.py
+notolog/exceptions/__init__.py
+notolog/exceptions/file_header_empty_exception.py
 notolog/helpers/__init__.py
 notolog/helpers/clipboard_helper.py
 notolog/helpers/file_helper.py
 notolog/helpers/theme_helper.py
 notolog/helpers/tooltip_helper.py
 notolog/helpers/update_helper.py
 notolog/highlight/__init__.py
 notolog/highlight/main_highlighter.py
 notolog/highlight/md_highlighter.py
 notolog/highlight/view_highlighter.py
+notolog/lexemes/__init__.py
+notolog/lexemes/lexemes.py
 notolog/ui/__init__.py
 notolog/ui/about_popup.py
 notolog/ui/ai_assistant.py
 notolog/ui/color_picker_dialog.py
 notolog/ui/common_dialog.py
 notolog/ui/enum_combo_box.py
 notolog/ui/file_system_model.py
```

### Comparing `notolog-0.9.0b0/setup.py` & `notolog-0.9.0b6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.0b0',
+    version='0.9.0b6',
     description='Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
+    py_modules=['main'],
     entry_points={
         'console_scripts': [
             'notolog=main:main',
         ],
     },
     classifiers=[
         # More info https://pypi.org/classifiers/
@@ -26,14 +27,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
     packages=find_packages(),  # Find all packages in the directory
+    include_package_data=True,
     python_requires='>=3.9, <4',
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/notolog/notolog-editor/issues',
         'Source': 'https://github.com/notolog/notolog-editor/',
     },
-)
+)
```

### Comparing `notolog-0.9.0b0/tests/test_enc_helper.py` & `notolog-0.9.0b6/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_enc_password.py` & `notolog-0.9.0b6/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_file_header.py` & `notolog-0.9.0b6/tests/test_file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_html_view.py` & `notolog-0.9.0b6/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_lexemes.py` & `notolog-0.9.0b6/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_notolog_editor.py` & `notolog-0.9.0b6/tests/test_notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_settings.py` & `notolog-0.9.0b6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_text_block_data.py` & `notolog-0.9.0b6/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_theme_helper.py` & `notolog-0.9.0b6/tests/test_theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_themes.py` & `notolog-0.9.0b6/tests/test_themes.py`

 * *Files identical despite different names*

