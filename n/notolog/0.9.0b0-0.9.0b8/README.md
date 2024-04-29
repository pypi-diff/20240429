# Comparing `tmp/notolog-0.9.0b0.tar.gz` & `tmp/notolog-0.9.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.0b0.tar", last modified: Sun Apr 28 22:53:55 2024, max compression
+gzip compressed data, was "notolog-0.9.0b8.tar", last modified: Mon Apr 29 00:41:54 2024, max compression
```

## Comparing `notolog-0.9.0b0.tar` & `notolog-0.9.0b8.tar`

### file list

```diff
@@ -1,75 +1,312 @@
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
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.515231 notolog-0.9.0b8/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8547 2024-04-28 21:48:22.000000 notolog-0.9.0b8/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b8/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      124 2024-04-29 00:40:08.000000 notolog-0.9.0b8/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    15876 2024-04-29 00:41:54.514160 notolog-0.9.0b8/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14414 2024-04-29 00:41:08.000000 notolog-0.9.0b8/README.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     2529 2024-04-28 22:15:02.000000 notolog-0.9.0b8/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.157300 notolog-0.9.0b8/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b8/notolog/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.168247 notolog-0.9.0b8/notolog/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4238 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88269 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.124765 notolog-0.9.0b8/notolog/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.195279 notolog-0.9.0b8/notolog/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2145 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6307 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.232348 notolog-0.9.0b8/notolog/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.292705 notolog-0.9.0b8/notolog/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7957 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.306119 notolog-0.9.0b8/notolog/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6410 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.319191 notolog-0.9.0b8/notolog/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7940 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.324387 notolog-0.9.0b8/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b8/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.328969 notolog-0.9.0b8/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1335 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.330518 notolog-0.9.0b8/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.357133 notolog-0.9.0b8/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b8/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.362868 notolog-0.9.0b8/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/highlight/view_highlighter.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.366079 notolog-0.9.0b8/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.368838 notolog-0.9.0b8/notolog/lexemes/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      164 2024-04-29 00:12:00.000000 notolog-0.9.0b8/notolog/lexemes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3221 2024-04-28 22:06:29.000000 notolog-0.9.0b8/notolog/lexemes/__pycache__/lexemes.cpython-39.pyc
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.376491 notolog-0.9.0b8/notolog/lexemes/de/
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6547 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3514 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.383320 notolog-0.9.0b8/notolog/lexemes/en/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.388420 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      883 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6660 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5428 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2083 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2492 2024-04-28 22:11:17.000000 notolog-0.9.0b8/notolog/lexemes/en/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6009 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3351 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.400066 notolog-0.9.0b8/notolog/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6517 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3615 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.408276 notolog-0.9.0b8/notolog/lexemes/fr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6677 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3690 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.420162 notolog-0.9.0b8/notolog/lexemes/ge/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9689 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5310 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.427740 notolog-0.9.0b8/notolog/lexemes/it/
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6327 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3562 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.433315 notolog-0.9.0b8/notolog/lexemes/ja/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.440307 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6809 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3780 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-04-28 22:06:30.000000 notolog-0.9.0b8/notolog/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7209 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3747 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.454200 notolog-0.9.0b8/notolog/lexemes/ko/
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6733 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3414 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.461175 notolog-0.9.0b8/notolog/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6204 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3505 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.468276 notolog-0.9.0b8/notolog/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6315 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3574 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.474202 notolog-0.9.0b8/notolog/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7899 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4504 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.486932 notolog-0.9.0b8/notolog/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5738 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3256 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-04-28 21:48:23.000000 notolog-0.9.0b8/notolog/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   176633 2024-04-28 22:15:02.000000 notolog-0.9.0b8/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.501358 notolog-0.9.0b8/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b8/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b8/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.512988 notolog-0.9.0b8/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    15876 2024-04-29 00:41:53.000000 notolog-0.9.0b8/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    10721 2024-04-29 00:41:54.000000 notolog-0.9.0b8/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-29 00:41:53.000000 notolog-0.9.0b8/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 00:41:53.000000 notolog-0.9.0b8/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-29 00:41:53.000000 notolog-0.9.0b8/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       19 2024-04-29 00:41:53.000000 notolog-0.9.0b8/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 00:41:54.515358 notolog-0.9.0b8/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1492 2024-04-29 00:41:48.000000 notolog-0.9.0b8/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 00:41:54.511011 notolog-0.9.0b8/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9205 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5661 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1158 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4073 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6186 2024-04-28 21:48:22.000000 notolog-0.9.0b8/tests/test_themes.py
```

### Comparing `notolog-0.9.0b0/LICENSE` & `notolog-0.9.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/PKG-INFO` & `notolog-0.9.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b0
+Version: 0.9.0b8
 Summary: Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -269,11 +269,11 @@
 
 This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
 
 As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
 
 ---
 
