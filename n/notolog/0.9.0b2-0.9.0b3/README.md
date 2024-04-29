# Comparing `tmp/notolog-0.9.0b2.tar.gz` & `tmp/notolog-0.9.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.0b2.tar", last modified: Sun Apr 28 23:54:12 2024, max compression
+gzip compressed data, was "notolog-0.9.0b3.tar", last modified: Mon Apr 29 00:00:50 2024, max compression
```

## Comparing `notolog-0.9.0b2.tar` & `notolog-0.9.0b3.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.334390 notolog-0.9.0b2/
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b2/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-28 23:54:12.333358 notolog-0.9.0b2/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14412 2024-04-28 22:22:21.000000 notolog-0.9.0b2/README.md
--rw-r--r--   0 vadikus    (501) staff       (20)     2529 2024-04-28 22:15:02.000000 notolog-0.9.0b2/main.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.269936 notolog-0.9.0b2/notolog/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b2/notolog/app_config.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b2/notolog/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.280519 notolog-0.9.0b2/notolog/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b2/notolog/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/encrypt/enc_password_reset_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/etree_extension.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.288623 notolog-0.9.0b2/notolog/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b2/notolog/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.294083 notolog-0.9.0b2/notolog/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b2/notolog/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)   176633 2024-04-28 22:15:02.000000 notolog-0.9.0b2/notolog/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.319231 notolog-0.9.0b2/notolog/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b2/notolog/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b2/notolog/view_widget.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.331924 notolog-0.9.0b2/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-28 23:54:12.000000 notolog-0.9.0b2/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)     1819 2024-04-28 23:54:12.000000 notolog-0.9.0b2/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-28 23:54:12.000000 notolog-0.9.0b2/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-28 23:54:12.000000 notolog-0.9.0b2/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-28 23:54:12.000000 notolog-0.9.0b2/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       19 2024-04-28 23:54:12.000000 notolog-0.9.0b2/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-28 23:54:12.334574 notolog-0.9.0b2/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     1445 2024-04-28 23:53:57.000000 notolog-0.9.0b2/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-28 23:54:12.330714 notolog-0.9.0b2/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9205 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5661 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1158 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4073 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6186 2024-04-28 21:48:22.000000 notolog-0.9.0b2/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.138756 notolog-0.9.0b3/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b3/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-29 00:00:50.137617 notolog-0.9.0b3/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14412 2024-04-28 22:22:21.000000 notolog-0.9.0b3/README.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     2529 2024-04-28 22:15:02.000000 notolog-0.9.0b3/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.062452 notolog-0.9.0b3/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b3/notolog/app_config.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b3/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.074414 notolog-0.9.0b3/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b3/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.084782 notolog-0.9.0b3/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1335 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/etree_extension.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.091171 notolog-0.9.0b3/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b3/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.096170 notolog-0.9.0b3/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b3/notolog/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   176633 2024-04-28 22:15:02.000000 notolog-0.9.0b3/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.120729 notolog-0.9.0b3/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b3/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b3/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.136209 notolog-0.9.0b3/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    15874 2024-04-29 00:00:49.000000 notolog-0.9.0b3/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)     1952 2024-04-29 00:00:49.000000 notolog-0.9.0b3/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-29 00:00:49.000000 notolog-0.9.0b3/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 00:00:49.000000 notolog-0.9.0b3/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-29 00:00:49.000000 notolog-0.9.0b3/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       19 2024-04-29 00:00:49.000000 notolog-0.9.0b3/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 00:00:50.139034 notolog-0.9.0b3/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1446 2024-04-29 00:00:46.000000 notolog-0.9.0b3/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:00:50.134901 notolog-0.9.0b3/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9205 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5661 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1158 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4073 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6186 2024-04-28 21:48:22.000000 notolog-0.9.0b3/tests/test_themes.py
```

### Comparing `notolog-0.9.0b2/LICENSE` & `notolog-0.9.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/PKG-INFO` & `notolog-0.9.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `notolog-0.9.0b2/README.md` & `notolog-0.9.0b3/README.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/main.py` & `notolog-0.9.0b3/main.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/app_config.py` & `notolog-0.9.0b3/notolog/app_config.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/edit_widget.py` & `notolog-0.9.0b3/notolog/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/editor_state.py` & `notolog-0.9.0b3/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/encrypt/enc_helper.py` & `notolog-0.9.0b3/notolog/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/encrypt/enc_new_password_dialog.py` & `notolog-0.9.0b3/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/encrypt/enc_password.py` & `notolog-0.9.0b3/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/encrypt/enc_password_dialog.py` & `notolog-0.9.0b3/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.0b3/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/etree_extension.py` & `notolog-0.9.0b3/notolog/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/file_header.py` & `notolog-0.9.0b3/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/file_system_watcher.py` & `notolog-0.9.0b3/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/helpers/file_helper.py` & `notolog-0.9.0b3/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/helpers/theme_helper.py` & `notolog-0.9.0b3/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/helpers/tooltip_helper.py` & `notolog-0.9.0b3/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/helpers/update_helper.py` & `notolog-0.9.0b3/notolog/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/highlight/main_highlighter.py` & `notolog-0.9.0b3/notolog/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/highlight/md_highlighter.py` & `notolog-0.9.0b3/notolog/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/highlight/view_highlighter.py` & `notolog-0.9.0b3/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/notolog_editor.py` & `notolog-0.9.0b3/notolog/notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/settings.py` & `notolog-0.9.0b3/notolog/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/text_block_data.py` & `notolog-0.9.0b3/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/theme.py` & `notolog-0.9.0b3/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/about_popup.py` & `notolog-0.9.0b3/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/ai_assistant.py` & `notolog-0.9.0b3/notolog/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/color_picker_dialog.py` & `notolog-0.9.0b3/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/common_dialog.py` & `notolog-0.9.0b3/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/enum_combo_box.py` & `notolog-0.9.0b3/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/file_system_model.py` & `notolog-0.9.0b3/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/line_numbers.py` & `notolog-0.9.0b3/notolog/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/rename_file_dialog.py` & `notolog-0.9.0b3/notolog/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/rotating_label.py` & `notolog-0.9.0b3/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/settings_dialog.py` & `notolog-0.9.0b3/notolog/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/sort_filter_proxy_model.py` & `notolog-0.9.0b3/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/statusbar.py` & `notolog-0.9.0b3/notolog/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/ui/toolbar.py` & `notolog-0.9.0b3/notolog/ui/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/view_decorator.py` & `notolog-0.9.0b3/notolog/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/view_processor.py` & `notolog-0.9.0b3/notolog/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog/view_widget.py` & `notolog-0.9.0b3/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/notolog.egg-info/PKG-INFO` & `notolog-0.9.0b3/notolog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `notolog-0.9.0b2/notolog.egg-info/SOURCES.txt` & `notolog-0.9.0b3/notolog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
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
 notolog/helpers/__init__.py
 notolog/helpers/clipboard_helper.py
 notolog/helpers/file_helper.py
 notolog/helpers/theme_helper.py
 notolog/helpers/tooltip_helper.py
 notolog/helpers/update_helper.py
 notolog/highlight/__init__.py
```

### Comparing `notolog-0.9.0b2/setup.py` & `notolog-0.9.0b3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.0b2',
+    version='0.9.0b3',
     description='Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     py_modules=['main'],
     entry_points={
@@ -27,15 +27,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
     packages=find_packages(),  # Find all packages in the directory
-    include_package_data=True,
+    #include_package_data=True,
     python_requires='>=3.9, <4',
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/notolog/notolog-editor/issues',
         'Source': 'https://github.com/notolog/notolog-editor/',
     },
 )
```

### Comparing `notolog-0.9.0b2/tests/test_enc_helper.py` & `notolog-0.9.0b3/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_enc_password.py` & `notolog-0.9.0b3/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_file_header.py` & `notolog-0.9.0b3/tests/test_file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_html_view.py` & `notolog-0.9.0b3/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_lexemes.py` & `notolog-0.9.0b3/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_notolog_editor.py` & `notolog-0.9.0b3/tests/test_notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_settings.py` & `notolog-0.9.0b3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_text_block_data.py` & `notolog-0.9.0b3/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_theme_helper.py` & `notolog-0.9.0b3/tests/test_theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b2/tests/test_themes.py` & `notolog-0.9.0b3/tests/test_themes.py`

 * *Files identical despite different names*