-`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░` 
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗` 
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║` 
+`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
+`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`</br>
+`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b0/README.md` & `notolog-0.9.0b8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -228,11 +228,11 @@
 
 This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
 
 As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
 
 ---
 
-`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░` 
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗` 
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║` 
+`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
+`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`</br>
+`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b0/notolog/app_config.py` & `notolog-0.9.0b8/notolog/app_config.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/edit_widget.py` & `notolog-0.9.0b8/notolog/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/editor_state.py` & `notolog-0.9.0b8/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_helper.py` & `notolog-0.9.0b8/notolog/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_new_password_dialog.py` & `notolog-0.9.0b8/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_password.py` & `notolog-0.9.0b8/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_password_dialog.py` & `notolog-0.9.0b8/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.0b8/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/etree_extension.py` & `notolog-0.9.0b8/notolog/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/file_header.py` & `notolog-0.9.0b8/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/file_system_watcher.py` & `notolog-0.9.0b8/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/file_helper.py` & `notolog-0.9.0b8/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/theme_helper.py` & `notolog-0.9.0b8/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/tooltip_helper.py` & `notolog-0.9.0b8/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/helpers/update_helper.py` & `notolog-0.9.0b8/notolog/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/highlight/main_highlighter.py` & `notolog-0.9.0b8/notolog/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/highlight/md_highlighter.py` & `notolog-0.9.0b8/notolog/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/highlight/view_highlighter.py` & `notolog-0.9.0b8/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/notolog_editor.py` & `notolog-0.9.0b8/notolog/notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/settings.py` & `notolog-0.9.0b8/notolog/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/text_block_data.py` & `notolog-0.9.0b8/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/theme.py` & `notolog-0.9.0b8/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/about_popup.py` & `notolog-0.9.0b8/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/ai_assistant.py` & `notolog-0.9.0b8/notolog/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/color_picker_dialog.py` & `notolog-0.9.0b8/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/common_dialog.py` & `notolog-0.9.0b8/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/enum_combo_box.py` & `notolog-0.9.0b8/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/file_system_model.py` & `notolog-0.9.0b8/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/line_numbers.py` & `notolog-0.9.0b8/notolog/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/rename_file_dialog.py` & `notolog-0.9.0b8/notolog/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/rotating_label.py` & `notolog-0.9.0b8/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/settings_dialog.py` & `notolog-0.9.0b8/notolog/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/sort_filter_proxy_model.py` & `notolog-0.9.0b8/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/statusbar.py` & `notolog-0.9.0b8/notolog/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/ui/toolbar.py` & `notolog-0.9.0b8/notolog/ui/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/view_decorator.py` & `notolog-0.9.0b8/notolog/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/view_processor.py` & `notolog-0.9.0b8/notolog/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog/view_widget.py` & `notolog-0.9.0b8/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/notolog.egg-info/PKG-INFO` & `notolog-0.9.0b8/notolog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b0
+Version: 0.9.0b8
 Summary: Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -269,11 +269,11 @@
 
 This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
 
 As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
 
 ---
 
-`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░` 
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗` 
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║` 
+`░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
+`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`</br>
+`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b0/tests/test_enc_helper.py` & `notolog-0.9.0b8/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_enc_password.py` & `notolog-0.9.0b8/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_file_header.py` & `notolog-0.9.0b8/tests/test_file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_html_view.py` & `notolog-0.9.0b8/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_lexemes.py` & `notolog-0.9.0b8/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_notolog_editor.py` & `notolog-0.9.0b8/tests/test_notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_settings.py` & `notolog-0.9.0b8/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_text_block_data.py` & `notolog-0.9.0b8/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_theme_helper.py` & `notolog-0.9.0b8/tests/test_theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b0/tests/test_themes.py` & `notolog-0.9.0b8/tests/test_themes.py`

 * *Files identical despite different names*

